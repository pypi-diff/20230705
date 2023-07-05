# Comparing `tmp/gpaw-23.6.0.tar.gz` & `tmp/gpaw-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpaw-23.6.0.tar", last modified: Fri Jun  9 07:55:42 2023, max compression
+gzip compressed data, was "gpaw-23.6.1.tar", last modified: Wed Jul  5 05:16:48 2023, max compression
```

## Comparing `gpaw-23.6.0.tar` & `gpaw-23.6.1.tar`

### file list

```diff
@@ -1,1213 +1,1213 @@
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.123446 gpaw-23.6.0/
--rw-r--r--   0 jensj     (1000) jensj     (1000)      108 2019-08-23 18:18:31.000000 gpaw-23.6.0/CHANGELOG.rst
--rw-r--r--   0 jensj     (1000) jensj     (1000)      220 2019-08-23 18:18:31.000000 gpaw-23.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2020-11-09 18:42:21.000000 gpaw-23.6.0/LICENSE
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      207 2020-11-09 18:42:21.000000 gpaw-23.6.0/MANIFEST.in
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3867 2023-06-09 07:55:42.123446 gpaw-23.6.0/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3045 2023-05-26 06:07:46.000000 gpaw-23.6.0/README.rst
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.751442 gpaw-23.6.0/c/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15143 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/_gpaw.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      234 2023-04-19 09:55:20.000000 gpaw-23.6.0/c/_gpaw_so.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5535 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/array.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8474 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/bc.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1451 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/bc.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    56659 2023-04-19 09:55:20.000000 gpaw-23.6.0/c/blacs.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4941 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/blas.c
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.755442 gpaw-23.6.0/c/bmgs/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      563 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/bmgs.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4288 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/bmgs/bmgs.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1003 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/cut.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      964 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/bmgs/fd.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2687 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/bmgs/interpolate.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      924 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/paste.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2095 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/bmgs/relax.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3616 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/bmgs/restrict.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6833 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/spherical_harmonics.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2098 2023-02-15 19:14:44.000000 gpaw-23.6.0/c/bmgs/spline.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4973 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/stencils.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1448 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/translate.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1399 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/bmgs/wfd.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2909 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/wrelax.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      446 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/bmgs/zero.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17980 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/constraints.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5950 2023-02-15 19:14:44.000000 gpaw-23.6.0/c/elpa.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1441 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/extensions.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      290 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/f2c.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13194 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/fd_preconditioner.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2136 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/fftw.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6021 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/lcao.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    58668 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/lfc.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4733 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/lfc.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13105 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/lfc2.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2420 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/main.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    40520 2023-06-05 15:36:49.000000 gpaw-23.6.0/c/mpi.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      232 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/mympi.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11886 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/operators.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      705 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/operators.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5521 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/plane_wave.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3084 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/plt.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5664 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/point_charges.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3913 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/spline.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      227 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/spline.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11753 2023-02-15 19:14:44.000000 gpaw-23.6.0/c/symmetry.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3850 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/tetra.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1275 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/threading.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6910 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/transformers.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      817 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/transformers.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    25373 2023-02-15 19:14:44.000000 gpaw-23.6.0/c/utilities.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1587 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/wigner_seitz.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14638 2022-05-04 08:34:37.000000 gpaw-23.6.0/c/woperators.c
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.755442 gpaw-23.6.0/c/xc/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/ensemble_gga.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7001 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/libvdwxc.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23092 2022-12-08 08:00:00.000000 gpaw-23.6.0/c/xc/libxc.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23689 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/m06l.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5026 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/pbe.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5285 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/pw91.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16506 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/revtpss.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14506 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/revtpss_c_pbe.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      716 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/rpbe.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16004 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/tpss.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6350 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/vdw.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9034 2023-05-26 06:07:46.000000 gpaw-23.6.0/c/xc/xc.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1008 2022-12-07 09:50:51.000000 gpaw-23.6.0/c/xc/xc_gpaw.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3860 2022-12-08 08:00:00.000000 gpaw-23.6.0/c/xc/xc_mgga.c
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1113 2021-03-25 20:49:04.000000 gpaw-23.6.0/c/xc/xc_mgga.h
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4501 2023-05-26 06:07:46.000000 gpaw-23.6.0/config.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.791442 gpaw-23.6.0/gpaw/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7268 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/__init__.py
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)       73 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/__main__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2137 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/ae.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2259 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/ah.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.795442 gpaw-23.6.0/gpaw/analyse/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       33 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/analyse/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3054 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/eed.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9840 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/expandyl.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6766 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/hirshfeld.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2607 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/multipole.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      531 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/analyse/observers.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3883 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/overlap.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8729 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/simple_stm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2510 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/vdwradii.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5655 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/analyse/wignerseitz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6641 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/arraydict.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.803442 gpaw-23.6.0/gpaw/atom/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/atom/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30177 2022-12-07 12:06:51.000000 gpaw-23.6.0/gpaw/atom/aeatom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    26652 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/all_electron.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4286 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/analyse_setup.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11278 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/atompaw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    24626 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/basis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9102 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/atom/check.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    52074 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/configurations.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6222 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/atom/filter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    32096 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/generator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    54079 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/atom/generator2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6975 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/atom/gpaw_basis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7773 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/gpaw_setup.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15109 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/atom/optimize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18475 2023-02-15 20:12:55.000000 gpaw-23.6.0/gpaw/atom/radialgd.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2251 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/atom/shapefunc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10610 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/band_descriptor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11232 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/basis_data.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15298 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/berryphase.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1722 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/bfield.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    21951 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/blacs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3721 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/borncharges.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5821 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/broadcast_imports.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14192 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/bztools.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    80338 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/calculator.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.803442 gpaw-23.6.0/gpaw/cdft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/cdft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    43072 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cdft/cdft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    41906 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/cdft/cdft_coupling.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.807442 gpaw-23.6.0/gpaw/cli/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/cli/__init__.py
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)     3479 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/complete.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      335 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/cli/completion.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6810 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/dos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      859 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/cli/gpw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3238 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/cli/info.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10386 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/install_data.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/main.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1669 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/python.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      832 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/cli/quick.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2282 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/run.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2089 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/cli/sbatch.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1279 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/cli/test.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3066 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/cluster.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3230 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/coding_style.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14459 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/convergence_criteria.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.811442 gpaw-23.6.0/gpaw/core/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      133 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/core/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8198 2023-06-07 08:43:09.000000 gpaw-23.6.0/gpaw/core/arrays.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13773 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/core/atom_arrays.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5334 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/core/atom_centered_functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4481 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/core/domain.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    31625 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/core/matrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23927 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/core/plane_waves.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17064 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/core/pwacf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    25915 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/core/uniform_grid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12503 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/coulomb.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.811442 gpaw-23.6.0/gpaw/data/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/data/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3270 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/data/g2_1_ref.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.811442 gpaw-23.6.0/gpaw/defects/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14325 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/defects/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7344 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/densities.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    31107 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/density.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.819442 gpaw-23.6.0/gpaw/dfpt/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3571 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17526 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/dynamicalmatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7591 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/electronphononcoupling.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      412 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/kpointcontainer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1648 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/dfpt/linearsolver.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16069 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/mixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      789 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/perturbation.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18713 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/dfpt/phononcalculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11031 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/dfpt/phononperturbation.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6709 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/dfpt/phonons.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2198 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/dfpt/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1697 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/dfpt/preconditioner.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14402 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/dfpt/responsecalculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2889 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/dfpt/scipylinearsolver.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6632 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/dfpt/sternheimeroperator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6730 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/dfpt/wavefunctions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5924 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/dipole_correction.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.823442 gpaw-23.6.0/gpaw/directmin/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2529 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    32802 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/directmin/derivatives.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    40120 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/etdm.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.823442 gpaw-23.6.0/gpaw/directmin/functional/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      543 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/functional/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5144 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/functional/ks.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.823442 gpaw-23.6.0/gpaw/directmin/lcao/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/directmin/lcao/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5397 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/lcao/directmin_lcao.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14008 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/ls_etdm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20442 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/sd_etdm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10920 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/directmin/tools.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7718 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/domain.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8537 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/dos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12693 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/dscf.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.827443 gpaw-23.6.0/gpaw/eigensolvers/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1306 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/eigensolvers/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9108 2023-05-10 10:07:50.000000 gpaw-23.6.0/gpaw/eigensolvers/cg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7528 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/eigensolvers/davidson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5626 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/eigensolvers/diagonalizerbackend.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1093 2023-05-10 10:07:08.000000 gpaw-23.6.0/gpaw/eigensolvers/direct.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9119 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/eigensolvers/eigensolver.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11500 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/eigensolvers/rmmdiis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4531 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/electrostatic_potential.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5513 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/elf.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.827443 gpaw-23.6.0/gpaw/elph/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2758 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/elph/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5382 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/elph/displacements.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    29954 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/elph/electronphonon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3172 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/elph/filter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13336 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/elph/gmatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6382 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/elph/raman_calculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5594 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/elph/raman_data.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12792 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/elph/supercell.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      283 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/entry_points.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13125 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/external.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13082 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/fd_operators.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.831442 gpaw-23.6.0/gpaw/fdtd/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       45 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/fdtd/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    42272 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/fdtd/poisson_fdtd.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23650 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/fdtd/polarizable_material.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7009 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/fdtd/potential_couplers.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10602 2023-06-07 10:43:27.000000 gpaw-23.6.0/gpaw/fftw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1134 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1212 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/fulldiag.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2256 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/gaunt.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4298 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/gauss.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.831442 gpaw-23.6.0/gpaw/gpu/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2019 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/gpu/__init__.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.835443 gpaw-23.6.0/gpaw/gpu/cpupy/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5979 2023-06-09 07:32:02.000000 gpaw-23.6.0/gpaw/gpu/cpupy/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      393 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/gpu/cpupy/cublas.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      269 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/gpu/cpupy/fft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      394 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/gpu/cpupy/linalg.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.835443 gpaw-23.6.0/gpaw/gpu/cpupyx/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      145 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/gpu/cpupyx/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1171 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/gpu/cpupyx/fft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       52 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/gpu/cpupyx/scipy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      445 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/gpu/kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3025 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/gpu/mpi.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    25447 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/grid_descriptor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30300 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      502 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/heg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6391 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/helmholtz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20096 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hgh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    28877 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/hgh_parameters.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5215 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hubbard.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.839443 gpaw-23.6.0/gpaw/hybrids/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      484 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/hybrids/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      779 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/hybrids/coulomb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10679 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hybrids/eigenvalues.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5705 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hybrids/energy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4250 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hybrids/forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3695 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/hybrids/kpts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1952 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/hybrids/paw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11796 2023-02-17 12:14:33.000000 gpaw-23.6.0/gpaw/hybrids/scf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6814 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hybrids/symmetry.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5439 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hybrids/wrapper.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3641 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/hybrids/wstc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12237 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/hyperfine.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.839443 gpaw-23.6.0/gpaw/inducedfield/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       62 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/inducedfield/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18155 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/inducedfield/inducedfield_base.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12149 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/inducedfield/inducedfield_fdtd.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5584 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/inducedfield/inducedfield_lrtddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17818 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/inducedfield/inducedfield_tddft.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.843443 gpaw-23.6.0/gpaw/io/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      425 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/io/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1814 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/io/fmf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5248 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/io/logger.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8774 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/io/old.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5947 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/io/tar.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2722 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/jellium.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    21858 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/kohnsham_layouts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2507 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/kpoint.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20028 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/kpt_descriptor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15543 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/kpt_refine.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.847443 gpaw-23.6.0/gpaw/lcao/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcao/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1846 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcao/analyse_basis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4437 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/atomic_correction.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3438 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/bsse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3205 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/lcao/dipoletransition.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5702 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/lcao/eigensolver.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14529 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/el_ph.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4430 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/generate_extended.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6879 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/generate_ngto_augmented.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    24335 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/local_orbitals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    26320 2023-04-19 09:28:43.000000 gpaw-23.6.0/gpaw/lcao/overlap.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14553 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/projected_wannier.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16108 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/pwf2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2849 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcao/scissors.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12517 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/tci.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6707 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcao/tightbinding.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    22448 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcao/tools.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.855443 gpaw-23.6.0/gpaw/lcaotddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7884 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2830 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcaotddft/densitymatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5221 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/dipolemomentwriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3411 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/energywriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6834 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcaotddft/frequencydensitymatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10288 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20869 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/ksdecomposition.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5022 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcaotddft/laser.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3976 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcaotddft/linedensity.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1360 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcaotddft/logger.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15539 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/magneticmomentwriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      791 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcaotddft/observer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17475 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcaotddft/propagators.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2953 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/qed.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3819 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/quadrupolemomentwriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1082 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lcaotddft/restartfilewriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7454 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/tcm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      789 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcaotddft/timedensitymatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4882 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/lcaotddft/utilities.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4358 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lcaotddft/wfwriter.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    38476 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/lfc.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.859443 gpaw-23.6.0/gpaw/lrtddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18559 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14534 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/apmb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6012 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/convergence.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4054 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/dielectric.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5402 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/excitation.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17749 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/excited_state.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5495 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/finite_differences.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    24104 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/kssingle.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23373 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/omega_matrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7835 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft/spectrum.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.863443 gpaw-23.6.0/gpaw/lrtddft2/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18471 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft2/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2029 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/eta.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    19705 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft2/k_matrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17699 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/lrtddft2/ks_singles.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5332 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/lr_communicators.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14800 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/lr_layouts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    25545 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/lr_response.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20849 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/lr_transitions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7014 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/lrtddft2/tools.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20791 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/matrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23237 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/matrix_descriptor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    27291 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/mixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12379 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/mom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    42428 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/mpi.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.871443 gpaw-23.6.0/gpaw/new/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2272 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18443 2023-06-09 07:52:47.000000 gpaw-23.6.0/gpaw/new/ase_interface.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6731 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/backwards_compatibility.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      884 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/basis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3154 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/brillouin.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15478 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/new/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13886 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/new/calculation.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9421 2023-06-07 15:03:23.000000 gpaw-23.6.0/gpaw/new/density.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      249 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/eigensolver.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.871443 gpaw-23.6.0/gpaw/new/fd/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/fd/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5445 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/fd/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5075 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/fd/pot_calc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8180 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/new/gpw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      184 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16929 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/new/ibzwfs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8030 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/input_parameters.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.875443 gpaw-23.6.0/gpaw/new/lcao/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/lcao/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5707 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/lcao/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1030 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/lcao/eigensolver.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7422 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/lcao/forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6500 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/lcao/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      781 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/lcao/hybrids.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6729 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/lcao/wave_functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1842 2023-06-09 07:32:02.000000 gpaw-23.6.0/gpaw/new/logger.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      535 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5558 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/pot_calc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2431 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/potential.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.875443 gpaw-23.6.0/gpaw/new/pw/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/pw/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7455 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/new/pw/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4859 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/pw/fulldiag.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4600 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/pw/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7335 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/new/pw/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7992 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/new/pw/pot_calc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4160 2023-06-07 15:02:45.000000 gpaw-23.6.0/gpaw/new/pw/stress.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.879443 gpaw-23.6.0/gpaw/new/pwfd/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/pwfd/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4924 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/pwfd/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11194 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/new/pwfd/davidson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16426 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/pwfd/wave_functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12943 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/rttddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7068 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/scf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2098 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/smearing.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1066 2023-04-19 09:28:43.000000 gpaw-23.6.0/gpaw/new/spinors.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1714 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/spinspiral.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4262 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/symmetry.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.879443 gpaw-23.6.0/gpaw/new/tb/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/new/tb/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11643 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/tb/builder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4587 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/wave_functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1087 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/new/xc.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.879443 gpaw-23.6.0/gpaw/nlopt/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/nlopt/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2936 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/nlopt/basic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3665 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/nlopt/linear.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9804 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/nlopt/matrixel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11923 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/nlopt/shg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5079 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/nlopt/shift.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    27831 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/occupations.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4794 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/output.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2532 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/overlap.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9020 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/pair_density.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20149 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/pair_overlap.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.883443 gpaw-23.6.0/gpaw/pes/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1497 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/pes/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2999 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/pes/continuum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1697 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/pes/dos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6905 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/pes/ds_beta.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3117 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/pes/state.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8951 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/pes/tddft.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.883443 gpaw-23.6.0/gpaw/point_groups/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      428 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/point_groups/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       64 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/point_groups/__main__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6343 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/point_groups/check.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3290 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/point_groups/cli.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1561 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/point_groups/group.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    62872 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/point_groups/groups.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    35010 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11434 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/poisson_extravacuum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8340 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/poisson_moment.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3562 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/preconditioner.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5660 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/projections.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10559 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/pseudopotential.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.887443 gpaw-23.6.0/gpaw/pw/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/pw/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4315 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/pw/density.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18186 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/pw/descriptor.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5731 2023-04-28 06:58:41.000000 gpaw-23.6.0/gpaw/pw/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15166 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/pw/lfc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4090 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/pw/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/py.typed
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3195 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/quiz.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.887443 gpaw-23.6.0/gpaw/raman/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/raman/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15120 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/raman/raman.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.907443 gpaw-23.6.0/gpaw/response/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      222 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    39663 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/bse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    29830 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/chi0.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8888 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/chi0_data.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20067 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/chiks.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2581 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/context.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6156 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/coulomb_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3519 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/density_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    22839 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/df.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7036 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/drude.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4158 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/dyson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5931 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/frequencies.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8039 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/fxc_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    43688 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/g0w0.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2207 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/g0w0_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1190 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/gamma_int.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5069 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/goldstone.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8267 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/groundstate.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7929 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/gw_bands.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5138 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/heisenberg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3292 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/hilbert.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7089 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/response/ibz2bz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20833 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/integrators.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6020 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/jdos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    26071 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/kspair.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    22927 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/response/localft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7116 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/matrix_elements.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6422 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/mft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    19962 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/pair.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    19157 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/pair_functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18454 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/pair_integrator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8297 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/pair_transitions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5117 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/paw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9785 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/pw_parallelization.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4785 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/q0_correction.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18279 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/qeh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15175 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/screened_interaction.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16996 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/site_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    19853 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/response/susceptibility.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    19235 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/response/symmetry.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4964 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/temp.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8391 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/response/tool.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7177 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/response/wgg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1730 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/rotation.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8623 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/scf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    57695 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/setup.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23983 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/setup_data.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.911443 gpaw-23.6.0/gpaw/solvation/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2231 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/solvation/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6429 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/solvation/calculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    35118 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/solvation/cavity.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3443 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/solvation/dielectric.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      306 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/solvation/gridmem.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10379 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/solvation/hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5718 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/solvation/interactions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11188 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/solvation/poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    51731 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/solvation/sjm.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.911443 gpaw-23.6.0/gpaw/sphere/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/sphere/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    28413 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/sphere/lebedev.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6413 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/sphere/rshe.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16072 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/spherical_harmonics.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30925 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/spinorbit.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2687 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/spline.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3441 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/stress.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    21337 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/symmetry.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.915444 gpaw-23.6.0/gpaw/tddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    21299 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/tddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11361 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/tddft/abc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6147 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/tddft/ehrenfest.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2845 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/tddft/folding.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1005 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/tddft/laser.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    45460 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/propagators.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.915444 gpaw-23.6.0/gpaw/tddft/solvers/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      508 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/solvers/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2145 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/solvers/base.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6863 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/solvers/bicgstab.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5006 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/solvers/cscg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15861 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/tddft/spectrum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30508 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/tddft/tdopers.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1691 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/tddft/units.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5086 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tddft/utils.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.939444 gpaw-23.6.0/gpaw/test/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2511 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/__init__.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.939444 gpaw-23.6.0/gpaw/test/ase_features/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/ase_features/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2432 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ase_features/autoneb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      749 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ase_features/test_ase3k.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      218 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ase_features/test_ase3k_version.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.939444 gpaw-23.6.0/gpaw/test/big/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/__init__.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.943444 gpaw-23.6.0/gpaw/test/big/dcdft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/dcdft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4167 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/big/dcdft/analyse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2903 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_fhi.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3371 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_hgh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3477 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_paw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4205 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_aims.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3870 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_gpaw_pw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2644 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/dcdft/pbe_gpaw_pw_verify.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.943444 gpaw-23.6.0/gpaw/test/big/g2_1/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6393 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/g2_1/analyse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      988 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/big/g2_1/g21gpaw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1060 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/g2_1/g21nwchem.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      171 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/big/g2_1/generate.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7169 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/big/g2_1/pbe_gpaw_nrel_plot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      131 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/big/g2_1/submit.agts.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.947444 gpaw-23.6.0/gpaw/test/big/hsk/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/hsk/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3254 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/hsk/hsk.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.947444 gpaw-23.6.0/gpaw/test/big/kpb/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      960 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/big/kpb/check.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2681 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/big/kpb/molecules.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      130 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/big/kpb/submit.agts.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.947444 gpaw-23.6.0/gpaw/test/big/setups/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/big/setups/__init__.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.947444 gpaw-23.6.0/gpaw/test/big/test_systems/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/big/test_systems/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1390 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/big/test_systems/agts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17010 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/big/test_systems/create.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30229 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/conftest.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.951444 gpaw-23.6.0/gpaw/test/corehole/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/corehole/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1768 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/corehole/si_nonortho.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1772 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/corehole/test_h2o.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1668 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/corehole/test_h2o_dks.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1191 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/corehole/test_h2o_recursion.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1336 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/corehole/test_li2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1627 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/corehole/test_si.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1228 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/crontab.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.951444 gpaw-23.6.0/gpaw/test/dscf/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/dscf/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2933 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/dscf/dscf_forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1294 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/dscf/test_dscf_lcao.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.951444 gpaw-23.6.0/gpaw/test/eigen/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/eigen/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      988 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/eigen/test_blocked_rmm_diis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      856 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/eigen/test_cg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1227 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/eigen/test_cg2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1524 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/eigen/test_davidson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      744 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/eigen/test_keep_htpsit.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.955444 gpaw-23.6.0/gpaw/test/elph/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/elph/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1746 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/elph/conftest.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2362 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/elph/test_displacements.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1525 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/elph/test_electronphonon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3077 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/elph/test_elph_li.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2287 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/elph/test_gmatrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2570 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/elph/test_gradient.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2713 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/elph/test_ramancalculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1583 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/elph/test_resonant_term.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1010 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/elph/test_supercell.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.959444 gpaw-23.6.0/gpaw/test/ext_potential/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/ext_potential/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7185 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/ext_potential/stark_shift.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1250 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_b_field.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1023 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_collection.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1536 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_constant_e_field.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1912 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_external.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2782 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_external_pw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2568 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_harmonic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3028 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_point_charge.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1128 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ext_potential/test_step.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.963444 gpaw-23.6.0/gpaw/test/exx/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/exx/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1819 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/exx/test_coarse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2551 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/exx/test_derivs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1573 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/exx/test_double_cell.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1973 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/exx/test_exx.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1730 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/exx/test_exx_scf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3865 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/exx/test_forces_ut.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1589 2023-04-26 11:01:30.000000 gpaw-23.6.0/gpaw/test/exx/test_kpts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2048 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/exx/test_unocc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      240 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/exx/test_xc.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.963444 gpaw-23.6.0/gpaw/test/fd_ops/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fd_ops/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1372 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_gd.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2838 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_gradient.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3598 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_laplace.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1205 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_nabla.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      686 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_non_periodic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1444 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fd_ops/test_transformations.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.967444 gpaw-23.6.0/gpaw/test/fdtd/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fdtd/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3591 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fdtd/test_ed.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7252 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fdtd/test_ed_inducedfield.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3423 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fdtd/test_ed_shapes.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2443 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fdtd/test_ed_wrapper.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.971444 gpaw-23.6.0/gpaw/test/fileio/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fileio/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1288 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/fileio/test_ascii_art.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1126 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_file_reference.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      447 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_idiotproof_setup.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/fileio/test_parallel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      330 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/fileio/test_read_old_gpw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1037 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/fileio/test_refine.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2333 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1785 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_restart_density.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      408 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_wfs_auto.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      654 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fileio/test_wfs_io.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      238 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/fileio/test_yaml.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12556 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/fuzz.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.975444 gpaw-23.6.0/gpaw/test/generic/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       74 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/generic/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      685 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/generic/colinear.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      940 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_2Al.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_8Si.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      402 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/generic/test_Cl_minus.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1080 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/generic/test_Cu.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1024 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/generic/test_H_force.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      748 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_IP_oxygen.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      539 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/generic/test_al_chain.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1121 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/generic/test_asym_box.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      680 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/generic/test_bulk.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2248 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/generic/test_guc_force.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1963 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_hydrogen.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      444 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/generic/test_mixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1588 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_move_across_cell.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1634 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/generic/test_proton.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3299 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_relax.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1188 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_si.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      722 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/generic/test_si_primitive.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.979444 gpaw-23.6.0/gpaw/test/gllb/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/gllb/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1885 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/gllb/test_atomic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5719 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/test/gllb/test_diamond.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      339 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gllb/test_gllbghost.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1326 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/gllb/test_metallic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1349 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/gllb/test_ne.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2169 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/gllb/test_ne_disc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3405 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/gllb/test_restart_eigenvalues.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1530 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/test/gllb/test_spin.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2597 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/gllb/test_variants.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.979444 gpaw-23.6.0/gpaw/test/gpu/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/gpu/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      403 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gpu/test_cpupy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1112 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gpu/test_matrix.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      395 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gpu/test_mpi.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      553 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gpu/test_precondition.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/gpu/test_pw.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.991444 gpaw-23.6.0/gpaw/test/lcao/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lcao/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      877 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      345 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_analyse_basis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_atomic_corrections.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1930 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_bsse.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1214 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_bulk.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1964 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_density.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3639 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/lcao/test_dipole_transition.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3851 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/lcao/test_dipole_transition2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1636 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_dos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1599 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_fd2lcao_restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      430 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_fftmixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2462 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/lcao/test_force.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3015 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_generate_ngto.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1079 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_gllb_si.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1044 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_h2o.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3498 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_kpts_many_combinations.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2122 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_largecellforce.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3516 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_complicated.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_elpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1193 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_elpa_kpts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1228 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_hamiltonian.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4873 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_parallel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5125 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_parallel_kpt.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1127 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_lcao_projections.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2209 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_local_orbitals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2460 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_pair_and_coulomb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      602 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcao/test_scissors.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.995444 gpaw-23.6.0/gpaw/test/lcaotddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3245 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3189 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/demo_tddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7836 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_circular_dichroism.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1579 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_is_xc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1695 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_rpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2286 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_vs_linearize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2296 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_laser.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3737 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1823 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft2_rpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10895 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_molecule.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2823 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_periodic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2198 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_replay.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3880 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3685 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_rremission.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2971 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lcaotddft/test_simple.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.995444 gpaw-23.6.0/gpaw/test/lfc/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lfc/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1757 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/lfc/test_derivatives.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      749 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lfc/test_lf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lfc/test_second_derivative.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.999444 gpaw-23.6.0/gpaw/test/linalg/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/linalg/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2332 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/linalg/test_blas.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      851 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/linalg/test_dot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      880 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/linalg/test_gemm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      811 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/linalg/test_gemm_complex.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      359 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/linalg/test_lapack.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      798 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/linalg/test_mmm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      962 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/linalg/test_zher.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.003445 gpaw-23.6.0/gpaw/test/lrtddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lrtddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1075 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lrtddft/d2Excdn2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1829 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/rraman.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2284 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/rraman_albrecht.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4631 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_1.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1429 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4380 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_3.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2471 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_apmb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1057 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_dielectric.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7335 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_excited_state.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2382 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_kssingles.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2827 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_kssingles_Be.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2321 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft_basics.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1576 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft_log.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2384 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_pes.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3187 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_placzek_profeta_albrecht.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      551 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_rraman.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      753 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft/test_select.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.003445 gpaw-23.6.0/gpaw/test/lrtddft2/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/lrtddft2/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2449 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft2/test_Al2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2285 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft2/test_H2O-lcao.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2299 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/lrtddft2/test_parameters.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.003445 gpaw-23.6.0/gpaw/test/maths/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/maths/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1365 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/maths/test_fftw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      913 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/maths/test_fsbt.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.007444 gpaw-23.6.0/gpaw/test/mgga/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/mgga/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1378 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/mgga/test_mgga_restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      629 2023-04-28 06:58:34.000000 gpaw-23.6.0/gpaw/test/mgga/test_mgga_sc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2293 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/mgga/test_nsc_MGGA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      717 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/mgga/test_symm.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.007444 gpaw-23.6.0/gpaw/test/mom/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/mom/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2350 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/mom/test_mom_fd_energy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1664 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/mom/test_mom_lcao_forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1506 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/mom/test_mom_lcao_smearing.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.007444 gpaw-23.6.0/gpaw/test/noncollinear/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/noncollinear/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      720 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/noncollinear/test_o2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1141 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/noncollinear/test_rad_pot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2301 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/noncollinear/test_soc.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.007444 gpaw-23.6.0/gpaw/test/ofdft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/ofdft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1400 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ofdft/test_ofdft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ofdft/test_ofdft_pbc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1321 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/ofdft/test_ofdft_scale.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.015445 gpaw-23.6.0/gpaw/test/parallel/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/parallel/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      892 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/parallel/scalapack_pdlasrt_hang.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2315 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/parallel/test_arraydict_redist.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1844 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_augment_grid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1847 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_blacsdist.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      493 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/parallel/test_compare.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1229 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/parallel/test_davidson_scalapack.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2251 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/test/parallel/test_diamond_gllb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5252 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/parallel/test_fd_parallel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5237 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/parallel/test_fd_parallel_kpt.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/parallel/test_kptpar.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1660 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/parallel/test_mpi.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2463 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_parallel_eigh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11365 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_pblas.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      126 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/parallel/test_redistribute_grid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7747 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/parallel/test_scalapack.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2096 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_scalapack_diag_simple.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1071 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/parallel/test_scalapack_mpirecv_crash.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      818 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/parallel/test_submatrix_redist.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.015445 gpaw-23.6.0/gpaw/test/pathological/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pathological/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      652 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pathological/test_LDA_unstable.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      714 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pathological/test_lcao_spos_derivative.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2219 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pathological/test_nonlocalset.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      879 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pathological/test_numpy_zdotc_graphite.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.019445 gpaw-23.6.0/gpaw/test/poisson/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/poisson/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4711 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/poisson/test_fastpoisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1746 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/poisson/test_generalizedlaue.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1289 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/poisson/test_metallic_poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1421 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/poisson/test_poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1454 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/poisson/test_poisson_asym.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5939 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/poisson/test_poisson_extravacuum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9519 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/poisson/test_poisson_moment.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3347 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/poisson/test_poisson_restart.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1379 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/poisson/test_pw_charged.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1718 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/poisson/test_screened_poisson.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.027445 gpaw-23.6.0/gpaw/test/pseudopotential/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)   114225 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pseudopotential/H_pz_hgh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    64903 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pseudopotential/H_sg15.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)   187223 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pseudopotential/O_pz_hgh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pseudopotential/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      512 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pseudopotential/test_ah.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1886 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/pseudopotential/test_atompaw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3380 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pseudopotential/test_hgh_h2o.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      985 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/pseudopotential/test_sg15_hydrogen.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2014 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pseudopotential/test_upf_h2o.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.035445 gpaw-23.6.0/gpaw/test/pw/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pw/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1781 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_augment_grids.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      554 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_bulk.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/pw/test_davidson_pw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      572 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pw/test_direct.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      311 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/pw/test_electrostatic_potential.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2922 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_expert_diag.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1608 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_fe_stress_mgga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      461 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_fftmixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1562 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_fulldiag.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      646 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_fulldiag_mgga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1883 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/pw/test_fulldiagk.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      695 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/pw/test_h.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2203 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_interpol.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1923 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_lfc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      443 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_moleculecg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2036 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/pw/test_par_strategies.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1665 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_reallfc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1105 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_si_stress.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1467 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_si_stress_mgga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1010 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/pw/test_slab.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      446 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_smallanglecell.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2099 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/pw/test_stresstest.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.035445 gpaw-23.6.0/gpaw/test/radial/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/radial/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      464 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/radial/test_integral4.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      300 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/radial/test_lebedev.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2057 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/radial/test_two_phi_plw_integrals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2207 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/radial/test_ylexpand.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5218 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/radial/test_yukawa_radial.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.039445 gpaw-23.6.0/gpaw/test/ralda/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/ralda/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1273 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/ralda/test_pbe_deriv.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      810 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/ralda/test_ralda_H2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1686 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/ralda/test_ralda_He.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      627 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/ralda/test_ralda_Ni.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.055445 gpaw-23.6.0/gpaw/test/response/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/response/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1563 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/hyd_chain_response.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4031 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_Na_EELS_RPA_tetra_point_comparison.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2920 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_WGG_GaAs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5442 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_afm_hchain_sf_gssALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2035 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_aluminum_EELS_ALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3935 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_aluminum_EELS_RPA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1889 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_au02_absorption.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2345 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_bse_MoS2_cut.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2083 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_bse_aluminum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2777 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_bse_silicon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2319 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_chi0.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1829 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_chi0_update.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    16400 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/response/test_chiks.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10702 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_cobalt_sf_gssALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3116 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_diamond_absorption.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3879 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_graphene.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3967 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_graphene_EELS.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1715 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_MoS2_cut.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      862 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_hBN_extrapolate.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      595 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_ppa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_restart_file.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3716 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_si.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1012 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_spinpol.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      880 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_too.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      700 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_gw_vertex.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6631 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_heisenberg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1072 2023-06-09 07:32:07.000000 gpaw-23.6.0/gpaw/test/response/test_hubbard.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9663 2023-05-26 12:00:52.000000 gpaw-23.6.0/gpaw/test/response/test_ibz2bz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5347 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_iron_sf_ALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7883 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/response/test_iron_sf_gssALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6000 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/response/test_jdos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9720 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_localft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9881 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_mft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4309 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_na_plasmon.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1775 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_na_plasmons.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2997 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_na_plasmons_tetrahedron.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5127 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_nicl2_sf_gssALDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4420 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/response/test_parallel_kptpair_extraction.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_parallelization.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4031 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_pdens_tool.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5524 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_qeh.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1606 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/response/test_response_band_cutoff.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3252 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_silicon_chi.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    24221 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_site_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6156 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_test_chi0_intraband.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1175 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_test_unit_sphere_area.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3512 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/test/response/test_tetra_point_smoothing.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3743 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/test/response/test_two-aluminum_chi_RPA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      453 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/response/test_two_phi_integrals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      339 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/response/test_wgg_factorization.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.055445 gpaw-23.6.0/gpaw/test/rpa/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/rpa/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      736 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/rpa/rpa_C6_He.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1683 2023-03-31 18:59:03.000000 gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_N2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1057 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Na.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      957 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Ni.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      649 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Si.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.059445 gpaw-23.6.0/gpaw/test/rsf_yukawa/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/rsf_yukawa/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2006 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/rsf_yukawa/test_lrtddft_short.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1593 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/rsf_yukawa/test_rsf_general.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1811 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/rsf_yukawa/test_rsf_ivo_sing_mg.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.059445 gpaw-23.6.0/gpaw/test/setups/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/setups/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    12594 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/setups/test_derivative_integrals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1020 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/setups/test_generator2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1580 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/setups/test_setup_basis_spec.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.059445 gpaw-23.6.0/gpaw/test/sic/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/sic/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1062 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/sic/test_nscfsic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/sic/test_scfsic_h2.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.063445 gpaw-23.6.0/gpaw/test/solvation/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/solvation/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2144 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/solvation/test_adm12.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     9957 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/solvation/test_forces.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1823 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_forces_symmetry.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1251 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/solvation/test_lrtddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      631 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_nan_radius.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      889 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_overlap.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1266 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_pbc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2740 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_pbc_pos_repeat.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4900 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/solvation/test_poisson.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1723 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/solvation/test_sfgcm06.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1753 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/solvation/test_sjm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5836 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_solvation_api.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2004 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_spinpol.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1801 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_sss09.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2359 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/solvation/test_swap_atoms.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1963 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/solvation/test_vacuum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2074 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/solvation/test_water_water.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1913 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/solvation/test_water_water_etdm_lcao.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.067445 gpaw-23.6.0/gpaw/test/spin/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/spin/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      800 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/spin/test_spinFe3plus.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1527 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/spin/test_spin_contamination.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      721 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/spin/test_spinpol.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.071445 gpaw-23.6.0/gpaw/test/symmetry/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/symmetry/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/symmetry/test_check.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1365 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1322 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations_big.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1319 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations_med.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2033 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/symmetry/test_kpoint_mapping.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      775 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/symmetry/test_symmetrize_wGG.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2981 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/symmetry/test_symmetry.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/symmetry/test_symmetry2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3597 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/symmetry/test_symmetry_ft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      658 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/symmetry/test_usesymm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1154 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/symmetry/test_usesymm2.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.071445 gpaw-23.6.0/gpaw/test/tddft/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/tddft/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1079 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/tddft/test_be_nltd_ip.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1041 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/tddft/test_ehrenfest_nacl.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2036 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/tddft/test_fxc_linearize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6204 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/tddft/test_molecule.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2510 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/tddft/test_td_na2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8220 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_AA_enthalpy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      632 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_Gauss.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      287 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/test_ae.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_aeatom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1215 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_aedensity.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_atomic_el_pot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1502 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_atoms_mismatch.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      386 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_atoms_too_close.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      744 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_broadcast_imports.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      510 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_broydenmixer.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2073 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_cluster.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      471 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_complete.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1181 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_complex.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      819 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_coreeig.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2189 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_coulomb.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2509 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_diagonalizer_backend.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3058 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_dipole.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1252 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_dipole_me.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      661 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_dipole_new.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1930 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_ds_beta.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      987 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_fermilevel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1407 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_fermisplit.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1474 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_fixdensity.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1906 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_fixdensity_mgga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      801 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_fixmom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1561 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_fixocc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      474 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_force_as_stop.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      306 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_fuzz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2818 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/test_gauss_func.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6425 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_gauss_wave.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_ibzqpt.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3239 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_inducedfield_lrtddft.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4184 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_inducedfield_td.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      725 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_initial_occs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1865 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_jellium.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1003 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_kpt.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      999 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_kpt_refine.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1059 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/test_libelpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1763 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_mpicomm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1011 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_muffintinpot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      848 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_multipoleH2O.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1465 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_multipoletest.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      582 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_negative_eigerror.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1863 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_new_calculator.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1679 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_occupations.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2606 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_overlap.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1410 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_potential.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1343 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_rattle.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2737 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_reuse_wfs.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2040 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_reuse_wfs_celldisp.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4365 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_scf_criteria.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_spectrum.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1692 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_spherical_harmonics.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      673 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/test_spinorbit_Kr.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      832 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_stdout.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1827 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_timelimit.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      663 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/test_timing.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      665 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/test_too_close.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_vdwradii.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2907 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/test_watermodel.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.075445 gpaw-23.6.0/gpaw/test/utilities/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       80 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/utilities/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      557 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/utilities/test_eed.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1899 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/utilities/test_elf.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5903 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/utilities/test_ewald.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      375 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/utilities/test_ibz2bz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3654 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/utilities/test_ldos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2849 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/utilities/test_partitioning.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2777 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/utilities/test_simple_stm.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/utilities/test_wannier_ethylene.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.079445 gpaw-23.6.0/gpaw/test/vdw/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/vdw/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      863 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/vdw/test_H_Hirshfeld.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1300 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/vdw/test_ar2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3482 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_functionals.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1815 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_h2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1075 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_mbeef.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2026 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_spin.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1475 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/vdw/test_potential.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      402 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/vdw/test_quick.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      732 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/vdw/test_quick_spin.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2362 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/vdw/test_ts09.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.087446 gpaw-23.6.0/gpaw/test/xc/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       71 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/xc/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2416 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/xc/test_XC2.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3060 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/xc/test_atomize.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2227 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_beef.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1272 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_degeneracy.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2170 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_gga_atom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3768 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_lb94.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3129 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/xc/test_lxc_xcatom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1162 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_nonselfconsistent.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1193 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_nonselfconsistentLDA.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1303 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/test/xc/test_pbe_pw91.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1473 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/xc/test_pplda.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1372 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/xc/test_pygga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1023 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_qna_band.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      971 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/xc/test_qna_force.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      971 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_qna_spinpol.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2303 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/test/xc/test_qna_stress.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      883 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_revPBE.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1120 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_revPBE_Li.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      867 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/test/xc/test_tb09.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2686 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/test/xc/test_tpss.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4064 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/xc/test_xc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1433 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/test/xc/test_xcatom.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11352 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/tetrahedron.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4741 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/transformers.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      497 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/typing.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    15727 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/unfold.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23370 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/upf.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.099446 gpaw-23.6.0/gpaw/utilities/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11235 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1203 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/utilities/bader.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8382 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/utilities/blas.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1264 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/cg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      575 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/debug.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3208 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/dipole.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    22457 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/dos.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2286 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/ekin.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3413 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/elpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4953 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/ewald.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1907 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/extend_grid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2338 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/extrapolate.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6390 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/folder.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8181 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/gauss.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11292 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/gl_quadrature.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2882 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/gpts.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7068 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/grid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    26834 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/utilities/grid_redistribute.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5612 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/hardware.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3344 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/hilbert.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3773 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/utilities/ibz2bz.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      367 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/jth.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8206 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/kspot.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5777 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/memory.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2479 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/nbrun.py
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)     7489 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/newrelease.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11728 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/partition.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3155 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/progressbar.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8653 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/ps2ae.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      593 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/pw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20394 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/utilities/scalapack.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3190 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/utilities/sic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6026 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/timelimit.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5356 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/timing.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14212 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/tools.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2029 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/utilities/urlcheck.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4155 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/utilities/watermodel.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.103446 gpaw-23.6.0/gpaw/wannier/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       74 2021-08-20 08:32:04.000000 gpaw-23.6.0/gpaw/wannier/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1974 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/wannier/edmiston_ruedenberg.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      915 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/wannier/functions.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    11579 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/wannier/overlaps.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6799 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/wannier/w90.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14076 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/wannier90.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.107446 gpaw-23.6.0/gpaw/wavefunctions/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/wavefunctions/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    14221 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/wavefunctions/arrays.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    24917 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/wavefunctions/base.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13588 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/wavefunctions/fd.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    20254 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/wavefunctions/fdpw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    44338 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/wavefunctions/lcao.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      604 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/wavefunctions/mode.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    32781 2023-05-26 12:00:48.000000 gpaw-23.6.0/gpaw/wavefunctions/pw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2945 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/wfd_operators.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    23833 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xas.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.115446 gpaw-23.6.0/gpaw/xc/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5769 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/xc/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8637 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/xc/bee.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3386 2023-03-20 20:28:10.000000 gpaw-23.6.0/gpaw/xc/functional.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    36897 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/xc/fxc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6825 2023-05-26 06:08:18.000000 gpaw-23.6.0/gpaw/xc/fxc_kernels.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17110 2023-03-20 20:28:10.000000 gpaw-23.6.0/gpaw/xc/gga.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.119446 gpaw-23.6.0/gpaw/xc/gllb/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       90 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/xc/gllb/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     6445 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/xc/gllb/c_gllbscr.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    27525 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/gllb/c_response.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1936 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/xc/gllb/c_xc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4171 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/gllb/coefficients.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1038 2021-07-05 14:53:36.000000 gpaw-23.6.0/gpaw/xc/gllb/contribution.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     5799 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/gllb/nonlocalfunctional.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3700 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/gllb/nonlocalfunctionalfactory.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    26624 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/hybrid.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2951 2023-03-20 20:28:10.000000 gpaw-23.6.0/gpaw/xc/kernel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      995 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/xc/lb94.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7376 2023-03-20 20:28:10.000000 gpaw-23.6.0/gpaw/xc/lda.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    30032 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/libvdwxc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2868 2021-12-21 11:47:26.000000 gpaw-23.6.0/gpaw/xc/libxc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    17190 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/xc/mgga.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2571 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/xc/noncollinear.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/xc/parametrizedxc.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4590 2022-05-04 08:34:37.000000 gpaw-23.6.0/gpaw/xc/pawcorrection.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     8492 2023-06-05 15:36:49.000000 gpaw-23.6.0/gpaw/xc/qna.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.119446 gpaw-23.6.0/gpaw/xc/ri/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3025 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/ri/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1551 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/ri/ribasis.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3962 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/ri/spherical_hse_kernel.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    18172 2023-05-26 06:07:47.000000 gpaw-23.6.0/gpaw/xc/rpa.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    44695 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/sic.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     4784 2021-06-14 18:26:24.000000 gpaw-23.6.0/gpaw/xc/tb09.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2348 2023-04-19 09:55:20.000000 gpaw-23.6.0/gpaw/xc/tools.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    29766 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/xc/vdw.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2704 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/yml.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     7457 2023-02-15 19:14:44.000000 gpaw-23.6.0/gpaw/zero_field_splitting.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:41.791442 gpaw-23.6.0/gpaw.egg-info/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     3867 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    31208 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/SOURCES.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/dependency_links.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       44 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/entry_points.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/requires.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       11 2023-06-09 07:55:41.000000 gpaw-23.6.0/gpaw.egg-info/top_level.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      105 2023-06-09 07:55:42.123446 gpaw-23.6.0/setup.cfg
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    13580 2023-06-05 15:36:49.000000 gpaw-23.6.0/setup.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     2317 2023-06-05 15:36:49.000000 gpaw-23.6.0/siteconfig_example.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-09 07:55:42.119446 gpaw-23.6.0/tools/
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)       73 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-analyse-basis
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)       70 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-basis
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)     7512 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-plot-parallel-timings
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)     4964 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-runscript
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)       70 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-setup
--rwxrwxr-x   0 jensj     (1000) jensj     (1000)       68 2021-03-25 20:50:34.000000 gpaw-23.6.0/tools/gpaw-upfplot
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.652473 gpaw-23.6.1/
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      108 2019-08-23 18:18:31.000000 gpaw-23.6.1/CHANGELOG.rst
+-rw-r--r--   0 jensj     (1000) jensj     (1000)      220 2019-08-23 18:18:31.000000 gpaw-23.6.1/CONTRIBUTING.rst
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2020-11-09 18:42:21.000000 gpaw-23.6.1/LICENSE
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      207 2020-11-09 18:42:21.000000 gpaw-23.6.1/MANIFEST.in
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3867 2023-07-05 05:16:48.652473 gpaw-23.6.1/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3045 2023-07-05 05:01:44.000000 gpaw-23.6.1/README.rst
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.500471 gpaw-23.6.1/c/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15143 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/_gpaw.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      234 2023-06-09 16:24:34.000000 gpaw-23.6.1/c/_gpaw_so.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5535 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/array.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8474 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/bc.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1451 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/bc.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    56659 2023-06-09 16:24:34.000000 gpaw-23.6.1/c/blacs.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4941 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/blas.c
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.500471 gpaw-23.6.1/c/bmgs/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      563 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/bmgs.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4288 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/bmgs/bmgs.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1003 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/cut.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      964 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/bmgs/fd.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2687 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/bmgs/interpolate.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      924 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/paste.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2095 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/bmgs/relax.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3616 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/bmgs/restrict.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6833 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/spherical_harmonics.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2098 2023-02-15 19:14:44.000000 gpaw-23.6.1/c/bmgs/spline.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4973 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/stencils.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1448 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/translate.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1399 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/bmgs/wfd.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2909 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/wrelax.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      446 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/bmgs/zero.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17980 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/constraints.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5950 2023-02-15 19:14:44.000000 gpaw-23.6.1/c/elpa.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1441 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/extensions.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      290 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/f2c.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13194 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/fd_preconditioner.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2136 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/fftw.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6021 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/lcao.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    58668 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/lfc.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4733 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/lfc.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13105 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/lfc2.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2420 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/main.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    40520 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/mpi.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      232 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/mympi.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11886 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/operators.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      705 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/operators.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5521 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/plane_wave.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3084 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/plt.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5664 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/point_charges.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3913 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/spline.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      227 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/spline.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11753 2023-02-15 19:14:44.000000 gpaw-23.6.1/c/symmetry.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3850 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/tetra.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1275 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/threading.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6910 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/transformers.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      817 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/transformers.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    25373 2023-02-15 19:14:44.000000 gpaw-23.6.1/c/utilities.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1587 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/wigner_seitz.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14638 2022-05-04 08:34:37.000000 gpaw-23.6.1/c/woperators.c
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.504471 gpaw-23.6.1/c/xc/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/ensemble_gga.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7001 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/libvdwxc.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23092 2022-12-08 08:00:00.000000 gpaw-23.6.1/c/xc/libxc.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23689 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/m06l.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5026 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/pbe.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5285 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/pw91.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16506 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/revtpss.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14506 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/revtpss_c_pbe.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      716 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/rpbe.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16004 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/tpss.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6350 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/vdw.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9034 2023-07-05 05:01:44.000000 gpaw-23.6.1/c/xc/xc.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1008 2022-12-07 09:50:51.000000 gpaw-23.6.1/c/xc/xc_gpaw.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3860 2022-12-08 08:00:00.000000 gpaw-23.6.1/c/xc/xc_mgga.c
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1113 2021-03-25 20:49:04.000000 gpaw-23.6.1/c/xc/xc_mgga.h
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4501 2023-07-05 05:01:44.000000 gpaw-23.6.1/config.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.520471 gpaw-23.6.1/gpaw/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7268 2023-07-05 05:04:48.000000 gpaw-23.6.1/gpaw/__init__.py
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)       73 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/__main__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2137 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/ae.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2259 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/ah.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.520471 gpaw-23.6.1/gpaw/analyse/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       33 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/analyse/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3054 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/eed.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9840 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/expandyl.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6766 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/hirshfeld.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2607 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/multipole.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      531 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/analyse/observers.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3883 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/overlap.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8729 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/simple_stm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2510 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/vdwradii.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5655 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/analyse/wignerseitz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6641 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/arraydict.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/atom/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/atom/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30177 2022-12-07 12:06:51.000000 gpaw-23.6.1/gpaw/atom/aeatom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    26644 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/atom/all_electron.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4286 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/analyse_setup.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11278 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/atompaw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    24626 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/basis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9102 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/atom/check.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    52074 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/configurations.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6222 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/atom/filter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    32092 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/atom/generator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    54082 2023-07-05 05:04:17.000000 gpaw-23.6.1/gpaw/atom/generator2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6975 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/atom/gpaw_basis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7773 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/gpaw_setup.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15109 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/atom/optimize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18475 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/atom/radialgd.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2251 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/atom/shapefunc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10610 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/band_descriptor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11232 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/basis_data.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15298 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/berryphase.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1722 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/bfield.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    21951 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/blacs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3721 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/borncharges.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5821 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/broadcast_imports.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14192 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/bztools.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    80338 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/calculator.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/cdft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/cdft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    43072 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cdft/cdft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    41906 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/cdft/cdft_coupling.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/cli/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/cli/__init__.py
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)     3479 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/complete.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      335 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/cli/completion.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6810 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/dos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      859 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/cli/gpw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3238 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/cli/info.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10386 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/install_data.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/main.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1669 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/python.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      832 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/cli/quick.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2282 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/run.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2089 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/cli/sbatch.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1279 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/cli/test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3066 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/cluster.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3230 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/coding_style.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14459 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/convergence_criteria.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/core/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      133 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/core/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8198 2023-06-28 06:27:32.000000 gpaw-23.6.1/gpaw/core/arrays.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13773 2023-06-28 06:27:32.000000 gpaw-23.6.1/gpaw/core/atom_arrays.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5334 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/core/atom_centered_functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4481 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/core/domain.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    31625 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/core/matrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23927 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/core/plane_waves.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17064 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/core/pwacf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    25915 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/core/uniform_grid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12503 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/coulomb.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/data/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/data/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3270 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/data/g2_1_ref.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.524471 gpaw-23.6.1/gpaw/defects/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14325 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/defects/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7344 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/densities.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    31107 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/density.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.532471 gpaw-23.6.1/gpaw/dfpt/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3571 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17526 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/dynamicalmatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7591 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/electronphononcoupling.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      412 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/kpointcontainer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1648 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/dfpt/linearsolver.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16069 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/mixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      789 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/perturbation.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18713 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/dfpt/phononcalculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11031 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/dfpt/phononperturbation.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6709 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/dfpt/phonons.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2198 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/dfpt/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1697 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/dfpt/preconditioner.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14402 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/dfpt/responsecalculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2889 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/dfpt/scipylinearsolver.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6632 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/dfpt/sternheimeroperator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6730 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/dfpt/wavefunctions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5924 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/dipole_correction.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.532471 gpaw-23.6.1/gpaw/directmin/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2529 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    32801 2023-07-05 05:04:17.000000 gpaw-23.6.1/gpaw/directmin/derivatives.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    40120 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/etdm.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.532471 gpaw-23.6.1/gpaw/directmin/functional/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      543 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/directmin/functional/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5144 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/functional/ks.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.532471 gpaw-23.6.1/gpaw/directmin/lcao/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/directmin/lcao/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5397 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/lcao/directmin_lcao.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14008 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/directmin/ls_etdm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20442 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/sd_etdm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10920 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/directmin/tools.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7715 2023-07-05 05:02:57.000000 gpaw-23.6.1/gpaw/domain.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8537 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/dos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12693 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/dscf.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.532471 gpaw-23.6.1/gpaw/eigensolvers/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1306 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/eigensolvers/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9108 2023-05-10 10:07:50.000000 gpaw-23.6.1/gpaw/eigensolvers/cg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7528 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/eigensolvers/davidson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5626 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/eigensolvers/diagonalizerbackend.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1093 2023-05-10 10:07:08.000000 gpaw-23.6.1/gpaw/eigensolvers/direct.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9119 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/eigensolvers/eigensolver.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11500 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/eigensolvers/rmmdiis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4531 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/electrostatic_potential.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5513 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/elf.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/elph/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2758 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5382 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/displacements.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    29954 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/electronphonon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3172 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/filter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13336 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/gmatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6382 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/raman_calculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5594 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/raman_data.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12792 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/elph/supercell.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      283 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/entry_points.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13125 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/external.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13082 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/fd_operators.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/fdtd/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       45 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/fdtd/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    42272 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/fdtd/poisson_fdtd.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23650 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/fdtd/polarizable_material.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7009 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/fdtd/potential_couplers.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10602 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/fftw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1134 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1212 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/fulldiag.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2256 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/gaunt.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4291 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/gauss.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/gpu/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2019 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/gpu/__init__.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/gpu/cpupy/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5979 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/gpu/cpupy/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      393 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/gpu/cpupy/cublas.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      269 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/gpu/cpupy/fft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      394 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/gpu/cpupy/linalg.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/gpu/cpupyx/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      145 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/gpu/cpupyx/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1171 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/gpu/cpupyx/fft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       52 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/gpu/cpupyx/scipy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      445 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/gpu/kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3025 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/gpu/mpi.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    25442 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/grid_descriptor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30300 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      502 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/heg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6391 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/helmholtz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20094 2023-07-05 05:04:31.000000 gpaw-23.6.1/gpaw/hgh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    28877 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/hgh_parameters.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5215 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hubbard.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.536471 gpaw-23.6.1/gpaw/hybrids/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      484 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/hybrids/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      779 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/hybrids/coulomb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10679 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hybrids/eigenvalues.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5705 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hybrids/energy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4250 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hybrids/forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3695 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/hybrids/kpts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1952 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/hybrids/paw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11796 2023-06-28 05:57:09.000000 gpaw-23.6.1/gpaw/hybrids/scf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6814 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hybrids/symmetry.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5439 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hybrids/wrapper.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3641 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/hybrids/wstc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12237 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/hyperfine.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.540471 gpaw-23.6.1/gpaw/inducedfield/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       62 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/inducedfield/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18155 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/inducedfield/inducedfield_base.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12149 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/inducedfield/inducedfield_fdtd.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5584 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/inducedfield/inducedfield_lrtddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17818 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/inducedfield/inducedfield_tddft.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.540471 gpaw-23.6.1/gpaw/io/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      425 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/io/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1814 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/io/fmf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5248 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/io/logger.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8774 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/io/old.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5947 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/io/tar.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2722 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/jellium.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    21858 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/kohnsham_layouts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2507 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/kpoint.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20028 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/kpt_descriptor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15543 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/kpt_refine.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.540471 gpaw-23.6.1/gpaw/lcao/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcao/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1846 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcao/analyse_basis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4437 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/atomic_correction.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3438 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/bsse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3205 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/lcao/dipoletransition.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5702 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/lcao/eigensolver.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14529 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/el_ph.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4430 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/generate_extended.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6879 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/generate_ngto_augmented.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    24335 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/local_orbitals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    26320 2023-04-19 09:28:43.000000 gpaw-23.6.1/gpaw/lcao/overlap.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14553 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/projected_wannier.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16108 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/pwf2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2849 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcao/scissors.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12517 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/tci.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6707 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcao/tightbinding.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    22448 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcao/tools.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.544472 gpaw-23.6.1/gpaw/lcaotddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7884 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/lcaotddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2830 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcaotddft/densitymatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5221 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/lcaotddft/dipolemomentwriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3411 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/energywriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6834 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcaotddft/frequencydensitymatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10288 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20869 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/ksdecomposition.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5022 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcaotddft/laser.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3976 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcaotddft/linedensity.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1360 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcaotddft/logger.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15539 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/magneticmomentwriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      791 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcaotddft/observer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17475 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcaotddft/propagators.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2953 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/qed.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3819 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/quadrupolemomentwriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1082 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lcaotddft/restartfilewriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7454 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/tcm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      789 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcaotddft/timedensitymatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4882 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/lcaotddft/utilities.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4358 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lcaotddft/wfwriter.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    38476 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/lfc.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.544472 gpaw-23.6.1/gpaw/lrtddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18559 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14534 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/apmb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6012 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/convergence.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4054 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/dielectric.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5402 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/excitation.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17749 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/excited_state.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5495 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/finite_differences.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    24104 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/kssingle.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23373 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/omega_matrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7835 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft/spectrum.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.544472 gpaw-23.6.1/gpaw/lrtddft2/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18471 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft2/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2029 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/eta.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    19708 2023-07-05 05:04:17.000000 gpaw-23.6.1/gpaw/lrtddft2/k_matrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17699 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/lrtddft2/ks_singles.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5332 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/lr_communicators.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14800 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/lr_layouts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    25545 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/lr_response.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20849 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/lr_transitions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7014 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/lrtddft2/tools.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20791 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/matrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23237 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/matrix_descriptor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    27291 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/mixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12379 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/mom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    42428 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/mpi.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.548472 gpaw-23.6.1/gpaw/new/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2272 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18055 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/new/ase_interface.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6731 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/backwards_compatibility.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      884 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/new/basis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3154 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/brillouin.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15478 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/new/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13886 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/calculation.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9421 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/new/density.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      249 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/eigensolver.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.548472 gpaw-23.6.1/gpaw/new/fd/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/fd/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5445 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/fd/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5075 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/fd/pot_calc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8180 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/gpw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      184 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16929 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/ibzwfs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8030 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/input_parameters.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.548472 gpaw-23.6.1/gpaw/new/lcao/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/lcao/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5707 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/new/lcao/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1030 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/new/lcao/eigensolver.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7422 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/lcao/forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6500 2023-07-05 05:01:24.000000 gpaw-23.6.1/gpaw/new/lcao/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      781 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/lcao/hybrids.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6729 2023-06-28 12:15:04.000000 gpaw-23.6.1/gpaw/new/lcao/wave_functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1842 2023-06-21 09:12:58.000000 gpaw-23.6.1/gpaw/new/logger.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      535 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5558 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pot_calc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2431 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/potential.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/new/pw/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/pw/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7455 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pw/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4859 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/pw/fulldiag.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4600 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/new/pw/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7335 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pw/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7992 2023-06-28 06:27:32.000000 gpaw-23.6.1/gpaw/new/pw/pot_calc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4160 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pw/stress.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/new/pwfd/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/pwfd/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4924 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pwfd/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11194 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pwfd/davidson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16426 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/pwfd/wave_functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12943 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/rttddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7068 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/scf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2098 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/smearing.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1066 2023-04-19 09:28:43.000000 gpaw-23.6.1/gpaw/new/spinors.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1714 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/spinspiral.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4262 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/symmetry.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/new/tb/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/new/tb/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11643 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/tb/builder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4587 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/wave_functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1087 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/new/xc.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/nlopt/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/nlopt/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2936 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/nlopt/basic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3665 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/nlopt/linear.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9804 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/nlopt/matrixel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11923 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/nlopt/shg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5079 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/nlopt/shift.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    27828 2023-07-05 05:02:57.000000 gpaw-23.6.1/gpaw/occupations.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4794 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/output.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2532 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/overlap.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9020 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/pair_density.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20149 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/pair_overlap.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/pes/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1497 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/pes/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2982 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/pes/continuum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1697 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/pes/dos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6905 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/pes/ds_beta.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3117 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/pes/state.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8951 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/pes/tddft.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/point_groups/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      428 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/point_groups/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       64 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/point_groups/__main__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6343 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/point_groups/check.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3290 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/point_groups/cli.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1561 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/point_groups/group.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    62872 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/point_groups/groups.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    35003 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11434 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/poisson_extravacuum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8340 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/poisson_moment.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3562 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/preconditioner.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5660 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/projections.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10559 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/pseudopotential.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/pw/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/pw/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4315 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/pw/density.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18186 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/pw/descriptor.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5731 2023-04-28 06:58:41.000000 gpaw-23.6.1/gpaw/pw/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15166 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/pw/lfc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4090 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/pw/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/py.typed
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3195 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/quiz.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.552471 gpaw-23.6.1/gpaw/raman/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/raman/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15120 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/raman/raman.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.564472 gpaw-23.6.1/gpaw/response/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      222 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    39663 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/bse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    29830 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/chi0.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8888 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/chi0_data.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20067 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/chiks.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2581 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/context.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6156 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/coulomb_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3519 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/density_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    22839 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/df.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7036 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/drude.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4158 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/dyson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5931 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/frequencies.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8039 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/fxc_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    43685 2023-07-05 05:02:57.000000 gpaw-23.6.1/gpaw/response/g0w0.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2207 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/g0w0_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1190 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/gamma_int.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5069 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/goldstone.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8267 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/groundstate.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7929 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/gw_bands.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5141 2023-07-05 05:04:17.000000 gpaw-23.6.1/gpaw/response/heisenberg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3292 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/hilbert.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7089 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/ibz2bz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20833 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/integrators.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6020 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/jdos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    26071 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/kspair.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    22927 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/localft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7116 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/matrix_elements.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6422 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/mft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    19962 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/pair.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    19157 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/pair_functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18454 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/pair_integrator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8297 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/pair_transitions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5117 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/paw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9785 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/pw_parallelization.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4785 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/q0_correction.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18279 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/qeh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15175 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/screened_interaction.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16996 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/site_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    19853 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/susceptibility.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    19235 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/symmetry.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4964 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/response/temp.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8391 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/response/tool.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7177 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/response/wgg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1730 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/rotation.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8623 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/scf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    57695 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/setup.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23983 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/setup_data.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.564472 gpaw-23.6.1/gpaw/solvation/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2231 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/solvation/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6429 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/solvation/calculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    35118 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/solvation/cavity.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3443 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/solvation/dielectric.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      306 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/solvation/gridmem.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10379 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/solvation/hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5718 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/solvation/interactions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11188 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/solvation/poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    51725 2023-07-05 05:02:57.000000 gpaw-23.6.1/gpaw/solvation/sjm.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.564472 gpaw-23.6.1/gpaw/sphere/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/sphere/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    28413 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/sphere/lebedev.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6413 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/sphere/rshe.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16072 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/spherical_harmonics.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30925 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/spinorbit.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2687 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/spline.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3441 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/stress.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    21337 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/symmetry.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.564472 gpaw-23.6.1/gpaw/tddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    21299 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/tddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11361 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/tddft/abc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6147 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/tddft/ehrenfest.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2845 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/tddft/folding.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1005 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/tddft/laser.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    45460 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/propagators.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.572472 gpaw-23.6.1/gpaw/tddft/solvers/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      508 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/solvers/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2145 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/solvers/base.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6863 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/solvers/bicgstab.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5006 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/solvers/cscg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15861 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/tddft/spectrum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30508 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/tddft/tdopers.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1691 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/tddft/units.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5086 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tddft/utils.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.576472 gpaw-23.6.1/gpaw/test/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2511 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/__init__.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.576472 gpaw-23.6.1/gpaw/test/ase_features/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/ase_features/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2432 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ase_features/autoneb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      749 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ase_features/test_ase3k.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      218 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ase_features/test_ase3k_version.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/__init__.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/dcdft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/dcdft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4167 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/big/dcdft/analyse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2903 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_fhi.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3371 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_hgh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3477 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_paw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4205 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_aims.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3870 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_gpaw_pw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2644 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/dcdft/pbe_gpaw_pw_verify.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/g2_1/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6393 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/g2_1/analyse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      988 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/big/g2_1/g21gpaw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1060 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/g2_1/g21nwchem.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      171 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/big/g2_1/generate.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7169 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/big/g2_1/pbe_gpaw_nrel_plot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      131 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/big/g2_1/submit.agts.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/hsk/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/hsk/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3254 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/hsk/hsk.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/kpb/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      960 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/big/kpb/check.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2681 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/big/kpb/molecules.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      130 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/big/kpb/submit.agts.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/setups/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/big/setups/__init__.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/big/test_systems/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/big/test_systems/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1390 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/big/test_systems/agts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17010 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/big/test_systems/create.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30229 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/conftest.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/corehole/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/corehole/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1768 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/corehole/si_nonortho.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1772 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/corehole/test_h2o.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1668 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/corehole/test_h2o_dks.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1191 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/corehole/test_h2o_recursion.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1336 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/corehole/test_li2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1627 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/corehole/test_si.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1228 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/crontab.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.580472 gpaw-23.6.1/gpaw/test/dscf/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/dscf/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2933 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/dscf/dscf_forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1294 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/dscf/test_dscf_lcao.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.588472 gpaw-23.6.1/gpaw/test/eigen/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/eigen/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      988 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/eigen/test_blocked_rmm_diis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      856 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/eigen/test_cg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1227 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/eigen/test_cg2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1524 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/eigen/test_davidson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      744 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/eigen/test_keep_htpsit.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.588472 gpaw-23.6.1/gpaw/test/elph/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/elph/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1746 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/elph/conftest.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2362 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/elph/test_displacements.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1525 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/elph/test_electronphonon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3077 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/elph/test_elph_li.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2287 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/elph/test_gmatrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2570 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/elph/test_gradient.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2713 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/elph/test_ramancalculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1583 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/elph/test_resonant_term.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1010 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/elph/test_supercell.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.588472 gpaw-23.6.1/gpaw/test/ext_potential/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/ext_potential/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7185 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/ext_potential/stark_shift.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1250 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_b_field.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1023 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_collection.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1536 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_constant_e_field.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1912 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_external.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2782 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_external_pw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2568 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_harmonic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3028 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_point_charge.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1128 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ext_potential/test_step.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.592472 gpaw-23.6.1/gpaw/test/exx/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/exx/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1819 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/exx/test_coarse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2551 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/exx/test_derivs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1573 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/exx/test_double_cell.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1973 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/exx/test_exx.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1730 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/exx/test_exx_scf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3865 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/exx/test_forces_ut.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1589 2023-04-26 11:01:30.000000 gpaw-23.6.1/gpaw/test/exx/test_kpts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2048 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/exx/test_unocc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      240 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/exx/test_xc.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.592472 gpaw-23.6.1/gpaw/test/fd_ops/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fd_ops/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1372 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_gd.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2838 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_gradient.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3598 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_laplace.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1205 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_nabla.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      686 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_non_periodic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1444 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fd_ops/test_transformations.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.592472 gpaw-23.6.1/gpaw/test/fdtd/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fdtd/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3591 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/fdtd/test_ed.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7252 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/fdtd/test_ed_inducedfield.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3423 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/fdtd/test_ed_shapes.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2443 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/fdtd/test_ed_wrapper.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.592472 gpaw-23.6.1/gpaw/test/fileio/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fileio/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1288 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/fileio/test_ascii_art.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1126 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_file_reference.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      447 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_idiotproof_setup.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/fileio/test_parallel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      330 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/fileio/test_read_old_gpw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1037 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/fileio/test_refine.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2333 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1785 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_restart_density.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      408 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_wfs_auto.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      654 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fileio/test_wfs_io.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      238 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/fileio/test_yaml.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12556 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/fuzz.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.596472 gpaw-23.6.1/gpaw/test/generic/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       74 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/generic/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      685 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/generic/colinear.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      940 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_2Al.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1617 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_8Si.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      402 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/generic/test_Cl_minus.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1080 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/generic/test_Cu.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1024 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/generic/test_H_force.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      748 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_IP_oxygen.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      539 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/generic/test_al_chain.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1121 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/generic/test_asym_box.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      680 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/generic/test_bulk.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2248 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/generic/test_guc_force.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1963 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_hydrogen.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      444 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/generic/test_mixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1588 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_move_across_cell.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1634 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/generic/test_proton.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3299 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_relax.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1188 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_si.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      722 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/generic/test_si_primitive.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.596472 gpaw-23.6.1/gpaw/test/gllb/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/gllb/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1885 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/gllb/test_atomic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5719 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/test/gllb/test_diamond.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      339 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gllb/test_gllbghost.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1326 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/gllb/test_metallic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1349 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/gllb/test_ne.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2169 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/gllb/test_ne_disc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3405 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/gllb/test_restart_eigenvalues.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1530 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/test/gllb/test_spin.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2597 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/gllb/test_variants.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.596472 gpaw-23.6.1/gpaw/test/gpu/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/gpu/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      403 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gpu/test_cpupy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1112 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gpu/test_matrix.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      395 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gpu/test_mpi.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      553 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gpu/test_precondition.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/gpu/test_pw.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.600472 gpaw-23.6.1/gpaw/test/lcao/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lcao/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      877 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      345 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_analyse_basis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_atomic_corrections.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1930 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_bsse.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1214 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_bulk.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1964 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_density.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3639 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/lcao/test_dipole_transition.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3851 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/lcao/test_dipole_transition2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1636 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_dos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1599 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_fd2lcao_restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      430 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_fftmixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2462 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/lcao/test_force.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3015 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_generate_ngto.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1079 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_gllb_si.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1044 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_h2o.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3498 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_kpts_many_combinations.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2122 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_largecellforce.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3516 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_complicated.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_elpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1193 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_elpa_kpts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1228 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_hamiltonian.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4873 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_parallel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5125 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_parallel_kpt.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1127 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_lcao_projections.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2209 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_local_orbitals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2460 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_pair_and_coulomb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      602 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcao/test_scissors.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.600472 gpaw-23.6.1/gpaw/test/lcaotddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3245 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3189 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/demo_tddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7836 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_circular_dichroism.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1579 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_is_xc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1695 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_rpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2286 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_vs_linearize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2296 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_laser.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3737 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1823 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft2_rpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10895 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_molecule.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2823 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_periodic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2198 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_replay.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3880 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3685 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_rremission.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2971 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/lcaotddft/test_simple.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.600472 gpaw-23.6.1/gpaw/test/lfc/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lfc/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1757 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/lfc/test_derivatives.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      749 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lfc/test_lf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lfc/test_second_derivative.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.604472 gpaw-23.6.1/gpaw/test/linalg/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/linalg/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2332 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/linalg/test_blas.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      851 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/linalg/test_dot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      880 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/linalg/test_gemm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      811 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/linalg/test_gemm_complex.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      359 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/linalg/test_lapack.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      798 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/linalg/test_mmm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      962 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/linalg/test_zher.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.604472 gpaw-23.6.1/gpaw/test/lrtddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lrtddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1075 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lrtddft/d2Excdn2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1829 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/rraman.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2284 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/rraman_albrecht.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4631 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_1.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1429 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4380 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_3.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2471 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_apmb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1057 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_dielectric.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7335 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_excited_state.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2382 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_kssingles.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2827 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_kssingles_Be.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2321 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1569 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft_basics.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1576 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft_log.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2384 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_pes.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3187 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_placzek_profeta_albrecht.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      551 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_rraman.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      753 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft/test_select.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.604472 gpaw-23.6.1/gpaw/test/lrtddft2/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/lrtddft2/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2449 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft2/test_Al2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2285 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft2/test_H2O-lcao.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2299 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/lrtddft2/test_parameters.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.604472 gpaw-23.6.1/gpaw/test/maths/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/maths/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1365 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/maths/test_fftw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      913 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/maths/test_fsbt.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.604472 gpaw-23.6.1/gpaw/test/mgga/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/mgga/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1378 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/mgga/test_mgga_restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      629 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/mgga/test_mgga_sc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2293 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/mgga/test_nsc_MGGA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      717 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/mgga/test_symm.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.608472 gpaw-23.6.1/gpaw/test/mom/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/mom/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2350 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/mom/test_mom_fd_energy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1664 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/mom/test_mom_lcao_forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1506 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/mom/test_mom_lcao_smearing.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.608472 gpaw-23.6.1/gpaw/test/noncollinear/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/noncollinear/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      720 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/noncollinear/test_o2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1141 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/noncollinear/test_rad_pot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2301 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/noncollinear/test_soc.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.608472 gpaw-23.6.1/gpaw/test/ofdft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/ofdft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1400 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ofdft/test_ofdft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ofdft/test_ofdft_pbc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1321 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/ofdft/test_ofdft_scale.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.608472 gpaw-23.6.1/gpaw/test/parallel/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/parallel/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      892 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/parallel/scalapack_pdlasrt_hang.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2315 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/parallel/test_arraydict_redist.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1844 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_augment_grid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1847 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_blacsdist.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      493 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/parallel/test_compare.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1229 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/parallel/test_davidson_scalapack.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2251 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/test/parallel/test_diamond_gllb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5252 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/parallel/test_fd_parallel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5237 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/parallel/test_fd_parallel_kpt.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/parallel/test_kptpar.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1660 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/parallel/test_mpi.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2463 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_parallel_eigh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11365 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_pblas.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      126 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/parallel/test_redistribute_grid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7747 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/parallel/test_scalapack.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2096 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_scalapack_diag_simple.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1071 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/parallel/test_scalapack_mpirecv_crash.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      818 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/parallel/test_submatrix_redist.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.608472 gpaw-23.6.1/gpaw/test/pathological/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pathological/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      652 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pathological/test_LDA_unstable.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      714 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pathological/test_lcao_spos_derivative.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2219 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pathological/test_nonlocalset.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      879 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pathological/test_numpy_zdotc_graphite.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.616472 gpaw-23.6.1/gpaw/test/poisson/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/poisson/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4711 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/poisson/test_fastpoisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1746 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/poisson/test_generalizedlaue.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1289 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/poisson/test_metallic_poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1421 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/poisson/test_poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1454 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/poisson/test_poisson_asym.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5939 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/poisson/test_poisson_extravacuum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9519 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/poisson/test_poisson_moment.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3347 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/poisson/test_poisson_restart.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1379 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/poisson/test_pw_charged.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1718 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/poisson/test_screened_poisson.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.616472 gpaw-23.6.1/gpaw/test/pseudopotential/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)   114225 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pseudopotential/H_pz_hgh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    64903 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pseudopotential/H_sg15.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)   187223 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pseudopotential/O_pz_hgh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pseudopotential/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      512 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pseudopotential/test_ah.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1886 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/pseudopotential/test_atompaw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3380 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pseudopotential/test_hgh_h2o.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      985 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/pseudopotential/test_sg15_hydrogen.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2014 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pseudopotential/test_upf_h2o.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.620473 gpaw-23.6.1/gpaw/test/pw/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pw/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1781 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_augment_grids.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      554 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_bulk.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/pw/test_davidson_pw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      572 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pw/test_direct.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      311 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/pw/test_electrostatic_potential.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2922 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_expert_diag.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1608 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_fe_stress_mgga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      461 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_fftmixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1562 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_fulldiag.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      646 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_fulldiag_mgga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1883 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/pw/test_fulldiagk.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      695 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/pw/test_h.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2203 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_interpol.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1923 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_lfc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      443 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_moleculecg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2036 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/pw/test_par_strategies.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1665 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_reallfc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1105 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_si_stress.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1467 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_si_stress_mgga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1010 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/pw/test_slab.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      446 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_smallanglecell.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2099 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/pw/test_stresstest.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.620473 gpaw-23.6.1/gpaw/test/radial/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/radial/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      464 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/radial/test_integral4.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      300 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/radial/test_lebedev.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2057 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/radial/test_two_phi_plw_integrals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2207 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/radial/test_ylexpand.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5218 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/radial/test_yukawa_radial.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.620473 gpaw-23.6.1/gpaw/test/ralda/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/ralda/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1273 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/ralda/test_pbe_deriv.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      810 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/ralda/test_ralda_H2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1686 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/ralda/test_ralda_He.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      627 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/ralda/test_ralda_Ni.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.632473 gpaw-23.6.1/gpaw/test/response/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/response/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1563 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/hyd_chain_response.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4031 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_Na_EELS_RPA_tetra_point_comparison.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2920 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_WGG_GaAs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5442 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_afm_hchain_sf_gssALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2035 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_aluminum_EELS_ALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3935 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_aluminum_EELS_RPA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1889 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_au02_absorption.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2345 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_bse_MoS2_cut.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2083 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_bse_aluminum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2777 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_bse_silicon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2319 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_chi0.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1829 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_chi0_update.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    16400 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_chiks.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10702 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_cobalt_sf_gssALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3116 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_diamond_absorption.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3879 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_graphene.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3967 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_graphene_EELS.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1715 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_gw_MoS2_cut.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      862 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_hBN_extrapolate.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      595 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_ppa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1274 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_restart_file.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3716 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_si.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1012 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_spinpol.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      880 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_too.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      700 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_gw_vertex.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6631 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_heisenberg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1072 2023-06-21 09:29:51.000000 gpaw-23.6.1/gpaw/test/response/test_hubbard.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9663 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_ibz2bz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5347 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_iron_sf_ALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7883 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_iron_sf_gssALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6000 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_jdos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9720 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_localft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9881 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_mft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4309 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_na_plasmon.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1775 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_na_plasmons.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2997 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_na_plasmons_tetrahedron.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5127 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_nicl2_sf_gssALDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4420 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_parallel_kptpair_extraction.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_parallelization.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4031 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_pdens_tool.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5524 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_qeh.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1606 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_response_band_cutoff.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3252 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_silicon_chi.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    24221 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_site_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6156 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/response/test_test_chi0_intraband.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1175 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_test_unit_sphere_area.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3512 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_tetra_point_smoothing.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3743 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_two-aluminum_chi_RPA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      453 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/response/test_two_phi_integrals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      339 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/response/test_wgg_factorization.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.632473 gpaw-23.6.1/gpaw/test/rpa/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/rpa/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      736 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/rpa/rpa_C6_He.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1683 2023-03-31 18:59:03.000000 gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_N2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1057 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Na.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      957 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Ni.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      649 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Si.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.632473 gpaw-23.6.1/gpaw/test/rsf_yukawa/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/rsf_yukawa/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2006 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/rsf_yukawa/test_lrtddft_short.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1593 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/rsf_yukawa/test_rsf_general.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1811 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/rsf_yukawa/test_rsf_ivo_sing_mg.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.632473 gpaw-23.6.1/gpaw/test/setups/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/setups/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    12594 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/setups/test_derivative_integrals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1020 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/setups/test_generator2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1580 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/setups/test_setup_basis_spec.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.632473 gpaw-23.6.1/gpaw/test/sic/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/sic/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1062 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/sic/test_nscfsic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/sic/test_scfsic_h2.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.636473 gpaw-23.6.1/gpaw/test/solvation/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/solvation/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2144 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/solvation/test_adm12.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     9957 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/solvation/test_forces.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1823 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_forces_symmetry.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1251 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/solvation/test_lrtddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      631 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_nan_radius.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      889 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_overlap.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1266 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_pbc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2740 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_pbc_pos_repeat.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4900 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/solvation/test_poisson.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1723 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/solvation/test_sfgcm06.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1753 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/solvation/test_sjm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5836 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_solvation_api.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2004 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_spinpol.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1801 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_sss09.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2359 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/solvation/test_swap_atoms.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1963 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/solvation/test_vacuum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2074 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/solvation/test_water_water.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1913 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/solvation/test_water_water_etdm_lcao.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.636473 gpaw-23.6.1/gpaw/test/spin/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/spin/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      800 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/spin/test_spinFe3plus.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1527 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/spin/test_spin_contamination.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      721 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/spin/test_spinpol.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.636473 gpaw-23.6.1/gpaw/test/symmetry/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/symmetry/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/symmetry/test_check.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1365 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1322 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations_big.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1319 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations_med.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2033 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/symmetry/test_kpoint_mapping.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      775 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/symmetry/test_symmetrize_wGG.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2981 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/symmetry/test_symmetry.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/symmetry/test_symmetry2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3597 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/symmetry/test_symmetry_ft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      658 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/symmetry/test_usesymm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1154 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/symmetry/test_usesymm2.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.636473 gpaw-23.6.1/gpaw/test/tddft/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/tddft/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1079 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/tddft/test_be_nltd_ip.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1041 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/tddft/test_ehrenfest_nacl.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2036 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/tddft/test_fxc_linearize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6204 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/tddft/test_molecule.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2510 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/tddft/test_td_na2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8220 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/test_AA_enthalpy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      632 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_Gauss.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      287 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_ae.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1146 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_aeatom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1215 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_aedensity.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      235 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_atomic_el_pot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1502 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_atoms_mismatch.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      386 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_atoms_too_close.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      744 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_broadcast_imports.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      510 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_broydenmixer.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2073 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_cluster.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      471 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_complete.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1181 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_complex.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      819 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_coreeig.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2189 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_coulomb.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2509 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_diagonalizer_backend.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3058 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_dipole.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1252 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_dipole_me.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      661 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_dipole_new.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1930 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_ds_beta.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      987 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_fermilevel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1407 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_fermisplit.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1474 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_fixdensity.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1906 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_fixdensity_mgga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      801 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_fixmom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1561 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_fixocc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      474 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_force_as_stop.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      306 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_fuzz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2818 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/test_gauss_func.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6425 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_gauss_wave.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      844 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_ibzqpt.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3239 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_inducedfield_lrtddft.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4184 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/test_inducedfield_td.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      725 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_initial_occs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1865 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_jellium.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1003 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/test_kpt.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      999 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_kpt_refine.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1059 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/test_libelpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1763 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_mpicomm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1011 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_muffintinpot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      848 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_multipoleH2O.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1461 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/test/test_multipoletest.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      582 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_negative_eigerror.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1863 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_new_calculator.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1679 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_occupations.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2606 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_overlap.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1410 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_potential.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1343 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_rattle.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2737 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_reuse_wfs.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2040 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_reuse_wfs_celldisp.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4365 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_scf_criteria.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      946 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_spectrum.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1692 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_spherical_harmonics.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      673 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/test_spinorbit_Kr.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      832 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_stdout.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1827 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/test_timelimit.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      663 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/test_timing.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      665 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/test_too_close.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      858 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_vdwradii.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2907 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/test_watermodel.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.636473 gpaw-23.6.1/gpaw/test/utilities/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       80 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/utilities/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      557 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/utilities/test_eed.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1899 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/utilities/test_elf.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5903 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/utilities/test_ewald.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      375 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/utilities/test_ibz2bz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3654 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/utilities/test_ldos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2849 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/utilities/test_partitioning.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2777 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/utilities/test_simple_stm.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2126 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/utilities/test_wannier_ethylene.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.640473 gpaw-23.6.1/gpaw/test/vdw/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/vdw/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      863 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/vdw/test_H_Hirshfeld.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1300 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/vdw/test_ar2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3482 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_functionals.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1815 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_h2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1075 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_mbeef.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2026 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_spin.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1475 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/vdw/test_potential.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      402 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/vdw/test_quick.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      732 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/vdw/test_quick_spin.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2362 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/vdw/test_ts09.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.640473 gpaw-23.6.1/gpaw/test/xc/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       71 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/xc/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2416 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/xc/test_XC2.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3060 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/xc/test_atomize.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2227 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_beef.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1272 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_degeneracy.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2170 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_gga_atom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3768 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_lb94.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3129 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/xc/test_lxc_xcatom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1162 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_nonselfconsistent.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1193 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_nonselfconsistentLDA.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1303 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/test/xc/test_pbe_pw91.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1473 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/xc/test_pplda.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1372 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/xc/test_pygga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1023 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_qna_band.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      971 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/xc/test_qna_force.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      971 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_qna_spinpol.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2303 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/test/xc/test_qna_stress.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      883 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_revPBE.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1120 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_revPBE_Li.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      867 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/test/xc/test_tb09.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2686 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/test/xc/test_tpss.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4064 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/xc/test_xc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1433 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/test/xc/test_xcatom.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11352 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/tetrahedron.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4737 2023-07-05 05:03:59.000000 gpaw-23.6.1/gpaw/transformers.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      497 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/typing.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    15727 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/unfold.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23370 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/upf.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.644473 gpaw-23.6.1/gpaw/utilities/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11235 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1203 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/utilities/bader.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8382 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/utilities/blas.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1264 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/cg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      575 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/debug.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3208 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/dipole.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    22457 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/dos.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2286 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/ekin.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3413 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/elpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4953 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/ewald.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1907 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/extend_grid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2338 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/extrapolate.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6390 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/folder.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8181 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/gauss.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11292 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/gl_quadrature.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2882 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/gpts.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7068 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/grid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    26834 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/utilities/grid_redistribute.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5612 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/hardware.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3344 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/hilbert.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3773 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/utilities/ibz2bz.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      367 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/jth.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8206 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/kspot.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5777 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/memory.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2479 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/nbrun.py
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)     7489 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/newrelease.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11728 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/partition.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3155 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/progressbar.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8653 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/ps2ae.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      593 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/pw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20394 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/utilities/scalapack.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3190 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/utilities/sic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6026 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/timelimit.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5356 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/timing.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14212 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/tools.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2029 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/utilities/urlcheck.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4155 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/utilities/watermodel.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.648473 gpaw-23.6.1/gpaw/wannier/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       74 2021-08-20 08:32:04.000000 gpaw-23.6.1/gpaw/wannier/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1974 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/wannier/edmiston_ruedenberg.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      915 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/wannier/functions.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    11579 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/wannier/overlaps.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6799 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/wannier/w90.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14076 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/wannier90.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.648473 gpaw-23.6.1/gpaw/wavefunctions/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        0 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/wavefunctions/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    14221 2023-05-26 06:07:47.000000 gpaw-23.6.1/gpaw/wavefunctions/arrays.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    24917 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/wavefunctions/base.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13588 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/wavefunctions/fd.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    20254 2023-05-26 12:00:48.000000 gpaw-23.6.1/gpaw/wavefunctions/fdpw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    44338 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/wavefunctions/lcao.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      604 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/wavefunctions/mode.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    32781 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/wavefunctions/pw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2945 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/wfd_operators.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    23833 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xas.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.648473 gpaw-23.6.1/gpaw/xc/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5769 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/xc/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8637 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/xc/bee.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3386 2023-03-20 20:28:10.000000 gpaw-23.6.1/gpaw/xc/functional.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    36897 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/xc/fxc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6825 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/xc/fxc_kernels.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17110 2023-03-20 20:28:10.000000 gpaw-23.6.1/gpaw/xc/gga.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.652473 gpaw-23.6.1/gpaw/xc/gllb/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       90 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/xc/gllb/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     6445 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/xc/gllb/c_gllbscr.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    27525 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/gllb/c_response.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1936 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/xc/gllb/c_xc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4171 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/gllb/coefficients.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1038 2021-07-05 14:53:36.000000 gpaw-23.6.1/gpaw/xc/gllb/contribution.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     5799 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/gllb/nonlocalfunctional.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3700 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/gllb/nonlocalfunctionalfactory.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    26624 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/hybrid.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2951 2023-03-20 20:28:10.000000 gpaw-23.6.1/gpaw/xc/kernel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      995 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/xc/lb94.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7376 2023-03-20 20:28:10.000000 gpaw-23.6.1/gpaw/xc/lda.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    30026 2023-07-05 05:02:57.000000 gpaw-23.6.1/gpaw/xc/libvdwxc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2868 2021-12-21 11:47:26.000000 gpaw-23.6.1/gpaw/xc/libxc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    17190 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/xc/mgga.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2571 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/xc/noncollinear.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1420 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/xc/parametrizedxc.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4590 2022-05-04 08:34:37.000000 gpaw-23.6.1/gpaw/xc/pawcorrection.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     8492 2023-06-21 06:37:30.000000 gpaw-23.6.1/gpaw/xc/qna.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.652473 gpaw-23.6.1/gpaw/xc/ri/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3025 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/ri/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1551 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/ri/ribasis.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3962 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/ri/spherical_hse_kernel.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    18172 2023-07-05 05:01:44.000000 gpaw-23.6.1/gpaw/xc/rpa.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    44695 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/sic.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     4784 2021-06-14 18:26:24.000000 gpaw-23.6.1/gpaw/xc/tb09.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2348 2023-06-09 16:24:34.000000 gpaw-23.6.1/gpaw/xc/tools.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    29766 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/xc/vdw.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2704 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/yml.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     7457 2023-02-15 19:14:44.000000 gpaw-23.6.1/gpaw/zero_field_splitting.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.520471 gpaw-23.6.1/gpaw.egg-info/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     3867 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    31208 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       44 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/entry_points.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      112 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/requires.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       11 2023-07-05 05:16:48.000000 gpaw-23.6.1/gpaw.egg-info/top_level.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      105 2023-07-05 05:16:48.652473 gpaw-23.6.1/setup.cfg
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    13580 2023-07-05 05:01:44.000000 gpaw-23.6.1/setup.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     2317 2023-06-09 16:24:34.000000 gpaw-23.6.1/siteconfig_example.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-07-05 05:16:48.652473 gpaw-23.6.1/tools/
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)       73 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-analyse-basis
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)       70 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-basis
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)     7512 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-plot-parallel-timings
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)     4964 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-runscript
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)       70 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-setup
+-rwxrwxr-x   0 jensj     (1000) jensj     (1000)       68 2021-03-25 20:50:34.000000 gpaw-23.6.1/tools/gpaw-upfplot
```

### Comparing `gpaw-23.6.0/LICENSE` & `gpaw-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/PKG-INFO` & `gpaw-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpaw
-Version: 23.6.0
+Version: 23.6.1
 Summary: GPAW: DFT and beyond within the projector-augmented wave method
 Home-page: https://wiki.fysik.dtu.dk/gpaw
 Maintainer: GPAW-community
 Maintainer-email: gpaw-users@listserv.fysik.dtu.dk
 License: GPLv3+
 Platform: unix
 Classifier: Development Status :: 6 - Mature
```

### Comparing `gpaw-23.6.0/README.rst` & `gpaw-23.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/_gpaw.h` & `gpaw-23.6.1/c/_gpaw.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/array.h` & `gpaw-23.6.1/c/array.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bc.c` & `gpaw-23.6.1/c/bc.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bc.h` & `gpaw-23.6.1/c/bc.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/blacs.c` & `gpaw-23.6.1/c/blacs.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/blas.c` & `gpaw-23.6.1/c/blas.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/bmgs.c` & `gpaw-23.6.1/c/bmgs/bmgs.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/bmgs.h` & `gpaw-23.6.1/c/bmgs/bmgs.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/cut.c` & `gpaw-23.6.1/c/bmgs/cut.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/fd.c` & `gpaw-23.6.1/c/bmgs/fd.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/interpolate.c` & `gpaw-23.6.1/c/bmgs/interpolate.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/paste.c` & `gpaw-23.6.1/c/bmgs/paste.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/relax.c` & `gpaw-23.6.1/c/bmgs/relax.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/restrict.c` & `gpaw-23.6.1/c/bmgs/restrict.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/spherical_harmonics.h` & `gpaw-23.6.1/c/bmgs/spherical_harmonics.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/spline.c` & `gpaw-23.6.1/c/bmgs/spline.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/stencils.c` & `gpaw-23.6.1/c/bmgs/stencils.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/translate.c` & `gpaw-23.6.1/c/bmgs/translate.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/wfd.c` & `gpaw-23.6.1/c/bmgs/wfd.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/bmgs/wrelax.c` & `gpaw-23.6.1/c/bmgs/wrelax.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/constraints.c` & `gpaw-23.6.1/c/constraints.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/elpa.c` & `gpaw-23.6.1/c/elpa.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/extensions.h` & `gpaw-23.6.1/c/extensions.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/fd_preconditioner.c` & `gpaw-23.6.1/c/fd_preconditioner.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/fftw.c` & `gpaw-23.6.1/c/fftw.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/lcao.c` & `gpaw-23.6.1/c/lcao.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/lfc.c` & `gpaw-23.6.1/c/lfc.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/lfc.h` & `gpaw-23.6.1/c/lfc.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/lfc2.c` & `gpaw-23.6.1/c/lfc2.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/main.c` & `gpaw-23.6.1/c/main.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/mpi.c` & `gpaw-23.6.1/c/mpi.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/operators.c` & `gpaw-23.6.1/c/operators.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/operators.h` & `gpaw-23.6.1/c/operators.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/plane_wave.c` & `gpaw-23.6.1/c/plane_wave.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/plt.c` & `gpaw-23.6.1/c/plt.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/point_charges.c` & `gpaw-23.6.1/c/point_charges.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/spline.c` & `gpaw-23.6.1/c/spline.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/symmetry.c` & `gpaw-23.6.1/c/symmetry.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/tetra.c` & `gpaw-23.6.1/c/tetra.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/threading.h` & `gpaw-23.6.1/c/threading.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/transformers.c` & `gpaw-23.6.1/c/transformers.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/transformers.h` & `gpaw-23.6.1/c/transformers.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/utilities.c` & `gpaw-23.6.1/c/utilities.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/wigner_seitz.c` & `gpaw-23.6.1/c/wigner_seitz.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/woperators.c` & `gpaw-23.6.1/c/woperators.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/ensemble_gga.c` & `gpaw-23.6.1/c/xc/ensemble_gga.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/libvdwxc.c` & `gpaw-23.6.1/c/xc/libvdwxc.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/libxc.c` & `gpaw-23.6.1/c/xc/libxc.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/m06l.c` & `gpaw-23.6.1/c/xc/m06l.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/pbe.c` & `gpaw-23.6.1/c/xc/pbe.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/pw91.c` & `gpaw-23.6.1/c/xc/pw91.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/revtpss.c` & `gpaw-23.6.1/c/xc/revtpss.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/revtpss_c_pbe.c` & `gpaw-23.6.1/c/xc/revtpss_c_pbe.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/rpbe.c` & `gpaw-23.6.1/c/xc/rpbe.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/tpss.c` & `gpaw-23.6.1/c/xc/tpss.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/vdw.c` & `gpaw-23.6.1/c/xc/vdw.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/xc.c` & `gpaw-23.6.1/c/xc/xc.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/xc_gpaw.h` & `gpaw-23.6.1/c/xc/xc_gpaw.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/xc_mgga.c` & `gpaw-23.6.1/c/xc/xc_mgga.c`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/c/xc/xc_mgga.h` & `gpaw-23.6.1/c/xc/xc_mgga.h`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/config.py` & `gpaw-23.6.1/config.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/__init__.py` & `gpaw-23.6.1/gpaw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """Main gpaw module."""
 import os
 import sys
 import contextlib
 from pathlib import Path
 from typing import List, Dict, Union, Any, TYPE_CHECKING
 
-__version__ = '23.6.0'
+__version__ = '23.6.1'
 __ase_version_required__ = '3.22.1'
 __all__ = ['GPAW',
            'Mixer', 'MixerSum', 'MixerDif', 'MixerSum2',
            'MixerFull',
            'CG', 'Davidson', 'RMMDIIS', 'DirectLCAO',
            'PoissonSolver',
            'FermiDirac', 'MethfesselPaxton', 'MarzariVanderbilt',
```

### Comparing `gpaw-23.6.0/gpaw/ae.py` & `gpaw-23.6.1/gpaw/ae.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/ah.py` & `gpaw-23.6.1/gpaw/ah.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/eed.py` & `gpaw-23.6.1/gpaw/analyse/eed.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/expandyl.py` & `gpaw-23.6.1/gpaw/analyse/expandyl.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/hirshfeld.py` & `gpaw-23.6.1/gpaw/analyse/hirshfeld.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/multipole.py` & `gpaw-23.6.1/gpaw/analyse/multipole.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/observers.py` & `gpaw-23.6.1/gpaw/analyse/observers.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/overlap.py` & `gpaw-23.6.1/gpaw/analyse/overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/simple_stm.py` & `gpaw-23.6.1/gpaw/analyse/simple_stm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/vdwradii.py` & `gpaw-23.6.1/gpaw/analyse/vdwradii.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/analyse/wignerseitz.py` & `gpaw-23.6.1/gpaw/analyse/wignerseitz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/arraydict.py` & `gpaw-23.6.1/gpaw/arraydict.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/aeatom.py` & `gpaw-23.6.1/gpaw/atom/aeatom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/all_electron.py` & `gpaw-23.6.1/gpaw/atom/all_electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,15 @@
 
     if scalarrel:
         x = 0.5 * alpha**2  # x = 1 / (2c^2)
         Mr = r * (1.0 + x * e) - x * vr
     else:
         Mr = r
     c0 = l * (l + 1) + 2 * Mr * (vr - e * r)
-    if gmax is None and np.alltrue(c0 > 0):
+    if gmax is None and (c0 > 0).all():
         raise ConvergenceError('Bad initial electron density guess!')
 
     c1 = c10
     if scalarrel:
         c0 += x * r2dvdr / Mr
         c1 = c10 - x * r * r2dvdr / (Mr * dr)
 
@@ -758,15 +758,15 @@
 
     if scalarrel:
         x = 0.5 * alpha**2  # x = 1 / (2c^2)
         Mr = r * (1.0 + x * e) - x * vr
     else:
         Mr = r
     c0 = l * (l + 1) + 2 * Mr * (vr - e * r)
-    if gmax is None and np.alltrue(c0 > 0):
+    if gmax is None and (c0 > 0).all():
         print("""
 Problem with initial electron density guess!  Try to run the program
 with the '-n' option (non-scalar-relativistic calculation) and then
 try again without the '-n' option (this will generate a good initial
 guess for the density).
 """)
         raise SystemExit
```

### Comparing `gpaw-23.6.0/gpaw/atom/analyse_setup.py` & `gpaw-23.6.1/gpaw/atom/analyse_setup.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/atompaw.py` & `gpaw-23.6.1/gpaw/atom/atompaw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/basis.py` & `gpaw-23.6.1/gpaw/atom/basis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/check.py` & `gpaw-23.6.1/gpaw/atom/check.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/configurations.py` & `gpaw-23.6.1/gpaw/atom/configurations.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/filter.py` & `gpaw-23.6.1/gpaw/atom/filter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/generator.py` & `gpaw-23.6.1/gpaw/atom/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
                     y = a[0] + r2 * (a[1] + r2 * (a[2] + r2 * (a[3])))
                     if 0:  # l < 2 and nodeless:
                         y = np.exp(y)
                     s[:gc] = rl1 * y
 
                 coefs.append(a)
                 if nodeless:
-                    if not np.alltrue(s[1:gc] > 0.0):
+                    if not (s[1:gc] > 0.0).all():
                         raise RuntimeError(
                             'Error: The %d%s pseudo wave has a node!' %
                             (n_ln[l][0], 'spdf'[l]))
                     # Only the first state for each l must be nodeless:
                     nodeless = False
 
         # Calculate pseudo core density:
```

### Comparing `gpaw-23.6.0/gpaw/atom/generator2.py` & `gpaw-23.6.1/gpaw/atom/generator2.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
             def spillage(alpha):
                 """Fraction of gaussian charge outside rc."""
                 x = alpha * rc**2
                 return 1 - erf(sqrt(x)) + 2 * sqrt(x / pi) * exp(-x)
 
             def f(alpha):
-                return log(spillage(alpha)) - log(eps)
+                return log(spillage(alpha[0])) - log(eps)
 
             self.alpha = fsolve(f, 7.0)[0]
 
             self.alpha = round(self.alpha, 1)
         elif alpha < 0:
             rc = min(rc)
             self.log('Shape function: (sin(pi*r/rc)/r)^2, rc={rc:.2f} Bohr'
```

### Comparing `gpaw-23.6.0/gpaw/atom/gpaw_basis.py` & `gpaw-23.6.1/gpaw/atom/gpaw_basis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/gpaw_setup.py` & `gpaw-23.6.1/gpaw/atom/gpaw_setup.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/optimize.py` & `gpaw-23.6.1/gpaw/atom/optimize.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/radialgd.py` & `gpaw-23.6.1/gpaw/atom/radialgd.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/atom/shapefunc.py` & `gpaw-23.6.1/gpaw/atom/shapefunc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/band_descriptor.py` & `gpaw-23.6.1/gpaw/band_descriptor.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/basis_data.py` & `gpaw-23.6.1/gpaw/basis_data.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/berryphase.py` & `gpaw-23.6.1/gpaw/berryphase.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/bfield.py` & `gpaw-23.6.1/gpaw/bfield.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/blacs.py` & `gpaw-23.6.1/gpaw/blacs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/borncharges.py` & `gpaw-23.6.1/gpaw/borncharges.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/broadcast_imports.py` & `gpaw-23.6.1/gpaw/broadcast_imports.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/bztools.py` & `gpaw-23.6.1/gpaw/bztools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/calculator.py` & `gpaw-23.6.1/gpaw/calculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cdft/cdft.py` & `gpaw-23.6.1/gpaw/cdft/cdft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cdft/cdft_coupling.py` & `gpaw-23.6.1/gpaw/cdft/cdft_coupling.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/complete.py` & `gpaw-23.6.1/gpaw/cli/complete.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/dos.py` & `gpaw-23.6.1/gpaw/cli/dos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/gpw.py` & `gpaw-23.6.1/gpaw/cli/gpw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/info.py` & `gpaw-23.6.1/gpaw/cli/info.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/install_data.py` & `gpaw-23.6.1/gpaw/cli/install_data.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/main.py` & `gpaw-23.6.1/gpaw/cli/main.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/python.py` & `gpaw-23.6.1/gpaw/cli/python.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/quick.py` & `gpaw-23.6.1/gpaw/cli/quick.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/run.py` & `gpaw-23.6.1/gpaw/cli/run.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/sbatch.py` & `gpaw-23.6.1/gpaw/cli/sbatch.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cli/test.py` & `gpaw-23.6.1/gpaw/cli/test.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/cluster.py` & `gpaw-23.6.1/gpaw/cluster.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/coding_style.py` & `gpaw-23.6.1/gpaw/coding_style.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/convergence_criteria.py` & `gpaw-23.6.1/gpaw/convergence_criteria.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/arrays.py` & `gpaw-23.6.1/gpaw/core/arrays.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/atom_arrays.py` & `gpaw-23.6.1/gpaw/core/atom_arrays.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/atom_centered_functions.py` & `gpaw-23.6.1/gpaw/core/atom_centered_functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/domain.py` & `gpaw-23.6.1/gpaw/core/domain.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/matrix.py` & `gpaw-23.6.1/gpaw/core/matrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/plane_waves.py` & `gpaw-23.6.1/gpaw/core/plane_waves.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/pwacf.py` & `gpaw-23.6.1/gpaw/core/pwacf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/core/uniform_grid.py` & `gpaw-23.6.1/gpaw/core/uniform_grid.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/coulomb.py` & `gpaw-23.6.1/gpaw/coulomb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/data/g2_1_ref.py` & `gpaw-23.6.1/gpaw/data/g2_1_ref.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/defects/__init__.py` & `gpaw-23.6.1/gpaw/defects/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/densities.py` & `gpaw-23.6.1/gpaw/densities.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/density.py` & `gpaw-23.6.1/gpaw/density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/__init__.py` & `gpaw-23.6.1/gpaw/dfpt/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/dynamicalmatrix.py` & `gpaw-23.6.1/gpaw/dfpt/dynamicalmatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/electronphononcoupling.py` & `gpaw-23.6.1/gpaw/dfpt/electronphononcoupling.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/linearsolver.py` & `gpaw-23.6.1/gpaw/dfpt/linearsolver.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/mixer.py` & `gpaw-23.6.1/gpaw/dfpt/mixer.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/perturbation.py` & `gpaw-23.6.1/gpaw/dfpt/perturbation.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/phononcalculator.py` & `gpaw-23.6.1/gpaw/dfpt/phononcalculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/phononperturbation.py` & `gpaw-23.6.1/gpaw/dfpt/phononperturbation.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/phonons.py` & `gpaw-23.6.1/gpaw/dfpt/phonons.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/poisson.py` & `gpaw-23.6.1/gpaw/dfpt/poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/preconditioner.py` & `gpaw-23.6.1/gpaw/dfpt/preconditioner.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/responsecalculator.py` & `gpaw-23.6.1/gpaw/dfpt/responsecalculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/scipylinearsolver.py` & `gpaw-23.6.1/gpaw/dfpt/scipylinearsolver.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/sternheimeroperator.py` & `gpaw-23.6.1/gpaw/dfpt/sternheimeroperator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dfpt/wavefunctions.py` & `gpaw-23.6.1/gpaw/dfpt/wavefunctions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dipole_correction.py` & `gpaw-23.6.1/gpaw/dipole_correction.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/__init__.py` & `gpaw-23.6.1/gpaw/directmin/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/derivatives.py` & `gpaw-23.6.1/gpaw/directmin/derivatives.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,15 +643,15 @@
         text = ''
         for i in range(self.l):
             text += '%10.6f '
         self.logger(text % tuple(self.lambda_e), flush=True)
         self.logger('\nResidual maximum components:\n', flush=True)
         self.logger(indices, flush=True)
         text = ''
-        temp = list(np.round_(deepcopy(self.error_e), 6))
+        temp = list(np.round(deepcopy(self.error_e), 6))
         for i in range(self.l):
             text += '%10s '
             temp[i] = str(temp[i])
             if self.converged_e[i]:
                 temp[i] += 'c'
         self.logger(text % tuple(temp), flush=True)
```

### Comparing `gpaw-23.6.0/gpaw/directmin/etdm.py` & `gpaw-23.6.1/gpaw/directmin/etdm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/functional/__init__.py` & `gpaw-23.6.1/gpaw/directmin/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/functional/ks.py` & `gpaw-23.6.1/gpaw/directmin/functional/ks.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/lcao/directmin_lcao.py` & `gpaw-23.6.1/gpaw/directmin/lcao/directmin_lcao.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/ls_etdm.py` & `gpaw-23.6.1/gpaw/directmin/ls_etdm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/sd_etdm.py` & `gpaw-23.6.1/gpaw/directmin/sd_etdm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/directmin/tools.py` & `gpaw-23.6.1/gpaw/directmin/tools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/domain.py` & `gpaw-23.6.1/gpaw/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             parsize_c = decompose_domain(N_c, comm.size)
         self.parsize_c = np.array(parsize_c)
 
         self.stride_c = np.array([parsize_c[1] * parsize_c[2],
                                   parsize_c[2],
                                   1])
 
-        if np.product(self.parsize_c) != self.comm.size:
+        if np.prod(self.parsize_c) != self.comm.size:
             raise RuntimeError('Bad domain decomposition! '
                                'CPU counts %s do not multiply to '
                                'communicator size %d' % (self.parsize_c,
                                                          self.comm.size))
 
         self.parpos_c = self.get_processor_position_from_rank()
         self.find_neighbor_processors()
```

### Comparing `gpaw-23.6.0/gpaw/dos.py` & `gpaw-23.6.1/gpaw/dos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/dscf.py` & `gpaw-23.6.1/gpaw/dscf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/__init__.py` & `gpaw-23.6.1/gpaw/eigensolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/cg.py` & `gpaw-23.6.1/gpaw/eigensolvers/cg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/davidson.py` & `gpaw-23.6.1/gpaw/eigensolvers/davidson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/diagonalizerbackend.py` & `gpaw-23.6.1/gpaw/eigensolvers/diagonalizerbackend.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/direct.py` & `gpaw-23.6.1/gpaw/eigensolvers/direct.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/eigensolver.py` & `gpaw-23.6.1/gpaw/eigensolvers/eigensolver.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/eigensolvers/rmmdiis.py` & `gpaw-23.6.1/gpaw/eigensolvers/rmmdiis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/electrostatic_potential.py` & `gpaw-23.6.1/gpaw/electrostatic_potential.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elf.py` & `gpaw-23.6.1/gpaw/elf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/__init__.py` & `gpaw-23.6.1/gpaw/elph/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/displacements.py` & `gpaw-23.6.1/gpaw/elph/displacements.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/electronphonon.py` & `gpaw-23.6.1/gpaw/elph/electronphonon.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/filter.py` & `gpaw-23.6.1/gpaw/elph/filter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/gmatrix.py` & `gpaw-23.6.1/gpaw/elph/gmatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/raman_calculator.py` & `gpaw-23.6.1/gpaw/elph/raman_calculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/raman_data.py` & `gpaw-23.6.1/gpaw/elph/raman_data.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/elph/supercell.py` & `gpaw-23.6.1/gpaw/elph/supercell.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/external.py` & `gpaw-23.6.1/gpaw/external.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fd_operators.py` & `gpaw-23.6.1/gpaw/fd_operators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fdtd/poisson_fdtd.py` & `gpaw-23.6.1/gpaw/fdtd/poisson_fdtd.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fdtd/polarizable_material.py` & `gpaw-23.6.1/gpaw/fdtd/polarizable_material.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fdtd/potential_couplers.py` & `gpaw-23.6.1/gpaw/fdtd/potential_couplers.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fftw.py` & `gpaw-23.6.1/gpaw/fftw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/forces.py` & `gpaw-23.6.1/gpaw/forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/fulldiag.py` & `gpaw-23.6.1/gpaw/fulldiag.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/gaunt.py` & `gpaw-23.6.1/gpaw/gaunt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/gauss.py` & `gpaw-23.6.1/gpaw/gauss.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def I1(R, ap1, b, alpha, beta, m=0):
     if ap1 == (0, 0, 0):
         if b != (0, 0, 0):
             return I1(-R, b, ap1, beta, alpha, m)
         else:
             f = 2 * np.sqrt(np.pi**5 / (alpha + beta)) / (alpha * beta)
-            if np.sometrue(R):
+            if R.any():
                 T = alpha * beta / (alpha + beta) * np.dot(R, R)
                 f1 = f * erf(T**0.5) * (np.pi / T)**0.5
                 if m == 0:
                     return 0.5 * f1
                 f2 = f * np.exp(-T) / T**m
                 if m == 1:
                     return 0.25 * f1 / T - 0.5 * f2
```

### Comparing `gpaw-23.6.0/gpaw/gpu/__init__.py` & `gpaw-23.6.1/gpaw/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/gpu/cpupy/__init__.py` & `gpaw-23.6.1/gpaw/gpu/cpupy/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/gpu/cpupyx/fft.py` & `gpaw-23.6.1/gpaw/gpu/cpupyx/fft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/gpu/mpi.py` & `gpaw-23.6.1/gpaw/gpu/mpi.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/grid_descriptor.py` & `gpaw-23.6.1/gpaw/grid_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             return result
 
     def coarsen(self):
         """Return coarsened `GridDescriptor` object.
 
         Reurned descriptor has 2x2x2 fewer grid points."""
 
-        if np.sometrue(self.N_c % 2):
+        if (self.N_c % 2).any():
             raise ValueError('Grid %s not divisible by 2!' % self.N_c)
 
         return self.new_descriptor(self.N_c // 2)
 
     def refine(self):
         """Return refined `GridDescriptor` object.
```

### Comparing `gpaw-23.6.0/gpaw/hamiltonian.py` & `gpaw-23.6.1/gpaw/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/helmholtz.py` & `gpaw-23.6.1/gpaw/helmholtz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hgh.py` & `gpaw-23.6.1/gpaw/hgh.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         nj = sum([v.nn for v in hghdata.v_l])
         if nj == 0:
             nj = 1  # Code assumes nj > 0 elsewhere, we fill out with zeroes
 
         if not hghdata.v_l:
             # No projectors.  But the remaining code assumes that everything
             # has projectors!  We'll just add the zero function then
-            hghdata.v_l = [VNonLocal(0, 0.01, [[0.]])]
+            hghdata.v_l = [VNonLocal(0, 0.01, [0.])]
 
         n_j = []
         l_j = []
 
         # j ordering is significant, must be nl rather than ln
         for n, l in self.hghdata.nl_iter():
             n_j.append(n + 1)  # Note: actual n must be positive!
```

### Comparing `gpaw-23.6.0/gpaw/hgh_parameters.py` & `gpaw-23.6.1/gpaw/hgh_parameters.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hubbard.py` & `gpaw-23.6.1/gpaw/hubbard.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/coulomb.py` & `gpaw-23.6.1/gpaw/hybrids/coulomb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/eigenvalues.py` & `gpaw-23.6.1/gpaw/hybrids/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/energy.py` & `gpaw-23.6.1/gpaw/hybrids/energy.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/forces.py` & `gpaw-23.6.1/gpaw/hybrids/forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/kpts.py` & `gpaw-23.6.1/gpaw/hybrids/kpts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/paw.py` & `gpaw-23.6.1/gpaw/hybrids/paw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/scf.py` & `gpaw-23.6.1/gpaw/hybrids/scf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/symmetry.py` & `gpaw-23.6.1/gpaw/hybrids/symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/wrapper.py` & `gpaw-23.6.1/gpaw/hybrids/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hybrids/wstc.py` & `gpaw-23.6.1/gpaw/hybrids/wstc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/hyperfine.py` & `gpaw-23.6.1/gpaw/hyperfine.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/inducedfield/inducedfield_base.py` & `gpaw-23.6.1/gpaw/inducedfield/inducedfield_base.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/inducedfield/inducedfield_fdtd.py` & `gpaw-23.6.1/gpaw/inducedfield/inducedfield_fdtd.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/inducedfield/inducedfield_lrtddft.py` & `gpaw-23.6.1/gpaw/inducedfield/inducedfield_lrtddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/inducedfield/inducedfield_tddft.py` & `gpaw-23.6.1/gpaw/inducedfield/inducedfield_tddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/io/fmf.py` & `gpaw-23.6.1/gpaw/io/fmf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/io/logger.py` & `gpaw-23.6.1/gpaw/io/logger.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/io/old.py` & `gpaw-23.6.1/gpaw/io/old.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/io/tar.py` & `gpaw-23.6.1/gpaw/io/tar.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/jellium.py` & `gpaw-23.6.1/gpaw/jellium.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/kohnsham_layouts.py` & `gpaw-23.6.1/gpaw/kohnsham_layouts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/kpoint.py` & `gpaw-23.6.1/gpaw/kpoint.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/kpt_descriptor.py` & `gpaw-23.6.1/gpaw/kpt_descriptor.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/kpt_refine.py` & `gpaw-23.6.1/gpaw/kpt_refine.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/analyse_basis.py` & `gpaw-23.6.1/gpaw/lcao/analyse_basis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/atomic_correction.py` & `gpaw-23.6.1/gpaw/lcao/atomic_correction.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/bsse.py` & `gpaw-23.6.1/gpaw/lcao/bsse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/dipoletransition.py` & `gpaw-23.6.1/gpaw/lcao/dipoletransition.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/eigensolver.py` & `gpaw-23.6.1/gpaw/lcao/eigensolver.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/el_ph.py` & `gpaw-23.6.1/gpaw/lcao/el_ph.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/generate_extended.py` & `gpaw-23.6.1/gpaw/lcao/generate_extended.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/generate_ngto_augmented.py` & `gpaw-23.6.1/gpaw/lcao/generate_ngto_augmented.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/local_orbitals.py` & `gpaw-23.6.1/gpaw/lcao/local_orbitals.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/overlap.py` & `gpaw-23.6.1/gpaw/lcao/overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/projected_wannier.py` & `gpaw-23.6.1/gpaw/lcao/projected_wannier.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/pwf2.py` & `gpaw-23.6.1/gpaw/lcao/pwf2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/scissors.py` & `gpaw-23.6.1/gpaw/lcao/scissors.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/tci.py` & `gpaw-23.6.1/gpaw/lcao/tci.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/tightbinding.py` & `gpaw-23.6.1/gpaw/lcao/tightbinding.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcao/tools.py` & `gpaw-23.6.1/gpaw/lcao/tools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/__init__.py` & `gpaw-23.6.1/gpaw/lcaotddft/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/densitymatrix.py` & `gpaw-23.6.1/gpaw/lcaotddft/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/dipolemomentwriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/dipolemomentwriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/energywriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/energywriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/frequencydensitymatrix.py` & `gpaw-23.6.1/gpaw/lcaotddft/frequencydensitymatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/hamiltonian.py` & `gpaw-23.6.1/gpaw/lcaotddft/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/ksdecomposition.py` & `gpaw-23.6.1/gpaw/lcaotddft/ksdecomposition.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/laser.py` & `gpaw-23.6.1/gpaw/lcaotddft/laser.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/linedensity.py` & `gpaw-23.6.1/gpaw/lcaotddft/linedensity.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/logger.py` & `gpaw-23.6.1/gpaw/lcaotddft/logger.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/magneticmomentwriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/magneticmomentwriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/observer.py` & `gpaw-23.6.1/gpaw/lcaotddft/observer.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/propagators.py` & `gpaw-23.6.1/gpaw/lcaotddft/propagators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/qed.py` & `gpaw-23.6.1/gpaw/lcaotddft/qed.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/quadrupolemomentwriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/quadrupolemomentwriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/restartfilewriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/restartfilewriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/tcm.py` & `gpaw-23.6.1/gpaw/lcaotddft/tcm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/timedensitymatrix.py` & `gpaw-23.6.1/gpaw/lcaotddft/timedensitymatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/utilities.py` & `gpaw-23.6.1/gpaw/lcaotddft/utilities.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lcaotddft/wfwriter.py` & `gpaw-23.6.1/gpaw/lcaotddft/wfwriter.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lfc.py` & `gpaw-23.6.1/gpaw/lfc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/__init__.py` & `gpaw-23.6.1/gpaw/lrtddft/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/apmb.py` & `gpaw-23.6.1/gpaw/lrtddft/apmb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/convergence.py` & `gpaw-23.6.1/gpaw/lrtddft/convergence.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/dielectric.py` & `gpaw-23.6.1/gpaw/lrtddft/dielectric.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/excitation.py` & `gpaw-23.6.1/gpaw/lrtddft/excitation.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/excited_state.py` & `gpaw-23.6.1/gpaw/lrtddft/excited_state.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/finite_differences.py` & `gpaw-23.6.1/gpaw/lrtddft/finite_differences.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/kssingle.py` & `gpaw-23.6.1/gpaw/lrtddft/kssingle.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/omega_matrix.py` & `gpaw-23.6.1/gpaw/lrtddft/omega_matrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft/spectrum.py` & `gpaw-23.6.1/gpaw/lrtddft/spectrum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/__init__.py` & `gpaw-23.6.1/gpaw/lrtddft2/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/eta.py` & `gpaw-23.6.1/gpaw/lrtddft2/eta.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/k_matrix.py` & `gpaw-23.6.1/gpaw/lrtddft2/k_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
             # self.timer.start('Write K')
             # Write only on dd_comm root
             if self.lr_comms.dd_comm.rank == 0:
 
                 # Write only lower triangle of K-matrix
                 for [i, p, j, q, Kipjq] in K:
                     self.Kfile.write("%5d %5d %5d %5d %22.16lf\n" %
-                                     (i, p, j, q, Kipjq))
+                                     (i, p, j, q, Kipjq[0]))
                 self.Kfile.flush()  # flush K-matrix before ready_rows
 
                 # Write and flush ready rows
                 self.ready_file.write("%d %d\n" %
                                       (kss_ip.occ_ind, kss_ip.unocc_ind))
                 self.ready_file.flush()
```

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/ks_singles.py` & `gpaw-23.6.1/gpaw/lrtddft2/ks_singles.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/lr_communicators.py` & `gpaw-23.6.1/gpaw/lrtddft2/lr_communicators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/lr_layouts.py` & `gpaw-23.6.1/gpaw/lrtddft2/lr_layouts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/lr_response.py` & `gpaw-23.6.1/gpaw/lrtddft2/lr_response.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/lr_transitions.py` & `gpaw-23.6.1/gpaw/lrtddft2/lr_transitions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/lrtddft2/tools.py` & `gpaw-23.6.1/gpaw/lrtddft2/tools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/matrix.py` & `gpaw-23.6.1/gpaw/matrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/matrix_descriptor.py` & `gpaw-23.6.1/gpaw/matrix_descriptor.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/mixer.py` & `gpaw-23.6.1/gpaw/mixer.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/mom.py` & `gpaw-23.6.1/gpaw/mom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/mpi.py` & `gpaw-23.6.1/gpaw/mpi.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/__init__.py` & `gpaw-23.6.1/gpaw/new/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/ase_interface.py` & `gpaw-23.6.1/gpaw/new/ase_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -351,32 +351,22 @@
                                  skip_core=False):
         assert spin is None
         n_sr = self.calculation.densities().all_electron_densities(
             grid_refinement=gridrefinement,
             skip_core=skip_core)
         return n_sr.to_pbc_grid().data.sum(0)
 
-    def get_eigenvalues(self, kpt=0, spin=0, broadcast=True):
+    def get_eigenvalues(self, kpt=0, spin=0):
         state = self.calculation.state
-        eig_n = state.ibzwfs.get_eigs_and_occs(k=kpt, s=spin)[0] * Ha
-        if broadcast:
-            if self.world.rank != 0:
-                eig_n = np.empty(state.ibzwfs.nbands)
-            self.world.broadcast(eig_n, 0)
-        return eig_n
+        return state.ibzwfs.get_eigs_and_occs(k=kpt, s=spin)[0] * Ha
 
-    def get_occupation_numbers(self, kpt=0, spin=0, broadcast=True):
+    def get_occupation_numbers(self, kpt=0, spin=0):
         state = self.calculation.state
         weight = state.ibzwfs.ibz.weight_k[kpt] * state.ibzwfs.spin_degeneracy
-        occ_n = state.ibzwfs.get_eigs_and_occs(k=kpt, s=spin)[1] * weight
-        if broadcast:
-            if self.world.rank != 0:
-                occ_n = np.empty(state.ibzwfs.nbands)
-            self.world.broadcast(occ_n, 0)
-        return occ_n
+        return state.ibzwfs.get_eigs_and_occs(k=kpt, s=spin)[1] * weight
 
     def get_reference_energy(self):
         return self.calculation.setups.Eref * Ha
 
     def get_number_of_iterations(self):
         return self.calculation.scf_loop.niter
```

### Comparing `gpaw-23.6.0/gpaw/new/backwards_compatibility.py` & `gpaw-23.6.1/gpaw/new/backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/basis.py` & `gpaw-23.6.1/gpaw/new/basis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/brillouin.py` & `gpaw-23.6.1/gpaw/new/brillouin.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/builder.py` & `gpaw-23.6.1/gpaw/new/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/calculation.py` & `gpaw-23.6.1/gpaw/new/calculation.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/density.py` & `gpaw-23.6.1/gpaw/new/density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/fd/builder.py` & `gpaw-23.6.1/gpaw/new/fd/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/fd/pot_calc.py` & `gpaw-23.6.1/gpaw/new/fd/pot_calc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/gpw.py` & `gpaw-23.6.1/gpaw/new/gpw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/ibzwfs.py` & `gpaw-23.6.1/gpaw/new/ibzwfs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/input_parameters.py` & `gpaw-23.6.1/gpaw/new/input_parameters.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/builder.py` & `gpaw-23.6.1/gpaw/new/lcao/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/eigensolver.py` & `gpaw-23.6.1/gpaw/new/lcao/eigensolver.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/forces.py` & `gpaw-23.6.1/gpaw/new/lcao/forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/hamiltonian.py` & `gpaw-23.6.1/gpaw/new/lcao/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/hybrids.py` & `gpaw-23.6.1/gpaw/new/lcao/hybrids.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/lcao/wave_functions.py` & `gpaw-23.6.1/gpaw/new/lcao/wave_functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/logger.py` & `gpaw-23.6.1/gpaw/new/logger.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/poisson.py` & `gpaw-23.6.1/gpaw/new/poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pot_calc.py` & `gpaw-23.6.1/gpaw/new/pot_calc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/potential.py` & `gpaw-23.6.1/gpaw/new/potential.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/builder.py` & `gpaw-23.6.1/gpaw/new/pw/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/fulldiag.py` & `gpaw-23.6.1/gpaw/new/pw/fulldiag.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/hamiltonian.py` & `gpaw-23.6.1/gpaw/new/pw/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/poisson.py` & `gpaw-23.6.1/gpaw/new/pw/poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/pot_calc.py` & `gpaw-23.6.1/gpaw/new/pw/pot_calc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pw/stress.py` & `gpaw-23.6.1/gpaw/new/pw/stress.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pwfd/builder.py` & `gpaw-23.6.1/gpaw/new/pwfd/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pwfd/davidson.py` & `gpaw-23.6.1/gpaw/new/pwfd/davidson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/pwfd/wave_functions.py` & `gpaw-23.6.1/gpaw/new/pwfd/wave_functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/rttddft.py` & `gpaw-23.6.1/gpaw/new/rttddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/scf.py` & `gpaw-23.6.1/gpaw/new/scf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/smearing.py` & `gpaw-23.6.1/gpaw/new/smearing.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/spinors.py` & `gpaw-23.6.1/gpaw/new/spinors.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/spinspiral.py` & `gpaw-23.6.1/gpaw/new/spinspiral.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/symmetry.py` & `gpaw-23.6.1/gpaw/new/symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/tb/builder.py` & `gpaw-23.6.1/gpaw/new/tb/builder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/wave_functions.py` & `gpaw-23.6.1/gpaw/new/wave_functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/new/xc.py` & `gpaw-23.6.1/gpaw/new/xc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/nlopt/basic.py` & `gpaw-23.6.1/gpaw/nlopt/basic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/nlopt/linear.py` & `gpaw-23.6.1/gpaw/nlopt/linear.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/nlopt/matrixel.py` & `gpaw-23.6.1/gpaw/nlopt/matrixel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/nlopt/shg.py` & `gpaw-23.6.1/gpaw/nlopt/shg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/nlopt/shift.py` & `gpaw-23.6.1/gpaw/nlopt/shift.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/occupations.py` & `gpaw-23.6.1/gpaw/occupations.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     e_entropy = (0.5 * coff_function(order) *
                  hermite_poly(2 * order, x) * np.exp(-x**2))
     e_entropy = -e_entropy * width
     return f, dfde, e_entropy
 
 
 def coff_function(n):
-    return (-1)**n / (np.product(np.arange(1, n + 1)) *
+    return (-1)**n / (np.prod(np.arange(1, n + 1)) *
                       4**n * np.sqrt(np.pi))
 
 
 def hermite_poly(n, x):
     if n == 0:
         return 1
     elif n == 1:
```

### Comparing `gpaw-23.6.0/gpaw/output.py` & `gpaw-23.6.1/gpaw/output.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/overlap.py` & `gpaw-23.6.1/gpaw/overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pair_density.py` & `gpaw-23.6.1/gpaw/pair_density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pair_overlap.py` & `gpaw-23.6.1/gpaw/pair_overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pes/__init__.py` & `gpaw-23.6.1/gpaw/pes/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pes/continuum.py` & `gpaw-23.6.1/gpaw/pes/continuum.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         hamiltonian = self.calculator.hamiltonian
         if 1:
             self.vt_G = hamiltonian.vt_sG[0]  # XXX treat spin
         else:
             self.vt_G = np.where(hamiltonian.vt_sG[0] > 0,
                                  0.0, hamiltonian.vt_sG[0])
         self.intvt = self.gd.integrate(self.vt_G)
-        print('# int(vt_G)=', self.intvt, np.sometrue(self.vt_G > 0))
+        print('# int(vt_G)=', self.intvt, (self.vt_G > 0).any())
 
         self.solve()
 
     def get_grid(self, k_c, r0):
         print('Correction:', self.gd.integrate(self.corrt_G))
         if not hasattr(self, 'written'):
             print('r0', r0, r0 * Bohr)
@@ -68,15 +68,15 @@
             r_R = AI.radii()
             psi_R = AI.average(self.corrt_G)
             v_R = AI.average(self.vt_G)
             with open('radial_dR' + str(dR) + '.dat', 'w') as fd:
                 print('# R  v(R)    psi(R)', file=fd)
                 for r, psi, v in zip(r_R, psi_R, v_R):
                     print(r, psi, v, file=fd)
-            
+
             self.written = True
 
         return self.pw.get_grid(k_c, r0) - 1e6 * self.corrt_G
 
     def solve(self):
         hamiltonian = self.calculator.hamiltonian
         self.poisson = PoissonSolver('fd', nn=hamiltonian.poisson.nn)
```

### Comparing `gpaw-23.6.0/gpaw/pes/dos.py` & `gpaw-23.6.1/gpaw/pes/dos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pes/ds_beta.py` & `gpaw-23.6.1/gpaw/pes/ds_beta.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pes/state.py` & `gpaw-23.6.1/gpaw/pes/state.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pes/tddft.py` & `gpaw-23.6.1/gpaw/pes/tddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/point_groups/check.py` & `gpaw-23.6.1/gpaw/point_groups/check.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/point_groups/cli.py` & `gpaw-23.6.1/gpaw/point_groups/cli.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/point_groups/group.py` & `gpaw-23.6.1/gpaw/point_groups/group.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/point_groups/groups.py` & `gpaw-23.6.1/gpaw/point_groups/groups.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/poisson.py` & `gpaw-23.6.1/gpaw/poisson.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,18 +457,18 @@
         while self.iterate2(self.step) > eps and niter < maxiter:
             niter += 1
         if niter == maxiter:
             msg = 'Poisson solver did not converge in %d iterations!' % maxiter
             raise PoissonConvergenceError(msg)
 
         # Set the average potential to zero in periodic systems
-        if np.alltrue(self.gd.pbc_c):
+        if (self.gd.pbc_c).all():
             phi_ave = self.gd.comm.sum(np.sum(phi.ravel()))
             N_c = self.gd.get_size_of_global_array()
-            phi_ave /= np.product(N_c)
+            phi_ave /= np.prod(N_c)
             phi -= phi_ave
 
         return niter
 
     def iterate2(self, step, level=0):
         """Smooths the solution in every multigrid level"""
         self._init()
```

### Comparing `gpaw-23.6.0/gpaw/poisson_extravacuum.py` & `gpaw-23.6.1/gpaw/poisson_extravacuum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/poisson_moment.py` & `gpaw-23.6.1/gpaw/poisson_moment.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/preconditioner.py` & `gpaw-23.6.1/gpaw/preconditioner.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/projections.py` & `gpaw-23.6.1/gpaw/projections.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pseudopotential.py` & `gpaw-23.6.1/gpaw/pseudopotential.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pw/density.py` & `gpaw-23.6.1/gpaw/pw/density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pw/descriptor.py` & `gpaw-23.6.1/gpaw/pw/descriptor.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pw/hamiltonian.py` & `gpaw-23.6.1/gpaw/pw/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pw/lfc.py` & `gpaw-23.6.1/gpaw/pw/lfc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/pw/poisson.py` & `gpaw-23.6.1/gpaw/pw/poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/quiz.py` & `gpaw-23.6.1/gpaw/quiz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/raman/raman.py` & `gpaw-23.6.1/gpaw/raman/raman.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/bse.py` & `gpaw-23.6.1/gpaw/response/bse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/chi0.py` & `gpaw-23.6.1/gpaw/response/chi0.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/chi0_data.py` & `gpaw-23.6.1/gpaw/response/chi0_data.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/chiks.py` & `gpaw-23.6.1/gpaw/response/chiks.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/context.py` & `gpaw-23.6.1/gpaw/response/context.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/coulomb_kernels.py` & `gpaw-23.6.1/gpaw/response/coulomb_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/density_kernels.py` & `gpaw-23.6.1/gpaw/response/density_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/df.py` & `gpaw-23.6.1/gpaw/response/df.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/drude.py` & `gpaw-23.6.1/gpaw/response/drude.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/dyson.py` & `gpaw-23.6.1/gpaw/response/dyson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/frequencies.py` & `gpaw-23.6.1/gpaw/response/frequencies.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/fxc_kernels.py` & `gpaw-23.6.1/gpaw/response/fxc_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/g0w0.py` & `gpaw-23.6.1/gpaw/response/g0w0.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                       flush=False)
         context.print('  Performing linear fit to %d points' % len(ecut_e))
         self.sigr2_skn = np.zeros(shape)
         self.dsigr2_skn = np.zeros(shape)
         self.sigma_skn = np.zeros(shape)
         self.dsigma_skn = np.zeros(shape)
         invN_i = ecut_e**(-3. / 2)
-        for m in range(np.product(shape)):
+        for m in range(np.prod(shape)):
             s, k, n = np.unravel_index(m, shape)
 
             slope, intercept, r_value, p_value, std_err = \
                 linregress(invN_i, sigma_eskn[:, s, k, n])
 
             self.sigr2_skn[s, k, n] = r_value**2
             self.sigma_skn[s, k, n] = intercept
```

### Comparing `gpaw-23.6.0/gpaw/response/g0w0_kernels.py` & `gpaw-23.6.1/gpaw/response/g0w0_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/gamma_int.py` & `gpaw-23.6.1/gpaw/response/gamma_int.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/goldstone.py` & `gpaw-23.6.1/gpaw/response/goldstone.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/groundstate.py` & `gpaw-23.6.1/gpaw/response/groundstate.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/gw_bands.py` & `gpaw-23.6.1/gpaw/response/gw_bands.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/heisenberg.py` & `gpaw-23.6.1/gpaw/response/heisenberg.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,10 +143,10 @@
 
 
 def get_q0_index(q_qc):
     """Find index corresponding q=0 in q-vector array."""
     q0_indices = np.argwhere(np.all(q_qc == 0, axis=1))
 
     if len(q0_indices) >= 1:
-        return int(q0_indices[0])
+        return int(q0_indices[0, 0])
     else:
         raise ValueError('q_qc has to include q=0, i.e. q_c = [0., 0., 0.]')
```

### Comparing `gpaw-23.6.0/gpaw/response/hilbert.py` & `gpaw-23.6.1/gpaw/response/hilbert.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/ibz2bz.py` & `gpaw-23.6.1/gpaw/response/ibz2bz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/integrators.py` & `gpaw-23.6.1/gpaw/response/integrators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/jdos.py` & `gpaw-23.6.1/gpaw/response/jdos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/kspair.py` & `gpaw-23.6.1/gpaw/response/kspair.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/localft.py` & `gpaw-23.6.1/gpaw/response/localft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/matrix_elements.py` & `gpaw-23.6.1/gpaw/response/matrix_elements.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/mft.py` & `gpaw-23.6.1/gpaw/response/mft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/pair.py` & `gpaw-23.6.1/gpaw/response/pair.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/pair_functions.py` & `gpaw-23.6.1/gpaw/response/pair_functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/pair_integrator.py` & `gpaw-23.6.1/gpaw/response/pair_integrator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/pair_transitions.py` & `gpaw-23.6.1/gpaw/response/pair_transitions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/paw.py` & `gpaw-23.6.1/gpaw/response/paw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/pw_parallelization.py` & `gpaw-23.6.1/gpaw/response/pw_parallelization.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/q0_correction.py` & `gpaw-23.6.1/gpaw/response/q0_correction.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/qeh.py` & `gpaw-23.6.1/gpaw/response/qeh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/screened_interaction.py` & `gpaw-23.6.1/gpaw/response/screened_interaction.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/site_kernels.py` & `gpaw-23.6.1/gpaw/response/site_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/susceptibility.py` & `gpaw-23.6.1/gpaw/response/susceptibility.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/symmetry.py` & `gpaw-23.6.1/gpaw/response/symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/temp.py` & `gpaw-23.6.1/gpaw/response/temp.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/tool.py` & `gpaw-23.6.1/gpaw/response/tool.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/response/wgg.py` & `gpaw-23.6.1/gpaw/response/wgg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/rotation.py` & `gpaw-23.6.1/gpaw/rotation.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/scf.py` & `gpaw-23.6.1/gpaw/scf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/setup.py` & `gpaw-23.6.1/gpaw/setup.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/setup_data.py` & `gpaw-23.6.1/gpaw/setup_data.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/__init__.py` & `gpaw-23.6.1/gpaw/solvation/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/calculator.py` & `gpaw-23.6.1/gpaw/solvation/calculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/cavity.py` & `gpaw-23.6.1/gpaw/solvation/cavity.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/dielectric.py` & `gpaw-23.6.1/gpaw/solvation/dielectric.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/hamiltonian.py` & `gpaw-23.6.1/gpaw/solvation/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/interactions.py` & `gpaw-23.6.1/gpaw/solvation/interactions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/poisson.py` & `gpaw-23.6.1/gpaw/solvation/poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/solvation/sjm.py` & `gpaw-23.6.1/gpaw/solvation/sjm.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
             previous_potentials.append(float(true_potential))
             if len(previous_electrons) > 1:
                 slope = _calculate_slope(previous_electrons,
                                          previous_potentials)
                 self.log('Slope regressed from last {:d} attempts is '
                          '{:.4f} V/electron,'
                          .format(len(previous_electrons[-4:]), slope))
-                area = np.product(np.diag(atoms.cell[:2, :2]))
+                area = np.prod(np.diag(atoms.cell[:2, :2]))
                 capacitance = -1.6022 * 1e3 / (area * slope)
                 self.log(f'or apparent capacitance of {capacitance:.4f} '
                          'muF/cm^2')
                 if p.slope is not None:
                     p.slope = p.mixer * p.slope + (1. - p.mixer) * slope
                     self.log(f'After mixing with {p.mixer:.2f}, new slope is '
                              f'{p.slope:.4f} V/electron.')
@@ -485,15 +485,15 @@
                 if iteration >= 2:
                     self.timer.stop('Potential equilibration loop')
                 if not p.always_adjust:
                     return
 
             # Guess slope if we don't have enough information yet.
             if p.slope is None:
-                area = np.product(np.diag(atoms.cell[:2, :2]))
+                area = np.prod(np.diag(atoms.cell[:2, :2]))
                 p.slope = -1.6022e3 / (area * 10.)
                 self.log('No slope provided, guessing a slope of '
                          f'{p.slope:.4f} corresponding\nto an apparent '
                          'capacitance of 10 muF/cm^2.')
 
             # Finally, update the number of electrons.
             p.excess_electrons += ((p.target_potential - true_potential)
```

### Comparing `gpaw-23.6.0/gpaw/sphere/lebedev.py` & `gpaw-23.6.1/gpaw/sphere/lebedev.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/sphere/rshe.py` & `gpaw-23.6.1/gpaw/sphere/rshe.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/spherical_harmonics.py` & `gpaw-23.6.1/gpaw/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/spinorbit.py` & `gpaw-23.6.1/gpaw/spinorbit.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/spline.py` & `gpaw-23.6.1/gpaw/spline.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/stress.py` & `gpaw-23.6.1/gpaw/stress.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/symmetry.py` & `gpaw-23.6.1/gpaw/symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/__init__.py` & `gpaw-23.6.1/gpaw/tddft/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/abc.py` & `gpaw-23.6.1/gpaw/tddft/abc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/ehrenfest.py` & `gpaw-23.6.1/gpaw/tddft/ehrenfest.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/folding.py` & `gpaw-23.6.1/gpaw/tddft/folding.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/laser.py` & `gpaw-23.6.1/gpaw/tddft/laser.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/propagators.py` & `gpaw-23.6.1/gpaw/tddft/propagators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/solvers/base.py` & `gpaw-23.6.1/gpaw/tddft/solvers/base.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/solvers/bicgstab.py` & `gpaw-23.6.1/gpaw/tddft/solvers/bicgstab.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/solvers/cscg.py` & `gpaw-23.6.1/gpaw/tddft/solvers/cscg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/spectrum.py` & `gpaw-23.6.1/gpaw/tddft/spectrum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/tdopers.py` & `gpaw-23.6.1/gpaw/tddft/tdopers.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/units.py` & `gpaw-23.6.1/gpaw/tddft/units.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tddft/utils.py` & `gpaw-23.6.1/gpaw/tddft/utils.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/__init__.py` & `gpaw-23.6.1/gpaw/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ase_features/autoneb.py` & `gpaw-23.6.1/gpaw/test/ase_features/autoneb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ase_features/test_ase3k.py` & `gpaw-23.6.1/gpaw/test/ase_features/test_ase3k.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/analyse.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/analyse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_fhi.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_fhi.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_hgh.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_hgh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_abinit_paw.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_abinit_paw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_aims.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_aims.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_gpaw_pw.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_gpaw_pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/dcdft/pbe_gpaw_pw_verify.py` & `gpaw-23.6.1/gpaw/test/big/dcdft/pbe_gpaw_pw_verify.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/g2_1/analyse.py` & `gpaw-23.6.1/gpaw/test/big/g2_1/analyse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/g2_1/g21gpaw.py` & `gpaw-23.6.1/gpaw/test/big/g2_1/g21gpaw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/g2_1/g21nwchem.py` & `gpaw-23.6.1/gpaw/test/big/g2_1/g21nwchem.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/g2_1/pbe_gpaw_nrel_plot.py` & `gpaw-23.6.1/gpaw/test/big/g2_1/pbe_gpaw_nrel_plot.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/hsk/hsk.py` & `gpaw-23.6.1/gpaw/test/big/hsk/hsk.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/kpb/check.py` & `gpaw-23.6.1/gpaw/test/big/kpb/check.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/kpb/molecules.py` & `gpaw-23.6.1/gpaw/test/big/kpb/molecules.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/test_systems/agts.py` & `gpaw-23.6.1/gpaw/test/big/test_systems/agts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/big/test_systems/create.py` & `gpaw-23.6.1/gpaw/test/big/test_systems/create.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/conftest.py` & `gpaw-23.6.1/gpaw/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/si_nonortho.py` & `gpaw-23.6.1/gpaw/test/corehole/si_nonortho.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/test_h2o.py` & `gpaw-23.6.1/gpaw/test/corehole/test_h2o.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/test_h2o_dks.py` & `gpaw-23.6.1/gpaw/test/corehole/test_h2o_dks.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/test_h2o_recursion.py` & `gpaw-23.6.1/gpaw/test/corehole/test_h2o_recursion.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/test_li2.py` & `gpaw-23.6.1/gpaw/test/corehole/test_li2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/corehole/test_si.py` & `gpaw-23.6.1/gpaw/test/corehole/test_si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/crontab.py` & `gpaw-23.6.1/gpaw/test/crontab.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/dscf/dscf_forces.py` & `gpaw-23.6.1/gpaw/test/dscf/dscf_forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/dscf/test_dscf_lcao.py` & `gpaw-23.6.1/gpaw/test/dscf/test_dscf_lcao.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/eigen/test_blocked_rmm_diis.py` & `gpaw-23.6.1/gpaw/test/eigen/test_blocked_rmm_diis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/eigen/test_cg.py` & `gpaw-23.6.1/gpaw/test/eigen/test_cg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/eigen/test_cg2.py` & `gpaw-23.6.1/gpaw/test/eigen/test_cg2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/eigen/test_davidson.py` & `gpaw-23.6.1/gpaw/test/eigen/test_davidson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/eigen/test_keep_htpsit.py` & `gpaw-23.6.1/gpaw/test/eigen/test_keep_htpsit.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/conftest.py` & `gpaw-23.6.1/gpaw/test/elph/conftest.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_displacements.py` & `gpaw-23.6.1/gpaw/test/elph/test_displacements.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_electronphonon.py` & `gpaw-23.6.1/gpaw/test/elph/test_electronphonon.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_elph_li.py` & `gpaw-23.6.1/gpaw/test/elph/test_elph_li.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_gmatrix.py` & `gpaw-23.6.1/gpaw/test/elph/test_gmatrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_gradient.py` & `gpaw-23.6.1/gpaw/test/elph/test_gradient.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_ramancalculator.py` & `gpaw-23.6.1/gpaw/test/elph/test_ramancalculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_resonant_term.py` & `gpaw-23.6.1/gpaw/test/elph/test_resonant_term.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/elph/test_supercell.py` & `gpaw-23.6.1/gpaw/test/elph/test_supercell.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/stark_shift.py` & `gpaw-23.6.1/gpaw/test/ext_potential/stark_shift.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_b_field.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_b_field.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_collection.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_collection.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_constant_e_field.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_constant_e_field.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_external.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_external.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_external_pw.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_external_pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_harmonic.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_harmonic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_point_charge.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_point_charge.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ext_potential/test_step.py` & `gpaw-23.6.1/gpaw/test/ext_potential/test_step.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_coarse.py` & `gpaw-23.6.1/gpaw/test/exx/test_coarse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_derivs.py` & `gpaw-23.6.1/gpaw/test/exx/test_derivs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_double_cell.py` & `gpaw-23.6.1/gpaw/test/exx/test_double_cell.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_exx.py` & `gpaw-23.6.1/gpaw/test/exx/test_exx.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_exx_scf.py` & `gpaw-23.6.1/gpaw/test/exx/test_exx_scf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_forces_ut.py` & `gpaw-23.6.1/gpaw/test/exx/test_forces_ut.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_kpts.py` & `gpaw-23.6.1/gpaw/test/exx/test_kpts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/exx/test_unocc.py` & `gpaw-23.6.1/gpaw/test/exx/test_unocc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_gd.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_gd.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_gradient.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_gradient.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_laplace.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_laplace.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_nabla.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_nabla.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_non_periodic.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_non_periodic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fd_ops/test_transformations.py` & `gpaw-23.6.1/gpaw/test/fd_ops/test_transformations.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fdtd/test_ed.py` & `gpaw-23.6.1/gpaw/test/fdtd/test_ed.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fdtd/test_ed_inducedfield.py` & `gpaw-23.6.1/gpaw/test/fdtd/test_ed_inducedfield.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fdtd/test_ed_shapes.py` & `gpaw-23.6.1/gpaw/test/fdtd/test_ed_shapes.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fdtd/test_ed_wrapper.py` & `gpaw-23.6.1/gpaw/test/fdtd/test_ed_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_ascii_art.py` & `gpaw-23.6.1/gpaw/test/fileio/test_ascii_art.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_file_reference.py` & `gpaw-23.6.1/gpaw/test/fileio/test_file_reference.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_parallel.py` & `gpaw-23.6.1/gpaw/test/fileio/test_parallel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_refine.py` & `gpaw-23.6.1/gpaw/test/fileio/test_refine.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_restart.py` & `gpaw-23.6.1/gpaw/test/fileio/test_restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_restart_density.py` & `gpaw-23.6.1/gpaw/test/fileio/test_restart_density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fileio/test_wfs_io.py` & `gpaw-23.6.1/gpaw/test/fileio/test_wfs_io.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/fuzz.py` & `gpaw-23.6.1/gpaw/test/fuzz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/colinear.py` & `gpaw-23.6.1/gpaw/test/generic/colinear.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_2Al.py` & `gpaw-23.6.1/gpaw/test/generic/test_2Al.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_8Si.py` & `gpaw-23.6.1/gpaw/test/generic/test_8Si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_Cu.py` & `gpaw-23.6.1/gpaw/test/generic/test_Cu.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_H_force.py` & `gpaw-23.6.1/gpaw/test/generic/test_H_force.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_IP_oxygen.py` & `gpaw-23.6.1/gpaw/test/generic/test_IP_oxygen.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_al_chain.py` & `gpaw-23.6.1/gpaw/test/generic/test_al_chain.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_asym_box.py` & `gpaw-23.6.1/gpaw/test/generic/test_asym_box.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_bulk.py` & `gpaw-23.6.1/gpaw/test/generic/test_bulk.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_guc_force.py` & `gpaw-23.6.1/gpaw/test/generic/test_guc_force.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_hydrogen.py` & `gpaw-23.6.1/gpaw/test/generic/test_hydrogen.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_move_across_cell.py` & `gpaw-23.6.1/gpaw/test/generic/test_move_across_cell.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_proton.py` & `gpaw-23.6.1/gpaw/test/generic/test_proton.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_relax.py` & `gpaw-23.6.1/gpaw/test/generic/test_relax.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_si.py` & `gpaw-23.6.1/gpaw/test/generic/test_si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/generic/test_si_primitive.py` & `gpaw-23.6.1/gpaw/test/generic/test_si_primitive.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_atomic.py` & `gpaw-23.6.1/gpaw/test/gllb/test_atomic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_diamond.py` & `gpaw-23.6.1/gpaw/test/gllb/test_diamond.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_metallic.py` & `gpaw-23.6.1/gpaw/test/gllb/test_metallic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_ne.py` & `gpaw-23.6.1/gpaw/test/gllb/test_ne.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_ne_disc.py` & `gpaw-23.6.1/gpaw/test/gllb/test_ne_disc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_restart_eigenvalues.py` & `gpaw-23.6.1/gpaw/test/gllb/test_restart_eigenvalues.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_spin.py` & `gpaw-23.6.1/gpaw/test/gllb/test_spin.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gllb/test_variants.py` & `gpaw-23.6.1/gpaw/test/gllb/test_variants.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gpu/test_matrix.py` & `gpaw-23.6.1/gpaw/test/gpu/test_matrix.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gpu/test_precondition.py` & `gpaw-23.6.1/gpaw/test/gpu/test_precondition.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/gpu/test_pw.py` & `gpaw-23.6.1/gpaw/test/gpu/test_pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/restart.py` & `gpaw-23.6.1/gpaw/test/lcao/restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_atomic_corrections.py` & `gpaw-23.6.1/gpaw/test/lcao/test_atomic_corrections.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_bsse.py` & `gpaw-23.6.1/gpaw/test/lcao/test_bsse.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_bulk.py` & `gpaw-23.6.1/gpaw/test/lcao/test_bulk.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_density.py` & `gpaw-23.6.1/gpaw/test/lcao/test_density.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_dipole_transition.py` & `gpaw-23.6.1/gpaw/test/lcao/test_dipole_transition.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_dipole_transition2.py` & `gpaw-23.6.1/gpaw/test/lcao/test_dipole_transition2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_dos.py` & `gpaw-23.6.1/gpaw/test/lcao/test_dos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_fd2lcao_restart.py` & `gpaw-23.6.1/gpaw/test/lcao/test_fd2lcao_restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_force.py` & `gpaw-23.6.1/gpaw/test/lcao/test_force.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_generate_ngto.py` & `gpaw-23.6.1/gpaw/test/lcao/test_generate_ngto.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_gllb_si.py` & `gpaw-23.6.1/gpaw/test/lcao/test_gllb_si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_h2o.py` & `gpaw-23.6.1/gpaw/test/lcao/test_h2o.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_kpts_many_combinations.py` & `gpaw-23.6.1/gpaw/test/lcao/test_kpts_many_combinations.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_largecellforce.py` & `gpaw-23.6.1/gpaw/test/lcao/test_largecellforce.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_complicated.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_complicated.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_elpa.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_elpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_elpa_kpts.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_elpa_kpts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_hamiltonian.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_parallel.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_parallel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_parallel_kpt.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_parallel_kpt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_lcao_projections.py` & `gpaw-23.6.1/gpaw/test/lcao/test_lcao_projections.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_local_orbitals.py` & `gpaw-23.6.1/gpaw/test/lcao/test_local_orbitals.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_pair_and_coulomb.py` & `gpaw-23.6.1/gpaw/test/lcao/test_pair_and_coulomb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcao/test_scissors.py` & `gpaw-23.6.1/gpaw/test/lcao/test_scissors.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/__init__.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/demo_tddft.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/demo_tddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_circular_dichroism.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_circular_dichroism.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_is_xc.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_is_xc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_rpa.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_rpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_fxc_vs_linearize.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_fxc_vs_linearize.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_laser.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_laser.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft2_rpa.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_lcaotddft_vs_lrtddft2_rpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_molecule.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_molecule.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_periodic.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_periodic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_replay.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_replay.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_restart.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_rremission.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_rremission.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lcaotddft/test_simple.py` & `gpaw-23.6.1/gpaw/test/lcaotddft/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lfc/test_derivatives.py` & `gpaw-23.6.1/gpaw/test/lfc/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lfc/test_lf.py` & `gpaw-23.6.1/gpaw/test/lfc/test_lf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lfc/test_second_derivative.py` & `gpaw-23.6.1/gpaw/test/lfc/test_second_derivative.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_blas.py` & `gpaw-23.6.1/gpaw/test/linalg/test_blas.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_dot.py` & `gpaw-23.6.1/gpaw/test/linalg/test_dot.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_gemm.py` & `gpaw-23.6.1/gpaw/test/linalg/test_gemm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_gemm_complex.py` & `gpaw-23.6.1/gpaw/test/linalg/test_gemm_complex.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_mmm.py` & `gpaw-23.6.1/gpaw/test/linalg/test_mmm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/linalg/test_zher.py` & `gpaw-23.6.1/gpaw/test/linalg/test_zher.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/d2Excdn2.py` & `gpaw-23.6.1/gpaw/test/lrtddft/d2Excdn2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/rraman.py` & `gpaw-23.6.1/gpaw/test/lrtddft/rraman.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/rraman_albrecht.py` & `gpaw-23.6.1/gpaw/test/lrtddft/rraman_albrecht.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_1.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_1.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_2.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_3.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_3.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_apmb.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_apmb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_dielectric.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_dielectric.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_excited_state.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_excited_state.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_kssingles.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_kssingles.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_kssingles_Be.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_kssingles_Be.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft2.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft_basics.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft_basics.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_lrtddft_log.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_lrtddft_log.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_pes.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_pes.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_placzek_profeta_albrecht.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_placzek_profeta_albrecht.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_rraman.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_rraman.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft/test_select.py` & `gpaw-23.6.1/gpaw/test/lrtddft/test_select.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft2/test_Al2.py` & `gpaw-23.6.1/gpaw/test/lrtddft2/test_Al2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft2/test_H2O-lcao.py` & `gpaw-23.6.1/gpaw/test/lrtddft2/test_H2O-lcao.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/lrtddft2/test_parameters.py` & `gpaw-23.6.1/gpaw/test/lrtddft2/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/maths/test_fftw.py` & `gpaw-23.6.1/gpaw/test/maths/test_fftw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/maths/test_fsbt.py` & `gpaw-23.6.1/gpaw/test/maths/test_fsbt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mgga/test_mgga_restart.py` & `gpaw-23.6.1/gpaw/test/mgga/test_mgga_restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mgga/test_mgga_sc.py` & `gpaw-23.6.1/gpaw/test/mgga/test_mgga_sc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mgga/test_nsc_MGGA.py` & `gpaw-23.6.1/gpaw/test/mgga/test_nsc_MGGA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mgga/test_symm.py` & `gpaw-23.6.1/gpaw/test/mgga/test_symm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mom/test_mom_fd_energy.py` & `gpaw-23.6.1/gpaw/test/mom/test_mom_fd_energy.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mom/test_mom_lcao_forces.py` & `gpaw-23.6.1/gpaw/test/mom/test_mom_lcao_forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/mom/test_mom_lcao_smearing.py` & `gpaw-23.6.1/gpaw/test/mom/test_mom_lcao_smearing.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/noncollinear/test_o2.py` & `gpaw-23.6.1/gpaw/test/noncollinear/test_o2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/noncollinear/test_rad_pot.py` & `gpaw-23.6.1/gpaw/test/noncollinear/test_rad_pot.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/noncollinear/test_soc.py` & `gpaw-23.6.1/gpaw/test/noncollinear/test_soc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ofdft/test_ofdft.py` & `gpaw-23.6.1/gpaw/test/ofdft/test_ofdft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ofdft/test_ofdft_pbc.py` & `gpaw-23.6.1/gpaw/test/ofdft/test_ofdft_pbc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ofdft/test_ofdft_scale.py` & `gpaw-23.6.1/gpaw/test/ofdft/test_ofdft_scale.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/scalapack_pdlasrt_hang.py` & `gpaw-23.6.1/gpaw/test/parallel/scalapack_pdlasrt_hang.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_arraydict_redist.py` & `gpaw-23.6.1/gpaw/test/parallel/test_arraydict_redist.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_augment_grid.py` & `gpaw-23.6.1/gpaw/test/parallel/test_augment_grid.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_blacsdist.py` & `gpaw-23.6.1/gpaw/test/parallel/test_blacsdist.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_davidson_scalapack.py` & `gpaw-23.6.1/gpaw/test/parallel/test_davidson_scalapack.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_diamond_gllb.py` & `gpaw-23.6.1/gpaw/test/parallel/test_diamond_gllb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_fd_parallel.py` & `gpaw-23.6.1/gpaw/test/parallel/test_fd_parallel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_fd_parallel_kpt.py` & `gpaw-23.6.1/gpaw/test/parallel/test_fd_parallel_kpt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_kptpar.py` & `gpaw-23.6.1/gpaw/test/parallel/test_kptpar.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_mpi.py` & `gpaw-23.6.1/gpaw/test/parallel/test_mpi.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_parallel_eigh.py` & `gpaw-23.6.1/gpaw/test/parallel/test_parallel_eigh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_pblas.py` & `gpaw-23.6.1/gpaw/test/parallel/test_pblas.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_scalapack.py` & `gpaw-23.6.1/gpaw/test/parallel/test_scalapack.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_scalapack_diag_simple.py` & `gpaw-23.6.1/gpaw/test/parallel/test_scalapack_diag_simple.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_scalapack_mpirecv_crash.py` & `gpaw-23.6.1/gpaw/test/parallel/test_scalapack_mpirecv_crash.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/parallel/test_submatrix_redist.py` & `gpaw-23.6.1/gpaw/test/parallel/test_submatrix_redist.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pathological/test_LDA_unstable.py` & `gpaw-23.6.1/gpaw/test/pathological/test_LDA_unstable.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pathological/test_lcao_spos_derivative.py` & `gpaw-23.6.1/gpaw/test/pathological/test_lcao_spos_derivative.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pathological/test_nonlocalset.py` & `gpaw-23.6.1/gpaw/test/pathological/test_nonlocalset.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pathological/test_numpy_zdotc_graphite.py` & `gpaw-23.6.1/gpaw/test/pathological/test_numpy_zdotc_graphite.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_fastpoisson.py` & `gpaw-23.6.1/gpaw/test/poisson/test_fastpoisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_generalizedlaue.py` & `gpaw-23.6.1/gpaw/test/poisson/test_generalizedlaue.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_metallic_poisson.py` & `gpaw-23.6.1/gpaw/test/poisson/test_metallic_poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_poisson.py` & `gpaw-23.6.1/gpaw/test/poisson/test_poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_poisson_asym.py` & `gpaw-23.6.1/gpaw/test/poisson/test_poisson_asym.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_poisson_extravacuum.py` & `gpaw-23.6.1/gpaw/test/poisson/test_poisson_extravacuum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_poisson_moment.py` & `gpaw-23.6.1/gpaw/test/poisson/test_poisson_moment.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_poisson_restart.py` & `gpaw-23.6.1/gpaw/test/poisson/test_poisson_restart.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_pw_charged.py` & `gpaw-23.6.1/gpaw/test/poisson/test_pw_charged.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/poisson/test_screened_poisson.py` & `gpaw-23.6.1/gpaw/test/poisson/test_screened_poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/H_pz_hgh.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/H_pz_hgh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/H_sg15.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/H_sg15.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/O_pz_hgh.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/O_pz_hgh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/test_ah.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/test_ah.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/test_atompaw.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/test_atompaw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/test_hgh_h2o.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/test_hgh_h2o.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/test_sg15_hydrogen.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/test_sg15_hydrogen.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pseudopotential/test_upf_h2o.py` & `gpaw-23.6.1/gpaw/test/pseudopotential/test_upf_h2o.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_augment_grids.py` & `gpaw-23.6.1/gpaw/test/pw/test_augment_grids.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_bulk.py` & `gpaw-23.6.1/gpaw/test/pw/test_bulk.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_davidson_pw.py` & `gpaw-23.6.1/gpaw/test/pw/test_davidson_pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_direct.py` & `gpaw-23.6.1/gpaw/test/pw/test_direct.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_expert_diag.py` & `gpaw-23.6.1/gpaw/test/pw/test_expert_diag.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_fe_stress_mgga.py` & `gpaw-23.6.1/gpaw/test/pw/test_fe_stress_mgga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_fulldiag.py` & `gpaw-23.6.1/gpaw/test/pw/test_fulldiag.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_fulldiag_mgga.py` & `gpaw-23.6.1/gpaw/test/pw/test_fulldiag_mgga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_fulldiagk.py` & `gpaw-23.6.1/gpaw/test/pw/test_fulldiagk.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_h.py` & `gpaw-23.6.1/gpaw/test/pw/test_h.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_interpol.py` & `gpaw-23.6.1/gpaw/test/pw/test_interpol.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_lfc.py` & `gpaw-23.6.1/gpaw/test/pw/test_lfc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_par_strategies.py` & `gpaw-23.6.1/gpaw/test/pw/test_par_strategies.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_reallfc.py` & `gpaw-23.6.1/gpaw/test/pw/test_reallfc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_si_stress.py` & `gpaw-23.6.1/gpaw/test/pw/test_si_stress.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_si_stress_mgga.py` & `gpaw-23.6.1/gpaw/test/pw/test_si_stress_mgga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_slab.py` & `gpaw-23.6.1/gpaw/test/pw/test_slab.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/pw/test_stresstest.py` & `gpaw-23.6.1/gpaw/test/pw/test_stresstest.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/radial/test_two_phi_plw_integrals.py` & `gpaw-23.6.1/gpaw/test/radial/test_two_phi_plw_integrals.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/radial/test_ylexpand.py` & `gpaw-23.6.1/gpaw/test/radial/test_ylexpand.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/radial/test_yukawa_radial.py` & `gpaw-23.6.1/gpaw/test/radial/test_yukawa_radial.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ralda/test_pbe_deriv.py` & `gpaw-23.6.1/gpaw/test/ralda/test_pbe_deriv.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ralda/test_ralda_H2.py` & `gpaw-23.6.1/gpaw/test/ralda/test_ralda_H2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ralda/test_ralda_He.py` & `gpaw-23.6.1/gpaw/test/ralda/test_ralda_He.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/ralda/test_ralda_Ni.py` & `gpaw-23.6.1/gpaw/test/ralda/test_ralda_Ni.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/hyd_chain_response.py` & `gpaw-23.6.1/gpaw/test/response/hyd_chain_response.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_Na_EELS_RPA_tetra_point_comparison.py` & `gpaw-23.6.1/gpaw/test/response/test_Na_EELS_RPA_tetra_point_comparison.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_WGG_GaAs.py` & `gpaw-23.6.1/gpaw/test/response/test_WGG_GaAs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_afm_hchain_sf_gssALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_afm_hchain_sf_gssALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_aluminum_EELS_ALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_aluminum_EELS_ALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_aluminum_EELS_RPA.py` & `gpaw-23.6.1/gpaw/test/response/test_aluminum_EELS_RPA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_au02_absorption.py` & `gpaw-23.6.1/gpaw/test/response/test_au02_absorption.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_bse_MoS2_cut.py` & `gpaw-23.6.1/gpaw/test/response/test_bse_MoS2_cut.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_bse_aluminum.py` & `gpaw-23.6.1/gpaw/test/response/test_bse_aluminum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_bse_silicon.py` & `gpaw-23.6.1/gpaw/test/response/test_bse_silicon.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_chi0.py` & `gpaw-23.6.1/gpaw/test/response/test_chi0.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_chi0_update.py` & `gpaw-23.6.1/gpaw/test/response/test_chi0_update.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_chiks.py` & `gpaw-23.6.1/gpaw/test/response/test_chiks.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_cobalt_sf_gssALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_cobalt_sf_gssALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_diamond_absorption.py` & `gpaw-23.6.1/gpaw/test/response/test_diamond_absorption.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_graphene.py` & `gpaw-23.6.1/gpaw/test/response/test_graphene.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_graphene_EELS.py` & `gpaw-23.6.1/gpaw/test/response/test_graphene_EELS.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_MoS2_cut.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_MoS2_cut.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_hBN_extrapolate.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_hBN_extrapolate.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_ppa.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_ppa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_restart_file.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_restart_file.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_si.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_spinpol.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_spinpol.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_too.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_too.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_gw_vertex.py` & `gpaw-23.6.1/gpaw/test/response/test_gw_vertex.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_heisenberg.py` & `gpaw-23.6.1/gpaw/test/response/test_heisenberg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_hubbard.py` & `gpaw-23.6.1/gpaw/test/response/test_hubbard.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_ibz2bz.py` & `gpaw-23.6.1/gpaw/test/response/test_ibz2bz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_iron_sf_ALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_iron_sf_ALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_iron_sf_gssALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_iron_sf_gssALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_jdos.py` & `gpaw-23.6.1/gpaw/test/response/test_jdos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_localft.py` & `gpaw-23.6.1/gpaw/test/response/test_localft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_mft.py` & `gpaw-23.6.1/gpaw/test/response/test_mft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_na_plasmon.py` & `gpaw-23.6.1/gpaw/test/response/test_na_plasmon.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_na_plasmons.py` & `gpaw-23.6.1/gpaw/test/response/test_na_plasmons.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_na_plasmons_tetrahedron.py` & `gpaw-23.6.1/gpaw/test/response/test_na_plasmons_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_nicl2_sf_gssALDA.py` & `gpaw-23.6.1/gpaw/test/response/test_nicl2_sf_gssALDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_parallel_kptpair_extraction.py` & `gpaw-23.6.1/gpaw/test/response/test_parallel_kptpair_extraction.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_parallelization.py` & `gpaw-23.6.1/gpaw/test/response/test_parallelization.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_pdens_tool.py` & `gpaw-23.6.1/gpaw/test/response/test_pdens_tool.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_qeh.py` & `gpaw-23.6.1/gpaw/test/response/test_qeh.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_response_band_cutoff.py` & `gpaw-23.6.1/gpaw/test/response/test_response_band_cutoff.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_silicon_chi.py` & `gpaw-23.6.1/gpaw/test/response/test_silicon_chi.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_site_kernels.py` & `gpaw-23.6.1/gpaw/test/response/test_site_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_test_chi0_intraband.py` & `gpaw-23.6.1/gpaw/test/response/test_test_chi0_intraband.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_test_unit_sphere_area.py` & `gpaw-23.6.1/gpaw/test/response/test_test_unit_sphere_area.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_tetra_point_smoothing.py` & `gpaw-23.6.1/gpaw/test/response/test_tetra_point_smoothing.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/response/test_two-aluminum_chi_RPA.py` & `gpaw-23.6.1/gpaw/test/response/test_two-aluminum_chi_RPA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rpa/rpa_C6_He.py` & `gpaw-23.6.1/gpaw/test/rpa/rpa_C6_He.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_N2.py` & `gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_N2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Na.py` & `gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Na.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Ni.py` & `gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Ni.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rpa/test_rpa_energy_Si.py` & `gpaw-23.6.1/gpaw/test/rpa/test_rpa_energy_Si.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rsf_yukawa/test_lrtddft_short.py` & `gpaw-23.6.1/gpaw/test/rsf_yukawa/test_lrtddft_short.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rsf_yukawa/test_rsf_general.py` & `gpaw-23.6.1/gpaw/test/rsf_yukawa/test_rsf_general.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/rsf_yukawa/test_rsf_ivo_sing_mg.py` & `gpaw-23.6.1/gpaw/test/rsf_yukawa/test_rsf_ivo_sing_mg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/setups/test_derivative_integrals.py` & `gpaw-23.6.1/gpaw/test/setups/test_derivative_integrals.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/setups/test_generator2.py` & `gpaw-23.6.1/gpaw/test/setups/test_generator2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/setups/test_setup_basis_spec.py` & `gpaw-23.6.1/gpaw/test/setups/test_setup_basis_spec.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/sic/test_nscfsic.py` & `gpaw-23.6.1/gpaw/test/sic/test_nscfsic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/sic/test_scfsic_h2.py` & `gpaw-23.6.1/gpaw/test/sic/test_scfsic_h2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_adm12.py` & `gpaw-23.6.1/gpaw/test/solvation/test_adm12.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_forces.py` & `gpaw-23.6.1/gpaw/test/solvation/test_forces.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_forces_symmetry.py` & `gpaw-23.6.1/gpaw/test/solvation/test_forces_symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_lrtddft.py` & `gpaw-23.6.1/gpaw/test/solvation/test_lrtddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_nan_radius.py` & `gpaw-23.6.1/gpaw/test/solvation/test_nan_radius.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_overlap.py` & `gpaw-23.6.1/gpaw/test/solvation/test_overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_pbc.py` & `gpaw-23.6.1/gpaw/test/solvation/test_pbc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_pbc_pos_repeat.py` & `gpaw-23.6.1/gpaw/test/solvation/test_pbc_pos_repeat.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_poisson.py` & `gpaw-23.6.1/gpaw/test/solvation/test_poisson.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_sfgcm06.py` & `gpaw-23.6.1/gpaw/test/solvation/test_sfgcm06.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_sjm.py` & `gpaw-23.6.1/gpaw/test/solvation/test_sjm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_solvation_api.py` & `gpaw-23.6.1/gpaw/test/solvation/test_solvation_api.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_spinpol.py` & `gpaw-23.6.1/gpaw/test/solvation/test_spinpol.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_sss09.py` & `gpaw-23.6.1/gpaw/test/solvation/test_sss09.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_swap_atoms.py` & `gpaw-23.6.1/gpaw/test/solvation/test_swap_atoms.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_vacuum.py` & `gpaw-23.6.1/gpaw/test/solvation/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_water_water.py` & `gpaw-23.6.1/gpaw/test/solvation/test_water_water.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/solvation/test_water_water_etdm_lcao.py` & `gpaw-23.6.1/gpaw/test/solvation/test_water_water_etdm_lcao.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/spin/test_spinFe3plus.py` & `gpaw-23.6.1/gpaw/test/spin/test_spinFe3plus.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/spin/test_spin_contamination.py` & `gpaw-23.6.1/gpaw/test/spin/test_spin_contamination.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/spin/test_spinpol.py` & `gpaw-23.6.1/gpaw/test/spin/test_spinpol.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_check.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_check.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations_big.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations_big.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_fractional_translations_med.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_fractional_translations_med.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_kpoint_mapping.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_kpoint_mapping.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_symmetrize_wGG.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_symmetrize_wGG.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_symmetry.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_symmetry2.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_symmetry2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_symmetry_ft.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_symmetry_ft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_usesymm.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_usesymm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/symmetry/test_usesymm2.py` & `gpaw-23.6.1/gpaw/test/symmetry/test_usesymm2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/tddft/test_be_nltd_ip.py` & `gpaw-23.6.1/gpaw/test/tddft/test_be_nltd_ip.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/tddft/test_ehrenfest_nacl.py` & `gpaw-23.6.1/gpaw/test/tddft/test_ehrenfest_nacl.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/tddft/test_fxc_linearize.py` & `gpaw-23.6.1/gpaw/test/tddft/test_fxc_linearize.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/tddft/test_molecule.py` & `gpaw-23.6.1/gpaw/test/tddft/test_molecule.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/tddft/test_td_na2.py` & `gpaw-23.6.1/gpaw/test/tddft/test_td_na2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_AA_enthalpy.py` & `gpaw-23.6.1/gpaw/test/test_AA_enthalpy.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_Gauss.py` & `gpaw-23.6.1/gpaw/test/test_Gauss.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_aeatom.py` & `gpaw-23.6.1/gpaw/test/test_aeatom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_aedensity.py` & `gpaw-23.6.1/gpaw/test/test_aedensity.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_atoms_mismatch.py` & `gpaw-23.6.1/gpaw/test/test_atoms_mismatch.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_broadcast_imports.py` & `gpaw-23.6.1/gpaw/test/test_broadcast_imports.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_cluster.py` & `gpaw-23.6.1/gpaw/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_complex.py` & `gpaw-23.6.1/gpaw/test/test_complex.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_coreeig.py` & `gpaw-23.6.1/gpaw/test/test_coreeig.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_coulomb.py` & `gpaw-23.6.1/gpaw/test/test_coulomb.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_diagonalizer_backend.py` & `gpaw-23.6.1/gpaw/test/test_diagonalizer_backend.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_dipole.py` & `gpaw-23.6.1/gpaw/test/test_dipole.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_dipole_me.py` & `gpaw-23.6.1/gpaw/test/test_dipole_me.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_dipole_new.py` & `gpaw-23.6.1/gpaw/test/test_dipole_new.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_ds_beta.py` & `gpaw-23.6.1/gpaw/test/test_ds_beta.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fermilevel.py` & `gpaw-23.6.1/gpaw/test/test_fermilevel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fermisplit.py` & `gpaw-23.6.1/gpaw/test/test_fermisplit.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fixdensity.py` & `gpaw-23.6.1/gpaw/test/test_fixdensity.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fixdensity_mgga.py` & `gpaw-23.6.1/gpaw/test/test_fixdensity_mgga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fixmom.py` & `gpaw-23.6.1/gpaw/test/test_fixmom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_fixocc.py` & `gpaw-23.6.1/gpaw/test/test_fixocc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_gauss_func.py` & `gpaw-23.6.1/gpaw/test/test_gauss_func.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_gauss_wave.py` & `gpaw-23.6.1/gpaw/test/test_gauss_wave.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_ibzqpt.py` & `gpaw-23.6.1/gpaw/test/test_ibzqpt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_inducedfield_lrtddft.py` & `gpaw-23.6.1/gpaw/test/test_inducedfield_lrtddft.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_inducedfield_td.py` & `gpaw-23.6.1/gpaw/test/test_inducedfield_td.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_initial_occs.py` & `gpaw-23.6.1/gpaw/test/test_initial_occs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_jellium.py` & `gpaw-23.6.1/gpaw/test/test_jellium.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_kpt.py` & `gpaw-23.6.1/gpaw/test/test_kpt.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_kpt_refine.py` & `gpaw-23.6.1/gpaw/test/test_kpt_refine.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_libelpa.py` & `gpaw-23.6.1/gpaw/test/test_libelpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_mpicomm.py` & `gpaw-23.6.1/gpaw/test/test_mpicomm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_muffintinpot.py` & `gpaw-23.6.1/gpaw/test/test_muffintinpot.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_multipoleH2O.py` & `gpaw-23.6.1/gpaw/test/test_multipoleH2O.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_multipoletest.py` & `gpaw-23.6.1/gpaw/test/test_multipoletest.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,14 @@
                 if l == 0:
                     Q0 -= 1.0
                     Q1_m[:] = 0.0
                 elif l == 1:
                     Q1_m[(m + 1) % 3] -= 1.0
                 print(soft, l, m, Q0, Q1_m)
                 assert abs(Q0) < 2e-6
-                assert np.alltrue(abs(Q1_m) < 3e-5)
+                assert (abs(Q1_m) < 3e-5).all()
         b_Lg = np.reshape(a_Lg, (9, -1))
         S_LL = np.inner(b_Lg, b_Lg)
         gd.comm.sum(S_LL)
         S_LL.ravel()[::10] = 0.0
         print(max(abs(S_LL).ravel()))
         assert max(abs(S_LL).ravel()) < 3e-4
```

### Comparing `gpaw-23.6.0/gpaw/test/test_negative_eigerror.py` & `gpaw-23.6.1/gpaw/test/test_negative_eigerror.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_new_calculator.py` & `gpaw-23.6.1/gpaw/test/test_new_calculator.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_occupations.py` & `gpaw-23.6.1/gpaw/test/test_occupations.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_overlap.py` & `gpaw-23.6.1/gpaw/test/test_overlap.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_potential.py` & `gpaw-23.6.1/gpaw/test/test_potential.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_rattle.py` & `gpaw-23.6.1/gpaw/test/test_rattle.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_reuse_wfs.py` & `gpaw-23.6.1/gpaw/test/test_reuse_wfs.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_reuse_wfs_celldisp.py` & `gpaw-23.6.1/gpaw/test/test_reuse_wfs_celldisp.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_scf_criteria.py` & `gpaw-23.6.1/gpaw/test/test_scf_criteria.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_spectrum.py` & `gpaw-23.6.1/gpaw/test/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_spherical_harmonics.py` & `gpaw-23.6.1/gpaw/test/test_spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_spinorbit_Kr.py` & `gpaw-23.6.1/gpaw/test/test_spinorbit_Kr.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_stdout.py` & `gpaw-23.6.1/gpaw/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_timelimit.py` & `gpaw-23.6.1/gpaw/test/test_timelimit.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_timing.py` & `gpaw-23.6.1/gpaw/test/test_timing.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_too_close.py` & `gpaw-23.6.1/gpaw/test/test_too_close.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_vdwradii.py` & `gpaw-23.6.1/gpaw/test/test_vdwradii.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/test_watermodel.py` & `gpaw-23.6.1/gpaw/test/test_watermodel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_eed.py` & `gpaw-23.6.1/gpaw/test/utilities/test_eed.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_elf.py` & `gpaw-23.6.1/gpaw/test/utilities/test_elf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_ewald.py` & `gpaw-23.6.1/gpaw/test/utilities/test_ewald.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_ldos.py` & `gpaw-23.6.1/gpaw/test/utilities/test_ldos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_partitioning.py` & `gpaw-23.6.1/gpaw/test/utilities/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_simple_stm.py` & `gpaw-23.6.1/gpaw/test/utilities/test_simple_stm.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/utilities/test_wannier_ethylene.py` & `gpaw-23.6.1/gpaw/test/utilities/test_wannier_ethylene.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_H_Hirshfeld.py` & `gpaw-23.6.1/gpaw/test/vdw/test_H_Hirshfeld.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_ar2.py` & `gpaw-23.6.1/gpaw/test/vdw/test_ar2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_functionals.py` & `gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_functionals.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_h2.py` & `gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_h2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_mbeef.py` & `gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_mbeef.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_libvdwxc_spin.py` & `gpaw-23.6.1/gpaw/test/vdw/test_libvdwxc_spin.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_potential.py` & `gpaw-23.6.1/gpaw/test/vdw/test_potential.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_quick_spin.py` & `gpaw-23.6.1/gpaw/test/vdw/test_quick_spin.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/vdw/test_ts09.py` & `gpaw-23.6.1/gpaw/test/vdw/test_ts09.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_XC2.py` & `gpaw-23.6.1/gpaw/test/xc/test_XC2.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_atomize.py` & `gpaw-23.6.1/gpaw/test/xc/test_atomize.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_beef.py` & `gpaw-23.6.1/gpaw/test/xc/test_beef.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_degeneracy.py` & `gpaw-23.6.1/gpaw/test/xc/test_degeneracy.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_gga_atom.py` & `gpaw-23.6.1/gpaw/test/xc/test_gga_atom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_lb94.py` & `gpaw-23.6.1/gpaw/test/xc/test_lb94.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_lxc_xcatom.py` & `gpaw-23.6.1/gpaw/test/xc/test_lxc_xcatom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_nonselfconsistent.py` & `gpaw-23.6.1/gpaw/test/xc/test_nonselfconsistent.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_nonselfconsistentLDA.py` & `gpaw-23.6.1/gpaw/test/xc/test_nonselfconsistentLDA.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_pbe_pw91.py` & `gpaw-23.6.1/gpaw/test/xc/test_pbe_pw91.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_pplda.py` & `gpaw-23.6.1/gpaw/test/xc/test_pplda.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_pygga.py` & `gpaw-23.6.1/gpaw/test/xc/test_pygga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_qna_band.py` & `gpaw-23.6.1/gpaw/test/xc/test_qna_band.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_qna_force.py` & `gpaw-23.6.1/gpaw/test/xc/test_qna_force.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_qna_spinpol.py` & `gpaw-23.6.1/gpaw/test/xc/test_qna_spinpol.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_qna_stress.py` & `gpaw-23.6.1/gpaw/test/xc/test_qna_stress.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_revPBE.py` & `gpaw-23.6.1/gpaw/test/xc/test_revPBE.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_revPBE_Li.py` & `gpaw-23.6.1/gpaw/test/xc/test_revPBE_Li.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_tb09.py` & `gpaw-23.6.1/gpaw/test/xc/test_tb09.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_tpss.py` & `gpaw-23.6.1/gpaw/test/xc/test_tpss.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_xc.py` & `gpaw-23.6.1/gpaw/test/xc/test_xc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/test/xc/test_xcatom.py` & `gpaw-23.6.1/gpaw/test/xc/test_xcatom.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/tetrahedron.py` & `gpaw-23.6.1/gpaw/tetrahedron.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/transformers.py` & `gpaw-23.6.1/gpaw/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             outpoints = gdout.n_c[0] * gdout.n_c[1]
 
             if inpoints > outpoints:
                 points = ' x '.join([str(N) for N in gdin.N_c])
                 raise ValueError('Cannot construct interpolator.  Grid %s '
                                  'may be too small' % points)
 
-        assert np.alltrue(pad_cd.ravel() >= 0)
+        assert (pad_cd.ravel() >= 0).all()
         self.ngpin = tuple(gdin.n_c)
         self.ngpout = tuple(gdout.n_c)
         assert dtype in [float, complex]
 
         self.pad_cd = pad_cd
         self.neighborpad_cd = neighborpad_cd
         self.skip_cd = skip_cd
```

### Comparing `gpaw-23.6.0/gpaw/unfold.py` & `gpaw-23.6.1/gpaw/unfold.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/upf.py` & `gpaw-23.6.1/gpaw/upf.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/__init__.py` & `gpaw-23.6.1/gpaw/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/bader.py` & `gpaw-23.6.1/gpaw/utilities/bader.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/blas.py` & `gpaw-23.6.1/gpaw/utilities/blas.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/cg.py` & `gpaw-23.6.1/gpaw/utilities/cg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/debug.py` & `gpaw-23.6.1/gpaw/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/dipole.py` & `gpaw-23.6.1/gpaw/utilities/dipole.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/dos.py` & `gpaw-23.6.1/gpaw/utilities/dos.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/ekin.py` & `gpaw-23.6.1/gpaw/utilities/ekin.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/elpa.py` & `gpaw-23.6.1/gpaw/utilities/elpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/ewald.py` & `gpaw-23.6.1/gpaw/utilities/ewald.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/extend_grid.py` & `gpaw-23.6.1/gpaw/utilities/extend_grid.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/extrapolate.py` & `gpaw-23.6.1/gpaw/utilities/extrapolate.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/folder.py` & `gpaw-23.6.1/gpaw/utilities/folder.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/gauss.py` & `gpaw-23.6.1/gpaw/utilities/gauss.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/gl_quadrature.py` & `gpaw-23.6.1/gpaw/utilities/gl_quadrature.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/gpts.py` & `gpaw-23.6.1/gpaw/utilities/gpts.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/grid.py` & `gpaw-23.6.1/gpaw/utilities/grid.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/grid_redistribute.py` & `gpaw-23.6.1/gpaw/utilities/grid_redistribute.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/hardware.py` & `gpaw-23.6.1/gpaw/utilities/hardware.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/hilbert.py` & `gpaw-23.6.1/gpaw/utilities/hilbert.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/ibz2bz.py` & `gpaw-23.6.1/gpaw/utilities/ibz2bz.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/kspot.py` & `gpaw-23.6.1/gpaw/utilities/kspot.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/memory.py` & `gpaw-23.6.1/gpaw/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/nbrun.py` & `gpaw-23.6.1/gpaw/utilities/nbrun.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/newrelease.py` & `gpaw-23.6.1/gpaw/utilities/newrelease.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/partition.py` & `gpaw-23.6.1/gpaw/utilities/partition.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/progressbar.py` & `gpaw-23.6.1/gpaw/utilities/progressbar.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/ps2ae.py` & `gpaw-23.6.1/gpaw/utilities/ps2ae.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/pw.py` & `gpaw-23.6.1/gpaw/utilities/pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/scalapack.py` & `gpaw-23.6.1/gpaw/utilities/scalapack.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/sic.py` & `gpaw-23.6.1/gpaw/utilities/sic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/timelimit.py` & `gpaw-23.6.1/gpaw/utilities/timelimit.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/timing.py` & `gpaw-23.6.1/gpaw/utilities/timing.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/tools.py` & `gpaw-23.6.1/gpaw/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/urlcheck.py` & `gpaw-23.6.1/gpaw/utilities/urlcheck.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/utilities/watermodel.py` & `gpaw-23.6.1/gpaw/utilities/watermodel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wannier/edmiston_ruedenberg.py` & `gpaw-23.6.1/gpaw/wannier/edmiston_ruedenberg.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wannier/functions.py` & `gpaw-23.6.1/gpaw/wannier/functions.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wannier/overlaps.py` & `gpaw-23.6.1/gpaw/wannier/overlaps.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wannier/w90.py` & `gpaw-23.6.1/gpaw/wannier/w90.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wannier90.py` & `gpaw-23.6.1/gpaw/wannier90.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/arrays.py` & `gpaw-23.6.1/gpaw/wavefunctions/arrays.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/base.py` & `gpaw-23.6.1/gpaw/wavefunctions/base.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/fd.py` & `gpaw-23.6.1/gpaw/wavefunctions/fd.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/fdpw.py` & `gpaw-23.6.1/gpaw/wavefunctions/fdpw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/lcao.py` & `gpaw-23.6.1/gpaw/wavefunctions/lcao.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/mode.py` & `gpaw-23.6.1/gpaw/wavefunctions/mode.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wavefunctions/pw.py` & `gpaw-23.6.1/gpaw/wavefunctions/pw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/wfd_operators.py` & `gpaw-23.6.1/gpaw/wfd_operators.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xas.py` & `gpaw-23.6.1/gpaw/xas.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/__init__.py` & `gpaw-23.6.1/gpaw/xc/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/bee.py` & `gpaw-23.6.1/gpaw/xc/bee.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/functional.py` & `gpaw-23.6.1/gpaw/xc/functional.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/fxc.py` & `gpaw-23.6.1/gpaw/xc/fxc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/fxc_kernels.py` & `gpaw-23.6.1/gpaw/xc/fxc_kernels.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gga.py` & `gpaw-23.6.1/gpaw/xc/gga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/c_gllbscr.py` & `gpaw-23.6.1/gpaw/xc/gllb/c_gllbscr.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/c_response.py` & `gpaw-23.6.1/gpaw/xc/gllb/c_response.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/c_xc.py` & `gpaw-23.6.1/gpaw/xc/gllb/c_xc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/coefficients.py` & `gpaw-23.6.1/gpaw/xc/gllb/coefficients.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/contribution.py` & `gpaw-23.6.1/gpaw/xc/gllb/contribution.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/nonlocalfunctional.py` & `gpaw-23.6.1/gpaw/xc/gllb/nonlocalfunctional.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/gllb/nonlocalfunctionalfactory.py` & `gpaw-23.6.1/gpaw/xc/gllb/nonlocalfunctionalfactory.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/hybrid.py` & `gpaw-23.6.1/gpaw/xc/hybrid.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/kernel.py` & `gpaw-23.6.1/gpaw/xc/kernel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/lb94.py` & `gpaw-23.6.1/gpaw/xc/lb94.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/lda.py` & `gpaw-23.6.1/gpaw/xc/lda.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/libvdwxc.py` & `gpaw-23.6.1/gpaw/xc/libvdwxc.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         self.timer.stop('redistribute')
         return energy
 
 
 class FFTDistribution:
     def __init__(self, gd, parsize_c):
         self.input_gd = gd
-        assert np.product(parsize_c) == gd.comm.size
+        assert np.prod(parsize_c) == gd.comm.size
         self.local_input_size_c = gd.n_c
         self.domains_in = Domains(gd.n_cp)
         N_c = gd.get_size_of_global_array(pad=True)
         self.domains_out = Domains([get_domains(N_c[i], parsize_c[i])
                                     for i in range(3)])
 
         if parsize_c[1] == 1 and parsize_c[2] == 1:
@@ -648,15 +648,15 @@
         v2x[:] += 0.5 * Ax * df_ds / (s_prefactor * grad_rho)
         # (We may or may not understand what that grad_rho is doing here.)
 
 
 def test_derivatives():
     gen = np.random.RandomState(1)
     shape = (1, 20, 20, 20)
-    ngpts = np.product(shape)
+    ngpts = np.prod(shape)
     n_sg = gen.rand(*shape)
     sigma_xg = np.zeros(shape)
     sigma_xg[:] = gen.rand(*shape)
 
     qe_kernel = CXGGAKernel(just_kidding=True)
     libxc_kernel = LibXC('GGA_X_RPW86+LDA_C_PW')
```

### Comparing `gpaw-23.6.0/gpaw/xc/libxc.py` & `gpaw-23.6.1/gpaw/xc/libxc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/mgga.py` & `gpaw-23.6.1/gpaw/xc/mgga.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/noncollinear.py` & `gpaw-23.6.1/gpaw/xc/noncollinear.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/parametrizedxc.py` & `gpaw-23.6.1/gpaw/xc/parametrizedxc.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/pawcorrection.py` & `gpaw-23.6.1/gpaw/xc/pawcorrection.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/qna.py` & `gpaw-23.6.1/gpaw/xc/qna.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/ri/__init__.py` & `gpaw-23.6.1/gpaw/xc/ri/__init__.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/ri/ribasis.py` & `gpaw-23.6.1/gpaw/xc/ri/ribasis.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/ri/spherical_hse_kernel.py` & `gpaw-23.6.1/gpaw/xc/ri/spherical_hse_kernel.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/rpa.py` & `gpaw-23.6.1/gpaw/xc/rpa.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/sic.py` & `gpaw-23.6.1/gpaw/xc/sic.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/tb09.py` & `gpaw-23.6.1/gpaw/xc/tb09.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/tools.py` & `gpaw-23.6.1/gpaw/xc/tools.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/xc/vdw.py` & `gpaw-23.6.1/gpaw/xc/vdw.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/yml.py` & `gpaw-23.6.1/gpaw/yml.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw/zero_field_splitting.py` & `gpaw-23.6.1/gpaw/zero_field_splitting.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/gpaw.egg-info/PKG-INFO` & `gpaw-23.6.1/gpaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpaw
-Version: 23.6.0
+Version: 23.6.1
 Summary: GPAW: DFT and beyond within the projector-augmented wave method
 Home-page: https://wiki.fysik.dtu.dk/gpaw
 Maintainer: GPAW-community
 Maintainer-email: gpaw-users@listserv.fysik.dtu.dk
 License: GPLv3+
 Platform: unix
 Classifier: Development Status :: 6 - Mature
```

### Comparing `gpaw-23.6.0/gpaw.egg-info/SOURCES.txt` & `gpaw-23.6.1/gpaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/setup.py` & `gpaw-23.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/siteconfig_example.py` & `gpaw-23.6.1/siteconfig_example.py`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/tools/gpaw-plot-parallel-timings` & `gpaw-23.6.1/tools/gpaw-plot-parallel-timings`

 * *Files identical despite different names*

### Comparing `gpaw-23.6.0/tools/gpaw-runscript` & `gpaw-23.6.1/tools/gpaw-runscript`

 * *Files identical despite different names*

