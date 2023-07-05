# Comparing `tmp/NeXpy-1.0.3.tar.gz` & `tmp/NeXpy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeXpy-1.0.3.tar", last modified: Tue Apr 18 15:01:55 2023, max compression
+gzip compressed data, was "NeXpy-1.0.4.tar", last modified: Wed Jul  5 18:50:57 2023, max compression
```

## Comparing `NeXpy-1.0.3.tar` & `NeXpy-1.0.4.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635950 NeXpy-1.0.3/
--rw-r--r--   0 rosborn    (504) 660979062      672 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.gitattributes
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.567221 NeXpy-1.0.3/.github/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.572295 NeXpy-1.0.3/.github/workflows/
--rw-r--r--   0 rosborn    (504) 660979062      654 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 rosborn    (504) 660979062      577 2023-04-15 18:57:55.000000 NeXpy-1.0.3/.gitignore
--rw-r--r--   0 rosborn    (504) 660979062     2378 2023-04-15 18:57:55.000000 NeXpy-1.0.3/COPYING
--rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-18 15:01:55.636113 NeXpy-1.0.3/PKG-INFO
--rw-r--r--   0 rosborn    (504) 660979062     4283 2023-04-15 18:57:55.000000 NeXpy-1.0.3/README.md
--rw-r--r--   0 rosborn    (504) 660979062     7060 2023-04-15 18:57:55.000000 NeXpy-1.0.3/README.rst
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.573353 NeXpy-1.0.3/conda-recipe/
--rw-r--r--   0 rosborn    (504) 660979062       51 2022-11-15 16:30:46.000000 NeXpy-1.0.3/conda-recipe/bld.bat
--rw-r--r--   0 rosborn    (504) 660979062      103 2022-11-15 16:30:46.000000 NeXpy-1.0.3/conda-recipe/build.sh
--rw-r--r--   0 rosborn    (504) 660979062      999 2023-04-15 18:57:55.000000 NeXpy-1.0.3/conda-recipe/meta.yaml
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.574028 NeXpy-1.0.3/doc/
--rw-r--r--   0 rosborn    (504) 660979062     5643 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/Makefile
--rw-r--r--   0 rosborn    (504) 660979062     5103 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/make.bat
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.576472 NeXpy-1.0.3/doc/source/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.576727 NeXpy-1.0.3/doc/source/_static/
--rw-r--r--   0 rosborn    (504) 660979062      102 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/_static/__ignore__.txt
--rw-r--r--   0 rosborn    (504) 660979062     8265 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/conf.py
--rw-r--r--   0 rosborn    (504) 660979062      526 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/examples.rst
--rw-r--r--   0 rosborn    (504) 660979062    90022 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/favicon.ico
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.589111 NeXpy-1.0.3/doc/source/images/
--rw-r--r--   0 rosborn    (504) 660979062    14509 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/axis-limits-bar.png
--rw-r--r--   0 rosborn    (504) 660979062   684819 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/customize-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   432231 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/limits-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   705341 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/nexpy-fits.png
--rw-r--r--   0 rosborn    (504) 660979062   364457 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/nexpy-gui.png
--rw-r--r--   0 rosborn    (504) 660979062    40568 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/nexpy-logo.png
--rw-r--r--   0 rosborn    (504) 660979062    43638 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/options-tab.png
--rw-r--r--   0 rosborn    (504) 660979062   496144 2023-04-15 18:57:55.000000 NeXpy-1.0.3/doc/source/images/projection-panel.png
--rw-r--r--   0 rosborn    (504) 660979062    20559 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/projection-tab.png
--rw-r--r--   0 rosborn    (504) 660979062   590841 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/scan-panel.png
--rw-r--r--   0 rosborn    (504) 660979062   598861 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/signal-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    73587 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/simple-plot.png
--rw-r--r--   0 rosborn    (504) 660979062   308220 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/skewed-axis.png
--rw-r--r--   0 rosborn    (504) 660979062    19535 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/x-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    29737 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/images/y-tab.png
--rw-r--r--   0 rosborn    (504) 660979062    20833 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/z-tab.png
--rw-r--r--   0 rosborn    (504) 660979062     8104 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/images/z-toolbar.png
--rw-r--r--   0 rosborn    (504) 660979062       30 2022-11-15 16:30:46.000000 NeXpy-1.0.3/doc/source/includeme.rst
--rw-r--r--   0 rosborn    (504) 660979062     1093 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/index.rst
--rw-r--r--   0 rosborn    (504) 660979062    62301 2023-04-17 14:57:59.000000 NeXpy-1.0.3/doc/source/pythongui.rst
--rw-r--r--   0 rosborn    (504) 660979062    44651 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/pythonshell.rst
--rw-r--r--   0 rosborn    (504) 660979062     2845 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/readers.rst
--rw-r--r--   0 rosborn    (504) 660979062      417 2023-04-15 18:57:56.000000 NeXpy-1.0.3/doc/source/treeapi.rst
--rw-r--r--   0 rosborn    (504) 660979062      181 2023-04-15 18:57:56.000000 NeXpy-1.0.3/pyproject.toml
--rw-r--r--   0 rosborn    (504) 660979062     1667 2023-04-18 15:01:55.636650 NeXpy-1.0.3/setup.cfg
--rwxr-xr-x   0 rosborn    (504) 660979062      410 2023-04-15 18:57:56.000000 NeXpy-1.0.3/setup.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.568241 NeXpy-1.0.3/src/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.590535 NeXpy-1.0.3/src/NeXpy.egg-info/
--rw-r--r--   0 rosborn    (504) 660979062     5299 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/PKG-INFO
--rw-r--r--   0 rosborn    (504) 660979062     9860 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/SOURCES.txt
--rw-r--r--   0 rosborn    (504) 660979062        1 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/dependency_links.txt
--rw-r--r--   0 rosborn    (504) 660979062       42 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/entry_points.txt
--rw-r--r--   0 rosborn    (504) 660979062       47 2017-06-13 21:39:09.000000 NeXpy-1.0.3/src/NeXpy.egg-info/pbr.json
--rw-r--r--   0 rosborn    (504) 660979062      244 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/requires.txt
--rw-r--r--   0 rosborn    (504) 660979062        6 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/NeXpy.egg-info/top_level.txt
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591076 NeXpy-1.0.3/src/nexpy/
--rw-r--r--   0 rosborn    (504) 660979062      395 2023-04-15 19:28:11.000000 NeXpy-1.0.3/src/nexpy/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062      160 2023-04-18 15:01:55.000000 NeXpy-1.0.3/src/nexpy/_version.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591385 NeXpy-1.0.3/src/nexpy/api/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591678 NeXpy-1.0.3/src/nexpy/api/frills/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/frills/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062     8480 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/fit.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.591869 NeXpy-1.0.3/src/nexpy/api/frills/functions/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/api/frills/functions/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.592698 NeXpy-1.0.3/src/nexpy/api/frills/models/
--rw-r--r--   0 rosborn    (504) 660979062        0 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062     1132 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/bose.py
--rw-r--r--   0 rosborn    (504) 660979062      931 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/critexp.py
--rw-r--r--   0 rosborn    (504) 660979062      916 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/op.py
--rw-r--r--   0 rosborn    (504) 660979062      942 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/api/frills/models/pdfdecay.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.592896 NeXpy-1.0.3/src/nexpy/definitions/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/definitions/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.600331 NeXpy-1.0.3/src/nexpy/definitions/applications/
--rw-r--r--   0 rosborn    (504) 660979062     6656 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXarchive.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5051 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXarpes.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    50836 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2667 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3803 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXfluo.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2774 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5070 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXiqproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5557 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXlauetof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5500 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXmonopd.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    30950 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXmx.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4469 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXrefscan.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4919 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXreftof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7147 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6974 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsastof.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4480 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXscan.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3495 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXspe.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4547 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXsqom.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    10592 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXstxm.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7230 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5530 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6031 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofraw.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5772 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6441 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomo.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6800 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomophase.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5033 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4687 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxas.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3565 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxasproc.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxbase.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4034 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxeuler.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3899 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxkappa.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2671 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaue.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2066 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3632 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxnb.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3868 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/NXxrot.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     9850 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/applications/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.616618 NeXpy-1.0.3/src/nexpy/definitions/base_classes/
--rw-r--r--   0 rosborn    (504) 660979062     2888 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3553 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6264 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3029 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3891 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3074 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2818 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcite.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    13934 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3997 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    16352 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdata.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    26917 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4068 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6385 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5447 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     8063 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXentry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2293 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5023 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6816 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3093 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3493 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3299 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3949 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     7713 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXguide.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3606 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3459 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5749 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXlog.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6041 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3284 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5290 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3398 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2853 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXnote.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     1397 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXobject.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4413 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3058 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2196 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6173 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2499 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2419 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3770 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2847 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    20356 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     4090 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXroot.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    14403 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6404 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     5297 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3723 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXshape.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2740 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXslit.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6942 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsource.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     6964 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     8599 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2993 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXuser.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3107 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3830 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     8463 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/base_classes/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.620176 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/
--rw-r--r--   0 rosborn    (504) 660979062     6935 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2862 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    10240 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2498 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2506 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     3113 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2143 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    13513 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    14352 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2137 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     1896 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062    15240 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml
--rw-r--r--   0 rosborn    (504) 660979062     2719 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
--rwxr-xr-x   0 rosborn    (504) 660979062     9805 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.621364 NeXpy-1.0.3/src/nexpy/examples/
--rw-r--r--   0 rosborn    (504) 660979062      615 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/README.rst
--rw-r--r--   0 rosborn    (504) 660979062   382712 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/chopper.nxs
--rw-r--r--   0 rosborn    (504) 660979062    53690 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/example.nxs
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.621965 NeXpy-1.0.3/src/nexpy/examples/plugins/
--rw-r--r--   0 rosborn    (504) 660979062     2026 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/README.rst
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.622315 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.624179 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/
--rw-r--r--   0 rosborn    (504) 660979062      244 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062      711 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc
--rw-r--r--   0 rosborn    (504) 660979062     4263 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py
--rw-r--r--   0 rosborn    (504) 660979062     6571 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc
--rw-r--r--   0 rosborn    (504) 660979062     2383 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py
--rw-r--r--   0 rosborn    (504) 660979062     3888 2016-08-04 20:27:34.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc
--rw-r--r--   0 rosborn    (504) 660979062      255 2023-04-17 14:57:59.000000 NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/pyproject.toml
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.624839 NeXpy-1.0.3/src/nexpy/examples/scripts/
--rw-r--r--   0 rosborn    (504) 660979062      634 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/README.rst
--rw-r--r--   0 rosborn    (504) 660979062      235 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/chopper_plot.py
--rw-r--r--   0 rosborn    (504) 660979062      203 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/examples/scripts/example.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.628288 NeXpy-1.0.3/src/nexpy/gui/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.3/src/nexpy/gui/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062    14081 2023-04-17 15:50:34.000000 NeXpy-1.0.3/src/nexpy/gui/consoleapp.py
--rw-r--r--   0 rosborn    (504) 660979062   178273 2023-04-17 20:23:53.000000 NeXpy-1.0.3/src/nexpy/gui/datadialogs.py
--rwxr-xr-x   0 rosborn    (504) 660979062    55605 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/fitdialogs.py
--rw-r--r--   0 rosborn    (504) 660979062     1283 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/importdialog.py
--rw-r--r--   0 rosborn    (504) 660979062    92974 2023-04-17 16:33:37.000000 NeXpy-1.0.3/src/nexpy/gui/mainwindow.py
--rw-r--r--   0 rosborn    (504) 660979062   150779 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/plotview.py
--rw-r--r--   0 rosborn    (504) 660979062     1201 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/pyqt.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.633639 NeXpy-1.0.3/src/nexpy/gui/resources/
--rw-r--r--   0 rosborn    (504) 660979062     1465 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/back.png
--rw-r--r--   0 rosborn    (504) 660979062      401 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/backward-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      905 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/customize.png
--rw-r--r--   0 rosborn    (504) 660979062      514 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/equal.png
--rw-r--r--   0 rosborn    (504) 660979062    37268 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/export-data.png
--rw-r--r--   0 rosborn    (504) 660979062    43660 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/export-figure.png
--rw-r--r--   0 rosborn    (504) 660979062     1121 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/filesave.png
--rw-r--r--   0 rosborn    (504) 660979062      410 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/forward-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1462 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/forward.png
--rw-r--r--   0 rosborn    (504) 660979062      979 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/hand.png
--rw-r--r--   0 rosborn    (504) 660979062     1338 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/home.png
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.634315 NeXpy-1.0.3/src/nexpy/gui/resources/icon/
--rw-r--r--   0 rosborn    (504) 660979062    95378 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.png
--rw-r--r--   0 rosborn    (504) 660979062   127292 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.svg
--rw-r--r--   0 rosborn    (504) 660979062      613 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/link-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      241 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/lock-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1439 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/lock-red-icon.png
--rw-r--r--   0 rosborn    (504) 660979062      713 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/move.png
--rw-r--r--   0 rosborn    (504) 660979062      290 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/pause-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1617 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/refresh-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     2713 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/subplots.png
--rw-r--r--   0 rosborn    (504) 660979062      258 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/unlock-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1415 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/resources/unlock-red-icon.png
--rw-r--r--   0 rosborn    (504) 660979062     1233 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/gui/resources/zoom_to_rect.png
--rw-r--r--   0 rosborn    (504) 660979062     8546 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/scripteditor.py
--rw-r--r--   0 rosborn    (504) 660979062    23583 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/treeview.py
--rw-r--r--   0 rosborn    (504) 660979062    28172 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/utils.py
--rw-r--r--   0 rosborn    (504) 660979062    42714 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/gui/widgets.py
--rwxr-xr-x   0 rosborn    (504) 660979062     1281 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/nexpygui.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.634644 NeXpy-1.0.3/src/nexpy/plugins/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/plugins/__init__.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635505 NeXpy-1.0.3/src/nexpy/readers/
--rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.3/src/nexpy/readers/__init__.py
--rw-r--r--   0 rosborn    (504) 660979062    15851 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readspec.py
--rw-r--r--   0 rosborn    (504) 660979062    10515 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readstack.py
--rw-r--r--   0 rosborn    (504) 660979062     1409 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readtiff.py
--rw-r--r--   0 rosborn    (504) 660979062     9571 2023-04-15 18:57:56.000000 NeXpy-1.0.3/src/nexpy/readers/readtxt.py
-drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-04-18 15:01:55.635746 NeXpy-1.0.3/tests/
--rw-r--r--   0 rosborn    (504) 660979062      997 2023-04-15 18:57:56.000000 NeXpy-1.0.3/tests/test_imports.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.977344 NeXpy-1.0.4/
+-rw-r--r--   0 rosborn    (504) 660979062      672 2023-04-15 18:57:55.000000 NeXpy-1.0.4/.gitattributes
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.886093 NeXpy-1.0.4/.github/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.891441 NeXpy-1.0.4/.github/workflows/
+-rw-r--r--   0 rosborn    (504) 660979062      654 2023-04-15 18:57:55.000000 NeXpy-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 rosborn    (504) 660979062      577 2023-04-15 18:57:55.000000 NeXpy-1.0.4/.gitignore
+-rw-r--r--   0 rosborn    (504) 660979062     2378 2023-04-15 18:57:55.000000 NeXpy-1.0.4/COPYING
+-rw-r--r--   0 rosborn    (504) 660979062     5299 2023-07-05 18:50:57.977519 NeXpy-1.0.4/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     4283 2023-04-15 18:57:55.000000 NeXpy-1.0.4/README.md
+-rw-r--r--   0 rosborn    (504) 660979062     7060 2023-04-15 18:57:55.000000 NeXpy-1.0.4/README.rst
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.892434 NeXpy-1.0.4/conda-recipe/
+-rw-r--r--   0 rosborn    (504) 660979062       51 2022-11-15 16:30:46.000000 NeXpy-1.0.4/conda-recipe/bld.bat
+-rw-r--r--   0 rosborn    (504) 660979062      103 2022-11-15 16:30:46.000000 NeXpy-1.0.4/conda-recipe/build.sh
+-rw-r--r--   0 rosborn    (504) 660979062     1008 2023-06-30 18:13:31.000000 NeXpy-1.0.4/conda-recipe/meta.yaml
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.893233 NeXpy-1.0.4/doc/
+-rw-r--r--   0 rosborn    (504) 660979062     5643 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/Makefile
+-rw-r--r--   0 rosborn    (504) 660979062     5103 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/make.bat
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.896296 NeXpy-1.0.4/doc/source/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.896530 NeXpy-1.0.4/doc/source/_static/
+-rw-r--r--   0 rosborn    (504) 660979062      102 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/_static/__ignore__.txt
+-rw-r--r--   0 rosborn    (504) 660979062     8265 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/conf.py
+-rw-r--r--   0 rosborn    (504) 660979062      526 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/examples.rst
+-rw-r--r--   0 rosborn    (504) 660979062    90022 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/favicon.ico
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.909370 NeXpy-1.0.4/doc/source/images/
+-rw-r--r--   0 rosborn    (504) 660979062    14509 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/axis-limits-bar.png
+-rw-r--r--   0 rosborn    (504) 660979062   684819 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/customize-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   432231 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/limits-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   705341 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/nexpy-fits.png
+-rw-r--r--   0 rosborn    (504) 660979062   364457 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/nexpy-gui.png
+-rw-r--r--   0 rosborn    (504) 660979062    40568 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/nexpy-logo.png
+-rw-r--r--   0 rosborn    (504) 660979062    43638 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/options-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062   496144 2023-04-15 18:57:55.000000 NeXpy-1.0.4/doc/source/images/projection-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062    20559 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/projection-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062   590841 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/images/scan-panel.png
+-rw-r--r--   0 rosborn    (504) 660979062   598861 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/images/signal-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    73587 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/simple-plot.png
+-rw-r--r--   0 rosborn    (504) 660979062   308220 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/images/skewed-axis.png
+-rw-r--r--   0 rosborn    (504) 660979062    19535 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/x-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    29737 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/images/y-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062    20833 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/z-tab.png
+-rw-r--r--   0 rosborn    (504) 660979062     8104 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/images/z-toolbar.png
+-rw-r--r--   0 rosborn    (504) 660979062       30 2022-11-15 16:30:46.000000 NeXpy-1.0.4/doc/source/includeme.rst
+-rw-r--r--   0 rosborn    (504) 660979062     1093 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/index.rst
+-rw-r--r--   0 rosborn    (504) 660979062    62301 2023-04-17 14:57:59.000000 NeXpy-1.0.4/doc/source/pythongui.rst
+-rw-r--r--   0 rosborn    (504) 660979062    44651 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/pythonshell.rst
+-rw-r--r--   0 rosborn    (504) 660979062     2845 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/readers.rst
+-rw-r--r--   0 rosborn    (504) 660979062      417 2023-04-15 18:57:56.000000 NeXpy-1.0.4/doc/source/treeapi.rst
+-rw-r--r--   0 rosborn    (504) 660979062      181 2023-04-15 18:57:56.000000 NeXpy-1.0.4/pyproject.toml
+-rw-r--r--   0 rosborn    (504) 660979062     1676 2023-07-05 18:50:57.978101 NeXpy-1.0.4/setup.cfg
+-rwxr-xr-x   0 rosborn    (504) 660979062      410 2023-04-15 18:57:56.000000 NeXpy-1.0.4/setup.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.886883 NeXpy-1.0.4/src/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.910827 NeXpy-1.0.4/src/NeXpy.egg-info/
+-rw-r--r--   0 rosborn    (504) 660979062     5299 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/PKG-INFO
+-rw-r--r--   0 rosborn    (504) 660979062     9860 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/SOURCES.txt
+-rw-r--r--   0 rosborn    (504) 660979062        1 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/dependency_links.txt
+-rw-r--r--   0 rosborn    (504) 660979062       42 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/entry_points.txt
+-rw-r--r--   0 rosborn    (504) 660979062       47 2017-06-13 21:39:09.000000 NeXpy-1.0.4/src/NeXpy.egg-info/pbr.json
+-rw-r--r--   0 rosborn    (504) 660979062      251 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/requires.txt
+-rw-r--r--   0 rosborn    (504) 660979062        6 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/NeXpy.egg-info/top_level.txt
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.911346 NeXpy-1.0.4/src/nexpy/
+-rw-r--r--   0 rosborn    (504) 660979062      395 2023-04-15 19:28:11.000000 NeXpy-1.0.4/src/nexpy/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062      160 2023-07-05 18:50:57.000000 NeXpy-1.0.4/src/nexpy/_version.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.911687 NeXpy-1.0.4/src/nexpy/api/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.4/src/nexpy/api/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.911937 NeXpy-1.0.4/src/nexpy/api/frills/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.4/src/nexpy/api/frills/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062     8480 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/fit.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.912196 NeXpy-1.0.4/src/nexpy/api/frills/functions/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.4/src/nexpy/api/frills/functions/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.913022 NeXpy-1.0.4/src/nexpy/api/frills/models/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/models/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062     1132 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/models/bose.py
+-rw-r--r--   0 rosborn    (504) 660979062      931 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/models/critexp.py
+-rw-r--r--   0 rosborn    (504) 660979062      916 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/models/op.py
+-rw-r--r--   0 rosborn    (504) 660979062      942 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/api/frills/models/pdfdecay.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.913353 NeXpy-1.0.4/src/nexpy/definitions/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.4/src/nexpy/definitions/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.924484 NeXpy-1.0.4/src/nexpy/definitions/applications/
+-rw-r--r--   0 rosborn    (504) 660979062     6656 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXarchive.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5051 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXarpes.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    50836 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2667 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3803 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXfluo.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2774 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5070 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXiqproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5557 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXlauetof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5500 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXmonopd.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    30950 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXmx.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4469 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXrefscan.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4919 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXreftof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7147 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXsas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6974 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXsastof.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4480 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXscan.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3495 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXspe.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4547 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXsqom.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    10592 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXstxm.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7230 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5530 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6031 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofraw.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5772 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6441 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomo.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6800 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomophase.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5033 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4687 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxas.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3565 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxasproc.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7413 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxbase.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4034 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxeuler.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3899 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxkappa.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2671 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxlaue.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2066 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3632 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxnb.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3868 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/NXxrot.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     9850 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/applications/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.948900 NeXpy-1.0.4/src/nexpy/definitions/base_classes/
+-rw-r--r--   0 rosborn    (504) 660979062     2888 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3553 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6264 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3029 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3891 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3074 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2818 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcite.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2413 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    13934 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3997 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    16352 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdata.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    26917 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4068 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6385 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5447 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     8063 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXentry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2293 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5023 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3254 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6816 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3093 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3493 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3299 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3949 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     7713 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXguide.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3606 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3459 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5749 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXlog.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6041 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3284 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5290 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3398 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2853 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXnote.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     1397 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXobject.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4413 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3058 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2196 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6173 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2499 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2419 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3770 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2847 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    20356 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     4090 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXroot.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    14403 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsample.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6404 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     5297 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3723 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXshape.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2740 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXslit.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6942 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsource.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     6964 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     8599 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2993 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXuser.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3107 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3830 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     8463 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/base_classes/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.954706 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/
+-rw-r--r--   0 rosborn    (504) 660979062     6935 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2862 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    10240 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2498 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2506 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     3113 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2143 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2725 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    13513 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    14352 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2137 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     1896 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062    15240 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml
+-rw-r--r--   0 rosborn    (504) 660979062     2719 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml
+-rwxr-xr-x   0 rosborn    (504) 660979062     9805 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.956374 NeXpy-1.0.4/src/nexpy/examples/
+-rw-r--r--   0 rosborn    (504) 660979062      615 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/README.rst
+-rw-r--r--   0 rosborn    (504) 660979062   382712 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/chopper.nxs
+-rw-r--r--   0 rosborn    (504) 660979062    53690 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/example.nxs
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.956894 NeXpy-1.0.4/src/nexpy/examples/plugins/
+-rw-r--r--   0 rosborn    (504) 660979062     2026 2023-04-17 14:57:59.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/README.rst
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.957300 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.959554 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/
+-rw-r--r--   0 rosborn    (504) 660979062      244 2023-04-17 14:57:59.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062      711 2016-08-04 20:27:34.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc
+-rw-r--r--   0 rosborn    (504) 660979062     4263 2023-04-17 14:57:59.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py
+-rw-r--r--   0 rosborn    (504) 660979062     6571 2016-08-04 20:27:34.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc
+-rw-r--r--   0 rosborn    (504) 660979062     2383 2023-04-17 14:57:59.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py
+-rw-r--r--   0 rosborn    (504) 660979062     3888 2016-08-04 20:27:34.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc
+-rw-r--r--   0 rosborn    (504) 660979062      255 2023-04-17 14:57:59.000000 NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/pyproject.toml
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.960974 NeXpy-1.0.4/src/nexpy/examples/scripts/
+-rw-r--r--   0 rosborn    (504) 660979062      634 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/scripts/README.rst
+-rw-r--r--   0 rosborn    (504) 660979062      235 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/scripts/chopper_plot.py
+-rw-r--r--   0 rosborn    (504) 660979062      203 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/examples/scripts/example.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.965011 NeXpy-1.0.4/src/nexpy/gui/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:46.000000 NeXpy-1.0.4/src/nexpy/gui/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062    14081 2023-04-17 15:50:34.000000 NeXpy-1.0.4/src/nexpy/gui/consoleapp.py
+-rw-r--r--   0 rosborn    (504) 660979062   177367 2023-07-05 18:40:45.000000 NeXpy-1.0.4/src/nexpy/gui/datadialogs.py
+-rwxr-xr-x   0 rosborn    (504) 660979062    55605 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/fitdialogs.py
+-rw-r--r--   0 rosborn    (504) 660979062     1283 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/importdialog.py
+-rw-r--r--   0 rosborn    (504) 660979062    92974 2023-04-17 16:33:37.000000 NeXpy-1.0.4/src/nexpy/gui/mainwindow.py
+-rw-r--r--   0 rosborn    (504) 660979062   150779 2023-06-22 14:25:41.000000 NeXpy-1.0.4/src/nexpy/gui/plotview.py
+-rw-r--r--   0 rosborn    (504) 660979062     1201 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/pyqt.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.974262 NeXpy-1.0.4/src/nexpy/gui/resources/
+-rw-r--r--   0 rosborn    (504) 660979062     1465 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/back.png
+-rw-r--r--   0 rosborn    (504) 660979062      401 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/backward-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      905 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/resources/customize.png
+-rw-r--r--   0 rosborn    (504) 660979062      514 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/equal.png
+-rw-r--r--   0 rosborn    (504) 660979062    37268 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/resources/export-data.png
+-rw-r--r--   0 rosborn    (504) 660979062    43660 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/resources/export-figure.png
+-rw-r--r--   0 rosborn    (504) 660979062     1121 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/filesave.png
+-rw-r--r--   0 rosborn    (504) 660979062      410 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/forward-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1462 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/forward.png
+-rw-r--r--   0 rosborn    (504) 660979062      979 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/hand.png
+-rw-r--r--   0 rosborn    (504) 660979062     1338 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/home.png
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.975290 NeXpy-1.0.4/src/nexpy/gui/resources/icon/
+-rw-r--r--   0 rosborn    (504) 660979062    95378 2023-05-05 16:48:33.000000 NeXpy-1.0.4/src/nexpy/gui/resources/icon/NeXpy.png
+-rw-r--r--   0 rosborn    (504) 660979062   127292 2023-05-05 16:48:36.000000 NeXpy-1.0.4/src/nexpy/gui/resources/icon/NeXpy.svg
+-rw-r--r--   0 rosborn    (504) 660979062      613 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/link-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      241 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/lock-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1439 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/resources/lock-red-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062      713 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/move.png
+-rw-r--r--   0 rosborn    (504) 660979062      290 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/pause-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1617 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/refresh-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     2713 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/subplots.png
+-rw-r--r--   0 rosborn    (504) 660979062      258 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/unlock-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1415 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/resources/unlock-red-icon.png
+-rw-r--r--   0 rosborn    (504) 660979062     1233 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/gui/resources/zoom_to_rect.png
+-rw-r--r--   0 rosborn    (504) 660979062     8546 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/scripteditor.py
+-rw-r--r--   0 rosborn    (504) 660979062    23691 2023-06-27 03:30:10.000000 NeXpy-1.0.4/src/nexpy/gui/treeview.py
+-rw-r--r--   0 rosborn    (504) 660979062    28172 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/gui/utils.py
+-rw-r--r--   0 rosborn    (504) 660979062    43131 2023-06-29 22:03:16.000000 NeXpy-1.0.4/src/nexpy/gui/widgets.py
+-rwxr-xr-x   0 rosborn    (504) 660979062     1281 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/nexpygui.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.976035 NeXpy-1.0.4/src/nexpy/plugins/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/plugins/__init__.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.976946 NeXpy-1.0.4/src/nexpy/readers/
+-rw-r--r--   0 rosborn    (504) 660979062        0 2022-11-15 16:30:47.000000 NeXpy-1.0.4/src/nexpy/readers/__init__.py
+-rw-r--r--   0 rosborn    (504) 660979062    15851 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/readers/readspec.py
+-rw-r--r--   0 rosborn    (504) 660979062    10515 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/readers/readstack.py
+-rw-r--r--   0 rosborn    (504) 660979062     1409 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/readers/readtiff.py
+-rw-r--r--   0 rosborn    (504) 660979062     9571 2023-04-15 18:57:56.000000 NeXpy-1.0.4/src/nexpy/readers/readtxt.py
+drwxr-xr-x   0 rosborn    (504) 660979062        0 2023-07-05 18:50:57.977124 NeXpy-1.0.4/tests/
+-rw-r--r--   0 rosborn    (504) 660979062      997 2023-04-15 18:57:56.000000 NeXpy-1.0.4/tests/test_imports.py
```

### Comparing `NeXpy-1.0.3/.gitattributes` & `NeXpy-1.0.4/.gitattributes`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/.github/workflows/ci.yml` & `NeXpy-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/.gitignore` & `NeXpy-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/COPYING` & `NeXpy-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/PKG-INFO` & `NeXpy-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeXpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python GUI to analyze NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexpy
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `NeXpy-1.0.3/README.md` & `NeXpy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/README.rst` & `NeXpy-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/conda-recipe/meta.yaml` & `NeXpy-1.0.4/conda-recipe/meta.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 package:
   name: nexpy
-  version: "1.0.3"
+  version: "1.0.4"
 
 source:
   git_url: https://github.com/nexpy/nexpy.git
-  git_tag: v1.0.3
+  git_tag: v1.0.4
 
 build:
   entry_points:
     - nexpy = nexpy.nexpygui:main
   number: 0
   noarch: generic
 
@@ -16,21 +16,21 @@
   build:
     - python >=3.7
     - setuptools
     - setuptools_scm
 
   run:
     - python >=3.7
-    - nexusformat >=1.0.0
+    - nexusformat >=1.0.2
     - numpy
     - scipy
     - h5py
     - qtpy
     - ipython
-    - qtconsole
+    - qtconsole >= 5.4.3
     - ipykernel >=6.15.2
     - matplotlib
     - lmfit >=1.0.3
     - ansi2html
     - pylatexenc
     - pillow
```

### Comparing `NeXpy-1.0.3/doc/Makefile` & `NeXpy-1.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/make.bat` & `NeXpy-1.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/conf.py` & `NeXpy-1.0.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/examples.rst` & `NeXpy-1.0.4/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/favicon.ico` & `NeXpy-1.0.4/doc/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/axis-limits-bar.png` & `NeXpy-1.0.4/doc/source/images/axis-limits-bar.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/customize-panel.png` & `NeXpy-1.0.4/doc/source/images/customize-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/limits-panel.png` & `NeXpy-1.0.4/doc/source/images/limits-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/nexpy-fits.png` & `NeXpy-1.0.4/doc/source/images/nexpy-fits.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/nexpy-gui.png` & `NeXpy-1.0.4/doc/source/images/nexpy-gui.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/nexpy-logo.png` & `NeXpy-1.0.4/doc/source/images/nexpy-logo.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/options-tab.png` & `NeXpy-1.0.4/doc/source/images/options-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/projection-panel.png` & `NeXpy-1.0.4/doc/source/images/projection-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/projection-tab.png` & `NeXpy-1.0.4/doc/source/images/projection-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/scan-panel.png` & `NeXpy-1.0.4/doc/source/images/scan-panel.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/signal-tab.png` & `NeXpy-1.0.4/doc/source/images/signal-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/simple-plot.png` & `NeXpy-1.0.4/doc/source/images/simple-plot.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/skewed-axis.png` & `NeXpy-1.0.4/doc/source/images/skewed-axis.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/x-tab.png` & `NeXpy-1.0.4/doc/source/images/x-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/y-tab.png` & `NeXpy-1.0.4/doc/source/images/y-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/z-tab.png` & `NeXpy-1.0.4/doc/source/images/z-tab.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/images/z-toolbar.png` & `NeXpy-1.0.4/doc/source/images/z-toolbar.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/index.rst` & `NeXpy-1.0.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/pythongui.rst` & `NeXpy-1.0.4/doc/source/pythongui.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/pythonshell.rst` & `NeXpy-1.0.4/doc/source/pythonshell.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/doc/source/readers.rst` & `NeXpy-1.0.4/doc/source/readers.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/setup.cfg` & `NeXpy-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 
 [options]
 packages = find:
 package_dir = 
 	=src
 python_requires = >=3.7
 install_requires = 
-	nexusformat >= 1.0.0
+	nexusformat >= 1.0.2
 	numpy
 	scipy
 	h5py >= 2.9
 	qtpy
-	qtconsole
+	qtconsole >= 5.4.3
 	ipython
 	ipykernel >= 6.15.2
 	matplotlib
 	lmfit >= 1.0.3
 	pylatexenc
 	ansi2html
 	pillow
```

### Comparing `NeXpy-1.0.3/src/NeXpy.egg-info/PKG-INFO` & `NeXpy-1.0.4/src/NeXpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeXpy
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python GUI to analyze NeXus data
 Home-page: https://nexpy.github.io/nexpy/
 Download-URL: https://github.com/nexpy/nexpy
 Author: Raymond Osborn
 Author-email: rayosborn@mac.com
 License: Modified BSD License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `NeXpy-1.0.3/src/NeXpy.egg-info/SOURCES.txt` & `NeXpy-1.0.4/src/NeXpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/api/frills/fit.py` & `NeXpy-1.0.4/src/nexpy/api/frills/fit.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/api/frills/models/bose.py` & `NeXpy-1.0.4/src/nexpy/api/frills/models/bose.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/api/frills/models/critexp.py` & `NeXpy-1.0.4/src/nexpy/api/frills/models/critexp.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/api/frills/models/op.py` & `NeXpy-1.0.4/src/nexpy/api/frills/models/op.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/api/frills/models/pdfdecay.py` & `NeXpy-1.0.4/src/nexpy/api/frills/models/pdfdecay.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXarchive.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXarchive.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXarpes.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXarpes.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXcanSAS.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXdirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXfluo.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXfluo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXindirecttof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXiqproc.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXiqproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXlauetof.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXlauetof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXmonopd.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXmonopd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXmx.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXmx.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXrefscan.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXrefscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXreftof.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXreftof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsas.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXsas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsastof.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXsastof.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXscan.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXscan.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXspe.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXspe.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXsqom.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXsqom.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXstxm.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXstxm.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtas.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofnpd.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofraw.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofraw.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtofsingle.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomo.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomo.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomophase.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomophase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXtomoproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxas.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxas.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxasproc.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxasproc.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxbase.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxbase.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxeuler.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxeuler.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxkappa.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxkappa.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaue.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxlaue.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxlaueplate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxnb.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxnb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/NXxrot.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/applications/NXxrot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/applications/nxdlformat.xsl` & `NeXpy-1.0.4/src/nexpy/definitions/applications/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXaperture.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXattenuator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbeam.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbeam_stop.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXbending_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcapillary.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcite.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcite.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcollection.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcollimator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcrystal.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXcylindrical_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdata.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector_group.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdetector_module.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXdisk_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXentry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXenvironment.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXevent_data.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfermi_chopper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfilter.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXflipper.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXfresnel_zone_plate.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXgeometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXgrating.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXguide.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXguide.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXinsertion_device.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXinstrument.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXlog.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXlog.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmirror.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmoderator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmonitor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXmonochromator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXnote.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXnote.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXobject.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXobject.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXoff_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXorientation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXparameters.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpdb.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpinhole.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpolarizer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXpositioner.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXprocess.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXreflections.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXroot.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXroot.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsample.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsample_component.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsensor.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXshape.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXshape.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXslit.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXslit.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsource.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsource.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXsubentry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXtransformations.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXtranslation.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXuser.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXuser.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXvelocity_selector.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/NXxraylens.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/base_classes/nxdlformat.xsl` & `NeXpy-1.0.4/src/nexpy/definitions/base_classes/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcontainer.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcsg.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXcxi_ptycho.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXelectrostatic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXmagnetic_kicker.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXquadric.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXquadrupole_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXseparator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsnsevent.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsnshisto.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsolenoid_magnet.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXsolid_geometry.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXspecdata.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/NXspin_rotator.nxdl.xml`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl` & `NeXpy-1.0.4/src/nexpy/definitions/contributed_definitions/nxdlformat.xsl`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/README.rst` & `NeXpy-1.0.4/src/nexpy/examples/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/chopper.nxs` & `NeXpy-1.0.4/src/nexpy/examples/chopper.nxs`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/example.nxs` & `NeXpy-1.0.4/src/nexpy/examples/example.nxs`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/README.rst` & `NeXpy-1.0.4/src/nexpy/examples/plugins/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc` & `NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/__init__.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py` & `NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc` & `NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/convert_qe.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py` & `NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc` & `NeXpy-1.0.4/src/nexpy/examples/plugins/chopper_plugin/chopper/get_ei.pyc`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/examples/scripts/README.rst` & `NeXpy-1.0.4/src/nexpy/examples/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/consoleapp.py` & `NeXpy-1.0.4/src/nexpy/gui/consoleapp.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/datadialogs.py` & `NeXpy-1.0.4/src/nexpy/gui/datadialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1337,18 +1337,15 @@
         self.prefix_box.textChanged.connect(self.select_prefix)
         prefix_layout = self.make_layout(NXLabel('Prefix'), self.prefix_box)
         grid = QtWidgets.QGridLayout()
         for i, f in enumerate(files):
             self.checkbox[f] = NXCheckBox(checked=True)
             grid.addWidget(NXLabel(f), i, 0)
             grid.addWidget(self.checkbox[f], i, 1)
-        scroll_widget = NXWidget()
-        scroll_widget.set_layout(grid)
-        scroll_area = NXScrollArea(scroll_widget)
-        self.set_layout(prefix_layout, scroll_area, self.close_layout())
+        self.set_layout(prefix_layout, NXScrollArea(grid), self.close_layout())
         self.prefix_box.setFocus()
 
     @property
     def files(self):
         return [f for f in self.checkbox if self.checkbox[f].isChecked()]
 
     def select_prefix(self):
@@ -1593,56 +1590,40 @@
                 pass
         self.file_box = NXDialog(parent=self)
         self.file_box.setWindowTitle('Select Files')
         self.file_box.setMinimumWidth(300)
         self.prefix_box = NXLineEdit()
         self.prefix_box.textChanged.connect(self.select_prefix)
         prefix_layout = self.make_layout(NXLabel('Prefix'), self.prefix_box)
-        self.scroll_area = NXScrollArea()
         self.files = GridParameters()
         i = 0
         for name in sorted(self.tree, key=natural_sort):
             root = self.tree[name]
             if self.data_path in root:
                 i += 1
                 if self.scan_path:
                     self.files.add(name, root[self.scan_path], name, True)
                 else:
                     self.files.add(name, i, name, True)
                     self.files[name].checkbox.stateChanged.connect(
                         self.update_files)
         self.file_grid = self.files.grid(header=('File', self.scan_header, ''))
-        self.scroll_widget = NXWidget()
-        self.scroll_widget.set_layout(self.make_layout(self.file_grid))
-        self.scroll_area.setWidget(self.scroll_widget)
+        self.scroll_area = NXScrollArea(self.make_layout(self.file_grid))
         self.file_box.set_layout(prefix_layout, self.scroll_area,
                                  self.file_box.close_layout())
         self.file_box.close_box.accepted.connect(self.choose_files)
         self.file_box.show()
 
     def select_prefix(self):
         prefix = self.prefix_box.text()
-        self.files = GridParameters()
-        i = 0
-        for name in [n for n in sorted(self.tree, key=natural_sort)
-                     if n.startswith(prefix)]:
-            root = self.tree[name]
-            if self.data_path in root:
-                i += 1
-                if self.scan_path:
-                    self.files.add(name, root[self.scan_path], name, True)
-                else:
-                    self.files.add(name, i, name, True)
-                    self.files[name].checkbox.stateChanged.connect(
-                        self.update_files)
-        self.file_grid = self.files.grid(header=('File', self.scan_header, ''))
-        self.scroll_widget.deleteLater()
-        self.scroll_widget = NXWidget()
-        self.scroll_widget.set_layout(self.make_layout(self.file_grid))
-        self.scroll_area.setWidget(self.scroll_widget)
+        for f in self.files:
+            if f.startswith(prefix):
+                self.files[f].checkbox.setChecked(True)
+            else:
+                self.files[f].checkbox.setChecked(False)
 
     def update_files(self):
         if self.scan_variable is None:
             i = 0
             for f in self.files:
                 if self.files[f].vary:
                     i += 1
```

### Comparing `NeXpy-1.0.3/src/nexpy/gui/fitdialogs.py` & `NeXpy-1.0.4/src/nexpy/gui/fitdialogs.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/importdialog.py` & `NeXpy-1.0.4/src/nexpy/gui/importdialog.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/mainwindow.py` & `NeXpy-1.0.4/src/nexpy/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/plotview.py` & `NeXpy-1.0.4/src/nexpy/gui/plotview.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/pyqt.py` & `NeXpy-1.0.4/src/nexpy/gui/pyqt.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/back.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/back.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/customize.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/customize.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/equal.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/equal.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/export-data.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/export-data.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/export-figure.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/export-figure.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/filesave.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/filesave.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/forward.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/forward.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/hand.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/hand.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/home.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/home.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/icon/NeXpy.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/icon/NeXpy.svg` & `NeXpy-1.0.4/src/nexpy/gui/resources/icon/NeXpy.svg`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/link-icon.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/link-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/lock-red-icon.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/lock-red-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/move.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/move.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/refresh-icon.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/refresh-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/subplots.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/subplots.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/unlock-red-icon.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/unlock-red-icon.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/resources/zoom_to_rect.png` & `NeXpy-1.0.4/src/nexpy/gui/resources/zoom_to_rect.png`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/scripteditor.py` & `NeXpy-1.0.4/src/nexpy/gui/scripteditor.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/treeview.py` & `NeXpy-1.0.4/src/nexpy/gui/treeview.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     def update(self):
         super().update()
 
     def selection_changed(self):
         """Enable and disable menu actions based on the selection."""
         self.mainwindow.savefile_action.setEnabled(False)
         self.mainwindow.duplicate_action.setEnabled(False)
+        self.mainwindow.reload_action.setEnabled(False)
         self.mainwindow.remove_action.setEnabled(False)
         self.mainwindow.lockfile_action.setEnabled(False)
         self.mainwindow.unlockfile_action.setEnabled(False)
         self.mainwindow.backup_action.setEnabled(False)
         self.mainwindow.restore_backup_action.setEnabled(False)
         self.mainwindow.plot_data_action.setEnabled(False)
         self.mainwindow.plot_line_action.setEnabled(False)
@@ -337,32 +338,31 @@
         self.mainwindow.default_action.setEnabled(False)
         self.mainwindow.fit_action.setEnabled(False)
         try:
             node = self.get_node()
         except Exception:
             node = None
         if node is None:
-            self.mainwindow.reload_action.setEnabled(False)
             self.mainwindow.reload_all_action.setEnabled(False)
             self.mainwindow.remove_all_action.setEnabled(False)
             self.mainwindow.collapse_action.setEnabled(False)
             self.mainwindow.view_action.setEnabled(False)
             return
         else:
-            self.mainwindow.reload_action.setEnabled(True)
             self.mainwindow.reload_all_action.setEnabled(True)
             self.mainwindow.remove_all_action.setEnabled(True)
             self.mainwindow.collapse_action.setEnabled(True)
             self.mainwindow.view_action.setEnabled(True)
             if node.nxgroup.is_modifiable():
                 self.mainwindow.rename_action.setEnabled(True)
             if node.is_modifiable() and not isinstance(node, NXlink):
                 self.mainwindow.add_action.setEnabled(True)
         if isinstance(node, NXroot):
             self.mainwindow.savefile_action.setEnabled(True)
+            self.mainwindow.reload_action.setEnabled(True)
             self.mainwindow.remove_action.setEnabled(True)
             if node.nxfilemode:
                 self.mainwindow.duplicate_action.setEnabled(True)
                 if node.nxfilemode == 'r':
                     self.mainwindow.unlockfile_action.setEnabled(True)
                 else:
                     self.mainwindow.lockfile_action.setEnabled(True)
@@ -465,16 +465,18 @@
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.fit_action)
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.signal_action)
         self.addMenu(self.mainwindow.default_action)
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.reload_action)
+        self.addMenu(self.mainwindow.reload_all_action)
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.remove_action)
+        self.addMenu(self.mainwindow.remove_all_action)
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.unlockfile_action)
         self.addMenu(self.mainwindow.lockfile_action)
         self.menu.addSeparator()
         self.addMenu(self.mainwindow.savefile_action)
         self.addMenu(self.mainwindow.duplicate_action)
         self.addMenu(self.mainwindow.export_action)
```

### Comparing `NeXpy-1.0.3/src/nexpy/gui/utils.py` & `NeXpy-1.0.4/src/nexpy/gui/utils.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/gui/widgets.py` & `NeXpy-1.0.4/src/nexpy/gui/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 A set of customized widgets both for dialogs and plot objects.
 """
 import math
 import warnings
 
 import numpy as np
-from matplotlib import cbook, colors
+from matplotlib import colors
 from matplotlib.patches import Ellipse, Polygon, Rectangle
 
 from .pyqt import QtCore, QtGui, QtWidgets
 from .utils import (boundaries, find_nearest, format_float, get_color,
                     natural_sort, report_error)
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
@@ -96,34 +96,43 @@
         except Exception:
             return True
 
 
 class NXScrollArea(QtWidgets.QScrollArea):
     """Scroll area embedding a widget."""
 
-    def __init__(self, widget=None, horizontal=False, parent=None):
+    def __init__(self, content=None, horizontal=False, parent=None):
         """Initialize the scroll area.
 
         Parameters
         ----------
-        widget : QtWidgets.QWidget
-            Widget contained within the scroll area.
+        content : QtWidgets.QWidget or QtWidgets.QLayout
+            Widget or layout to be contained within the scroll area.
         horizontal : bool
             True if a horizontal scroll bar is enabled, default False.
         """
         super().__init__(parent=parent)
-        if widget:
-            self.setWidget(widget)
+        if content:
+            if isinstance(content, QtWidgets.QWidget):
+                self.setWidget(content)
+            elif isinstance(content, QtWidgets.QLayout):
+                widget = QtWidgets.QWidget()
+                widget.setLayout(content)
+                self.setWidget(widget)
         if not horizontal:
             self.setHorizontalScrollBarPolicy(QtCore.Qt.ScrollBarAlwaysOff)
         self.setWidgetResizable(True)
         self.setSizePolicy(QtWidgets.QSizePolicy.Expanding,
                            QtWidgets.QSizePolicy.Expanding)
 
     def setWidget(self, widget):
+        if isinstance(widget, QtWidgets.QLayout):
+            w = QtWidgets.QWidget()
+            w.setLayout(widget)
+            widget = w
         super().setWidget(widget)
         widget.setMinimumWidth(widget.sizeHint().width() +
                                self.verticalScrollBar().sizeHint().width())
 
 
 class NXLabel(QtWidgets.QLabel):
     """A text label.
```

### Comparing `NeXpy-1.0.3/src/nexpy/nexpygui.py` & `NeXpy-1.0.4/src/nexpy/nexpygui.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/readers/readspec.py` & `NeXpy-1.0.4/src/nexpy/readers/readspec.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/readers/readstack.py` & `NeXpy-1.0.4/src/nexpy/readers/readstack.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/readers/readtiff.py` & `NeXpy-1.0.4/src/nexpy/readers/readtiff.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/src/nexpy/readers/readtxt.py` & `NeXpy-1.0.4/src/nexpy/readers/readtxt.py`

 * *Files identical despite different names*

### Comparing `NeXpy-1.0.3/tests/test_imports.py` & `NeXpy-1.0.4/tests/test_imports.py`

 * *Files identical despite different names*

