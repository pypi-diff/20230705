# Comparing `tmp/fastsim-2.0.22.tar.gz` & `tmp/fastsim-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsim-2.0.22.tar", last modified: Thu Apr 20 18:32:40 2023, max compression
+gzip compressed data, was "fastsim-2.1.0.tar", last modified: Wed Jul  5 20:03:19 2023, max compression
```

## Comparing `fastsim-2.0.22.tar` & `fastsim-2.1.0.tar`

### file list

```diff
@@ -1,272 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.619307 fastsim-2.0.22/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-20 18:32:30.000000 fastsim-2.0.22/BUILD.md
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-20 18:32:30.000000 fastsim-2.0.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-20 18:32:30.000000 fastsim-2.0.22/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-20 18:32:30.000000 fastsim-2.0.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-20 18:32:40.619307 fastsim-2.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-04-20 18:32:30.000000 fastsim-2.0.22/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-20 18:32:30.000000 fastsim-2.0.22/build_and_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.563306 fastsim-2.0.22/fastsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    37910 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/cycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.567306 fastsim-2.0.22/fastsim/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/2017_Ford_F150_thermal_val.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/accel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/demo_abc_drag_coef_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/demo_eu_vehicle_wltp.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/fastsim-icon-web-131x172.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/fusion_thermal_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/fusion_thermal_cal_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/fusion_thermal_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/mp_parallel_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/stop_start_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/time_dilation_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/docs/wltc_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/inspect_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.567306 fastsim-2.0.22/fastsim/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/FASTSim_py_veh_db.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.575306 fastsim-2.0.22/fastsim/resources/cycles/
--rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/NREL13.csv
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/accel.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.559306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.575306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.575306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/
--rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
--rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.575306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4105836_2/
--rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.579306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/
--rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.583306 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/
--rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.587307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/
--rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
--rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.587307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/
--rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.591307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/
--rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
--rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
--rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.591307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/
--rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
--rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.591307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4113492_1/
--rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.591307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4114555_1/
--rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_1/
--rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_2/
--rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115957_1/
--rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115985_1/
--rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116361_1/
--rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.595307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116721_2/
--rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.599307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116728_1/
--rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.599307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_1/
--rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.599307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_2/
--rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.599307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116880_1/
--rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.599307 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/
--rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
--rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
--rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/ftpmc1b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/hwfet.csv
--rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/longHaulDriveCycle.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/udds.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/us06.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_extra_high3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_high3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_high3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_low3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_med3a.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_med3b.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wmtc_all.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wmtc_part1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wmtc_part2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/cycles/wmtc_part3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/longparams.json
--rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/master_benchmark_vars.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/res_excel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.607307 fastsim-2.0.22/fastsim/resources/vehdb/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Focus.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Focus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Fusion.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Class_4_Box_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Line_Haul_Conv.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Line_Haul_Conv.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/fail_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/fail_overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/legacy_template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/legacy_template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/template.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/test_overrides.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/test_overrides.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.607307 fastsim-2.0.22/fastsim/resources/vehdb/thermal/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/rustext.py
--rw-r--r--   0 runner    (1001) docker     (123)   116204 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/simdrivelabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/fastsim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_auxiliaries.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_cav_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_cav_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)    60185 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_coasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_eco_cruise.py
--rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_following.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15838 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_rust.py
--rw-r--r--   0 runner    (1001) docker     (123)    10689 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_simdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_simdrive_sweep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_soc_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/tests/test_vs_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33293 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-20 18:32:30.000000 fastsim-2.0.22/fastsim/vehicle_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.563306 fastsim-2.0.22/fastsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 18:32:40.000000 fastsim-2.0.22/fastsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 18:32:30.000000 fastsim-2.0.22/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/rust/fastsim-cli/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-cli/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.559306 fastsim-2.0.22/rust/fastsim-cli/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/rust/fastsim-cli/src/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-cli/src/bin/fastsim-cli.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/rust/fastsim-core/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.611307 fastsim-2.0.22/rust/fastsim-core/proc-macros/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.615307 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/proc-macros/src/utilities.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.615307 fastsim-2.0.22/rust/fastsim-core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/air.rs
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/cycle.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.615307 fastsim-2.0.22/rust/fastsim-core/src/html/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/html/docs-header.html
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/imports.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/macros.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/pyo3imports.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.619307 fastsim-2.0.22/rust/fastsim-core/src/simdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/simdrive/cyc_mods.rs
--rw-r--r--   0 runner    (1001) docker     (123)    77871 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/simdrive/simdrive_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/simdrive.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41715 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/simdrivelabel.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48266 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14064 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)    59542 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/vehicle.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17999 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/vehicle_thermal.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-core/src/vehicle_utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.619307 fastsim-2.0.22/rust/fastsim-py/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:32:40.619307 fastsim-2.0.22/rust/fastsim-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-20 18:32:30.000000 fastsim-2.0.22/rust/fastsim-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:32:40.619307 fastsim-2.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-20 18:32:30.000000 fastsim-2.0.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-05 20:01:16.000000 fastsim-2.1.0/BUILD.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-05 20:01:16.000000 fastsim-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-05 20:01:16.000000 fastsim-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-05 20:01:16.000000 fastsim-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-05 20:03:19.302652 fastsim-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-05 20:01:16.000000 fastsim-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-07-05 20:01:16.000000 fastsim-2.1.0/build_and_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.250649 fastsim-2.1.0/fastsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:03:19.000000 fastsim-2.1.0/fastsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-05 20:01:16.000000 fastsim-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.242648 fastsim-2.1.0/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.246649 fastsim-2.1.0/python/fastsim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.254649 fastsim-2.1.0/python/fastsim/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/2017_Ford_F150_thermal_val.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/accel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/cav_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/cav_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27541 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/demo_abc_drag_coef_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/demo_eu_vehicle_wltp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/fastsim-icon-web-131x172.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/fusion_thermal_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/fusion_thermal_cal_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/fusion_thermal_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/mp_parallel_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/stop_start_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/time_dilation_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/demos/wltc_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.254649 fastsim-2.1.0/python/fastsim/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/FASTSim_py_veh_db.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.262649 fastsim-2.1.0/python/fastsim/resources/cycles/
+-rw-r--r--   0 runner    (1001) docker     (123)    49682 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/HHDDTCruiseSmooth.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/NREL13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/accel.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.246649 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.262649 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.262649 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/
+-rw-r--r--   0 runner    (1001) docker     (123)   149857 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   240397 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318393 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    66850 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56703 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.266650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4105836_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   175923 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.266650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   143524 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   254608 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   358839 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   261035 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   578615 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   152533 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    62840 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   154950 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.274650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/
+-rw-r--r--   0 runner    (1001) docker     (123)  1380121 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   449212 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   318370 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  1381956 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48275 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114099 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.274650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   447581 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   176220 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   480975 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    49873 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.278650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    84156 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   118485 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106313 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   142029 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   149249 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    87544 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   106482 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.278650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    92398 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50999 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   109463 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    52807 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.278650 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   103811 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   113799 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    45830 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4113492_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   123630 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4114555_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   215417 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   916166 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   186344 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30353 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115957_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   414317 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.282651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115985_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34877 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15032 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116361_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   127523 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116721_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   307321 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116728_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   213547 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   362996 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    31394 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_2/
+-rw-r--r--   0 runner    (1001) docker     (123)   457419 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39844 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.286651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116880_1/
+-rw-r--r--   0 runner    (1001) docker     (123)    58973 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.290651 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/
+-rw-r--r--   0 runner    (1001) docker     (123)   194122 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41186 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    32224 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/ftpmc1b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/hwfet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  2119331 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/longHaulDriveCycle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/udds.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/us06.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_extra_high3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_high3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_high3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_low3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_med3a.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_med3b.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_all.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20507 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/longparams.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64802 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/master_benchmark_vars.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/res_excel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/python/fastsim/resources/vehdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Focus.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Focus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Fusion.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Fusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Class_4_Box_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Class_4_Box_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Line_Haul_Conv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Line_Haul_Conv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/fail_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/fail_overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/legacy_template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/legacy_template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/template.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/test_overrides.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/test_overrides.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/python/fastsim/resources/vehdb/thermal/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-05 20:01:16.000000 fastsim-2.1.0/python/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/fastsim-cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-cli/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.246649 fastsim-2.1.0/rust/fastsim-cli/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/fastsim-cli/src/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    18323 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-cli/src/bin/fastsim-cli.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/fastsim-core/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/fastsim-core/proc-macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.298651 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/proc-macros/src/utilities.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/rust/fastsim-core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/air.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    38619 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/cycle.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/rust/fastsim-core/src/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/html/docs-header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/imports.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/macros.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/pyo3imports.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/rust/fastsim-core/src/simdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    47388 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/simdrive/cyc_mods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    77870 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/simdrive/simdrive_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    21488 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/simdrive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    45055 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/simdrivelabel.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    48334 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14402 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    43972 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/vehicle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/vehicle_thermal.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-core/src/vehicle_utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/rust/fastsim-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:03:19.302652 fastsim-2.1.0/rust/fastsim-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-05 20:01:16.000000 fastsim-2.1.0/rust/fastsim-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 20:03:19.302652 fastsim-2.1.0/setup.cfg
```

### Comparing `fastsim-2.0.22/BUILD.md` & `fastsim-2.1.0/BUILD.md`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/LICENSE` & `fastsim-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/LICENSE.md` & `fastsim-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/PKG-INFO` & `fastsim-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.22
+Version: 2.1.0
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -58,37 +58,28 @@
 
 - Command Prompt (windows):
     1. Create: `python -m venv fastsim-venv` -- name is user decision
     1. Activate: `fastsim-venv/Scripts/activate.bat`
 
 ## FASTSim
 ### Via PyPI
-In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
+In an active Python environment created above, run `pip install fastsim`.
 
 ### Building from Scratch
-Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
+Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  To do this, you'll need to have the [Rust toolchain](https://www.rust-lang.org/tools/install) installed.
 
-- Easy way: run `sh build_and_test.sh` in root folder.  
-- Hard way (a couple of extra steps are required): 
-    1. First install the python code in place:  
-    `DEVELOP_MODE=True pip install -e ".[dev]"`   
-    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
-    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-    1. Within the same python environment, navigate to `fastsim/rust/` and run  
-    `pip install maturin`.
-    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
-
-After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
-
-### Testing
-At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
+- Option 1: run `sh build_and_test.sh` in root folder.  
+- Option 2:  
+    1. Run `pip install -e ".[dev]"`  
+    Optional testing steps:
+    1. Run `cd rust/ && cargo test`
+    1. Run `pytest -v python/fastsim/tests/`
 
 # Usage
-To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
+To see and run examples, navigate to `./python/fastsim/demos` and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
 
 # Adding FASTSim as a Depency in Rust
 ## Via GitHub
 Add this line:  
 `fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
 to your Cargo.toml file, modifying the `branch` key as appropriate.  
@@ -122,14 +113,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
+2.1.0 -- release and installation improvements, RustVehicle init cleanup, calibration improvements
 2.0.11 - 2.0.22 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`
```

### Comparing `fastsim-2.0.22/README.md` & `fastsim-2.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -26,37 +26,28 @@
 
 - Command Prompt (windows):
     1. Create: `python -m venv fastsim-venv` -- name is user decision
     1. Activate: `fastsim-venv/Scripts/activate.bat`
 
 ## FASTSim
 ### Via PyPI
-In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
+In an active Python environment created above, run `pip install fastsim`.
 
 ### Building from Scratch
-Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
+Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  To do this, you'll need to have the [Rust toolchain](https://www.rust-lang.org/tools/install) installed.
 
-- Easy way: run `sh build_and_test.sh` in root folder.  
-- Hard way (a couple of extra steps are required): 
-    1. First install the python code in place:  
-    `DEVELOP_MODE=True pip install -e ".[dev]"`   
-    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
-    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-    1. Within the same python environment, navigate to `fastsim/rust/` and run  
-    `pip install maturin`.
-    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
-
-After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
-
-### Testing
-At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
+- Option 1: run `sh build_and_test.sh` in root folder.  
+- Option 2:  
+    1. Run `pip install -e ".[dev]"`  
+    Optional testing steps:
+    1. Run `cd rust/ && cargo test`
+    1. Run `pytest -v python/fastsim/tests/`
 
 # Usage
-To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
+To see and run examples, navigate to `./python/fastsim/demos` and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
 
 # Adding FASTSim as a Depency in Rust
 ## Via GitHub
 Add this line:  
 `fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
 to your Cargo.toml file, modifying the `branch` key as appropriate.  
@@ -90,14 +81,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
+2.1.0 -- release and installation improvements, RustVehicle init cleanup, calibration improvements
 2.0.11 - 2.0.22 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`
```

### Comparing `fastsim-2.0.22/fastsim/cycle.py` & `fastsim-2.1.0/rust/fastsim-core/src/cycle.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,1033 +1,1099 @@
-"""Module containing classes and methods for cycle data."""
+//! Module containing drive cycle struct and related functions.
 
-from __future__ import annotations
-from typing_extensions import Self
-from typing import Dict, Set, Optional, Any
-# Import necessary python modules
-from dataclasses import dataclass
-import copy
-import cmath
-import os
-import numpy as np
-from scipy.interpolate import interp1d
-import pandas as pd
-from pathlib import Path
-from copy import deepcopy
-
-# local modules
-from . import parameters as params
-from . import inspect_utils
-from .rustext import RUST_AVAILABLE
-
-if RUST_AVAILABLE:
-    import fastsimrust as fsr
-    from fastsimrust import RustCycle
-
-# Logging
-import logging
-logger = logging.getLogger(__name__)
-
-THIS_DIR = Path(__file__).parent
-CYCLES_DIR = THIS_DIR / 'resources' / 'cycles'
-
-# dicts for switching between legacy and new cycle keys
-OLD_TO_NEW = {
-    'cycSecs': 'time_s',
-    'cycMps': 'mps',
-    'cycGrade': 'grade',
-    'cycRoadType': 'road_type',
-    'name': 'name'
-}
-NEW_TO_OLD = {val: key for key, val in OLD_TO_NEW.items()}
-STANDARD_CYCLE_KEYS = OLD_TO_NEW.values()
-
-class CycleCache:
-    grade_all_zero: bool
-    trapz_step_distances_m: np.ndarray(1, dtype=float)
-    trapz_distances_m: np.ndarray(1, dtype=float)
-    trapz_elevations_m: np.ndarray(1, dtype=float)
-    stops: np.ndarray(False, dtype=bool)
-    _interp_ds: np.ndarray(1, dtype=float)
-    _interp_is: np.ndarray(1, dtype=float)
-    _interp_hs: np.ndarray(1, dtype=float)
-    _grades: np.ndarray(1, dtype=float)
-
-    def __init__(self, cyc: Cycle):
-        tol = 1e-6
-        self.grade_all_zero = (np.array(cyc.grade) == 0.0).all()
-        self.trapz_step_distances_m = trapz_step_distances(cyc)
-        self.trapz_distances_m = self.trapz_step_distances_m.cumsum()
-        if (self.grade_all_zero):
-            self.trapz_elevations_m = np.zeros(len(cyc.time_s))
-        else:
-            self.trapz_elevations_m = np.cumsum(np.cos(np.arctan(cyc.grade)) * self.trapz_step_distances_m * np.array(cyc.grade))
-        self.stops = np.array(cyc.mps) <= tol
-        interp_ds = []
-        interp_is = []
-        interp_hs = []
-        for (idx, d) in enumerate(self.trapz_distances_m):
-            if len(interp_ds) == 0 or d > interp_ds[-1]:
-                interp_ds.append(d)
-                interp_is.append(idx)
-                interp_hs.append(self.trapz_elevations_m[idx])
-        self._interp_ds = np.array(interp_ds, dtype=float)
-        self._interp_is = np.array(interp_is, dtype=float)
-        self._interp_hs = np.array(interp_hs, dtype=float)
-        self._grades = np.copy(cyc.grade)
-
-    def interp_grade(self, dist: float):
-        """
-        Interpolate the single-point grade at the given distance.
-        Assumes that the grade at i applies from sample point (i-1, i]
-        """
-        if self.grade_all_zero:
-            return 0.0
-        if dist <= self._interp_ds[0]:
-            return self._grades[0]
-        if dist > self._interp_ds[-1]:
-            return self._grades[-1]
-        idx = int(np.ceil(np.interp(dist, self._interp_ds, self._interp_is)))
-        return self._grades[idx]
-    
-    def interp_elevation(self, dist: float):
-        """
-        Interpolate the elevation at the given distance
-        """
-        if self.grade_all_zero:
-            return 0.0
-        return np.interp(dist, self._interp_ds, self._interp_hs)
-
-
-@dataclass
-class Cycle(object):
-    """Object for containing time, speed, road grade, and road charging vectors 
-    for drive cycle.  Instantiate with the `from_file` or `from_dict` method.  
-    """
-
-    time_s: np.ndarray(1, dtype=float)
-    mps: np.ndarray(1, dtype=float)
-    grade: np.ndarray(1, dtype=float)
-    road_type: np.ndarray(1, dtype=float)
-    name: str
-
-    @classmethod
-    def from_file(cls, filename: str) -> Self:
-        """
-        Load cycle from filename (str).
-        Can be absolute or relative path.  If relative, looks in working dir first
-        and then in `fastsim/resources/cycles`.  
-
-        File must contain columns for:
-        -- `cycSecs` or `time_s`
-        -- `cycMps` or `mps`
-        -- `cycGrade` or `grade` (optional)
-        -- `cycRoadType` or `road_type` (optional)
-        """
-        filename = str(filename)
-
-        if not filename.endswith('.csv'):
-            filename += ".csv"
-        if not Path(filename).exists() and (CYCLES_DIR / filename).exists():
-            filename = CYCLES_DIR / filename
-        elif Path(filename).exists():
-            filename = Path(filename)
-        else:
-            raise ValueError("Invalid cycle filename.")
-
-        cyc_df = pd.read_csv(filename)
-        cyc_dict = cyc_df.to_dict(orient='list')
-        cyc_dict = {key: np.array(val, dtype=float)
-                    for key, val in cyc_dict.items()}
-        cyc_dict['name'] = filename.stem
-
-        return cls.from_dict(cyc_dict)
-
-    @classmethod
-    def from_dict(cls, cyc_dict: dict) -> Self:
-        """
-        Load cycle from dict, which must contain keys for:
-        -- `cycSecs` or `time_s`
-        -- `cycMps` or `mps`
-        -- `cycGrade` or `grade` (optional)
-        -- `cycRoadType` or `road_type` (optional)
-        """
-        new_cyc_dict = {}
-        for key, val in cyc_dict.items():
-            # generate keys from legacy or current mapping
-            new_key = OLD_TO_NEW.get(key, key)
-            if new_key == 'name':
-                aval = val
-            else:
-                try:
-                    aval = np.array(val, dtype=float)
-                except Exception:
-                    aval = val
-            new_cyc_dict[new_key] = aval
-        new_cyc_dict['name'] = cyc_dict.get('name', '')
-        # set zeros if not provided
-        new_cyc_dict['grade'] = new_cyc_dict.get(
-            'grade', np.zeros(len(new_cyc_dict['time_s'])))
-        new_cyc_dict['road_type'] = new_cyc_dict.get(
-            'road_type', np.zeros(len(new_cyc_dict['time_s'])))
-
-        # check for invalid keys
-        assert len(set(new_cyc_dict.keys()) - set(STANDARD_CYCLE_KEYS)) == 0
-        return cls(**new_cyc_dict)
-
-    def get_numba_cyc(self):
-        """Deprecated."""
-        raise NotImplementedError(
-            "This method has been deprecated.")
-
-    def build_cache(self) -> CycleCache:
-        """
-        Calculates a dataclass containing expensive-to-calculate items. The data created
-        can persist between calls and optionally be passed into methods that can use
-        it which will result in a performance enhancement.
-        RETURN: CycleCache
-        """
-        return CycleCache(self)
-
-    # Properties
-
-    def get_mph(self) -> np.ndarray:
-        return self.mps * params.MPH_PER_MPS
-
-    def set_mph(self, new_value):
-        self.mps = new_value / params.MPH_PER_MPS
-
-    mph = property(get_mph, set_mph)
-
-    # time step deltas
-    @property
-    def dt_s(self) -> np.ndarray:
-        return np.array(np.diff(self.time_s, prepend=0), dtype=float)
-
-    def dt_s_at_i(self, i: int) -> float:
-        """
-        Calculate the time-step duration for time-step `i`.
-        Returns: the time-step duration in seconds
-        """
-        if i < 1:
-            return 0.0
-        return self.time_s[i] - self.time_s[i - 1]
-
-    # distance at each time step
-    @property
-    def dist_m(self) -> np.ndarray:
-        return self.mps * self.dt_s
-
-    @property
-    def delta_elev_m(self) -> np.ndarray:
-        """
-        Cumulative elevation change w.r.t. to initial
-        """
-        return (self.dist_m * self.grade).cumsum()
-
-    @property
-    def len(self) -> int:
-        "return cycle length"
-        return len(self.time_s)
-
-    def get_cyc_dict(self) -> Dict[str, np.ndarray]:
-        """Returns cycle as dict rather than class instance."""
-        keys = STANDARD_CYCLE_KEYS
-
-        cyc = {}
-        for key in keys:
-            cyc[key] = copy.deepcopy(self.__getattribute__(key))
-
-        return cyc
-
-    def to_rust(self) -> RustCycle:
-        return copy_cycle(self, return_type='rust', deep=False)
-
-    def reset_orphaned(self):
-        """Dummy method for flexibility between Rust/Python version interfaces"""
-        pass
-
-    def copy(self) -> Self:
-        """
-        Return a copy of this Cycle instance.
-        """
-        return copy.deepcopy(self)
-
-    def average_grade_over_range(self, distance_start_m, delta_distance_m, cache:Optional[CycleCache]=None):
-        """
-        Returns the average grade over the given range of distances
-        - distance_start_m: non-negative-number, the distance at start of evaluation area (m)
-        - delta_distance_m: non-negative-number, the distance traveled from distance_start_m (m)
-        RETURN: number, the average grade (rise over run) over the given distance range
-        Note: grade is assumed to be constant from just after the previous sample point
-        until the current sample point. That is, grade[i] applies over the range of
-        distances, d, from (d[i - 1], d[i]]
-        """
-        tol = 1e-6
-        if cache is None:
-            grade_all_zero = (self.grade == 0.0).all()
-            if grade_all_zero:
-                return 0.0
-            delta_dists = trapz_step_distances(self)
-            trapz_distances_m = delta_dists.cumsum()
-            if delta_distance_m <= tol:
-                if distance_start_m <= trapz_distances_m[0]:
-                    return self.grade[0]
-                if distance_start_m > trapz_distances_m[-1]:
-                    return self.grade[-1]
-                for idx in range(1, len(self.time_s)):
-                    if distance_start_m > trapz_distances_m[idx-1] and distance_start_m <= trapz_distances_m[idx]:
-                        return self.grade[idx]
-                return self.grade[-1]
-            # NOTE: we use the following instead of delta_elev_m in order to use
-            # a more-accurate trapezoidal integration. This also uses the fully
-            # accurate trig functions in case we have large slope angles.
-            trapz_elevations_m = np.cumsum(np.cos(np.arctan(self.grade)) * delta_dists * self.grade)
-            e0 = np.interp(distance_start_m, xp=trapz_distances_m, fp=trapz_elevations_m)
-            e1 = np.interp(distance_start_m + delta_distance_m,
-                        xp=trapz_distances_m, fp=trapz_elevations_m)
-        else:
-            if cache.grade_all_zero:
-                return 0.0
-            if delta_distance_m <= tol:
-                return cache.interp_grade(distance_start_m)
-            e0 = cache.interp_elevation(distance_start_m)
-            e1 = cache.interp_elevation(distance_start_m + delta_distance_m)
-        return np.tan(np.arcsin((e1 - e0) / delta_distance_m))
-
-    def calc_distance_to_next_stop_from(self, distance_m: float, cache: Optional[CycleCache]=None) -> float:
-        """
-        Calculate the distance to next stop from `distance_m`
-        - distance_m: non-negative-number, the current distance from start (m)
-        RETURN: returns the distance to the next stop from distance_m
-        NOTE: distance may be negative if we're beyond the last stop
-        """
-        tol = 1e-6
-        #d = 0.0
-        if cache:
-            ds = cache.trapz_distances_m
-            stops = cache.stops
-        else:
-            ds = trapz_step_distances(self).cumsum()
-            stops = self.mps <= tol
-        argmax = np.argmax(np.logical_and(ds > distance_m, stops))
-        return ds[argmax] - distance_m
-
-    def modify_by_const_jerk_trajectory(self, idx, n, jerk_m__s3, accel0_m__s2):
-        """
-        Modifies the cycle using the given constant-jerk trajectory parameters
-        - idx: non-negative integer, the point in the cycle to initiate
-        modification (note: THIS point is modified since trajectory should be calculated from idx-1)
-        - jerk_m__s3: number, the "Jerk" associated with the trajectory (m/s3)
-        - accel0_m__s2: number, the initial acceleration (m/s2)
-        NOTE:
-        - modifies cyc in place to hit any critical rendezvous_points by a trajectory adjustment
-        - CAUTION: NOT ROBUST AGAINST VARIABLE DURATION TIME-STEPS
-        RETURN: Number, final modified speed (m/s)
-        """
-        num_samples = len(self.time_s)
-        v0 = self.mps[idx-1]
-        dt = self.dt_s_at_i(idx)
-        v = v0
-        for ni in range(1, int(n)+1):
-            idx_to_set = (int(idx) - 1) + ni
-            if idx_to_set >= num_samples:
-                break
-            v = speed_for_constant_jerk(ni, v0, accel0_m__s2, jerk_m__s3, dt)
-            self.mps[idx_to_set] = max(v, 0.0)
-        return v
-
-    def modify_with_braking_trajectory(self, brake_accel_m__s2: float, idx: int, dts_m: Optional[float] = None) -> tuple:
-        """
-        Add a braking trajectory that would cover the same distance as the given constant brake deceleration
-        - brake_accel_m__s2: negative number, the braking acceleration (m/s2)
-        - idx: non-negative integer, the index where to initiate the stop trajectory, start of the step (i in FASTSim)
-        - dts_m: None | float: if given, this is the desired distance-to-stop in meters. If not given, it is
-            calculated based on braking deceleration.
-        RETURN: (non-negative-number, positive-integer)
-        - the final speed of the modified trajectory (m/s) 
-        - the number of time-steps required to complete the braking maneuver
-        NOTE:
-        - modifies the cycle in place for the braking trajectory
-        """
-        assert brake_accel_m__s2 < 0.0
-        i = int(idx)
-        if i >= len(self.time_s):
-            return self.mps[-1], 0
-        v0 = self.mps[i-1]
-        dt = self.dt_s_at_i(i)
-        # distance-to-stop (m)
-        if dts_m is None or dts_m <= 0.0:
-            dts_m = -0.5 * v0 * v0 / brake_accel_m__s2
-        if dts_m <= 0.0:
-            return v0, 0
-        # time-to-stop (s)
-        tts_s = -v0 / brake_accel_m__s2
-        # number of steps to take
-        n = int(np.round(tts_s / dt))
-        if n < 2:
-            # need at least 2 steps
-            n = 2
-        jerk_m__s3, accel_m__s2 = calc_constant_jerk_trajectory(
-            n, 0.0, v0, dts_m, 0.0, dt)
-        return self.modify_by_const_jerk_trajectory(i, n, jerk_m__s3, accel_m__s2), n
-
-
-class LegacyCycle(object):
-    """
-    Implementation of Cycle with legacy keys.
-    """
-
-    def __init__(self, cycle: Cycle):
-        """
-        Given cycle, returns legacy cycle.
-        """
-        for key, val in NEW_TO_OLD.items():
-            self.__setattr__(val, copy.deepcopy(cycle.__getattribute__(key)))
-
-
-def cyc_equal(a: Cycle, b: Cycle) -> bool:
-    "Return True if a and b are equal"
-    if a is b:
-        return True
-    a_dict = copy_cycle(a, 'dict')
-    b_dict = copy_cycle(b, 'dict')
-    return equals(a_dict, b_dict)
-
-
-def to_microtrips(cycle, stop_speed_m__s=1e-6, keep_name=False):
-    """
-    Split a cycle into an array of microtrips with one microtrip being a start
-    to subsequent stop plus any idle (stopped time).
-
-    Arguments:
-    ----------
-    cycle: drive cycle converted to dictionary by cycle.get_cyc_dict()
-    stop_speed_m__s: speed at which vehicle is considered stopped for trip
-        separation
-    keep_name: (optional) bool, if True and cycle contains "name", adds
-        that name to all microtrips
-    """
-    microtrips = []
-    ts = np.array(cycle['time_s'])
-    vs = np.array(cycle['mps'])
-    gs = np.array(cycle['grade'])
-    rs = np.array(cycle['road_type'])
-    mt = make_cycle([], [])
-    moving = False
-    for idx, (t, v, g, r) in enumerate(zip(ts, vs, gs, rs)):
-        if v > stop_speed_m__s and not moving:
-            if len(mt['time_s']) > 1:
-                temp = make_cycle(
-                    [mt['time_s'][-1]],
-                    [mt['mps'][-1]],
-                    [mt['grade'][-1]],
-                    [mt['road_type'][-1]])
-                mt['time_s'] = mt['time_s'] - mt['time_s'][0]
-                for k in mt:
-                    mt[k] = np.array(mt[k])
-                microtrips.append(mt)
-                mt = temp
-        mt['time_s'] = np.append(mt['time_s'], [t])
-        mt['mps'] = np.append(mt['mps'], [v])
-        mt['grade'] = np.append(mt['grade'], [g])
-        mt['road_type'] = np.append(mt['road_type'], [r])
-        moving = v > stop_speed_m__s
-    if len(mt['time_s']) > 0:
-        mt['time_s'] = mt['time_s'] - mt['time_s'][0]
-        microtrips.append(mt)
-    if keep_name and "name" in cycle:
-        for m in microtrips:
-            m["name"] = cycle["name"]
-    return microtrips
-
-
-def make_cycle(ts, vs, gs=None, rs=None) -> dict:
-    """
-    (Array Num) (Array Num) (Array Num)? -> Dict
-    Create a cycle from times, speeds, and grades. If grades is not
-    specified, it is set to zero.
-    Arguments:
-    ----------
-    ts: array of times [s]
-    vs: array of vehicle speeds [mps]
-    gs: array of grades
-    rs: array of road types (charging or not)
-    """
-    assert len(ts) == len(vs)
-    if gs is None:
-        gs = np.zeros(len(ts))
-    else:
-        assert len(ts) == len(gs)
-    if rs is None:
-        rs = np.zeros(len(ts))
-    else:
-        assert len(ts) == len(rs)
-    return {'time_s': np.array(ts),
-            'mps': np.array(vs),
-            'grade': np.array(gs),
-            'road_type': np.array(rs)}
-
-
-def equals(c1, c2) -> bool:
-    """
-    Dict Dict -> Bool
-    Returns true if the two cycles are equal, false otherwise
-    Arguments:
-    ----------
-    c1: cycle as dictionary from get_cyc_dict()
-    c2: cycle as dictionary from get_cyc_dict()
-    """
-    if c1.keys() != c2.keys():
-        c2missing = set(c1.keys()) - set(c2.keys())
-        c1missing = set(c2.keys()) - set(c1.keys())
-        if len(c1missing) > 0:
-            logger.debug(f"c2 keys not contained in c1: {c1missing}")
-        if len(c2missing) > 0:
-            logger.debug(f"c1 keys not contained in c2: {c2missing}")
-        return False
-    for k in c1.keys():
-        if len(c1[k]) != len(c2[k]):
-            logger.debug(f"{k} has a length discrepancy")
-            return False
-        if np.any(np.array(c1[k]) != np.array(c2[k])):
-            logger.debug(f"{k} has a value discrepancy")
-            return False
-    return True
-
-
-def concat(cycles, name=None):
-    """
-    Concatenates cycles together one after another into a single dictionary
-    (Array Dict) String -> Dict
-    Arguments:
-    ----------
-    cycles: (Array Dict)
-    name: (optional) string or None, if a string, adds the "name" key to the output
-    """
-    final_cycle = {'time_s': np.array([]),
-                   'mps': np.array([]),
-                   'grade': np.array([]),
-                   'road_type': np.array([])}
-    keys = [k for k in final_cycle.keys()]
-    first = True
-    for cycle in cycles:
-        if first:
-            for k in keys:
-                final_cycle[k] = np.array(cycle[k])
-            first = False
-        # if len(final_cycle['time_s']) == 0: # ???
-        #     t0 = 0.0
-        else:
-            for k in keys:
-                if k == 'time_s':
-                    t0 = final_cycle[k][-1]
-                    final_cycle[k] = np.concatenate([
-                        final_cycle[k], np.array(cycle[k][1:]) + t0])
-                else:
-                    final_cycle[k] = np.concatenate([
-                        final_cycle[k], np.array(cycle[k][1:])])
-    if name is not None:
-        final_cycle["name"] = name
-    return final_cycle
-
-
-def resample(cycle: Dict[str, Any], new_dt: Optional[float]=None, start_time: Optional[float]=None, end_time: Optional[float]=None,
-             hold_keys:Optional[Set[str]]=None, hold_keys_next:Optional[Set[str]]=None, rate_keys:Optional[Set[str]]=None):
-    """
-    Cycle new_dt=?Real start_time=?Real end_time=?Real -> Cycle
-    Resample a cycle with a new delta time from start time to end time.
-
-    - cycle: Dict with keys
-        'time_s': numpy.array Real giving the elapsed time
-    - new_dt: Real, optional
-        the new delta time of the sampling. Defaults to the
-        difference between the first two times of the cycle passed in
-    - start_time: Real, optional
-        the start time of the sample. Defaults to 0.0 seconds
-    - end_time: Real, optional
-        the end time of the cycle. Defaults to the last time of the passed in
-        cycle.
-    - hold_keys: None or (Set String), if specified, yields values that
-                 should be interpolated step-wise, holding their value until
-                 an explicit change (i.e., NOT interpolated)
-    - hold_keys_next: None or (Set String), similar to hold_keys but yields
-                 values that should be interpolated step-wise, taking the
-                 NEXT value as the value (vs hold_keys which uses the previous)
-    - rate_keys: None or (Set String), if specified, yields values that maintain
-                 the interpolated value of the given rate. So, for example,
-                 if a speed, will set the speed such that the distance traveled
-                 is consistent. Note: using rate keys for mps may result in
-                 non-zero starting and ending speeds
-    Resamples all non-time metrics by the new sample time.
-    """
-    def check_keys(set_name, the_set):
-        the_set = set(the_set) if the_set is not None else None
-        if the_set is not None:
-            for k in the_set:
-                if k not in STANDARD_CYCLE_KEYS and k not in cycle.keys():
-                    raise Exception(f"invalid {set_name} value '{k}'; this key is not in {sorted(STANDARD_CYCLE_KEYS)} or the cycle")
-        return the_set
-    hold_keys = check_keys('hold_keys', hold_keys)
-    hold_keys_next = check_keys('hold_keys_next', hold_keys_next)
-    rate_keys = check_keys('rate_keys', rate_keys)
-    if new_dt is None:
-        new_dt = cycle['time_s'][1] - cycle['time_s'][0]
-    if start_time is None:
-        start_time = 0.0
-    if end_time is None:
-        end_time = cycle['time_s'][-1]
-    new_cycle = {}
-    eps = new_dt / 10.0
-    new_cycle['time_s'] = np.arange(start_time, end_time + eps, step=new_dt)
-    for k in cycle:
-        if k == 'time_s':
-            continue
-        elif hold_keys is not None and k in hold_keys:
-            f = interp1d(cycle['time_s'], cycle[k], 0)
-            new_cycle[k] = f(new_cycle['time_s'])
-            continue
-        elif hold_keys_next is not None and k in hold_keys_next:
-            f = interp1d(cycle['time_s'], cycle[k], 'next')
-            new_cycle[k] = f(new_cycle['time_s'])
-            continue
-        elif rate_keys is not None and k in rate_keys:
-            rate_var = np.array(cycle[k])
-            # below is same as [(rate_var[i+1] + rate_var[i])/2.0 for i in range(len(rate_var) - 1)]
-            avg_rate_var = (rate_var[1:] + rate_var[:-1]) / 2.0
-            dts_orig = np.diff(cycle['time_s'])
-            step_averages = np.diff(
-                np.interp(
-                    x=new_cycle['time_s'],
-                    xp=cycle['time_s'],
-                    fp=np.insert((avg_rate_var * dts_orig).cumsum(), 0, 0.0)
-                ),
-            ) / new_dt
-            step_averages = np.append(step_averages[0], step_averages)
-            step_averages = np.append(step_averages, step_averages[-1])
-            midstep_times = np.concatenate(
-                (
-                    [0.0],
-                    np.arange(
-                        start_time + (0.5 * new_dt), end_time - (0.5 * new_dt) + eps, step=new_dt),
-                    [end_time],
-                ))
-            new_cycle[k] = np.interp(
-                x=new_cycle['time_s'],
-                xp=midstep_times,
-                fp=step_averages
-            )
-            continue
-        try:
-            new_cycle[k] = np.interp(
-                new_cycle['time_s'], cycle['time_s'], cycle[k])
-        except:
-            # if the value can't be interpolated, it must not be a numerical
-            # array. Just add it back in as is.
-            new_cycle[k] = deepcopy(cycle[k])
-    return new_cycle
-
-
-def clip_by_times(cycle, t_end, t_start=0):
-    """
-    Cycle Number Number -> Cycle
-    INPUT:
-    - cycle: Dict, a legitimate driving cycle
-    - t_start: Number, time to start
-    - t_end: Number, time to end
-    RETURNS: Dict, the cycle with fields snipped
-        to times >= t_start and <= t_end
-    Clip the cycle to the given times and return
-    """
-    idx = np.logical_and(np.array(cycle['time_s']) >= t_start,
-                         np.array(cycle['time_s']) <= t_end)
-    new_cycle = {}
-    for k in cycle:
-        try:
-            new_cycle[k] = np.array(cycle[k])[idx]
-        except:
-            new_cycle[k] = cycle[k]
-
-    # reset time to start at zero
-    new_cycle['time_s'] -= new_cycle['time_s'][0]
-    return new_cycle
-
-
-def accelerations(cycle):
-    """
-    Cycle -> Real
-    Return the acceleration of the given cycle
-    INPUTS:
-    - cycle: Dict, a legitimate driving cycle
-    OUTPUTS: Real, the maximum acceleration
-    """
-    accels = (np.diff(np.array(cycle['mps']))
-              / np.diff(np.array(cycle['time_s'])))
-    return accels
-
-
-def peak_acceleration(cycle):
-    """
-    Cycle -> Real
-    Return the maximum acceleration of the given cycle
-    INPUTS:
-    - cycle: Dict, a legitimate driving cycle
-    OUTPUTS: Real, the maximum acceleration
-    """
-    return np.max(accelerations(cycle))
-
-
-def peak_deceleration(cycle):
-    """
-    Cycle -> Real
-    Return the minimum acceleration (maximum deceleration) of the given cycle
-    INPUTS:
-    - cycle: Dict, a legitimate driving cycle
-    OUTPUTS: Real, the maximum acceleration
-    """
-    return np.min(accelerations(cycle))
-
-
-def calc_constant_jerk_trajectory(n: int, D0: float, v0: float, Dr: float, vr: float, dt: float) -> tuple:
-    """
-    Num Num Num Num Num Int -> (Tuple 'jerk_m__s3': Num, 'accel_m__s2': Num)
-    INPUTS:
-    - n: Int, number of time-steps away from rendezvous
-    - D0: Num, distance of simulated vehicle (m/s)
-    - v0: Num, speed of simulated vehicle (m/s)
-    - Dr: Num, distance of rendezvous point (m)
-    - vr: Num, speed of rendezvous point (m/s)
-    - dt: Num, step duration (s)
-    RETURNS: (Tuple 'jerk_m__s3': Num, 'accel_m__s2': Num)
-    Returns the constant jerk and acceleration for initial time step.
-    """
-    assert n > 1, f"n = {n}"
-    assert Dr > D0, f"Dr = {Dr}; D0 = {D0}"
-    dDr = Dr - D0
-    dvr = vr - v0
-    k = (dvr - (2.0 * dDr / (n * dt)) + 2.0 * v0) / (
-        0.5 * n * (n - 1) * dt
-        - (1.0 / 3) * (n - 1) * (n - 2) * dt
-        - 0.5 * (n - 1) * dt * dt
-    )
-    a0 = (
-        (dDr / dt)
+extern crate ndarray;
+
+#[cfg(feature = "pyo3")]
+use std::collections::HashMap;
+use std::fs::File;
+use std::path::PathBuf;
+
+// local
+use crate::imports::*;
+use crate::params::*;
+use crate::proc_macros::add_pyo3_api;
+#[cfg(feature = "pyo3")]
+use crate::pyo3imports::*;
+use crate::utils::*;
+
+#[cfg_attr(feature = "pyo3", pyfunction)]
+/// # Arguments
+/// - n: Int, number of time-steps away from rendezvous
+/// - d0: Num, distance of simulated vehicle, $\frac{m}{s}$
+/// - v0: Num, speed of simulated vehicle, $\frac{m}{s}$
+/// - dr: Num, distance of rendezvous point, $m$
+/// - vr: Num, speed of rendezvous point, $\frac{m}{s}$
+/// - dt: Num, step duration, $s$
+///
+/// # Returns
+/// (Tuple 'jerk_m__s3': Num, 'accel_m__s2': Num)
+/// - Constant jerk and acceleration for initial time step.
+pub fn calc_constant_jerk_trajectory(
+    n: usize,
+    d0: f64,
+    v0: f64,
+    dr: f64,
+    vr: f64,
+    dt: f64,
+) -> (f64, f64) {
+    assert!(n > 1);
+    assert!(dr > d0);
+    let n = n as f64;
+    let ddr = dr - d0;
+    let dvr = vr - v0;
+    let k = (dvr - (2.0 * ddr / (n * dt)) + 2.0 * v0)
+        / (0.5 * n * (n - 1.0) * dt
+            - (1.0 / 3.0) * (n - 1.0) * (n - 2.0) * dt
+            - 0.5 * (n - 1.0) * dt * dt);
+    let a0 = ((ddr / dt)
         - n * v0
-        - ((1.0 / 6) * n * (n - 1) * (n - 2) *
-           dt + 0.25 * n * (n - 1) * dt * dt) * k
-    ) / (0.5 * n * n * dt)
-    return (k, a0)
-
-
-def accel_for_constant_jerk(n, a0, k, dt):
-    """
-    Calculate the acceleration n timesteps away
-    INPUTS:
-    - n: Int, number of times steps away to calculate
-    - a0: Num, initial acceleration (m/s2)
-    - k: Num, constant jerk (m/s3)
-    - dt: Num, time-step duration in seconds
-    NOTE:
-    - this is the constant acceleration over the time-step from sample n to sample n+1
-    RETURN: Num, the acceleration n timesteps away (m/s2)
-    """
-    return a0 + (n * k * dt)
-
-
-def speed_for_constant_jerk(n, v0, a0, k, dt):
-    """
-    Int Num Num Num Num -> Num
-    Calculate speed (m/s) n timesteps away
-    INPUTS:
-    - n: Int, numer of timesteps away to calculate
-    - v0: Num, initial speed (m/s)
-    - a0: Num, initial acceleration (m/s2)
-    - k: Num, constant jerk
-    - dt: Num, duration of a timestep (s)
-    NOTE:
-    - this is the speed at sample n
-    - if n == 0, speed is v0
-    - if n == 1, speed is v0 + a0*dt, etc.
-    RETURN: Num, the speed n timesteps away (m/s)
-    """
-    return v0 + (n * a0 * dt) + (0.5 * n * (n - 1) * k * dt)
-
-
-def dist_for_constant_jerk(n, d0, v0, a0, k, dt):
-    """
-    Calculate distance (m) after n timesteps
-    INPUTS:
-    - n: Int, numer of timesteps away to calculate
-    - d0: Num, initial distance (m)
-    - v0: Num, initial speed (m/s)
-    - a0: Num, initial acceleration (m/s2)
-    - k: Num, constant jerk
-    - dt: Num, duration of a timestep (s)
-    NOTE:
-    - this is the distance traveled from start (i.e., n=0) measured at sample point n
-    RETURN: Num, the distance at n timesteps away (m)
-    """
-    term1 = dt * (
-        (n * v0)
-        + (0.5 * n * (n - 1) * a0 * dt)
-        + ((1.0 / 6.0) * k * dt * (n - 2) * (n - 1) * n)
-    )
-    term2 = 0.5 * dt * dt * ((n * a0) + (0.5 * n * (n - 1) * k * dt))
-    return d0 + term1 + term2
-
-@dataclass
-class PassingInfo:
-   # True if first cycle passes the second
-   has_collision: bool
-   # the index where first cycle passes the second
-   idx: int
-   # the number of time-steps until idx from i
-   num_steps: int
-   # the starting distance of the first cycle at i
-   start_distance_m: float
-   # the distance (m) traveled of the second cycle when first passes
-   distance_m: float
-   # the starting speed (m/s) of the first cycle at i
-   start_speed_m_per_s: float
-   # the speed (m/s) of the second cycle when first passes
-   speed_m_per_s: float
-   # the time step duration throught the passing investigation
-   time_step_duration_s: float
-
-def detect_passing(cyc: Cycle, cyc0: Cycle, i: int, dist_tol_m: float=0.1) -> PassingInfo:
-    """
-    Reports back information of the first point where cyc passes cyc0, starting at
-    step i until the next stop of cyc.
-    - cyc: fastsim.Cycle, the proposed cycle of the vehicle under simulation
-    - cyc0: fastsim.Cycle, the reference/lead vehicle/shadow cycle to compare with
-    - i: int, the time-step index to consider
-    - dist_tol_m: float, the distance tolerance away from lead vehicle to be seen as
-        "deviated" from the reference/shadow trace (m)
-    RETURNS: PassingInfo
-    """
-    if i >= len(cyc.time_s):
-        return PassingInfo(
-            has_collision=False,
-            idx=0,
-            num_steps=0,
-            start_distance_m=0.0,
-            distance_m=0.0,
-            start_speed_m_per_s=0.0,
-            speed_m_per_s=0.0,
-            time_step_duration_s=1.0,
+        - ((1.0 / 6.0) * n * (n - 1.0) * (n - 2.0) * dt + 0.25 * n * (n - 1.0) * dt * dt) * k)
+        / (0.5 * n * n * dt);
+    (k, a0)
+}
+
+#[cfg_attr(feature = "pyo3", pyfunction)]
+/// Calculate distance (m) after n timesteps
+///
+/// INPUTS:
+/// - n: Int, numer of timesteps away to calculate
+/// - d0: Num, initial distance (m)
+/// - v0: Num, initial speed (m/s)
+/// - a0: Num, initial acceleration (m/s2)
+/// - k: Num, constant jerk
+/// - dt: Num, duration of a timestep (s)
+///
+/// NOTE:
+/// - this is the distance traveled from start (i.e., n=0) measured at sample point n
+/// RETURN: Num, the distance at n timesteps away (m)
+pub fn dist_for_constant_jerk(n: usize, d0: f64, v0: f64, a0: f64, k: f64, dt: f64) -> f64 {
+    let n = n as f64;
+    let term1 = dt
+        * ((n * v0)
+            + (0.5 * n * (n - 1.0) * a0 * dt)
+            + ((1.0 / 6.0) * k * dt * (n - 2.0) * (n - 1.0) * n));
+    let term2 = 0.5 * dt * dt * ((n * a0) + (0.5 * n * (n - 1.0) * k * dt));
+    d0 + term1 + term2
+}
+
+#[cfg_attr(feature = "pyo3", pyfunction)]
+/// Calculate speed (m/s) n timesteps away via a constant-jerk acceleration
+///
+/// INPUTS:
+/// - n: Int, numer of timesteps away to calculate
+/// - v0: Num, initial speed (m/s)
+/// - a0: Num, initial acceleration (m/s2)
+/// - k: Num, constant jerk
+/// - dt: Num, duration of a timestep (s)
+///
+/// NOTE:
+/// - this is the speed at sample n
+/// - if n == 0, speed is v0
+/// - if n == 1, speed is v0 + a0*dt, etc.
+///
+/// RETURN: Num, the speed n timesteps away (m/s)
+pub fn speed_for_constant_jerk(n: usize, v0: f64, a0: f64, k: f64, dt: f64) -> f64 {
+    let n = n as f64;
+    v0 + (n * a0 * dt) + (0.5 * n * (n - 1.0) * k * dt)
+}
+
+#[cfg_attr(feature = "pyo3", pyfunction)]
+/// Calculate the acceleration n timesteps away
+///
+/// INPUTS:
+/// - n: Int, number of times steps away to calculate
+/// - a0: Num, initial acceleration (m/s2)
+/// - k: Num, constant jerk (m/s3)
+/// - dt: Num, time-step duration in seconds
+///
+/// NOTE:
+/// - this is the constant acceleration over the time-step from sample n to sample n+1
+///
+/// RETURN: Num, the acceleration n timesteps away (m/s2)
+pub fn accel_for_constant_jerk(n: usize, a0: f64, k: f64, dt: f64) -> f64 {
+    let n = n as f64;
+    a0 + (n * k * dt)
+}
+
+/// Apply `accel_for_constant_jerk` to full
+pub fn accel_array_for_constant_jerk(nmax: usize, a0: f64, k: f64, dt: f64) -> Array1<f64> {
+    let mut accels: Vec<f64> = Vec::new();
+    for n in 0..nmax {
+        accels.push(accel_for_constant_jerk(n, a0, k, dt));
+    }
+    Array1::from_vec(accels)
+}
+
+/// Calculate the average speed per each step in m/s
+pub fn average_step_speeds(cyc: &RustCycle) -> Array1<f64> {
+    let mut result: Vec<f64> = Vec::with_capacity(cyc.len());
+    result.push(0.0);
+    for i in 1..cyc.len() {
+        result.push(0.5 * (cyc.mps[i] + cyc.mps[i - 1]));
+    }
+    Array1::from_vec(result)
+}
+
+/// Calculate the average step speed at step i in m/s
+/// (i.e., from sample point i-1 to i)
+pub fn average_step_speed_at(cyc: &RustCycle, i: usize) -> f64 {
+    0.5 * (cyc.mps[i] + cyc.mps[i - 1])
+}
+
+/// Sum of the distance traveled over each step using
+/// trapezoidal integration
+pub fn trapz_step_distances(cyc: &RustCycle) -> Array1<f64> {
+    average_step_speeds(cyc) * cyc.dt_s()
+}
+
+pub fn trapz_step_distances_primitive(time_s: &Array1<f64>, mps: &Array1<f64>) -> Array1<f64> {
+    let mut delta_dists_m: Vec<f64> = Vec::with_capacity(time_s.len());
+    delta_dists_m.push(0.0);
+    for i in 1..time_s.len() {
+        delta_dists_m.push((time_s[i] - time_s[i - 1]) * 0.5 * (mps[i] + mps[i - 1]));
+    }
+    Array1::from_vec(delta_dists_m)
+}
+
+/// The distance traveled from start at the beginning of step i
+/// (i.e., distance traveled up to sample point i-1)
+/// Distance is in meters.
+pub fn trapz_step_start_distance(cyc: &RustCycle, i: usize) -> f64 {
+    let mut dist_m: f64 = 0.0;
+    for i in 1..i {
+        dist_m += (cyc.time_s[i] - cyc.time_s[i - 1]) * 0.5 * (cyc.mps[i] + cyc.mps[i - 1]);
+    }
+    dist_m
+}
+
+/// The distance traveled during step i in meters
+/// (i.e., from sample point i-1 to i)
+pub fn trapz_distance_for_step(cyc: &RustCycle, i: usize) -> f64 {
+    average_step_speed_at(cyc, i) * cyc.dt_s_at_i(i)
+}
+
+/// Calculate the distance from step i_start to the start of step i_end
+/// (i.e., distance from sample point i_start-1 to i_end-1)
+pub fn trapz_distance_over_range(cyc: &RustCycle, i_start: usize, i_end: usize) -> f64 {
+    trapz_step_distances(cyc).slice(s![i_start..i_end]).sum()
+}
+
+/// Calculate the time in a cycle spent moving
+/// - stopped_speed_m_per_s: the speed above which we are considered to be moving
+/// RETURN: the time spent moving in seconds
+pub fn time_spent_moving(cyc: &RustCycle, stopped_speed_m_per_s: Option<f64>) -> f64 {
+    let mut t_move_s = 0.0;
+    let stopped_speed_m_per_s = stopped_speed_m_per_s.unwrap_or(0.0);
+    for idx in 1..cyc.time_s.len() {
+        let dt = cyc.time_s[idx] - cyc.time_s[idx - 1];
+        let vavg = (cyc.mps[idx] + cyc.mps[idx - 1]) / 2.0;
+        if vavg > stopped_speed_m_per_s {
+            t_move_s += dt;
+        }
+    }
+    t_move_s
+}
+
+/// Split a cycle into an array of microtrips with one microtrip being a start
+/// to subsequent stop plus any idle (stopped time).
+/// Arguments:
+/// ----------
+/// cycle: drive cycle converted to dictionary by cycle.get_cyc_dict()
+/// stop_speed_m__s: speed at which vehicle is considered stopped for trip
+///     separation
+/// keep_name: (optional) bool, if True and cycle contains "name", adds
+///     that name to all microtrips
+pub fn to_microtrips(cycle: &RustCycle, stop_speed_m_per_s: Option<f64>) -> Vec<RustCycle> {
+    let stop_speed_m_per_s = stop_speed_m_per_s.unwrap_or(1e-6);
+    let mut microtrips: Vec<RustCycle> = Vec::new();
+    let ts = cycle.time_s.to_vec();
+    let vs = cycle.mps.to_vec();
+    let gs = cycle.grade.to_vec();
+    let rs = cycle.road_type.to_vec();
+    let mut mt_ts: Vec<f64> = Vec::new();
+    let mut mt_vs: Vec<f64> = Vec::new();
+    let mut mt_gs: Vec<f64> = Vec::new();
+    let mut mt_rs: Vec<f64> = Vec::new();
+    let mut moving = false;
+    for idx in 0..ts.len() {
+        let t = ts[idx];
+        let v = vs[idx];
+        let g = gs[idx];
+        let r = rs[idx];
+        if v > stop_speed_m_per_s && !moving && mt_ts.len() > 1 {
+            let last_idx = mt_ts.len() - 1;
+            let last_t = mt_ts[last_idx];
+            let last_v = mt_vs[last_idx];
+            let last_g = mt_gs[last_idx];
+            let last_r = mt_rs[last_idx];
+            mt_ts = mt_ts.iter().map(|t| -> f64 { t - mt_ts[0] }).collect();
+            microtrips.push(RustCycle::new(
+                mt_ts.clone(),
+                mt_vs.clone(),
+                mt_gs.clone(),
+                mt_rs.clone(),
+                cycle.name.clone(),
+            ));
+            mt_ts = vec![last_t];
+            mt_vs = vec![last_v];
+            mt_gs = vec![last_g];
+            mt_rs = vec![last_r];
+        }
+        mt_ts.push(t);
+        mt_vs.push(v);
+        mt_gs.push(g);
+        mt_rs.push(r);
+        moving = v > stop_speed_m_per_s;
+    }
+    if !mt_ts.is_empty() {
+        mt_ts = mt_ts.iter().map(|t| -> f64 { t - mt_ts[0] }).collect();
+        microtrips.push(RustCycle::new(
+            mt_ts,
+            mt_vs,
+            mt_gs,
+            mt_rs,
+            cycle.name.clone(),
+        ));
+    }
+    microtrips
+}
+
+/// Create distance and target speeds by microtrip
+/// This helper function splits a cycle up into microtrips and returns a list of 2-tuples of:
+/// (distance from start in meters, target speed in meters/second)
+/// - cyc: the cycle to operate on
+/// - blend_factor: float, from 0 to 1
+///     if 0, use average speed of the microtrip
+///     if 1, use average speed while moving (i.e., no stopped time)
+///     else something in between
+/// - min_target_speed_mps: float, the minimum target speed allowed (m/s)
+/// RETURN: list of 2-tuple of (float, float) representing the distance of start of
+///     each microtrip and target speed for that microtrip
+/// NOTE: target speed per microtrip is not allowed to be below min_target_speed_mps
+pub fn create_dist_and_target_speeds_by_microtrip(
+    cyc: &RustCycle,
+    blend_factor: f64,
+    min_target_speed_mps: f64,
+) -> Vec<(f64, f64)> {
+    let blend_factor = if blend_factor < 0.0 {
+        0.0
+    } else if blend_factor > 1.0 {
+        1.0
+    } else {
+        blend_factor
+    };
+    let mut dist_and_tgt_speeds: Vec<(f64, f64)> = Vec::new();
+    // Split cycle into microtrips
+    let microtrips = to_microtrips(cyc, None);
+    let mut dist_at_start_of_microtrip_m = 0.0;
+    for mt_cyc in microtrips {
+        let mt_dist_m = mt_cyc.dist_m().sum();
+        let mt_time_s = mt_cyc.time_s.last().unwrap() - mt_cyc.time_s.first().unwrap();
+        let mt_moving_time_s = time_spent_moving(&mt_cyc, None);
+        let mt_avg_spd_m_per_s = if mt_time_s > 0.0 {
+            mt_dist_m / mt_time_s
+        } else {
+            0.0
+        };
+        let mt_moving_avg_spd_m_per_s = if mt_moving_time_s > 0.0 {
+            mt_dist_m / mt_moving_time_s
+        } else {
+            0.0
+        };
+        let mt_target_spd_m_per_s =
+            (blend_factor * (mt_moving_avg_spd_m_per_s - mt_avg_spd_m_per_s) + mt_avg_spd_m_per_s)
+                .min(mt_moving_avg_spd_m_per_s)
+                .max(mt_avg_spd_m_per_s);
+        if mt_dist_m > 0.0 {
+            dist_and_tgt_speeds.push((
+                dist_at_start_of_microtrip_m,
+                mt_target_spd_m_per_s.max(min_target_speed_mps),
+            ));
+            dist_at_start_of_microtrip_m += mt_dist_m;
+        }
+    }
+    dist_and_tgt_speeds
+}
+
+/// - cyc: fastsim.cycle.Cycle
+/// - absolute_time_s: float, the seconds to extend
+/// - time_fraction: float, the fraction of the original cycle time to add on
+/// - use_rust: bool, if True, return a RustCycle instance, else a normal Python Cycle
+/// RETURNS: fastsim.cycle.Cycle (or fastsimrust.RustCycle), the new cycle with stopped time appended
+/// NOTE: additional time is rounded to the nearest second
+pub fn extend_cycle(
+    cyc: &RustCycle,
+    absolute_time_s: Option<f64>, // =0.0,
+    time_fraction: Option<f64>,   // =0.0,
+) -> RustCycle {
+    let absolute_time_s = absolute_time_s.unwrap_or(0.0);
+    let time_fraction = time_fraction.unwrap_or(0.0);
+    let mut ts = cyc.time_s.to_vec();
+    let mut vs = cyc.mps.to_vec();
+    let mut gs = cyc.grade.to_vec();
+    let mut rs = cyc.road_type.to_vec();
+    let extra_time_s = (absolute_time_s + (time_fraction * ts.last().unwrap())).round() as i32;
+    if extra_time_s == 0 {
+        return cyc.clone();
+    }
+    let dt = 1;
+    let t_end = *ts.last().unwrap();
+    let mut idx = 1;
+    while dt * idx <= extra_time_s {
+        let dt_extra = (dt * idx) as f64;
+        ts.push(t_end + dt_extra);
+        vs.push(0.0);
+        gs.push(0.0);
+        rs.push(0.0);
+        idx += 1;
+    }
+    RustCycle::new(ts, vs, gs, rs, cyc.name.clone())
+}
+
+#[cfg(feature = "pyo3")]
+#[allow(unused)]
+pub fn register(_py: Python<'_>, m: &PyModule) -> Result<(), anyhow::Error> {
+    m.add_function(wrap_pyfunction!(calc_constant_jerk_trajectory, m)?)?;
+    m.add_function(wrap_pyfunction!(accel_for_constant_jerk, m)?)?;
+    m.add_function(wrap_pyfunction!(speed_for_constant_jerk, m)?)?;
+    m.add_function(wrap_pyfunction!(dist_for_constant_jerk, m)?)?;
+    Ok(())
+}
+
+#[derive(Default, PartialEq, Clone, Debug, Deserialize, Serialize)]
+pub struct RustCycleElement {
+    /// time [s]
+    #[serde(alias = "cycSecs")]
+    pub time_s: f64,
+    /// speed [m/s]
+    #[serde(alias = "cycMps")]
+    pub mps: f64,
+    /// grade [rise/run]
+    #[serde(alias = "cycGrade")]
+    pub grade: f64,
+    /// max possible charge rate from roadway
+    #[serde(alias = "cycRoadType")]
+    pub road_type: f64,
+}
+
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Default)]
+#[add_pyo3_api(
+    #[new]
+    pub fn __new__(
+        cyc: &RustCycle,
+    ) -> Self {
+        Self::new(cyc)
+    }
+)]
+pub struct RustCycleCache {
+    pub grade_all_zero: bool,
+    pub trapz_step_distances_m: Array1<f64>,
+    pub trapz_distances_m: Array1<f64>,
+    pub trapz_elevations_m: Array1<f64>,
+    pub stops: Array1<bool>,
+    interp_ds: Array1<f64>,
+    interp_is: Array1<f64>,
+    interp_hs: Array1<f64>,
+    grades: Array1<f64>,
+}
+
+impl SerdeAPI for RustCycleCache {}
+
+impl RustCycleCache {
+    pub fn new(cyc: &RustCycle) -> Self {
+        let tol = 1e-6;
+        let num_items = cyc.time_s.len();
+        let grade_all_zero = cyc.grade.iter().all(|g| *g == 0.0);
+        let trapz_step_distances_m = trapz_step_distances(cyc);
+        let trapz_distances_m = ndarrcumsum(&trapz_step_distances_m);
+        let trapz_elevations_m = if grade_all_zero {
+            Array::zeros(num_items)
+        } else {
+            let xs = Array::from_iter(
+                cyc.grade
+                    .iter()
+                    .zip(&trapz_step_distances_m)
+                    .map(|(g, dd)| g.atan().cos() * dd * g),
+            );
+            ndarrcumsum(&xs)
+        };
+        let stops = Array::from_iter(cyc.mps.iter().map(|v| v <= &tol));
+        let mut interp_ds: Vec<f64> = Vec::with_capacity(num_items);
+        let mut interp_is: Vec<f64> = Vec::with_capacity(num_items);
+        let mut interp_hs: Vec<f64> = Vec::with_capacity(num_items);
+        for idx in 0..num_items {
+            let d = trapz_distances_m[idx];
+            if interp_ds.is_empty() || d > *interp_ds.last().unwrap() {
+                interp_ds.push(d);
+                interp_is.push(idx as f64);
+                interp_hs.push(trapz_elevations_m[idx]);
+            }
+        }
+        let interp_ds = Array::from_vec(interp_ds);
+        let interp_is = Array::from_vec(interp_is);
+        let interp_hs = Array::from_vec(interp_hs);
+        Self {
+            grade_all_zero,
+            trapz_step_distances_m,
+            trapz_distances_m,
+            trapz_elevations_m,
+            stops,
+            interp_ds,
+            interp_is,
+            interp_hs,
+            grades: cyc.grade.clone(),
+        }
+    }
+
+    /// Interpolate the single-point grade at the given distance.
+    /// Assumes that the grade at i applies from sample point (i-1, i]
+    pub fn interp_grade(&self, dist_m: f64) -> f64 {
+        if self.grade_all_zero {
+            0.0
+        } else if dist_m <= self.interp_ds[0] {
+            self.grades[0]
+        } else if dist_m > *self.interp_ds.last().unwrap() {
+            *self.grades.last().unwrap()
+        } else {
+            let raw_idx = interpolate(&dist_m, &self.interp_ds, &self.interp_is, false);
+            let idx = raw_idx.ceil() as usize;
+            self.grades[idx]
+        }
+    }
+
+    /// Interpolate the elevation at the given distance
+    pub fn interp_elevation(&self, dist_m: f64) -> f64 {
+        if self.grade_all_zero {
+            0.0
+        } else {
+            interpolate(&dist_m, &self.interp_ds, &self.interp_hs, false)
+        }
+    }
+}
+
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Default)]
+#[add_pyo3_api(
+    #[new]
+    pub fn __new__(
+        time_s: Vec<f64>,
+        mps: Vec<f64>,
+        grade: Vec<f64>,
+        road_type: Vec<f64>,
+        name: String,
+    ) -> Self {
+        Self::new(time_s, mps, grade, road_type, name)
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn __getnewargs__(&self) -> PyResult<(Vec<f64>, Vec<f64>, Vec<f64>, Vec<f64>, &str)> {
+        Ok((self.time_s.to_vec(), self.mps.to_vec(), self.grade.to_vec(), self.road_type.to_vec(), &self.name))
+    }
+
+    #[classmethod]
+    #[pyo3(name = "from_csv_file")]
+    pub fn from_csv_file_py(_cls: &PyType, pathstr: String) -> anyhow::Result<Self> {
+        Self::from_csv_file(&pathstr)
+    }
+
+    pub fn to_rust(&self) -> anyhow::Result<Self> {
+        Ok(self.clone())
+    }
+
+    /// Return a HashMap representing the cycle
+    pub fn get_cyc_dict(&self) -> anyhow::Result<HashMap<String, Vec<f64>>> {
+        let dict: HashMap<String, Vec<f64>> = HashMap::from([
+            ("time_s".to_string(), self.time_s.to_vec()),
+            ("mps".to_string(), self.mps.to_vec()),
+            ("grade".to_string(), self.grade.to_vec()),
+            ("road_type".to_string(), self.road_type.to_vec()),
+        ]);
+        Ok(dict)
+    }
+
+    #[pyo3(name = "modify_by_const_jerk_trajectory")]
+    pub fn modify_by_const_jerk_trajectory_py(
+        &mut self,
+        idx: usize,
+        n: usize,
+        jerk_m_per_s3: f64,
+        accel0_m_per_s2: f64,
+    ) -> PyResult<f64> {
+        Ok(self.modify_by_const_jerk_trajectory(idx, n, jerk_m_per_s3, accel0_m_per_s2))
+    }
+
+    #[pyo3(name = "modify_with_braking_trajectory")]
+    pub fn modify_with_braking_trajectory_py(
+        &mut self,
+        brake_accel_m_per_s2: f64,
+        idx: usize,
+        dts_m: Option<f64>
+    ) -> PyResult<(f64, usize)> {
+        Ok(self.modify_with_braking_trajectory(brake_accel_m_per_s2, idx, dts_m))
+    }
+
+    #[pyo3(name = "calc_distance_to_next_stop_from")]
+    pub fn calc_distance_to_next_stop_from_py(&self, distance_m: f64) -> PyResult<f64> {
+        Ok(self.calc_distance_to_next_stop_from(distance_m, None))
+    }
+
+    #[pyo3(name = "average_grade_over_range")]
+    pub fn average_grade_over_range_py(
+        &self,
+        distance_start_m: f64,
+        delta_distance_m: f64,
+    ) -> PyResult<f64> {
+        Ok(self.average_grade_over_range(distance_start_m, delta_distance_m, None))
+    }
+
+    #[pyo3(name = "build_cache")]
+    pub fn build_cache_py(&self) -> PyResult<RustCycleCache> {
+        Ok(self.build_cache())
+    }
+
+    #[pyo3(name = "dt_s_at_i")]
+    pub fn dt_s_at_i_py(&self, i: usize) -> PyResult<f64> {
+        if i == 0 {
+            Ok(0.0)
+        } else {
+            Ok(self.dt_s_at_i(i))
+        }
+    }
+
+    #[getter]
+    pub fn get_mph(&self) -> PyResult<Vec<f64>> {
+        Ok((&self.mps * crate::params::MPH_PER_MPS).to_vec())
+    }
+    #[setter]
+    pub fn set_mph(&mut self, new_value: Vec<f64>) -> PyResult<()> {
+        self.mps = Array::from_vec(new_value) / MPH_PER_MPS;
+        Ok(())
+    }
+    #[getter]
+    /// array of time steps
+    pub fn get_dt_s(&self) -> PyResult<Vec<f64>> {
+        Ok(self.dt_s().to_vec())
+    }
+    #[getter]
+    /// cycle length
+    pub fn get_len(&self) -> PyResult<usize> {
+        Ok(self.len())
+    }
+    #[getter]
+    /// distance for each time step based on final speed
+    pub fn get_dist_m(&self) -> PyResult<Vec<f64>> {
+        Ok(self.dist_m().to_vec())
+    }
+    #[getter]
+    pub fn get_delta_elev_m(&self) -> PyResult<Vec<f64>> {
+        Ok(self.delta_elev_m().to_vec())
+    }
+)]
+/// Struct for containing:
+/// * time_s, cycle time, $s$
+/// * mps, vehicle speed, $\frac{m}{s}$
+/// * grade, road grade/slope, $\frac{rise}{run}$
+/// * road_type, $kW$
+/// * legacy, will likely change to road charging capacity
+///    * Another sublist.
+pub struct RustCycle {
+    /// array of time [s]
+    #[serde(alias = "cycSecs")]
+    pub time_s: Array1<f64>,
+    /// array of speed [m/s]
+    #[serde(alias = "cycMps")]
+    pub mps: Array1<f64>,
+    /// array of grade [rise/run]
+    #[serde(alias = "cycGrade")]
+    pub grade: Array1<f64>,
+    /// array of max possible charge rate from roadway
+    #[serde(alias = "cycRoadType")]
+    pub road_type: Array1<f64>,
+    pub name: String,
+    #[serde(skip)]
+    pub orphaned: bool,
+}
+
+impl SerdeAPI for RustCycle {
+    fn from_file(filename: &str) -> Result<Self, anyhow::Error> {
+        // check if the extension is csv, and if it is, then call Self::from_csv_file
+        let pathbuf = PathBuf::from(filename);
+        let file = File::open(filename)?;
+        let extension = pathbuf.extension().unwrap().to_str().unwrap();
+        match extension {
+            "yaml" => Ok(serde_yaml::from_reader(file)?),
+            "json" => Ok(serde_json::from_reader(file)?),
+            "csv" => Ok(Self::from_csv_file(filename)?),
+            _ => Err(anyhow!("Unsupported file extension {}", extension)),
+        }
+    }
+}
+
+/// pure Rust methods that need to be separate due to pymethods incompatibility
+impl RustCycle {
+    pub fn new(
+        time_s: Vec<f64>,
+        mps: Vec<f64>,
+        grade: Vec<f64>,
+        road_type: Vec<f64>,
+        name: String,
+    ) -> Self {
+        let time_s = Array::from_vec(time_s);
+        let mps = Array::from_vec(mps);
+        let grade = Array::from_vec(grade);
+        let road_type = Array::from_vec(road_type);
+        Self {
+            time_s,
+            mps,
+            grade,
+            road_type,
+            name,
+            orphaned: false,
+        }
+    }
+
+    pub fn build_cache(&self) -> RustCycleCache {
+        RustCycleCache::new(self)
+    }
+
+    pub fn push(&mut self, cyc_elem: RustCycleElement) {
+        self.time_s
+            .append(Axis(0), array![cyc_elem.time_s].view())
+            .unwrap();
+        self.mps
+            .append(Axis(0), array![cyc_elem.mps].view())
+            .unwrap();
+        self.grade
+            .append(Axis(0), array![cyc_elem.grade].view())
+            .unwrap();
+        self.road_type
+            .append(Axis(0), array![cyc_elem.road_type].view())
+            .unwrap();
+    }
+
+    #[allow(clippy::len_without_is_empty)]
+    pub fn len(&self) -> usize {
+        self.time_s.len()
+    }
+
+    pub fn test_cyc() -> Self {
+        let time_s = Array1::<f64>::range(0.0, 10.0, 1.0).to_vec();
+        let speed_mps = Array1::<f64>::range(0.0, 10.0, 1.0).to_vec();
+        let grade = Array::zeros(10).to_vec();
+        let road_type = Array::zeros(10).to_vec();
+        let name = String::from("test");
+        Self::new(time_s, speed_mps, grade, road_type, name)
+    }
+
+    /// Returns the average grade over the given range of distances
+    /// - distance_start_m: non-negative-number, the distance at start of evaluation area (m)
+    /// - delta_distance_m: non-negative-number, the distance traveled from distance_start_m (m)
+    /// RETURN: number, the average grade (rise over run) over the given distance range
+    /// Note: grade is assumed to be constant from just after the previous sample point
+    /// until the current sample point. That is, grade[i] applies over the range of
+    /// distances, d, from (d[i - 1], d[i]]
+    pub fn average_grade_over_range(
+        &self,
+        distance_start_m: f64,
+        delta_distance_m: f64,
+        cache: Option<&RustCycleCache>,
+    ) -> f64 {
+        let tol = 1e-6;
+        match &cache {
+            Some(rcc) => {
+                if rcc.grade_all_zero {
+                    0.0
+                } else if delta_distance_m <= tol {
+                    rcc.interp_grade(distance_start_m)
+                } else {
+                    let e0 = rcc.interp_elevation(distance_start_m);
+                    let e1 = rcc.interp_elevation(distance_start_m + delta_distance_m);
+                    ((e1 - e0) / delta_distance_m).asin().tan()
+                }
+            }
+            None => {
+                let grade_all_zero = {
+                    let mut all0 = true;
+                    for idx in 0..self.len() {
+                        if self.grade[idx] != 0.0 {
+                            all0 = false;
+                            break;
+                        }
+                    }
+                    all0
+                };
+                if grade_all_zero {
+                    0.0
+                } else {
+                    let delta_dists = trapz_step_distances(self);
+                    let trapz_distances_m = ndarrcumsum(&delta_dists);
+                    if delta_distance_m <= tol {
+                        if distance_start_m <= trapz_distances_m[0] {
+                            return self.grade[0];
+                        }
+                        let max_idx = self.len() - 1;
+                        if distance_start_m > trapz_distances_m[max_idx] {
+                            return self.grade[max_idx];
+                        }
+                        for idx in 1..self.time_s.len() {
+                            if distance_start_m > trapz_distances_m[idx - 1]
+                                && distance_start_m <= trapz_distances_m[idx]
+                            {
+                                return self.grade[idx];
+                            }
+                        }
+                        self.grade[max_idx]
+                    } else {
+                        // NOTE: we use the following instead of delta_elev_m in order to use
+                        // more precise trapezoidal distance and elevation at sample points.
+                        // This also uses the fully accurate trig functions in case we have large slope angles.
+                        let trapz_elevations_m = ndarrcumsum(
+                            &(self.grade.mapv(|g| g.atan().cos()) * delta_dists * &self.grade),
+                        );
+                        let e0 = interpolate(
+                            &distance_start_m,
+                            &trapz_distances_m,
+                            &trapz_elevations_m,
+                            false,
+                        );
+                        let e1 = interpolate(
+                            &(distance_start_m + delta_distance_m),
+                            &trapz_distances_m,
+                            &trapz_elevations_m,
+                            false,
+                        );
+                        ((e1 - e0) / delta_distance_m).asin().tan()
+                    }
+                }
+            }
+        }
+    }
+
+    /// Calculate the distance to next stop from `distance_m`
+    /// - distance_m: non-negative-number, the current distance from start (m)
+    /// RETURN: returns the distance to the next stop from distance_m
+    /// NOTE: distance may be negative if we're beyond the last stop
+    pub fn calc_distance_to_next_stop_from(
+        &self,
+        distance_m: f64,
+        cache: Option<&RustCycleCache>,
+    ) -> f64 {
+        let tol: f64 = 1e-6;
+        match cache {
+            Some(rcc) => {
+                for (&dist, &v) in rcc.trapz_distances_m.iter().zip(self.mps.iter()) {
+                    if (v < tol) && (dist > (distance_m + tol)) {
+                        return dist - distance_m;
+                    }
+                }
+                rcc.trapz_distances_m.last().unwrap() - distance_m
+            }
+            None => {
+                let ds = ndarrcumsum(&trapz_step_distances(self));
+                for (&dist, &v) in ds.iter().zip(self.mps.iter()) {
+                    if (v < tol) && (dist > (distance_m + tol)) {
+                        return dist - distance_m;
+                    }
+                }
+                ds.last().unwrap() - distance_m
+            }
+        }
+    }
+
+    /// Modifies the cycle using the given constant-jerk trajectory parameters
+    /// - idx: non-negative integer, the point in the cycle to initiate
+    ///   modification (note: THIS point is modified since trajectory should be
+    ///   calculated from idx-1)
+    /// - n: non-negative integer, the number of steps ahead
+    /// - jerk_m__s3: number, the "Jerk" associated with the trajectory (m/s3)
+    /// - accel0_m__s2: number, the initial acceleration (m/s2)
+    /// NOTE:
+    /// - modifies cyc in place to hit any critical rendezvous_points by a trajectory adjustment
+    /// - CAUTION: NOT ROBUST AGAINST VARIABLE DURATION TIME-STEPS
+    /// RETURN: Number, final modified speed (m/s)
+    pub fn modify_by_const_jerk_trajectory(
+        &mut self,
+        i: usize,
+        n: usize,
+        jerk_m_per_s3: f64,
+        accel0_m_per_s2: f64,
+    ) -> f64 {
+        if n == 0 {
+            return 0.0;
+        }
+        let num_samples = self.mps.len();
+        if i >= num_samples {
+            if num_samples > 0 {
+                return self.mps[num_samples - 1];
+            }
+            return 0.0;
+        }
+        let v0 = self.mps[i - 1];
+        let dt = self.dt_s_at_i(i);
+        let mut v = v0;
+        for ni in 1..(n + 1) {
+            let idx_to_set = (i - 1) + ni;
+            if idx_to_set >= num_samples {
+                break;
+            }
+            v = speed_for_constant_jerk(ni, v0, accel0_m_per_s2, jerk_m_per_s3, dt);
+            self.mps[idx_to_set] = max(v, 0.0);
+        }
+        v
+    }
+
+    /// Add a braking trajectory that would cover the same distance as the given constant brake deceleration
+    /// - brake_accel_m__s2: negative number, the braking acceleration (m/s2)
+    /// - idx: non-negative integer, the index where to initiate the stop trajectory, start of the step (i in FASTSim)
+    /// - dts_m: None | float: if given, this is the desired distance-to-stop in meters. If not given, it is
+    ///     calculated based on braking deceleration.
+    /// RETURN: (non-negative-number, positive-integer)
+    /// - the final speed of the modified trajectory (m/s)
+    /// - the number of time-steps required to complete the braking maneuver
+    /// NOTE:
+    /// - modifies the cycle in place for the braking trajectory
+    pub fn modify_with_braking_trajectory(
+        &mut self,
+        brake_accel_m_per_s2: f64,
+        i: usize,
+        dts_m: Option<f64>,
+    ) -> (f64, usize) {
+        assert!(brake_accel_m_per_s2 < 0.0);
+        if i >= self.time_s.len() {
+            return (*self.mps.last().unwrap(), 0);
+        }
+        let v0 = self.mps[i - 1];
+        let dt = self.dt_s_at_i(i);
+        // distance-to-stop (m)
+        let dts_m = match dts_m {
+            Some(value) => {
+                if value > 0.0 {
+                    value
+                } else {
+                    -0.5 * v0 * v0 / brake_accel_m_per_s2
+                }
+            }
+            None => -0.5 * v0 * v0 / brake_accel_m_per_s2,
+        };
+        if dts_m <= 0.0 {
+            return (v0, 0);
+        }
+        // time-to-stop (s)
+        let tts_s = -v0 / brake_accel_m_per_s2;
+        // number of steps to take
+        let n: usize = (tts_s / dt).round() as usize;
+        let n: usize = if n < 2 { 2 } else { n }; // need at least 2 steps
+        let (jerk_m_per_s3, accel_m_per_s2) =
+            calc_constant_jerk_trajectory(n, 0.0, v0, dts_m, 0.0, dt);
+        (
+            self.modify_by_const_jerk_trajectory(i, n, jerk_m_per_s3, accel_m_per_s2),
+            n,
         )
-    zero_speed_tol_m_per_s = 1e-6
-    v0 = cyc.mps[i-1]
-    d0 = trapz_step_start_distance(cyc, i)
-    v0_lv = cyc0.mps[i-1]
-    d0_lv = trapz_step_start_distance(cyc0, i)
-    d = d0
-    d_lv = d0_lv
-    dt_total = 0.0
-    rendezvous_idx = None
-    rendezvous_num_steps = 0
-    rendezvous_distance_m = 0
-    rendezvous_speed_m_per_s = 0
-    for di in range(len(cyc.mps) - i):
-        idx = i + di
-        v = cyc.mps[idx]
-        v_lv = cyc0.mps[idx]
-        vavg = (v + v0) * 0.5
-        vavg_lv = (v_lv + v0_lv) * 0.5
-        dd = vavg * cyc.dt_s_at_i(idx)
-        dd_lv = vavg_lv * cyc0.dt_s_at_i(idx)
-        dt_total += cyc0.dt_s_at_i(idx)
-        d += dd
-        d_lv += dd_lv
-        dtlv = d_lv - d
-        v0 = v
-        v0_lv = v_lv
-        if di > 0 and dtlv < -dist_tol_m:
-            rendezvous_idx = idx
-            rendezvous_num_steps = di + 1
-            rendezvous_distance_m = d_lv
-            rendezvous_speed_m_per_s = v_lv
-            break
-        if v <= zero_speed_tol_m_per_s:
-            break
-    return PassingInfo(
-        has_collision=rendezvous_idx is not None and rendezvous_distance_m > d0,
-        idx=rendezvous_idx if not rendezvous_idx is None else 0,
-        num_steps=rendezvous_num_steps,
-        start_distance_m=d0,
-        distance_m=rendezvous_distance_m,
-        start_speed_m_per_s=cyc.mps[i-1],
-        speed_m_per_s=rendezvous_speed_m_per_s,
-        time_step_duration_s=cyc.dt_s_at_i(i),
-    )
-
-def average_step_speeds(cyc: Cycle) -> np.ndarray:
-    """
-    Calculate the average speed per each step in m/s
-    """
-    mps = np.array(cyc.mps)
-    return np.append(0.0, 0.5 * (mps[1:] + mps[:-1]))
-
-def average_step_speed_at(cyc: Cycle, i: int) -> float:
-    """
-    Calculate the average step speed at step i in m/s
-    (i.e., from sample point i-1 to i)
-    """
-    return 0.5 * (cyc.mps[i] + cyc.mps[i-1])
-
-def trapz_step_distances(cyc: Cycle) -> np.ndarray:
-    """
-    Sum of the distance traveled over each step using
-    trapezoidal integration
-    """
-    return average_step_speeds(cyc) * cyc.dt_s
-
-def trapz_step_start_distance(cyc: Cycle, i: int) -> float:
-    """
-    The distance traveled from start at the beginning of step i
-    (i.e., distance traveled up to sample point i-1)
-    Distance is in meters.
-    """
-    time_s = np.array(cyc.time_s)
-    mps = np.array(cyc.mps)
-    return (np.diff(time_s[:i]) * (0.5 * (mps[:max(i-1,0)] + mps[1:i]))).sum()
-
-def trapz_distance_for_step(cyc: Cycle, i: int) -> float:
-    """
-    The distance traveled during step i in meters
-    (i.e., from sample point i-1 to i)
-    """
-    return average_step_speed_at(cyc, i) * cyc.dt_s_at_i(i)
-
-def trapz_distance_over_range(cyc: Cycle, i_start: int, i_end: int) -> float:
-    """
-    Calculate the distance from step i_start to the start of step i_end
-    (i.e., distance from sample point i_start-1 to i_end-1)
-    """
-    return trapz_step_distances(cyc)[i_start:i_end].sum()
-
-def extend_cycle(
-    cyc: Cycle,
-    absolute_time_s:float=0.0,
-    time_fraction:float=0.0,
-    use_rust:bool=False
-) -> Cycle:
-    """
-    - cyc: fastsim.cycle.Cycle
-    - absolute_time_s: float, the seconds to extend
-    - time_fraction: float, the fraction of the original cycle time to add on
-    - use_rust: bool, if True, return a RustCycle instance, else a normal Python Cycle
-    RETURNS: fastsim.cycle.Cycle (or fastsimrust.RustCycle), the new cycle with stopped time appended
-    NOTE: additional time is rounded to the nearest second
-    """
-    cyc0 = cyc.get_cyc_dict()
-    extra_time_s = absolute_time_s + float(int(round(time_fraction * cyc.time_s[-1])))
-    # Zero-velocity cycle segment so simulation doesn't end while moving
-    cyc_stop = resample(
-        make_cycle([0.0, extra_time_s], [0.0, 0.0]),
-        new_dt=1.0,
-    )
-    new_cyc = Cycle.from_dict(concat([cyc0, cyc_stop]))
-    if use_rust:
-        return new_cyc.to_rust()
-    return new_cyc
-
-def create_dist_and_target_speeds_by_microtrip(cyc: Cycle, blend_factor: float=0.0, min_target_speed_mps: float=8.0) -> list:
-    """
-    Create distance and target speeds by microtrip
-    This helper function splits a cycle up into microtrips and returns a list of 2-tuples of:
-    (distance from start in meters, target speed in meters/second)
-
-    - cyc: the cycle to operate on
-    - blend_factor: float, from 0 to 1
-        if 0, use average speed of the microtrip
-        if 1, use average speed while moving (i.e., no stopped time)
-        else something in between
-    - min_target_speed_mps: float, the minimum target speed allowed (m/s)
-    RETURN: list of 2-tuple of (float, float) representing the distance of start of
-        each microtrip and target speed for that microtrip
-    NOTE: target speed per microtrip is not allowed to be below min_target_speed_mps
-    """
-    def time_spent_moving(cycle):
-        t_move_s = 0.0
-        for (t1, t0, vavg) in zip(cycle['time_s'][1:], cycle['time_s'][:-1], np.array(cycle['mps'][1:] + cycle['mps'][:-1]) / 2.0):
-            dt = t1 - t0
-            if vavg > 0:
-                t_move_s += dt
-        return t_move_s
-    blend_factor = max(0.0, min(1.0, blend_factor))
-    dist_and_tgt_speeds = []
-    # Split cycle into microtrips
-    microtrips = to_microtrips(cyc.get_cyc_dict())
-    dist_at_start_of_microtrip_m = 0.0
-    for mt in microtrips:
-        mt_cyc = Cycle.from_dict(mt)
-        mt_dist_m = sum(mt_cyc.dist_m)
-        mt_time_s = mt_cyc.time_s[-1] - mt_cyc.time_s[0]
-        mt_moving_time_s = time_spent_moving(mt_cyc.get_cyc_dict())
-        mt_avg_spd_m_per_s = mt_dist_m / mt_time_s if mt_time_s > 0.0 else 0.0
-        mt_moving_avg_spd_m_per_s = mt_dist_m / mt_moving_time_s if mt_moving_time_s > 0.0 else 0.0
-        mt_target_spd_m_per_s = max(
-            min(
-                blend_factor * (mt_moving_avg_spd_m_per_s - mt_avg_spd_m_per_s) + mt_avg_spd_m_per_s,
-                mt_moving_avg_spd_m_per_s
-            ),
-            mt_avg_spd_m_per_s)
-        if mt_dist_m > 0.0:
-            dist_and_tgt_speeds.append(
-                (dist_at_start_of_microtrip_m, max(mt_target_spd_m_per_s, min_target_speed_mps))
-            )
-            dist_at_start_of_microtrip_m += mt_dist_m
-    return dist_and_tgt_speeds
-
-
-ref_cyc = Cycle.from_file('udds')
-
-
-def copy_cycle(cyc: Cycle, return_type: str = None, deep: bool = True) -> Dict[str, np.ndarray] | Cycle | LegacyCycle | RustCycle:
-    """Returns copy of Cycle.
-    Arguments:
-    cyc: instantianed Cycle or CycleJit
-    return_type: 
-        default: infer from type of cyc
-        'dict': dict
-        'python': Cycle 
-        'legacy': LegacyCycle
-        'rust': RustCycle
-    deep: if True, uses deepcopy on everything
-    """
-
-    cyc_dict = {}
-
-    for key in inspect_utils.get_attrs(ref_cyc):
-        val_to_copy = cyc.__getattribute__(key)
-        array_types = [np.ndarray] if not RUST_AVAILABLE else [
-            np.ndarray, fsr.Pyo3ArrayF64]
-        if type(val_to_copy) in array_types:
-            # has to be float or time_s will get converted to int
-            cyc_dict[key] = copy.deepcopy(np.array(
-                val_to_copy, dtype=float) if deep else val_to_copy)
-        else:
-            cyc_dict[key] = copy.deepcopy(val_to_copy) if deep else val_to_copy
-
-    if return_type is None:
-        if RUST_AVAILABLE and isinstance(cyc, RustCycle):
-            return_type = 'rust'
-        elif isinstance(cyc, Cycle):
-            return_type = 'python'
-        elif isinstance(cyc, LegacyCycle):
-            return_type = "legacy"
-        else:
-            raise NotImplementedError(
-                "Only implemented for rust, python, or legacy.")
-
-    if return_type == 'dict':
-        return cyc_dict
-    elif return_type == 'python':
-        return Cycle.from_dict(cyc_dict)
-    elif return_type == 'legacy':
-        return LegacyCycle(cyc_dict)
-    elif RUST_AVAILABLE and return_type == 'rust':
-        return RustCycle(**cyc_dict)
-    else:
-        raise ValueError(f"Invalid return_type: '{return_type}'")
+    }
+
+    /// rust-internal time steps
+    pub fn dt_s(&self) -> Array1<f64> {
+        diff(&self.time_s)
+    }
+
+    /// rust-internal time steps at i
+    pub fn dt_s_at_i(&self, i: usize) -> f64 {
+        self.time_s[i] - self.time_s[i - 1]
+    }
+
+    /// distance covered in each time step
+    pub fn dist_m(&self) -> Array1<f64> {
+        &self.mps * self.dt_s()
+    }
+
+    /// get mph from self.mps
+    pub fn mph_at_i(&self, i: usize) -> f64 {
+        self.mps[i] * MPH_PER_MPS
+    }
+
+    /// Load cycle from csv file
+    pub fn from_csv_file(pathstr: &str) -> Result<Self, anyhow::Error> {
+        let pathbuf = PathBuf::from(&pathstr);
+
+        // create empty cycle to be populated
+        let mut cyc = Self::default();
+
+        // unwrap is ok because if statement checks existence
+        let file = File::open(&pathbuf).unwrap();
+        let name = String::from(pathbuf.file_stem().unwrap().to_str().unwrap());
+        cyc.name = name;
+        let mut rdr = csv::ReaderBuilder::new()
+            .has_headers(true)
+            .from_reader(file);
+        for result in rdr.deserialize() {
+            // TODO: make this more elegant than unwrap
+            let cyc_elem: RustCycleElement = result?;
+            cyc.push(cyc_elem);
+        }
+
+        Ok(cyc)
+    }
+
+    /// elevation change w.r.t. to initial
+    pub fn delta_elev_m(&self) -> Array1<f64> {
+        ndarrcumsum(&(self.dist_m() * self.grade.clone()))
+    }
+
+    // load a cycle from a string representation of a csv file
+    pub fn from_csv_string(data: &str, name: String) -> Result<Self, anyhow::Error> {
+        let mut cyc = Self {
+            name,
+            ..Self::default()
+        };
+
+        let mut rdr = csv::ReaderBuilder::new()
+            .has_headers(true)
+            .from_reader(data.as_bytes());
+        for result in rdr.deserialize() {
+            let cyc_elem: RustCycleElement = result?;
+            cyc.push(cyc_elem);
+        }
 
+        Ok(cyc)
+    }
+}
+
+pub struct PassingInfo {
+    /// True if first cycle passes the second
+    pub has_collision: bool,
+    /// the index where first cycle passes the second
+    pub idx: usize,
+    /// the number of time-steps until idx from i
+    pub num_steps: usize,
+    /// the starting distance of the first cycle at i
+    pub start_distance_m: f64,
+    /// the distance (m) traveled of the second cycle when first passes
+    pub distance_m: f64,
+    /// the starting speed (m/s) of the first cycle at i
+    pub start_speed_m_per_s: f64,
+    /// the speed (m/s) of the second cycle when first passes
+    pub speed_m_per_s: f64,
+    /// the time step duration throught the passing investigation
+    pub time_step_duration_s: f64,
+}
+
+/// Reports back information of the first point where cyc passes cyc0, starting at
+/// step i until the next stop of cyc.
+/// - cyc: fastsim.Cycle, the proposed cycle of the vehicle under simulation
+/// - cyc0: fastsim.Cycle, the reference/lead vehicle/shadow cycle to compare with
+/// - i: int, the time-step index to consider
+/// - dist_tol_m: float, the distance tolerance away from lead vehicle to be seen as
+///     "deviated" from the reference/shadow trace (m)
+/// RETURNS: PassingInfo
+pub fn detect_passing(
+    cyc: &RustCycle,
+    cyc0: &RustCycle,
+    i: usize,
+    dist_tol_m: Option<f64>,
+) -> PassingInfo {
+    if i >= cyc.time_s.len() {
+        return PassingInfo {
+            has_collision: false,
+            idx: 0,
+            num_steps: 0,
+            start_distance_m: 0.0,
+            distance_m: 0.0,
+            start_speed_m_per_s: 0.0,
+            speed_m_per_s: 0.0,
+            time_step_duration_s: 1.0,
+        };
+    }
+    let zero_speed_tol_m_per_s = 1e-6;
+    let dist_tol_m = dist_tol_m.unwrap_or(0.1);
+    let mut v0: f64 = cyc.mps[i - 1];
+    let d0: f64 = trapz_step_start_distance(cyc, i);
+    let mut v0_lv: f64 = cyc0.mps[i - 1];
+    let d0_lv: f64 = trapz_step_start_distance(cyc0, i);
+    let mut d = d0;
+    let mut d_lv = d0_lv;
+    let mut rendezvous_idx: Option<usize> = None;
+    let mut rendezvous_num_steps: usize = 0;
+    let mut rendezvous_distance_m: f64 = 0.0;
+    let mut rendezvous_speed_m_per_s: f64 = 0.0;
+    for di in 0..(cyc.mps.len() - i) {
+        let idx = i + di;
+        let v = cyc.mps[idx];
+        let v_lv = cyc0.mps[idx];
+        let vavg = (v + v0) * 0.5;
+        let vavg_lv = (v_lv + v0_lv) * 0.5;
+        let dd = vavg * cyc.dt_s_at_i(idx);
+        let dd_lv = vavg_lv * cyc0.dt_s_at_i(idx);
+        d += dd;
+        d_lv += dd_lv;
+        let dtlv = d_lv - d;
+        v0 = v;
+        v0_lv = v_lv;
+        if di > 0 && dtlv < -dist_tol_m {
+            rendezvous_idx = Some(idx);
+            rendezvous_num_steps = di + 1;
+            rendezvous_distance_m = d_lv;
+            rendezvous_speed_m_per_s = v_lv;
+            break;
+        }
+        if v <= zero_speed_tol_m_per_s {
+            break;
+        }
+    }
+    PassingInfo {
+        has_collision: rendezvous_idx.is_some(),
+        idx: rendezvous_idx.unwrap_or(0),
+        num_steps: rendezvous_num_steps,
+        start_distance_m: d0,
+        distance_m: rendezvous_distance_m,
+        start_speed_m_per_s: cyc.mps[i - 1],
+        speed_m_per_s: rendezvous_speed_m_per_s,
+        time_step_duration_s: cyc.dt_s_at_i(i),
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_dist() {
+        let cyc = RustCycle::test_cyc();
+        assert_eq!(cyc.dist_m().sum(), 45.0);
+    }
+
+    #[test]
+    fn test_average_speeds_and_distances() {
+        let time_s = vec![0.0, 10.0, 30.0, 34.0, 40.0];
+        let speed_mps = vec![0.0, 10.0, 10.0, 0.0, 0.0];
+        let grade = Array::zeros(5).to_vec();
+        let road_type = Array::zeros(5).to_vec();
+        let name = String::from("test");
+        let cyc = RustCycle::new(time_s, speed_mps, grade, road_type, name);
+        let avg_mps = average_step_speeds(&cyc);
+        let expected_avg_mps = Array::from_vec(vec![0.0, 5.0, 10.0, 5.0, 0.0]);
+        assert_eq!(expected_avg_mps.len(), avg_mps.len());
+        for (expected, actual) in expected_avg_mps.iter().zip(avg_mps.iter()) {
+            assert_eq!(expected, actual);
+        }
+        let dist_m = trapz_step_distances(&cyc);
+        let expected_dist_m = Array::from_vec(vec![0.0, 50.0, 200.0, 20.0, 0.0]);
+        assert_eq!(expected_dist_m.len(), dist_m.len());
+        for (expected, actual) in expected_dist_m.iter().zip(dist_m.iter()) {
+            assert_eq!(expected, actual);
+        }
+    }
+
+    #[test]
+    fn test_loading_a_cycle_from_the_filesystem() {
+        let mut cyc_file_path = resources_path();
+        cyc_file_path.push("cycles/udds.csv");
+        let expected_udds_length: usize = 1370;
+        let cyc = RustCycle::from_csv_file(cyc_file_path.as_os_str().to_str().unwrap()).unwrap();
+        assert_eq!(cyc.name, String::from("udds"));
+        let num_entries = cyc.time_s.len();
+        assert!(num_entries > 0);
+        assert_eq!(num_entries, cyc.time_s.len());
+        assert_eq!(num_entries, cyc.mps.len());
+        assert_eq!(num_entries, cyc.grade.len());
+        assert_eq!(num_entries, cyc.road_type.len());
+        assert_eq!(num_entries, expected_udds_length);
+    }
+}
```

### Comparing `fastsim-2.0.22/fastsim/docs/2017_Ford_F150_thermal_val.py` & `fastsim-2.1.0/python/fastsim/demos/2017_Ford_F150_thermal_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import time
 import pickle
 import argparse
 import re
 
 import fastsim as fsim
-import fastsimrust as fsr
+import fastsim.fastsimrust as fsr
 
 # 4wd is assumed to be not engaged on cycles used because
 # "Veh_4WD_engaged_CAN[]" and "Veh_4WD_L_engaged_CAN[]" are always zero
 
 f150_resampled_data_dir = Path(
     fsim.__file__).parent / "resources/DownloadableDynamometerDatabase/2017_Ford_F150_Ecoboost"
```

### Comparing `fastsim-2.0.22/fastsim/docs/accel_demo.py` & `fastsim-2.1.0/python/fastsim/demos/accel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/cav_demo.py` & `fastsim-2.1.0/python/fastsim/demos/cav_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 import fastsim as fsim
 from fastsim.tests.test_coasting import make_coasting_plot
-from fastsim.rustext import RUST_AVAILABLE
 
 RAN_SUCCESSFULLY = False
 
 def maybe_str_to_bool(x, default=True):
     """
     Turn values of None or string to bool
     - x: str | None, some parameter, a string or None
@@ -43,68 +42,60 @@
 
 # %% [markdown]
 # ## Create a Vehicle and Cycle
 # 
 # We're going to use a conventional vehicle with
 # the UDDS cycle.
 # %%
-if RUST_AVAILABLE:
-    cyc = fsim.cycle.Cycle.from_file('udds').to_rust()
-    veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
-    sd = fsim.simdrive.RustSimDrive(cyc, veh)
-    sd.sim_drive()
+cyc = fsim.cycle.Cycle.from_file('udds').to_rust()
+veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
+sd = fsim.simdrive.RustSimDrive(cyc, veh)
+sd.sim_drive()
 
-    base_mpg = sd.mpgge
-    if IS_INTERACTIVE:
-        print(f"Base fuel economy over UDDS: {sd.mpgge} mpg")
-        make_coasting_plot(sd.cyc0, sd.cyc, do_show=True)
+base_mpg = sd.mpgge
+if IS_INTERACTIVE:
+    print(f"Base fuel economy over UDDS: {sd.mpgge} mpg")
+    make_coasting_plot(sd.cyc0, sd.cyc, do_show=True)
 
 # %% [markdown]
 # ## Eco-Coasting
 # %%
-if RUST_AVAILABLE:
-    cyc = fsim.cycle.Cycle.from_file('udds').to_rust()
-    veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
-    sd = fsim.simdrive.RustSimDrive(cyc, veh)
-    sd.sim_params = fsim.auxiliaries.set_nested_values(sd.sim_params,
-        coast_allow=True,
-        coast_allow_passing=False,
-        coast_start_speed_m_per_s=-1.0
-    )
-    sd.sim_drive()
+cyc = fsim.cycle.Cycle.from_file('udds').to_rust()
+veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
+sd = fsim.simdrive.RustSimDrive(cyc, veh)
+sd.sim_params = fsim.auxiliaries.set_nested_values(sd.sim_params,
+    coast_allow=True,
+    coast_allow_passing=False,
+    coast_start_speed_m_per_s=-1.0
+)
+sd.sim_drive()
 
-    coast_mpg = sd.mpgge
-    if IS_INTERACTIVE:
-        print(f"Coast fuel economy over UDDS: {sd.mpgge} mpg")
-        pct_savings = ((1.0/base_mpg) - (1.0/coast_mpg)) * 100.0 / ((1.0/base_mpg))
-        print(f"Percent Savings: {pct_savings} %")
-        make_coasting_plot(sd.cyc0, sd.cyc, do_show=True)
+coast_mpg = sd.mpgge
+if IS_INTERACTIVE:
+    print(f"Coast fuel economy over UDDS: {sd.mpgge} mpg")
+    pct_savings = ((1.0/base_mpg) - (1.0/coast_mpg)) * 100.0 / ((1.0/base_mpg))
+    print(f"Percent Savings: {pct_savings} %")
+    make_coasting_plot(sd.cyc0, sd.cyc, do_show=True)
 
 # %% [markdown]
 # # Car Following at Average Speed
 #
 # Here we set up an "automated cruise control" for a system
 # that drives the average speed of the cycle.
 cyc_udds = fsim.cycle.Cycle.from_file('udds').get_cyc_dict()
 cyc_stop = fsim.cycle.resample(
     fsim.cycle.make_cycle([0.0, 200.0], [0.0, 0.0]),
     new_dt=1.0,
 )
-if RUST_AVAILABLE:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    ).to_rust()
-    veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
-    sd = fsim.simdrive.RustSimDrive(cyc, veh)
-else:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    )
-    veh = fsim.vehicle.Vehicle.from_vehdb(1)
-    sd = fsim.simdrive.SimDrive(cyc, veh)
+cyc = fsim.cycle.Cycle.from_dict(
+    fsim.cycle.concat([cyc_udds, cyc_stop])
+).to_rust()
+veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
+sd = fsim.simdrive.RustSimDrive(cyc, veh)
+
 sd.sim_params = fsim.auxiliaries.set_nested_values(sd.sim_params,
     idm_allow=True,
     idm_accel_m_per_s2=1.0,
     idm_decel_m_per_s2=-2.5,
     idm_dt_headway_s=2.0,
     idm_minimum_gap_m=0.0,
     idm_v_desired_m_per_s=np.average(np.array(cyc.mps))
@@ -126,33 +117,25 @@
 # is able to get the average speed per microtrip from some
 # external source.
 cyc_udds = fsim.cycle.Cycle.from_file('udds').get_cyc_dict()
 cyc_stop = fsim.cycle.resample(
     fsim.cycle.make_cycle([0.0, 200.0], [0.0, 0.0]),
     new_dt=1.0,
 )
-if RUST_AVAILABLE:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    ).to_rust()
-    veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
-    sd = fsim.simdrive.RustSimDrive(cyc, veh)
-else:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    )
-    veh = fsim.vehicle.Vehicle.from_vehdb(1)
-    sd = fsim.simdrive.SimDrive(cyc, veh)
+cyc = fsim.cycle.Cycle.from_dict(
+    fsim.cycle.concat([cyc_udds, cyc_stop])
+).to_rust()
+veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
+sd = fsim.simdrive.RustSimDrive(cyc, veh)
 dist_and_avg_speeds = []
 microtrips = fsim.cycle.to_microtrips(cyc.get_cyc_dict())
 dist_at_start_of_microtrip_m = 0.0
 for mt in microtrips:
     mt_cyc = fsim.cycle.Cycle.from_dict(mt)
-    if RUST_AVAILABLE:
-        mt_cyc = mt_cyc.to_rust()
+    mt_cyc = mt_cyc.to_rust()
     mt_dist_m = sum(mt_cyc.dist_m)
     mt_time_s = mt_cyc.time_s[-1]
     mt_avg_spd_m_per_s = mt_dist_m / mt_time_s if mt_time_s > 0.0 else 0.0
     if IS_INTERACTIVE:
         print(f"mt num points      : {len(mt_cyc.time_s)}")
         print(f"mt dist (m)        : {mt_dist_m}")
         print(f"mt time (s)        : {mt_time_s}")
@@ -202,26 +185,19 @@
 #
 # Here, we run an Eco-Cruise and Eco-Approach at the same time.
 cyc_udds = fsim.cycle.Cycle.from_file('udds').get_cyc_dict()
 cyc_stop = fsim.cycle.resample(
     fsim.cycle.make_cycle([0.0, 400.0], [0.0, 0.0]),
     new_dt=1.0,
 )
-if RUST_AVAILABLE:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    ).to_rust()
-    veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
-    sd = fsim.simdrive.RustSimDrive(cyc, veh)
-else:
-    cyc = fsim.cycle.Cycle.from_dict(
-        fsim.cycle.concat([cyc_udds, cyc_stop])
-    )
-    veh = fsim.vehicle.Vehicle.from_vehdb(1)
-    sd = fsim.simdrive.SimDrive(cyc, veh)
+cyc = fsim.cycle.Cycle.from_dict(
+    fsim.cycle.concat([cyc_udds, cyc_stop])
+).to_rust()
+veh = fsim.vehicle.Vehicle.from_vehdb(1).to_rust()
+sd = fsim.simdrive.RustSimDrive(cyc, veh)
 params = sd.sim_params
 params.reset_orphaned()
 params.coast_allow = True
 params.coast_allow_passing = False
 params.coast_start_speed_m_per_s = -1.0
 params.idm_allow = True
 params.idm_accel_m_per_s2 = 0.5
```

### Comparing `fastsim-2.0.22/fastsim/docs/cav_sweep.py` & `fastsim-2.1.0/python/fastsim/demos/cav_sweep.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/demo.py` & `fastsim-2.1.0/python/fastsim/demos/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # To add a new cell, type '# %%'
 # To add a new markdown cell, type '# %% [markdown]'
-# %%
-from IPython import get_ipython
 
 # %% [markdown]
 # # FASTSim Demonstration
 # |
 # ![fastsim icon](fastsim-icon-web-131x172.jpg)
 #
 # Developed by NREL, the Future Automotive Systems Technology Simulator (FASTSim) evaluates the impact of technology improvements on efficiency, performance, cost, and battery life in conventional vehicles, hybrid electric vehicles (HEVs), plug-in hybrid electric vehicles (PHEVs), and all-electric vehicles (EVs).
@@ -19,27 +17,23 @@
 #
 # FASTSim was originally implemented in Microsoft Excel. The pythonic implementation of FASTSim, demonstrated here, captures the drive cycle energy consumption simulation component of the software. The python version of FASTSim is more convenient than the Excel version when very high computational speed is desired, such as for simulating a large batch of drive cycles.
 
 # %%
 import sys
 import os
 from pathlib import Path
-from fastsimrust import abc_to_drag_coeffs
+from fastsim.fastsimrust import abc_to_drag_coeffs
 import numpy as np
 import time
 import pandas as pd
 import matplotlib.pyplot as plt
 import importlib
 # import seaborn as sns
 # sns.set(font_scale=2, style='whitegrid')
 
-if not __name__ == "__main__":
-    get_ipython().run_line_magic('matplotlib', 'inline')
-
-
 # local modules
 import fastsim as fsim
 # importlib.reload(simdrive)
 # importlib.reload(cycle)
 
 #%%
 
@@ -115,16 +109,21 @@
 ax[1].set_xlabel('Cycle Time [s]')
 ax[1].set_ylabel('Speed [MPH]')
 
 plt.show()
 
 # %%
 fig, ax = plt.subplots(2, 1, figsize=(9, 5))
+fig.suptitle(
+    'Absolute Engine Input\nPower Error for Rust v. Python'
+)
 ax[0].plot(cyc.time_s, sdr.fc_kw_in_ach - sim_drive.fc_kw_in_ach)
-ax[0].set_ylabel('Engine Input\nPower Error [kW]')
+ax[0].set_ylabel(
+    'Power[kW]' 
+)
 
 ax[1].plot(cyc.time_s, sim_drive.mph_ach)
 ax[1].set_xlabel('Cycle Time [s]')
 ax[1].set_ylabel('Speed [MPH]')
 
 plt.show()
 
@@ -804,24 +803,25 @@
 
 ax2 = ax.twinx()
 speed_line = ax2.plot(sim_drive.cyc.time_s, sim_drive.mph_ach ,color='xkcd:pale red', label='Speed')
 
 ax.set_xlabel('Cycle Time [s]', weight='bold')
 ax.set_ylabel('Engine Input Power [kW]', weight='bold', color='xkcd:bluish')
 ax.tick_params('y', colors='xkcd:bluish')
-
 ax2.set_ylabel('Speed [MPH]', weight='bold', color='xkcd:pale red')
 ax2.grid(False)
 ax2.tick_params('y', colors='xkcd:pale red')
 plt.show()
 
 # %% [markdown]
 # ### Test Coefficients Calculation
 # 
 # Test drag and wheel rolling resistance calculation from coastdown test values.
 
 # %%
 test_veh = fsim.vehicle.Vehicle.from_vehdb(5, to_rust=True).to_rust()
 (drag_coef, wheel_rr_coef) = abc_to_drag_coeffs(test_veh, 25.91, 0.1943, 0.01796, simdrive_optimize=True)
-print(f'Drag Coefficient: {drag_coef}')
-print(f'Wheel Rolling Resistance Coefficient: {wheel_rr_coef}')
+
+# %%
+print(f'Drag Coefficient: {drag_coef:.3g}')
+print(f'Wheel Rolling Resistance Coefficient: {wheel_rr_coef:.3g}')
 # %%
```

### Comparing `fastsim-2.0.22/fastsim/docs/demo_abc_drag_coef_conv.py` & `fastsim-2.1.0/python/fastsim/demos/demo_abc_drag_coef_conv.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/demo_eu_vehicle_wltp.py` & `fastsim-2.1.0/python/fastsim/demos/demo_eu_vehicle_wltp.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/fastsim-icon-web-131x172.jpg` & `fastsim-2.1.0/python/fastsim/demos/fastsim-icon-web-131x172.jpg`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/fusion_thermal_cal.py` & `fastsim-2.1.0/python/fastsim/demos/fusion_thermal_cal.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import pickle
 from cycler import cycler
 
 import fastsim as fsim
-import fastsimrust as fsr
+import fastsim.fastsimrust as fsr
 
 
+use_nsga2 = True
+
 def load_data() -> Dict[str, pd.DataFrame]:
     # full data
     dfs_raw = dict()
     # resampled to 1 Hz
     dfs = dict()
     for sub in trip_dir.iterdir():
         if sub.is_dir():
@@ -31,16 +33,17 @@
                     dfs_raw[file.stem]['Fuel_Energy_Calc[MJ]'] = (
                         dfs_raw[file.stem]['Fuel_Power_Calc[kW]'] *
                         dfs_raw[file.stem]['Time[s]'].diff().fillna(0.0)
                     ).cumsum() / 1e3
 
                     dfs[file.stem] = fsim.resample(
                         dfs_raw[file.stem],
-                        rate_vars=('Eng_FuelFlow_Direct[cc/s]')
+                        rate_vars=('Eng_FuelFlow_Direct[cc/s]',)
                     )
+    assert len(dfs) > 0 
     return dfs
 
 
 def get_cal_and_val_objs():
     dfs = load_data()
 
     # Separate calibration and validation cycles
@@ -117,25 +120,27 @@
     ]
 
     cal_objectives = fsim.calibration.ModelObjectives(
         models=cal_sim_drives,
         dfs=dfs_cal,
         obj_names=obj_names,
         params=params,
-        verbose=False
+        use_simdrivehot=True,
+        verbose=False,
     )
 
     # to ensure correct key order
     val_sim_drives = {key: val_sim_drives[key] for key in dfs_val.keys()}
     val_objectives = fsim.calibration.ModelObjectives(
         models=val_sim_drives,
         dfs=dfs_val,
         obj_names=obj_names,
         params=params,
-        verbose=False
+        use_simdrivehot=True,
+        verbose=False,
     )
 
     return cal_objectives, val_objectives, params_bounds
 
 
 # load test data which can be obtained at
 # https://www.anl.gov/taps/d3-2012-ford-fusion-v6
@@ -164,30 +169,38 @@
     # should be at least as big as n_processes
     pop_size = args.pop_size
     run_minimize = not(args.skip_minimize)
     save_path = Path(args.save_path)
     save_path.mkdir(exist_ok=True)
     show_plots = args.show
     make_plots = args.make_plots
+    # override default of False
+    use_simdrivehot = True
 
     cal_objectives, val_objectives, params_bounds = get_cal_and_val_objs()
 
     if run_minimize:
         print("Starting calibration.")
-
-        algorithm = fsim.calibration.NSGA3(
-            ref_dirs=fsim.calibration.get_reference_directions(
-                "energy",
-                n_dim=cal_objectives.n_obj,  # must be at least cal_objectives.n_obj
-                n_points=pop_size,  # must be at least pop_size
-            ),
-            # size of each population
-            pop_size=pop_size,
-            sampling=fsim.calibration.LHS(),
-        )
+        if use_nsga2:
+            algorithm = fsim.calibration.NSGA2(
+                # size of each population
+                pop_size=pop_size,
+                sampling=fsim.calibration.LHS(),
+            )
+        else:
+            algorithm = fsim.calibration.NSGA3(
+                ref_dirs=fsim.calibration.get_reference_directions(
+                    "energy",
+                    n_dim=cal_objectives.n_obj,  # must be at least cal_objectives.n_obj
+                    n_points=pop_size,  # must be at least pop_size
+                ),
+                # size of each population
+                pop_size=pop_size,
+                sampling=fsim.calibration.LHS(),
+            )
         termination = fsim.calibration.DMOT(
             # max number of generations, default of 10 is very small
             n_max_gen=n_max_gen,
             # evaluate tolerance over this interval of generations every
             period=5,
         )
 
@@ -241,18 +254,21 @@
     param_vals = res_df.iloc[best_row, :len(cal_objectives.params)].to_numpy()
 
     _, sdhots = cal_objectives.get_errors(
         cal_objectives.update_params(param_vals),
         plot_save_dir=save_path,
         show=show_plots and make_plots,
         plot=make_plots,
+        plotly=make_plots,
         return_mods=True,
     )
     val_objectives.get_errors(
         val_objectives.update_params(param_vals),
         plot_save_dir=save_path,
         show=show_plots,
+        plot=make_plots,
+        plotly=make_plots,
     )
 
     # save calibrated vehicle to file
     sdhots[list(sdhots.keys())[0]].vehthrm.to_file(
         str(save_path / "2012_Ford_Fusion_thrml.yaml"))
```

### Comparing `fastsim-2.0.22/fastsim/docs/fusion_thermal_cal_post.py` & `fastsim-2.1.0/python/fastsim/demos/fusion_thermal_cal_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import pickle
 from cycler import cycler
 
 import fastsim as fsim
-import fastsimrust as fsr
+import fastsim.fastsimrust as fsr
 
 import fusion_thermal_cal as ftc
 
 trip_dir = ftc.trip_dir
 
 cal_objectives, val_objectives, params_bounds = ftc.get_cal_and_val_objs()
 # save_path = "fusion_pymoo_res_2022_08_18"
@@ -41,20 +41,22 @@
 show_plots = False
 
 cal_errs, cal_mods = cal_objectives.get_errors(
     cal_objectives.update_params(param_vals),
     plot_save_dir=Path(save_path),
     show=show_plots,
     return_mods=True,
+    plotly=True,
 )
 val_errs, val_mods = val_objectives.get_errors(
     val_objectives.update_params(param_vals),
     plot_save_dir=Path(save_path),
     show=show_plots,
     return_mods=True,
+    plotly=True
 )
 
 # %%
 
 # generate data for scatter plot
 
 l_per_cc = 1e-3
```

### Comparing `fastsim-2.0.22/fastsim/docs/fusion_thermal_demo.py` & `fastsim-2.1.0/python/fastsim/demos/fusion_thermal_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # To add a new cell, type '# %%'
 # To add a new markdown cell, type '# %% [markdown]'
 # %%
-import fastsimrust as fsr
+import fastsim.fastsimrust as fsr
 import fastsim as fsim
 import seaborn as sns
 import matplotlib.pyplot as plt
 import pandas as pd
 import time
 import numpy as np
 from pathlib import Path
 import os
 import sys
-from IPython import get_ipython
-get_ipython().run_line_magic('matplotlib', 'inline')
-
 
 # %%
 sns.set()
 
 
 # local modules
 
@@ -98,16 +95,16 @@
 ax[3].set_xlabel("Time")
 ax[3].set_ylabel("Climate Power [kW]")
 
 ax[-1].plot(sdh.sd.cyc.time_s, sdh.sd.mph_ach)
 ax[-1].set_xlabel("Time")
 ax[-1].set_ylabel("Speed [mph]")
 plt.tight_layout()
-plt.savefig("plots/fusion udds cold start.png")
-plt.savefig("plots/fusion udds cold start.svg")
+# plt.savefig("plots/fusion udds cold start.png")
+# plt.savefig("plots/fusion udds cold start.svg")
 
 # %% Case with cabin cooling
 
 hvac_model = fsr.HVACModel.default()
 fusion_thermal_clng = fusion_thermal_base.copy()
 fusion_thermal_clng.set_cabin_hvac_model_internal(hvac_model)
 cyc = fsr.RustCycle.from_file(str(fsim.cycle.CYCLES_DIR / "udds.csv"))
@@ -146,16 +143,16 @@
 ax[3].set_xlabel("Time")
 ax[3].set_ylabel("Climate Power [kW]")
 
 ax[-1].plot(sdh.sd.cyc.time_s, sdh.sd.mph_ach)
 ax[-1].set_xlabel("Time")
 ax[-1].set_ylabel("Speed [mph]")
 plt.tight_layout()
-plt.savefig("plots/fusion udds hot start.png")
-plt.savefig("plots/fusion udds hot start.svg")
+# plt.savefig("plots/fusion udds hot start.png")
+# plt.savefig("plots/fusion udds hot start.svg")
 
 
 # %% sweep ambient
 
 hvac_model = fsr.HVACModel.default()
 fusion_thermal_hvac = fusion_thermal_base.copy()
 fusion_thermal_hvac.set_cabin_hvac_model_internal(hvac_model)
@@ -191,10 +188,10 @@
 ax.plot(amb_te_deg_c_arr, mpg, color=colors[0], label='w/ HVAC')
 ax.plot(amb_te_deg_c_arr, mpg_no_hvac, color=colors[1], label='w/o HVAC')
 ax.axhline(sdh_no_thrml.mpgge, color=colors[2], label='no thermal')
 ax.legend()
 ax.set_xlabel('Ambient/Init. Temp [°C]')
 ax.set_ylabel('Fuel Economy [mpg]')
 plt.tight_layout()
-plt.savefig("plots/fusion FE vs temp sweep.png")
-plt.savefig("plots/fusion FE vs temp sweep.svg")
+# plt.savefig("plots/fusion FE vs temp sweep.png")
+# plt.savefig("plots/fusion FE vs temp sweep.svg")
 # %%
```

### Comparing `fastsim-2.0.22/fastsim/docs/mp_parallel_demo.py` & `fastsim-2.1.0/python/fastsim/demos/mp_parallel_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/stop_start_demo.py` & `fastsim-2.1.0/python/fastsim/demos/stop_start_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/time_dilation_demo.py` & `fastsim-2.1.0/python/fastsim/demos/time_dilation_demo.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/docs/wltc_calibration.py` & `fastsim-2.1.0/python/fastsim/demos/wltc_calibration.py`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/FASTSim_py_veh_db.csv` & `fastsim-2.1.0/python/fastsim/resources/FASTSim_py_veh_db.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/HHDDTCruiseSmooth.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/HHDDTCruiseSmooth.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/NREL13.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/NREL13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/TSDC_tripno_42648_cycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/accel.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/accel.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_1/2007-08-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-20.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/2007-08-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4033363_3/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4105836_2/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4105836_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/2007-05-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4107032_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-25.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/2007-06-26.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/2007-06-27.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4108468_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-18.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4109114_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-19.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-21.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-22.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/2007-05-24.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4111928_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-03.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/2007-07-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4112082_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4113492_1/2007-05-17.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4113492_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4114555_1/2007-05-31.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4114555_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_1/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_2/2007-03-28.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115766_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115957_1/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115957_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115985_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4115985_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116361_1/2007-03-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116361_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116721_2/2007-04-09.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116721_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116728_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116728_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_1/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_2/2007-04-05.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116813_2/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116880_1/2007-04-23.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4116880_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-13.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/2007-08-14.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/cmap_subset/4118093_1/trips.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/ftpmc1b.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/ftpmc1b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/hwfet.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/hwfet.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/longHaulDriveCycle.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/longHaulDriveCycle.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/udds.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/udds.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/us06.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/us06.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_extra_high3.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_extra_high3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_high3a.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_high3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_high3b.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_high3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_low3.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_low3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_med3a.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_med3a.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wltc_class3_med3b.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wltc_class3_med3b.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wmtc_all.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_all.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wmtc_part1.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part1.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wmtc_part2.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part2.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/cycles/wmtc_part3.csv` & `fastsim-2.1.0/python/fastsim/resources/cycles/wmtc_part3.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/longparams.json` & `fastsim-2.1.0/python/fastsim/resources/longparams.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/master_benchmark_vars.csv` & `fastsim-2.1.0/python/fastsim/resources/master_benchmark_vars.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/res_excel.json` & `fastsim-2.1.0/python/fastsim/resources/res_excel.json`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2010_Mazda_3_i-Stop.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Focus.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Focus.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Focus.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Focus.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Fusion.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Fusion.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2012_Ford_Fusion.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2012_Ford_Fusion.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 drag_coef: 0.393
 frontal_area_m2: 2.12
 glider_kg: 791.0702892
 veh_cg_m: 0.53
 drive_axle_weight_frac: 0.59
 wheel_base_m: 2.72
 cargo_kg: 136.0
-veh_override_kg: 0.0
+veh_override_kg: 
 comp_mass_multiplier: 1.4
 fs_max_kw: 1000.0
 fs_secs_to_peak_pwr: 1.0
 fs_kwh: 590.0
 fs_kwh_per_kg: 9.89473291
 fc_max_kw: 130.5
 fc_pwr_out_perc:
```

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_EU_VW_Golf_1.4TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Corolla_4cyl_2WD.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 drag_coef: 0.3
 frontal_area_m2: 2.574
 glider_kg: 1045.636
 veh_cg_m: 0.53
 drive_axle_weight_frac: 0.61
 wheel_base_m: 2.6
 cargo_kg: 136.0
-veh_override_kg: 0.0
+veh_override_kg: 
 comp_mass_multiplier: 1.4
 fs_max_kw: 2000.0
 fs_secs_to_peak_pwr: 1.0
 fs_kwh: 441.0
 fs_kwh_per_kg: 9.89
 fc_max_kw: 98.0
 fc_pwr_out_perc:
```

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2016_TOYOTA_Prius_Two.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Ford_F-150_Ecoboost.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2017_Toyota_Highlander_3.5_L.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_1.5TSI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2020_EU_VW_Golf_2.0TDI.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2020_Hero_Splendor+_100cc_2W.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/2022_TOYOTA_Yaris_Hybrid_Mid.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Class_4_Box_Truck.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Class_4_Box_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Class_4_Box_Truck.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Class_4_Box_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Line_Haul_Conv.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Line_Haul_Conv.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Line_Haul_Conv.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Line_Haul_Conv.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 drag_coef: 0.546
 frontal_area_m2: 10.4
 glider_kg: 11776.0
 veh_cg_m: 0.46
 drive_axle_weight_frac: 0.8
 wheel_base_m: 2.26
 cargo_kg: 17236.0
-veh_override_kg: 0.0
+veh_override_kg: 
 comp_mass_multiplier: 1.2
 fs_max_kw: 5000.0
 fs_secs_to_peak_pwr: 1.0
 fs_kwh: 11385.0
 fs_kwh_per_kg: 12.67
 fc_max_kw: 331.0
 fc_pwr_out_perc:
```

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/Regional_Delivery_Class_8_Truck.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/fail_overrides.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/fail_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/fail_overrides.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/fail_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/legacy_template.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/legacy_template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/legacy_template.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/legacy_template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/template.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/template.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/template.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/template.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/test_overrides.csv` & `fastsim-2.1.0/python/fastsim/resources/vehdb/test_overrides.csv`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/test_overrides.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/test_overrides.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml` & `fastsim-2.1.0/python/fastsim/resources/vehdb/thermal/2012_Ford_Fusion_thrml.yaml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/fastsim.egg-info/PKG-INFO` & `fastsim-2.1.0/fastsim.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsim
-Version: 2.0.22
+Version: 2.1.0
 Summary: Tool for modeling vehicle powertrains
 Author-email: NREL/MTES/CIMS/MBAP Group <fastsim@nrel.gov>
 License: Future Automotive Systems Technology Simulator (FASTSim(TM)) Copyright (c) 2020 Alliance for Sustainable Energy, LLC All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -58,37 +58,28 @@
 
 - Command Prompt (windows):
     1. Create: `python -m venv fastsim-venv` -- name is user decision
     1. Activate: `fastsim-venv/Scripts/activate.bat`
 
 ## FASTSim
 ### Via PyPI
-In an active Python environment (either [venv](https://docs.python.org/3/library/venv.html) or [Conda](https://www.anaconda.com/)), run `pip install fastsim`.
+In an active Python environment created above, run `pip install fastsim`.
 
 ### Building from Scratch
-Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  
+Developers might want to install the code in place so that FASTSim files can be editable (the `-e` flag for pip provides this behavior). This option can be handy since FASTSim will be installed in place from the installation location and any updates will be propagated each time FASTSim is freshly imported.  To do this, you'll need to have the [Rust toolchain](https://www.rust-lang.org/tools/install) installed.
 
-- Easy way: run `sh build_and_test.sh` in root folder.  
-- Hard way (a couple of extra steps are required): 
-    1. First install the python code in place:  
-    `DEVELOP_MODE=True pip install -e ".[dev]"`   
-    if on Mac OS, Linux, or Windows Bash (e.g. git bash, VSCode bash).  On Windows in Power Shell or Command Prompt, run  
-    `set DEVELOP_MODE=True` then `pip install -e ".[dev]"`.
-    1. Within the same python environment, navigate to `fastsim/rust/` and run  
-    `pip install maturin`.
-    1. _Optional_: Within the `rust/` folder (which contains the rust `src/` folder), run `cargo test --release` to build and run the tests.
-    1. In `fastsim/rust/fastsim-py`, you should now be able to run `maturin develop --release`, which will enable the tests that use rust to run.  You should also now be able to run `fastsim/fastsim/docs/demo.py`.
-
-After FASTSim has been installed as editable per the above instructions, you can rebuild and test everything with `sh build_and_test.sh` in Windows bash or `./build_and_test.sh` in Linux/Unix in the `fastsim/` dir.  
-
-### Testing
-At the root level of the git repository: `pytest -v fastsim/tests/`.  This can also be run in the python environment directly.  
+- Option 1: run `sh build_and_test.sh` in root folder.  
+- Option 2:  
+    1. Run `pip install -e ".[dev]"`  
+    Optional testing steps:
+    1. Run `cd rust/ && cargo test`
+    1. Run `pytest -v python/fastsim/tests/`
 
 # Usage
-To see and run examples, navigate to fastsim/docs and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
+To see and run examples, navigate to `./python/fastsim/demos` and run the various *demo.py files to see fastsim use cases. There are other examples in fastsim/tests.  
 
 
 # Adding FASTSim as a Depency in Rust
 ## Via GitHub
 Add this line:  
 `fastsim-core = { git = "https://github.nrel.gov/MBAP/fastsim", branch = "rust-port" }`  
 to your Cargo.toml file, modifying the `branch` key as appropriate.  
@@ -122,14 +113,15 @@
 in = component input  
 out = component output  
 
 # Known Issues
 Rust versions of classes have limited Language Server Protocol integration, and we are actively working on fixing this.  
 
 # Release Notes
+2.1.0 -- release and installation improvements, RustVehicle init cleanup, calibration improvements
 2.0.11 - 2.0.22 -- PyPI fixes.  Also, Rust version is now >100x faster than Python version.   
 2.0.10 -- logging fixes, proc macro reorganization, some CAVs performance fixes  
 2.0.9 -- support for mac ARM/RISC architecture  
 2.0.8 -- performance improvements  
 2.0.6 -- `dist_v2_m` fixes and preliminary CAV functionality  
 2.0.5 -- added `to_rust` method for cycle  
 2.0.4 -- exposed `veh.set_veh_mass`
```

### Comparing `fastsim-2.0.22/pyproject.toml` & `fastsim-2.1.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 [build-system]
-requires = [
-    "setuptools>=40.6.0",
-    "wheel",
-    "setuptools-rust>=0.11.4",
-]
-build-backend = "setuptools.build_meta"
+requires = ["maturin>=0.15,<0.16"]
+build-backend = "maturin"
 
 [project]
 name = "fastsim"
-version = "2.0.22"
+version = "2.1.0"
 authors = [{ name = "NREL/MTES/CIMS/MBAP Group", email = "fastsim@nrel.gov" }]
 description = "Tool for modeling vehicle powertrains"
 readme = "README.md"
 license = {file = "LICENSE.md"}
 requires-python = ">=3.8,<3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -21,28 +17,41 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
 dependencies = [
     "pandas>=1",
     "matplotlib>=3.3",
     "numpy>=1.18",
+    "scipy",
     "seaborn>=0.10",
-    "pymoo==0.6",
     "typing_extensions",
+    "pyyaml",
+    "pytest",
 ]
 
 [project.urls]
-"Homepage" = "https://www.nrel.gov/transportation/fastsim.html" 
+Homepage = "https://www.nrel.gov/transportation/fastsim.html" 
 
 [project.optional-dependencies]
-dev = ["black", "pytest", "maturin"]
+dev = ["black", "maturin", "plotly", "ipykernel", "pymoo==0.6.0.1",]
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["."]  # list of folders that contain the packages (["."] by default)
 include = ["fastsim*"]  # package names should match these glob patterns (["*"] by default)
 namespaces = false  # to disable scanning PEP 420 namespaces (true by default)
 
-
-
+[tool.maturin]
+python-source="python"
+features = ["pyo3/extension-module"]
+module-name = "fastsim.fastsimrust"
+manifest-path = "rust/fastsim-py/Cargo.toml"
+include = [
+    { format = "sdist", path = "rust/fastsim-core/Cargo.toml"},
+    { format = "sdist", path = "rust/fastsim-core/src/*"},
+    { format = "sdist", path = "rust/fastsim-core/proc-macros/Cargo.toml"},
+    { format = "sdist", path = "rust/fastsim-core/proc-macros/src/*"},
+    { format = "sdist", path = "rust/fastsim-py/Cargo.toml"},
+    { format = "sdist", path = "rust/fastsim-py/src/*"},
+]
```

### Comparing `fastsim-2.0.22/rust/Cargo.toml` & `fastsim-2.1.0/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-cli/src/bin/fastsim-cli.rs` & `fastsim-2.1.0/rust/fastsim-cli/src/bin/fastsim-cli.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 use clap::{ArgGroup, Parser};
 use serde::{Deserialize, Serialize};
 use serde_json::{json, Value};
 
 use std::fs;
 
-extern crate fastsim_core;
 use fastsim_core::{
     cycle::RustCycle, params::MPH_PER_MPS, simdrive::RustSimDrive, simdrivelabel::get_label_fe,
-    simdrivelabel::get_net_accel, simdrivelabel::make_accel_trace,
+    simdrivelabel::get_net_accel, simdrivelabel::make_accel_trace, traits::SerdeAPI,
     utils::interpolate_vectors as interp, vehicle::RustVehicle, vehicle_utils::abc_to_drag_coeffs,
 };
 
 /// Wrapper for fastsim.
 /// After running `cargo build --release`, run with
 /// ```bash
 /// ./target/release/fastsim-cli --veh-file ~/Documents/GitHub/fastsim/fastsim/resources/vehdb/2012_Ford_Fusion.yaml --cyc-file ~/Documents/GitHub/fastsim/fastsim/resources/cycles/udds.csv
@@ -71,46 +70,42 @@
     /// coastdown coefficients for road load vs speed (lbf/mph)
     b: Option<f64>,
     #[clap(long, value_parser)]
     /// coastdown coefficients for road load vs speed (lbf/mph^2)
     c: Option<f64>,
 }
 
-#[derive(Debug, Deserialize, Serialize)]
+#[derive(Debug, Deserialize, Serialize, PartialEq, Clone)]
 #[allow(non_snake_case)]
 struct AdoptResults {
     adjCombMpgge: f64,
     rangeMiles: f64,
     UF: f64,
     adjCombKwhPerMile: f64,
     accel: f64,
     traceMissInMph: f64,
     h2AndDiesel: Option<H2AndDieselResults>,
 }
 
+impl SerdeAPI for AdoptResults {}
+
 #[derive(Debug, Deserialize, Serialize)]
 #[allow(non_snake_case)]
 struct AdoptHDResults {
     adjCombMpgge: f64,
     rangeMiles: f64,
     UF: f64,
     adjCombKwhPerMile: f64,
     accel: f64,
     // add more results here
 }
 
-trait SerdeAPI: Serialize + for<'a> Deserialize<'a> {
-    fn to_json(&self) -> String {
-        serde_json::to_string(&self).unwrap()
-    }
-}
-
-impl<T> SerdeAPI for T where T: Serialize + for<'a> Deserialize<'a> {}
+impl SerdeAPI for H2AndDieselResults {}
 
-#[derive(Debug, Deserialize, Serialize)]
+#[derive(Debug, Deserialize, Serialize, PartialEq, Clone)]
 pub struct H2AndDieselResults {
     pub h2_kwh: f64,
     pub h2_gge: f64,
     pub h2_mpgge: f64,
     pub diesel_kwh: f64,
     pub diesel_gals: f64,
     pub diesel_gge: f64,
@@ -302,14 +297,16 @@
             main_separator!(),
             "..",
             main_separator!(),
             "..",
             main_separator!(),
             "..",
             main_separator!(),
+            "python",
+            main_separator!(),
             "fastsim",
             main_separator!(),
             "resources",
             main_separator!(),
             "cycles",
             main_separator!(),
             "HHDDTCruiseSmooth.csv"
@@ -377,15 +374,15 @@
     } else if x == 4 {
         String::from("BEV")
     } else {
         x.to_string()
     }
 }
 
-#[derive(Debug, Deserialize, Serialize)]
+#[derive(Debug, Deserialize, Serialize, Clone, PartialEq)]
 struct ArrayObject {
     pub v: i64,
     pub dim: Vec<usize>,
     pub data: Vec<f64>,
 }
 
 /// Takes a vector of floats and transforms it into an object representation
@@ -410,14 +407,19 @@
     vec_of_f64
 }
 
 fn transform_array_of_value_to_ndarray_representation(array_of_values: &Vec<Value>) -> ArrayObject {
     array_to_object_representation(&transform_array_of_value_to_vec_of_f64(array_of_values))
 }
 
+#[derive(Debug, Deserialize, Serialize, Clone, PartialEq)]
+struct ParsedValue(Value);
+
+impl SerdeAPI for ParsedValue {}
+
 /// Rewrites the ADOPT JSON string to be in compliance with what FASTSim expects for JSON input.
 fn json_rewrite(x: String) -> (String, Option<Vec<f64>>, Option<Vec<f64>>) {
     let adoptstring = x;
 
     let mut fc_pwr_out_perc: Option<Vec<f64>> = None;
     let mut hd_h2_diesel_ice_h2share: Option<Vec<f64>> = None;
 
@@ -509,11 +511,11 @@
     if mc_max_elec_in_kw_raw.is_number() {
         let mc_max_elec_in_kw_value = mc_max_elec_in_kw_raw.as_f64().unwrap();
         parsed_data["mcMaxElecInKw"] = json!(mc_max_elec_in_kw_value);
     }
 
     parsed_data["stop_start"] = json!(false);
 
-    let adoptstring = parsed_data.to_json();
+    let adoptstring = ParsedValue(parsed_data).to_json();
 
     return (adoptstring, fc_pwr_out_perc, hd_h2_diesel_ice_h2share);
 }
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/Cargo.toml` & `fastsim-2.1.0/rust/fastsim-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [package]
 name = "fastsim-core"
 version = "0.1.0"
 edition = "2021"
 
 [dependencies]
-pyo3 = { workspace = true, features = ["extension-module"], optional = true }
+pyo3 = { workspace = true, features = ["extension-module", "anyhow"], optional = true }
 anyhow = { workspace = true }
 serde = { workspace = true, features = ["derive"] }
 serde_yaml = {workspace = true}
 ndarray = { version = "0.15.4", features=["serde"] }
 csv = "1.1"
 proc-macros = { path = "proc-macros" }
 serde_json = "1.0.81"
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs` & `fastsim-2.1.0/rust/fastsim-core/proc-macros/src/add_pyo3_api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -129,15 +129,18 @@
                         (
                             Regex::new(r"Array1 < (.+) >").unwrap(),
                             "Array1".parse::<TokenStream2>().unwrap(),
                             "Self(Array1::from_vec(v))".parse::<TokenStream2>().unwrap(),
                             "self.0.to_vec()".parse::<TokenStream2>().unwrap(),
                         )
                     } else {
-                        panic!("Invalid container type.  Must be Array1 or Vec.")
+                        abort!(
+                            ftype.span(),
+                            "Invalid container type.  Must be Array1 or Vec."
+                        )
                         // replace with proc_macro_error::abort macro
                     };
 
                     // println!("{}", type_str);
                     // println!("{}", &re.captures(&type_str).unwrap()[1]);
                     let contained_dtype: TokenStream2 = re.captures(&type_str).unwrap()[1]
                         .to_string()
@@ -189,18 +192,20 @@
                         pub fn new(value: #container<#contained_dtype>) -> Self {
                             Self(value)
                         }
                     });
                 }
             }
         } else {
-            panic!("Likely invalid use of `add_pyo3_api` macro.");
+            abort_call_site!(
+                "`add_pyo3_api` works only on tuple structs with `Vec` or `Array` in the name"
+            );
         }
     } else {
-        panic!("Likely invalid use of `add_pyo3_api` macro.");
+        abort_call_site!("`add_pyo3_api` works only on named and tuple structs.");
     };
 
     // py_impl_block.extend::<TokenStream2>(quote! {
     //     #[classmethod]
     //     #[pyo3(name = "default")]
     //     pub fn default_py(_cls: &PyType) -> PyResult<Self> {
     //         Ok(Self::default())
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs` & `fastsim-2.1.0/rust/fastsim-core/proc-macros/src/approx_eq_derive.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 use crate::imports::*;
 
 pub fn approx_eq_derive(input: TokenStream) -> TokenStream {
     let ast: DeriveInput = syn::parse(input).unwrap();
     let name = &ast.ident;
 
-    let mut fields = Vec::new();
-    match ast.data {
-        syn::Data::Struct(s) => {
-            for field in s.fields.iter() {
-                fields.push(field.clone());
-            }
-        }
-        _ => panic!("#[derive(ApproxEq)] only works on structs"),
-    }
+    let fields = match ast.data {
+        syn::Data::Struct(s) => s.fields,
+        _ => abort_call_site!("#[derive(ApproxEq)] only works on structs"),
+    };
 
     let field_names = fields
         .iter()
         .map(|f| f.ident.as_ref().unwrap())
         .collect::<Vec<_>>();
 
     let mut generated = TokenStream2::new();
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/proc-macros/src/history_vec_derive.rs` & `fastsim-2.1.0/rust/fastsim-core/proc-macros/src/history_vec_derive.rs`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     let mut fields = Vec::new();
     match ast.data {
         syn::Data::Struct(s) => {
             for field in s.fields.iter() {
                 fields.push(field.clone());
             }
         }
-        _ => panic!("#[derive(HistoryVec)] only works on structs"),
+        _ => abort_call_site!("#[derive(HistoryVec)] only works on structs"),
     }
     let field_names = fields
         .iter()
         .map(|f| f.ident.as_ref().unwrap())
         .collect::<Vec<_>>();
 
     let field_names_no_orphaned = field_names
@@ -104,14 +104,16 @@
             }
 
             pub fn is_empty(&self) -> bool {
                 self.#first_field.is_empty()
             }
         }
 
+        impl SerdeAPI for #new_name {}
+
         impl Default for #new_name {
             fn default() -> #new_name {
                 #new_name::new()
             }
         }
     });
     generated.into()
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/proc-macros/src/lib.rs` & `fastsim-2.1.0/rust/fastsim-core/proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/proc-macros/src/utilities.rs` & `fastsim-2.1.0/rust/fastsim-core/proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/air.rs` & `fastsim-2.1.0/rust/fastsim-core/src/air.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/cycle.rs` & `fastsim-2.1.0/rust/fastsim-core/src/vehicle.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,1092 +1,1230 @@
-//! Module containing drive cycle struct and related functions.
-
-extern crate ndarray;
-
-#[cfg(feature = "pyo3")]
-use std::collections::HashMap;
-use std::fs::File;
-use std::path::PathBuf;
+//! Module containing vehicle struct and related functions.
 
 // local
 use crate::imports::*;
 use crate::params::*;
-use crate::proc_macros::add_pyo3_api;
+use crate::proc_macros::{add_pyo3_api, ApproxEq};
 #[cfg(feature = "pyo3")]
 use crate::pyo3imports::*;
-use crate::utils::*;
-
-#[cfg_attr(feature = "pyo3", pyfunction)]
-/// # Arguments
-/// - n: Int, number of time-steps away from rendezvous
-/// - d0: Num, distance of simulated vehicle, $\frac{m}{s}$
-/// - v0: Num, speed of simulated vehicle, $\frac{m}{s}$
-/// - dr: Num, distance of rendezvous point, $m$
-/// - vr: Num, speed of rendezvous point, $\frac{m}{s}$
-/// - dt: Num, step duration, $s$
-///
-/// # Returns
-/// (Tuple 'jerk_m__s3': Num, 'accel_m__s2': Num)
-/// - Constant jerk and acceleration for initial time step.
-pub fn calc_constant_jerk_trajectory(
-    n: usize,
-    d0: f64,
-    v0: f64,
-    dr: f64,
-    vr: f64,
-    dt: f64,
-) -> (f64, f64) {
-    assert!(n > 1);
-    assert!(dr > d0);
-    let n = n as f64;
-    let ddr = dr - d0;
-    let dvr = vr - v0;
-    let k = (dvr - (2.0 * ddr / (n * dt)) + 2.0 * v0)
-        / (0.5 * n * (n - 1.0) * dt
-            - (1.0 / 3.0) * (n - 1.0) * (n - 2.0) * dt
-            - 0.5 * (n - 1.0) * dt * dt);
-    let a0 = ((ddr / dt)
-        - n * v0
-        - ((1.0 / 6.0) * n * (n - 1.0) * (n - 2.0) * dt + 0.25 * n * (n - 1.0) * dt * dt) * k)
-        / (0.5 * n * n * dt);
-    (k, a0)
-}
-
-#[cfg_attr(feature = "pyo3", pyfunction)]
-/// Calculate distance (m) after n timesteps
-///
-/// INPUTS:
-/// - n: Int, numer of timesteps away to calculate
-/// - d0: Num, initial distance (m)
-/// - v0: Num, initial speed (m/s)
-/// - a0: Num, initial acceleration (m/s2)
-/// - k: Num, constant jerk
-/// - dt: Num, duration of a timestep (s)
-///
-/// NOTE:
-/// - this is the distance traveled from start (i.e., n=0) measured at sample point n
-/// RETURN: Num, the distance at n timesteps away (m)
-pub fn dist_for_constant_jerk(n: usize, d0: f64, v0: f64, a0: f64, k: f64, dt: f64) -> f64 {
-    let n = n as f64;
-    let term1 = dt
-        * ((n * v0)
-            + (0.5 * n * (n - 1.0) * a0 * dt)
-            + ((1.0 / 6.0) * k * dt * (n - 2.0) * (n - 1.0) * n));
-    let term2 = 0.5 * dt * dt * ((n * a0) + (0.5 * n * (n - 1.0) * k * dt));
-    d0 + term1 + term2
-}
-
-#[cfg_attr(feature = "pyo3", pyfunction)]
-/// Calculate speed (m/s) n timesteps away via a constant-jerk acceleration
-///
-/// INPUTS:
-/// - n: Int, numer of timesteps away to calculate
-/// - v0: Num, initial speed (m/s)
-/// - a0: Num, initial acceleration (m/s2)
-/// - k: Num, constant jerk
-/// - dt: Num, duration of a timestep (s)
-///
-/// NOTE:
-/// - this is the speed at sample n
-/// - if n == 0, speed is v0
-/// - if n == 1, speed is v0 + a0*dt, etc.
-///
-/// RETURN: Num, the speed n timesteps away (m/s)
-pub fn speed_for_constant_jerk(n: usize, v0: f64, a0: f64, k: f64, dt: f64) -> f64 {
-    let n = n as f64;
-    v0 + (n * a0 * dt) + (0.5 * n * (n - 1.0) * k * dt)
-}
-
-#[cfg_attr(feature = "pyo3", pyfunction)]
-/// Calculate the acceleration n timesteps away
-///
-/// INPUTS:
-/// - n: Int, number of times steps away to calculate
-/// - a0: Num, initial acceleration (m/s2)
-/// - k: Num, constant jerk (m/s3)
-/// - dt: Num, time-step duration in seconds
-///
-/// NOTE:
-/// - this is the constant acceleration over the time-step from sample n to sample n+1
-///
-/// RETURN: Num, the acceleration n timesteps away (m/s2)
-pub fn accel_for_constant_jerk(n: usize, a0: f64, k: f64, dt: f64) -> f64 {
-    let n = n as f64;
-    a0 + (n * k * dt)
-}
-
-/// Apply `accel_for_constant_jerk` to full
-pub fn accel_array_for_constant_jerk(nmax: usize, a0: f64, k: f64, dt: f64) -> Array1<f64> {
-    let mut accels: Vec<f64> = Vec::new();
-    for n in 0..nmax {
-        accels.push(accel_for_constant_jerk(n, a0, k, dt));
-    }
-    Array1::from_vec(accels)
-}
-
-/// Calculate the average speed per each step in m/s
-pub fn average_step_speeds(cyc: &RustCycle) -> Array1<f64> {
-    let mut result: Vec<f64> = Vec::with_capacity(cyc.len());
-    result.push(0.0);
-    for i in 1..cyc.len() {
-        result.push(0.5 * (cyc.mps[i] + cyc.mps[i - 1]));
-    }
-    Array1::from_vec(result)
-}
-
-/// Calculate the average step speed at step i in m/s
-/// (i.e., from sample point i-1 to i)
-pub fn average_step_speed_at(cyc: &RustCycle, i: usize) -> f64 {
-    0.5 * (cyc.mps[i] + cyc.mps[i - 1])
-}
 
-/// Sum of the distance traveled over each step using
-/// trapezoidal integration
-pub fn trapz_step_distances(cyc: &RustCycle) -> Array1<f64> {
-    average_step_speeds(cyc) * cyc.dt_s()
+use lazy_static::lazy_static;
+use regex::Regex;
+use validator::Validate;
+
+// veh_pt_type options
+pub const CONV: &str = "Conv";
+pub const HEV: &str = "HEV";
+pub const PHEV: &str = "PHEV";
+pub const BEV: &str = "BEV";
+pub const VEH_PT_TYPES: [&str; 4] = [CONV, HEV, PHEV, BEV];
+lazy_static! {
+    static ref VEH_PT_TYPE_OPTIONS_REGEX: Regex = Regex::new("Conv|HEV|PHEV|BEV").unwrap();
+}
+
+// fc_eff_type options
+pub const SI: &str = "SI";
+pub const ATKINSON: &str = "Atkinson";
+pub const DIESEL: &str = "Diesel";
+pub const H2FC: &str = "H2FC";
+pub const HD_DIESEL: &str = "HD_Diesel";
+pub const FC_EFF_TYPES: [&str; 5] = [SI, ATKINSON, DIESEL, H2FC, HD_DIESEL];
+lazy_static! {
+    static ref FC_EFF_TYPE_OPTIONS_REGEX: Regex =
+        Regex::new("SI|Atkinson|Diesel|H2FC|HD_Diesel").unwrap();
 }
 
-pub fn trapz_step_distances_primitive(time_s: &Array1<f64>, mps: &Array1<f64>) -> Array1<f64> {
-    let mut delta_dists_m: Vec<f64> = Vec::with_capacity(time_s.len());
-    delta_dists_m.push(0.0);
-    for i in 1..time_s.len() {
-        delta_dists_m.push((time_s[i] - time_s[i - 1]) * 0.5 * (mps[i] + mps[i - 1]));
+#[derive(Default, Serialize, Deserialize, Clone, Debug, PartialEq, ApproxEq, Validate)]
+#[add_pyo3_api(
+    #[pyo3(name = "set_veh_mass")]
+    pub fn set_veh_mass_py(&mut self) {
+        self.set_veh_mass()
     }
-    Array1::from_vec(delta_dists_m)
-}
 
-/// The distance traveled from start at the beginning of step i
-/// (i.e., distance traveled up to sample point i-1)
-/// Distance is in meters.
-pub fn trapz_step_start_distance(cyc: &RustCycle, i: usize) -> f64 {
-    let mut dist_m: f64 = 0.0;
-    for i in 1..i {
-        dist_m += (cyc.time_s[i] - cyc.time_s[i - 1]) * 0.5 * (cyc.mps[i] + cyc.mps[i - 1]);
+    pub fn get_max_regen_kwh(&self) -> f64 {
+        self.max_regen_kwh()
     }
-    dist_m
-}
-
-/// The distance traveled during step i in meters
-/// (i.e., from sample point i-1 to i)
-pub fn trapz_distance_for_step(cyc: &RustCycle, i: usize) -> f64 {
-    average_step_speed_at(cyc, i) * cyc.dt_s_at_i(i)
-}
-
-/// Calculate the distance from step i_start to the start of step i_end
-/// (i.e., distance from sample point i_start-1 to i_end-1)
-pub fn trapz_distance_over_range(cyc: &RustCycle, i_start: usize, i_end: usize) -> f64 {
-    trapz_step_distances(cyc).slice(s![i_start..i_end]).sum()
-}
 
-/// Calculate the time in a cycle spent moving
-/// - stopped_speed_m_per_s: the speed above which we are considered to be moving
-/// RETURN: the time spent moving in seconds
-pub fn time_spent_moving(cyc: &RustCycle, stopped_speed_m_per_s: Option<f64>) -> f64 {
-    let mut t_move_s = 0.0;
-    let stopped_speed_m_per_s = stopped_speed_m_per_s.unwrap_or(0.0);
-    for idx in 1..cyc.time_s.len() {
-        let dt = cyc.time_s[idx] - cyc.time_s[idx - 1];
-        let vavg = (cyc.mps[idx] + cyc.mps[idx - 1]) / 2.0;
-        if vavg > stopped_speed_m_per_s {
-            t_move_s += dt;
-        }
+    #[getter]
+    pub fn get_mc_peak_eff(&self) -> f64 {
+        self.mc_peak_eff()
     }
-    t_move_s
-}
 
-/// Split a cycle into an array of microtrips with one microtrip being a start
-/// to subsequent stop plus any idle (stopped time).
-/// Arguments:
-/// ----------
-/// cycle: drive cycle converted to dictionary by cycle.get_cyc_dict()
-/// stop_speed_m__s: speed at which vehicle is considered stopped for trip
-///     separation
-/// keep_name: (optional) bool, if True and cycle contains "name", adds
-///     that name to all microtrips
-pub fn to_microtrips(cycle: &RustCycle, stop_speed_m_per_s: Option<f64>) -> Vec<RustCycle> {
-    let stop_speed_m_per_s = stop_speed_m_per_s.unwrap_or(1e-6);
-    let mut microtrips: Vec<RustCycle> = Vec::new();
-    let ts = cycle.time_s.to_vec();
-    let vs = cycle.mps.to_vec();
-    let gs = cycle.grade.to_vec();
-    let rs = cycle.road_type.to_vec();
-    let mut mt_ts: Vec<f64> = Vec::new();
-    let mut mt_vs: Vec<f64> = Vec::new();
-    let mut mt_gs: Vec<f64> = Vec::new();
-    let mut mt_rs: Vec<f64> = Vec::new();
-    let mut moving = false;
-    for idx in 0..ts.len() {
-        let t = ts[idx];
-        let v = vs[idx];
-        let g = gs[idx];
-        let r = rs[idx];
-        if v > stop_speed_m_per_s && !moving && mt_ts.len() > 1 {
-            let last_idx = mt_ts.len() - 1;
-            let last_t = mt_ts[last_idx];
-            let last_v = mt_vs[last_idx];
-            let last_g = mt_gs[last_idx];
-            let last_r = mt_rs[last_idx];
-            mt_ts = mt_ts.iter().map(|t| -> f64 { t - mt_ts[0] }).collect();
-            microtrips.push(RustCycle::new(
-                mt_ts.clone(),
-                mt_vs.clone(),
-                mt_gs.clone(),
-                mt_rs.clone(),
-                cycle.name.clone(),
-            ));
-            mt_ts = vec![last_t];
-            mt_vs = vec![last_v];
-            mt_gs = vec![last_g];
-            mt_rs = vec![last_r];
-        }
-        mt_ts.push(t);
-        mt_vs.push(v);
-        mt_gs.push(g);
-        mt_rs.push(r);
-        moving = v > stop_speed_m_per_s;
-    }
-    if !mt_ts.is_empty() {
-        mt_ts = mt_ts.iter().map(|t| -> f64 { t - mt_ts[0] }).collect();
-        microtrips.push(RustCycle::new(
-            mt_ts,
-            mt_vs,
-            mt_gs,
-            mt_rs,
-            cycle.name.clone(),
-        ));
+    // TODO: refactor this to have a non-py and `_py` version
+    #[setter]
+    pub fn set_mc_peak_eff(&mut self, new_peak: f64) {
+        let mc_max_eff = ndarrmax(&self.mc_eff_array);
+        self.mc_eff_array *= new_peak / mc_max_eff;
+        let mc_max_full_eff = arrmax(&self.mc_full_eff_array);
+        self.mc_full_eff_array = self
+            .mc_full_eff_array
+            .iter()
+            .map(|e: &f64| -> f64 { e * (new_peak / mc_max_full_eff) })
+            .collect();
     }
-    microtrips
-}
 
-/// Create distance and target speeds by microtrip
-/// This helper function splits a cycle up into microtrips and returns a list of 2-tuples of:
-/// (distance from start in meters, target speed in meters/second)
-/// - cyc: the cycle to operate on
-/// - blend_factor: float, from 0 to 1
-///     if 0, use average speed of the microtrip
-///     if 1, use average speed while moving (i.e., no stopped time)
-///     else something in between
-/// - min_target_speed_mps: float, the minimum target speed allowed (m/s)
-/// RETURN: list of 2-tuple of (float, float) representing the distance of start of
-///     each microtrip and target speed for that microtrip
-/// NOTE: target speed per microtrip is not allowed to be below min_target_speed_mps
-pub fn create_dist_and_target_speeds_by_microtrip(
-    cyc: &RustCycle,
-    blend_factor: f64,
-    min_target_speed_mps: f64,
-) -> Vec<(f64, f64)> {
-    let blend_factor = if blend_factor < 0.0 {
-        0.0
-    } else if blend_factor > 1.0 {
-        1.0
-    } else {
-        blend_factor
-    };
-    let mut dist_and_tgt_speeds: Vec<(f64, f64)> = Vec::new();
-    // Split cycle into microtrips
-    let microtrips = to_microtrips(cyc, None);
-    let mut dist_at_start_of_microtrip_m = 0.0;
-    for mt_cyc in microtrips {
-        let mt_dist_m = mt_cyc.dist_m().sum();
-        let mt_time_s = mt_cyc.time_s.last().unwrap() - mt_cyc.time_s.first().unwrap();
-        let mt_moving_time_s = time_spent_moving(&mt_cyc, None);
-        let mt_avg_spd_m_per_s = if mt_time_s > 0.0 {
-            mt_dist_m / mt_time_s
-        } else {
-            0.0
-        };
-        let mt_moving_avg_spd_m_per_s = if mt_moving_time_s > 0.0 {
-            mt_dist_m / mt_moving_time_s
-        } else {
-            0.0
-        };
-        let mt_target_spd_m_per_s =
-            (blend_factor * (mt_moving_avg_spd_m_per_s - mt_avg_spd_m_per_s) + mt_avg_spd_m_per_s)
-                .min(mt_moving_avg_spd_m_per_s)
-                .max(mt_avg_spd_m_per_s);
-        if mt_dist_m > 0.0 {
-            dist_and_tgt_speeds.push((
-                dist_at_start_of_microtrip_m,
-                mt_target_spd_m_per_s.max(min_target_speed_mps),
-            ));
-            dist_at_start_of_microtrip_m += mt_dist_m;
-        }
+    #[getter]
+    pub fn get_max_fc_eff_kw(&self) -> f64 {
+        self.max_fc_eff_kw()
     }
-    dist_and_tgt_speeds
-}
 
-/// - cyc: fastsim.cycle.Cycle
-/// - absolute_time_s: float, the seconds to extend
-/// - time_fraction: float, the fraction of the original cycle time to add on
-/// - use_rust: bool, if True, return a RustCycle instance, else a normal Python Cycle
-/// RETURNS: fastsim.cycle.Cycle (or fastsimrust.RustCycle), the new cycle with stopped time appended
-/// NOTE: additional time is rounded to the nearest second
-pub fn extend_cycle(
-    cyc: &RustCycle,
-    absolute_time_s: Option<f64>, // =0.0,
-    time_fraction: Option<f64>,   // =0.0,
-) -> RustCycle {
-    let absolute_time_s = absolute_time_s.unwrap_or(0.0);
-    let time_fraction = time_fraction.unwrap_or(0.0);
-    let mut ts = cyc.time_s.to_vec();
-    let mut vs = cyc.mps.to_vec();
-    let mut gs = cyc.grade.to_vec();
-    let mut rs = cyc.road_type.to_vec();
-    let extra_time_s = (absolute_time_s + (time_fraction * ts.last().unwrap())).round() as i32;
-    if extra_time_s == 0 {
-        return cyc.clone();
-    }
-    let dt = 1;
-    let t_end = *ts.last().unwrap();
-    let mut idx = 1;
-    while dt * idx <= extra_time_s {
-        let dt_extra = (dt * idx) as f64;
-        ts.push(t_end + dt_extra);
-        vs.push(0.0);
-        gs.push(0.0);
-        rs.push(0.0);
-        idx += 1;
+    #[getter]
+    pub fn get_fc_peak_eff(&self) -> f64 {
+        self.fc_peak_eff()
     }
-    RustCycle::new(ts, vs, gs, rs, cyc.name.clone())
-}
-
-#[cfg(feature = "pyo3")]
-#[allow(unused)]
-pub fn register(_py: Python<'_>, m: &PyModule) -> Result<(), anyhow::Error> {
-    m.add_function(wrap_pyfunction!(calc_constant_jerk_trajectory, m)?)?;
-    m.add_function(wrap_pyfunction!(accel_for_constant_jerk, m)?)?;
-    m.add_function(wrap_pyfunction!(speed_for_constant_jerk, m)?)?;
-    m.add_function(wrap_pyfunction!(dist_for_constant_jerk, m)?)?;
-    Ok(())
-}
-
-#[derive(Default, PartialEq, Clone, Debug, Deserialize, Serialize)]
-pub struct RustCycleElement {
-    /// time [s]
-    #[serde(alias = "cycSecs")]
-    pub time_s: f64,
-    /// speed [m/s]
-    #[serde(alias = "cycMps")]
-    pub mps: f64,
-    /// grade [rise/run]
-    #[serde(alias = "cycGrade")]
-    pub grade: f64,
-    /// max possible charge rate from roadway
-    #[serde(alias = "cycRoadType")]
-    pub road_type: f64,
-}
 
-#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Default)]
-#[add_pyo3_api(
-    #[new]
-    pub fn __new__(
-        cyc: &RustCycle,
-    ) -> Self {
-        Self::new(cyc)
+    #[setter]
+    pub fn set_fc_peak_eff(&mut self, new_peak: f64) {
+        let old_fc_peak_eff = self.fc_peak_eff();
+        let multiplier = new_peak / old_fc_peak_eff;
+        self.fc_eff_array = self
+            .fc_eff_array
+            .iter()
+            .map(|eff: &f64| -> f64 { eff * multiplier })
+            .collect();
+        let new_fc_peak_eff = self.fc_peak_eff();
+        let eff_map_multiplier = new_peak / new_fc_peak_eff;
+        self.fc_eff_map = self
+            .fc_eff_map
+            .map(|eff| -> f64 { eff * eff_map_multiplier });
+    }
+
+    #[pyo3(name = "set_derived")]
+    pub fn set_derived_py(&mut self) {
+        self.set_derived().unwrap()
+    }
+
+    /// An identify function to allow RustVehicle to be used as a python vehicle and respond to this method
+    /// Returns a clone of the current object
+    pub fn to_rust(&self) -> PyResult<Self> {
+        Ok(self.clone())
     }
 )]
-pub struct RustCycleCache {
-    pub grade_all_zero: bool,
-    pub trapz_step_distances_m: Array1<f64>,
-    pub trapz_distances_m: Array1<f64>,
-    pub trapz_elevations_m: Array1<f64>,
-    pub stops: Array1<bool>,
-    interp_ds: Array1<f64>,
-    interp_is: Array1<f64>,
-    interp_hs: Array1<f64>,
-    grades: Array1<f64>,
+/// Struct containing vehicle attributes
+/// # Python Examples
+/// ```python
+/// import fastsim
+///
+/// ## Load drive cycle by name
+/// cyc_py = fastsim.cycle.Cycle.from_file("udds")
+/// cyc_rust = cyc_py.to_rust()
+/// ```
+pub struct RustVehicle {
+    #[serde(skip)]
+    #[api(has_orphaned)]
+    /// Physical properties, see [RustPhysicalProperties](RustPhysicalProperties)
+    pub props: RustPhysicalProperties,
+    /// Vehicle name
+    #[serde(alias = "name")]
+    pub scenario_name: String,
+    /// Vehicle database ID
+    #[serde(skip)]
+    pub selection: u32,
+    /// Vehicle year
+    #[serde(alias = "vehModelYear")]
+    pub veh_year: u32,
+    /// Vehicle powertrain type, one of \[[CONV](CONV), [HEV](HEV), [PHEV](PHEV), [BEV](BEV)\]
+    #[serde(alias = "vehPtType")]
+    #[validate(regex(
+        path = "VEH_PT_TYPE_OPTIONS_REGEX",
+        message = "must be one of [\"Conv\", \"HEV\", \"PHEV\", \"BEV\"]"
+    ))]
+    pub veh_pt_type: String,
+    /// Aerodynamic drag coefficient
+    #[serde(alias = "dragCoef")]
+    #[validate(range(min = 0))]
+    pub drag_coef: f64,
+    /// Frontal area, $m^2$
+    #[serde(alias = "frontalAreaM2")]
+    #[validate(range(min = 0))]
+    pub frontal_area_m2: f64,
+    /// Vehicle mass excluding cargo, passengers, and powertrain components, $kg$
+    #[serde(alias = "gliderKg")]
+    #[validate(range(min = 0))]
+    pub glider_kg: f64,
+    /// Vehicle center of mass height, $m$  
+    /// **NOTE:** positive for FWD, negative for RWD, AWD, 4WD
+    #[serde(alias = "vehCgM")]
+    pub veh_cg_m: f64,
+    /// Fraction of weight on the drive axle while stopped
+    #[serde(alias = "driveAxleWeightFrac")]
+    #[validate(range(min = 0, max = 1))]
+    pub drive_axle_weight_frac: f64,
+    /// Wheelbase, $m$
+    #[serde(alias = "wheelBaseM")]
+    #[validate(range(min = 0))]
+    pub wheel_base_m: f64,
+    /// Cargo mass including passengers, $kg$
+    #[serde(alias = "cargoKg")]
+    #[validate(range(min = 0))]
+    pub cargo_kg: f64,
+    /// Total vehicle mass, overrides mass calculation, $kg$
+    #[serde(alias = "vehOverrideKg")]
+    #[validate(range(min = 0))]
+    pub veh_override_kg: Option<f64>,
+    /// Component mass multiplier for vehicle mass calculation
+    #[serde(alias = "compMassMultiplier")]
+    #[validate(range(min = 0))]
+    pub comp_mass_multiplier: f64,
+    /// Fuel storage max power output, $kW$
+    #[serde(alias = "maxFuelStorKw")]
+    #[validate(range(min = 0))]
+    pub fs_max_kw: f64,
+    /// Fuel storage time to peak power, $s$
+    #[serde(alias = "fuelStorSecsToPeakPwr")]
+    #[validate(range(min = 0))]
+    pub fs_secs_to_peak_pwr: f64,
+    /// Fuel storage energy capacity, $kWh$
+    #[serde(alias = "fuelStorKwh")]
+    #[validate(range(min = 0))]
+    pub fs_kwh: f64,
+    /// Fuel specific energy, $\frac{kWh}{kg}$
+    #[serde(alias = "fuelStorKwhPerKg")]
+    #[validate(range(min = 0))]
+    pub fs_kwh_per_kg: f64,
+    /// Fuel converter peak continuous power, $kW$
+    #[serde(alias = "maxFuelConvKw")]
+    #[validate(range(min = 0))]
+    pub fc_max_kw: f64,
+    /// Fuel converter output power percentage map, x-values of [fc_eff_map](RustVehicle::fc_eff_map)
+    #[serde(alias = "fcPwrOutPerc")]
+    pub fc_pwr_out_perc: Array1<f64>,
+    /// Fuel converter efficiency map
+    #[serde(default)]
+    pub fc_eff_map: Array1<f64>,
+    /// Fuel converter efficiency type, one of \[[SI](SI), [ATKINSON](ATKINSON), [DIESEL](DIESEL), [H2FC](H2FC), [HD_DIESEL](HD_DIESEL)\]  
+    /// Used for calculating [fc_eff_map](RustVehicle::fc_eff_map), and other calculations if H2FC
+    #[serde(alias = "fcEffType")]
+    #[validate(regex(
+        path = "FC_EFF_TYPE_OPTIONS_REGEX",
+        message = "must be one of [\"SI\", \"Atkinson\", \"Diesel\", \"H2FC\", \"HD_Diesel\"]"
+    ))]
+    pub fc_eff_type: String,
+    /// Fuel converter time to peak power, $s$
+    #[serde(alias = "fuelConvSecsToPeakPwr")]
+    #[validate(range(min = 0))]
+    pub fc_sec_to_peak_pwr: f64,
+    /// Fuel converter base mass, $kg$
+    #[serde(alias = "fuelConvBaseKg")]
+    #[validate(range(min = 0))]
+    pub fc_base_kg: f64,
+    /// Fuel converter specific power (power-to-weight ratio), $\frac{kW}{kg}$
+    #[serde(alias = "fuelConvKwPerKg")]
+    #[validate(range(min = 0))]
+    pub fc_kw_per_kg: f64,
+    /// Minimum time fuel converter must be on before shutoff (for HEV, PHEV)
+    #[serde(alias = "minFcTimeOn")]
+    #[validate(range(min = 0))]
+    pub min_fc_time_on: f64,
+    /// Fuel converter idle power, $kW$
+    #[serde(alias = "idleFcKw")]
+    #[validate(range(min = 0))]
+    pub idle_fc_kw: f64,
+    /// Peak continuous electric motor power, $kW$
+    #[serde(alias = "mcMaxElecInKw")]
+    #[validate(range(min = 0))]
+    pub mc_max_kw: f64,
+    /// Electric motor output power percentage map, x-values of [mc_eff_map](RustVehicle::mc_eff_map)
+    #[serde(alias = "mcPwrOutPerc")]
+    pub mc_pwr_out_perc: Array1<f64>,
+    /// Electric motor efficiency map
+    #[serde(alias = "mcEffArray")]
+    pub mc_eff_map: Array1<f64>,
+    /// Electric motor time to peak power, $s$
+    #[serde(alias = "motorSecsToPeakPwr")]
+    #[validate(range(min = 0))]
+    pub mc_sec_to_peak_pwr: f64,
+    /// Motor power electronics mass per power output, $\frac{kg}{kW}$
+    #[serde(alias = "mcPeKgPerKw")]
+    #[validate(range(min = 0))]
+    pub mc_pe_kg_per_kw: f64,
+    /// Motor power electronics base mass, $kg$
+    #[serde(alias = "mcPeBaseKg")]
+    #[validate(range(min = 0))]
+    pub mc_pe_base_kg: f64,
+    /// Traction battery maximum power output, $kW$
+    #[serde(alias = "maxEssKw")]
+    #[validate(range(min = 0))]
+    pub ess_max_kw: f64,
+    /// Traction battery energy capacity, $kWh$
+    #[serde(alias = "maxEssKwh")]
+    #[validate(range(min = 0))]
+    pub ess_max_kwh: f64,
+    /// Traction battery mass per energy, $\frac{kg}{kWh}$
+    #[serde(alias = "essKgPerKwh")]
+    #[validate(range(min = 0))]
+    pub ess_kg_per_kwh: f64,
+    /// Traction battery base mass, $kg$
+    #[serde(alias = "essBaseKg")]
+    #[validate(range(min = 0))]
+    pub ess_base_kg: f64,
+    /// Traction battery round-trip efficiency
+    #[serde(alias = "essRoundTripEff")]
+    #[validate(range(min = 0, max = 1))]
+    pub ess_round_trip_eff: f64,
+    /// Traction battery cycle life coefficient A, see [reference](https://web.archive.org/web/20090529194442/http://www.ocean.udel.edu/cms/wkempton/Kempton-V2G-pdfFiles/PDF%20format/Duvall-V2G-batteries-June05.pdf)
+    #[serde(alias = "essLifeCoefA")]
+    pub ess_life_coef_a: f64,
+    /// Traction battery cycle life coefficient B, see [reference](https://web.archive.org/web/20090529194442/http://www.ocean.udel.edu/cms/wkempton/Kempton-V2G-pdfFiles/PDF%20format/Duvall-V2G-batteries-June05.pdf)
+    #[serde(alias = "essLifeCoefB")]
+    pub ess_life_coef_b: f64,
+    /// Traction battery minimum state of charge
+    #[serde(alias = "minSoc")]
+    #[validate(range(min = 0, max = 1))]
+    pub min_soc: f64,
+    /// Traction battery maximum state of charge
+    #[serde(alias = "maxSoc")]
+    #[validate(range(min = 0, max = 1))]
+    pub max_soc: f64,
+    /// ESS discharge effort toward max FC efficiency
+    #[serde(alias = "essDischgToFcMaxEffPerc")]
+    #[validate(range(min = 0, max = 1))]
+    pub ess_dischg_to_fc_max_eff_perc: f64,
+    /// ESS charge effort toward max FC efficiency
+    #[serde(alias = "essChgToFcMaxEffPerc")]
+    #[validate(range(min = 0, max = 1))]
+    pub ess_chg_to_fc_max_eff_perc: f64,
+    /// Mass moment of inertia per wheel, $kg \cdot m^2$
+    #[serde(alias = "wheelInertiaKgM2")]
+    #[validate(range(min = 0))]
+    pub wheel_inertia_kg_m2: f64,
+    /// Number of wheels
+    #[serde(alias = "numWheels")]
+    #[validate(range(min = 0))]
+    pub num_wheels: f64, // TODO: Shouldn't this just be a unsigned integer? u8 would work fine.
+    /// Rolling resistance coefficient
+    #[serde(alias = "wheelRrCoef")]
+    #[validate(range(min = 0))]
+    pub wheel_rr_coef: f64,
+    /// Wheel radius, $m$
+    #[serde(alias = "wheelRadiusM")]
+    #[validate(range(min = 0))]
+    pub wheel_radius_m: f64,
+    /// Wheel coefficient of friction
+    #[serde(alias = "wheelCoefOfFric")]
+    #[validate(range(min = 0))]
+    pub wheel_coef_of_fric: f64,
+    /// Speed where the battery reserved for accelerating is zero
+    #[serde(alias = "maxAccelBufferMph")]
+    #[validate(range(min = 0))]
+    pub max_accel_buffer_mph: f64,
+    /// Percent of usable battery energy reserved to help accelerate
+    #[serde(alias = "maxAccelBufferPercOfUseableSoc")]
+    #[validate(range(min = 0, max = 1))]
+    pub max_accel_buffer_perc_of_useable_soc: f64,
+    /// Percent SOC buffer for high accessory loads during cycles with long idle time
+    #[serde(alias = "percHighAccBuf")]
+    #[validate(range(min = 0))]
+    pub perc_high_acc_buf: f64,
+    /// Speed at which the fuel converter must turn on, $mph$
+    #[serde(alias = "mphFcOn")]
+    #[validate(range(min = 0))]
+    pub mph_fc_on: f64,
+    /// Power demand above which to require fuel converter on, $kW$
+    #[serde(alias = "kwDemandFcOn")]
+    #[validate(range(min = 0))]
+    pub kw_demand_fc_on: f64,
+    /// Maximum brake regeneration efficiency
+    #[serde(alias = "maxRegen")]
+    #[validate(range(min = 0, max = 1))]
+    pub max_regen: f64,
+    /// Stop/start micro-HEV flag
+    pub stop_start: bool,
+    /// Force auxiliary power load to come from fuel converter
+    #[serde(alias = "forceAuxOnFC")]
+    pub force_aux_on_fc: bool,
+    /// Alternator efficiency
+    #[serde(alias = "altEff")]
+    #[validate(range(min = 0, max = 1))]
+    pub alt_eff: f64,
+    /// Charger efficiency
+    #[serde(alias = "chgEff")]
+    #[validate(range(min = 0, max = 1))]
+    pub chg_eff: f64,
+    /// Auxiliary load power, $kW$
+    #[serde(alias = "auxKw")]
+    #[validate(range(min = 0))]
+    pub aux_kw: f64,
+    /// Transmission mass, $kg$
+    #[serde(alias = "transKg")]
+    #[validate(range(min = 0))]
+    pub trans_kg: f64,
+    /// Transmission efficiency
+    #[serde(alias = "transEff")]
+    #[validate(range(min = 0, max = 1))]
+    pub trans_eff: f64,
+    /// Maximum acceptable ratio of change in ESS energy to expended fuel energy (used in hybrid SOC balancing), $\frac{\Delta E_{ESS}}{\Delta E_{fuel}}$
+    #[serde(alias = "essToFuelOkError")]
+    #[validate(range(min = 0))]
+    pub ess_to_fuel_ok_error: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub small_motor_power_kw: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub large_motor_power_kw: f64,
+    // this and other fixed-size arrays can probably be vectors
+    // without any performance penalty with the current implementation
+    // of the functions in utils.rs
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub fc_perc_out_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub regen_a: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub regen_b: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub charging_on: bool,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub no_elec_sys: bool,
+    #[doc(hidden)]
+    // all of the parameters that are set in `set_derived` should be skipped by serde
+    #[serde(skip)]
+    pub no_elec_aux: bool,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub max_roadway_chg_kw: Array1<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub input_kw_out_array: Array1<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub fc_kw_out_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(default)]
+    #[serde(alias = "fcEffArray")]
+    pub fc_eff_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub modern_max: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_eff_array: Array1<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_kw_in_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_kw_out_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_max_elec_in_kw: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_full_eff_array: Vec<f64>,
+    #[doc(hidden)]
+    #[serde(alias = "vehKg")]
+    pub veh_kg: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub max_trac_mps2: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub ess_mass_kg: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_mass_kg: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub fc_mass_kg: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub fs_mass_kg: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub mc_perc_out_array: Vec<f64>,
+    // these probably don't need to be in rust
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_udds_mpgge: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_hwy_mpgge: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_comb_mpgge: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_udds_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_hwy_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_comb_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_cd_range_mi: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_const65_mph_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_const60_mph_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_const55_mph_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_const45_mph_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_unadj_udds_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_unadj_hwy_kwh_per_mile: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val0_to60_mph: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_ess_life_miles: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_range_miles: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_veh_base_cost: f64,
+    #[doc(hidden)]
+    #[serde(skip)]
+    pub val_msrp: f64,
+    /// Fuel converter efficiency peak override, scales entire curve
+    #[serde(skip)]
+    #[validate(range(min = 0, max = 1))]
+    pub fc_peak_eff_override: Option<f64>,
+    /// Motor efficiency peak override, scales entire curve
+    #[serde(skip)]
+    #[validate(range(min = 0, max = 1))]
+    pub mc_peak_eff_override: Option<f64>,
+    #[serde(skip)]
+    #[doc(hidden)]
+    pub orphaned: bool,
 }
 
-impl RustCycleCache {
-    pub fn new(cyc: &RustCycle) -> Self {
-        let tol = 1e-6;
-        let num_items = cyc.time_s.len();
-        let grade_all_zero = cyc.grade.iter().fold(true, |flag, &g| flag && g == 0.0);
-        let trapz_step_distances_m = trapz_step_distances(cyc);
-        let trapz_distances_m = ndarrcumsum(&trapz_step_distances_m);
-        let trapz_elevations_m = if grade_all_zero {
-            Array::zeros(num_items)
+/// RustVehicle rust methods
+impl RustVehicle {
+    /// Sets the following parameters:
+    /// - `ess_mass_kg`
+    /// - `mc_mass_kg`
+    /// - `fc_mass_kg`
+    /// - `fs_mass_kg`
+    /// - `veh_kg`
+    /// - `max_trac_mps2`
+    #[allow(clippy::neg_cmp_op_on_partial_ord)]
+    pub fn set_veh_mass(&mut self) {
+        if self.veh_override_kg.is_none() {
+            self.ess_mass_kg = if self.ess_max_kwh == 0.0 || self.ess_max_kw == 0.0 {
+                0.0
+            } else {
+                ((self.ess_max_kwh * self.ess_kg_per_kwh) + self.ess_base_kg)
+                    * self.comp_mass_multiplier
+            };
+            self.mc_mass_kg = if self.mc_max_kw == 0.0 {
+                0.0
+            } else {
+                (self.mc_pe_base_kg + (self.mc_pe_kg_per_kw * self.mc_max_kw))
+                    * self.comp_mass_multiplier
+            };
+            self.fc_mass_kg = if self.fc_max_kw == 0.0 {
+                0.0
+            } else {
+                (1.0 / self.fc_kw_per_kg * self.fc_max_kw + self.fc_base_kg)
+                    * self.comp_mass_multiplier
+            };
+            self.fs_mass_kg = if self.fs_max_kw == 0.0 {
+                0.0
+            } else {
+                ((1.0 / self.fs_kwh_per_kg) * self.fs_kwh) * self.comp_mass_multiplier
+            };
+            self.veh_kg = self.cargo_kg
+                + self.glider_kg
+                + self.trans_kg * self.comp_mass_multiplier
+                + self.ess_mass_kg
+                + self.mc_mass_kg
+                + self.fc_mass_kg
+                + self.fs_mass_kg;
         } else {
-            let xs = Array::from_iter(
-                cyc.grade
-                    .iter()
-                    .zip(&trapz_step_distances_m)
-                    .map(|(g, dd)| g.atan().cos() * dd * g),
-            );
-            ndarrcumsum(&xs)
-        };
-        let stops = Array::from_iter(cyc.mps.iter().map(|v| v <= &tol));
-        let mut interp_ds: Vec<f64> = Vec::with_capacity(num_items);
-        let mut interp_is: Vec<f64> = Vec::with_capacity(num_items);
-        let mut interp_hs: Vec<f64> = Vec::with_capacity(num_items);
-        for idx in 0..num_items {
-            let d = trapz_distances_m[idx];
-            if interp_ds.len() == 0 || d > *interp_ds.last().unwrap() {
-                interp_ds.push(d);
-                interp_is.push(idx as f64);
-                interp_hs.push(trapz_elevations_m[idx]);
-            }
+            // if positive real number is specified for veh_override_kg, use that
+            self.veh_kg = self.veh_override_kg.unwrap();
         }
-        let interp_ds = Array::from_vec(interp_ds);
-        let interp_is = Array::from_vec(interp_is);
-        let interp_hs = Array::from_vec(interp_hs);
-        Self {
-            grade_all_zero,
-            trapz_step_distances_m,
-            trapz_distances_m,
-            trapz_elevations_m,
-            stops,
-            interp_ds,
-            interp_is,
-            interp_hs,
-            grades: cyc.grade.clone(),
-        }
-    }
 
-    /// Interpolate the single-point grade at the given distance.
-    /// Assumes that the grade at i applies from sample point (i-1, i]
-    pub fn interp_grade(&self, dist_m: f64) -> f64 {
-        if self.grade_all_zero {
-            0.0
-        } else if dist_m <= self.interp_ds[0] {
-            self.grades[0]
-        } else if dist_m > *self.interp_ds.last().unwrap() {
-            *self.grades.last().unwrap()
-        } else {
-            let raw_idx = interpolate(&dist_m, &self.interp_ds, &self.interp_is, false);
-            let idx = raw_idx.ceil() as usize;
-            self.grades[idx]
-        }
-    }
+        self.max_trac_mps2 = (self.wheel_coef_of_fric
+            * self.drive_axle_weight_frac
+            * self.veh_kg
+            * self.props.a_grav_mps2
+            / (1.0 + self.veh_cg_m * self.wheel_coef_of_fric / self.wheel_base_m))
+            / (self.veh_kg * self.props.a_grav_mps2)
+            * self.props.a_grav_mps2;
+    }
+
+    pub fn max_regen_kwh(&self) -> f64 {
+        0.5 * self.veh_kg * (27.0 * 27.0) / (3_600.0 * 1_000.0)
+    }
+
+    pub fn mc_peak_eff(&self) -> f64 {
+        arrmax(&self.mc_full_eff_array)
+    }
+
+    pub fn max_fc_eff_kw(&self) -> f64 {
+        let fc_eff_arr_max_i =
+            first_eq(&self.fc_eff_array, arrmax(&self.fc_eff_array)).unwrap_or(0);
+        self.fc_kw_out_array[fc_eff_arr_max_i]
+    }
+
+    pub fn fc_peak_eff(&self) -> f64 {
+        arrmax(&self.fc_eff_array)
+    }
+
+    /// Sets derived parameters:
+    /// - `no_elec_sys`
+    /// - `no_elec_aux`
+    /// - `fc_perc_out_array`
+    /// - `input_kw_out_array`
+    /// - `fc_kw_out_array`
+    /// - `fc_eff_array`
+    /// - `modern_diff`
+    /// - `large_baseline_eff_adj`
+    /// - `mc_kw_adj_perc`
+    /// - `mc_eff_map`
+    /// - `mc_eff_array`
+    /// - `mc_perc_out_array`
+    /// - `mc_kw_out_array`
+    /// - `mc_full_eff_array`
+    /// - `mc_kw_in_array`
+    /// - `mc_max_elec_in_kw`
+    /// - `set_fc_peak_eff()`
+    /// - `set_mc_peak_eff()`
+    /// - `set_veh_mass()`
+    ///     - `ess_mass_kg`
+    ///     - `mc_mass_kg`
+    ///     - `fc_mass_kg`
+    ///     - `fs_mass_kg`
+    ///     - `veh_kg`
+    ///     - `max_trac_mps2`
+    pub fn set_derived(&mut self) -> Result<(), anyhow::Error> {
+        // Vehicle input validation
+        match self.validate() {
+            Ok(_) => (),
+            Err(e) => bail!(e),
+        };
 
-    /// Interpolate the elevation at the given distance
-    pub fn interp_elevation(&self, dist_m: f64) -> f64 {
-        if self.grade_all_zero {
-            0.0
-        } else {
-            interpolate(&dist_m, &self.interp_ds, &self.interp_hs, false)
+        if self.scenario_name != "Template Vehicle for setting up data types" {
+            if self.veh_pt_type == BEV {
+                assert!(
+                    self.fs_max_kw == 0.0,
+                    "max_fuel_stor_kw must be zero for provided BEV powertrain type in {}",
+                    self.scenario_name
+                );
+                assert!(
+                    self.fs_kwh == 0.0,
+                    "fuel_stor_kwh must be zero for provided BEV powertrain type in {}",
+                    self.scenario_name
+                );
+                assert!(
+                    self.fc_max_kw == 0.0,
+                    "max_fuel_conv_kw must be zero for provided BEV powertrain type in {}",
+                    self.scenario_name
+                );
+            } else if (self.veh_pt_type == CONV) && !self.stop_start {
+                assert!(
+                    self.mc_max_kw == 0.0,
+                    "max_mc_kw must be zero for provided Conv powertrain type in {}",
+                    self.scenario_name
+                );
+                assert!(
+                    self.ess_max_kw == 0.0,
+                    "max_ess_kw must be zero for provided Conv powertrain type in {}",
+                    self.scenario_name
+                );
+                assert!(
+                    self.ess_max_kwh == 0.0,
+                    "max_ess_kwh must be zero for provided Conv powertrain type in {}",
+                    self.scenario_name
+                );
+            }
         }
-    }
-}
-
-#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Default)]
-#[add_pyo3_api(
-    #[new]
-    pub fn __new__(
-        time_s: Vec<f64>,
-        mps: Vec<f64>,
-        grade: Vec<f64>,
-        road_type: Vec<f64>,
-        name: String,
-    ) -> Self {
-        Self::new(time_s, mps, grade, road_type, name)
-    }
-
-    #[allow(clippy::type_complexity)]
-    pub fn __getnewargs__(&self) -> PyResult<(Vec<f64>, Vec<f64>, Vec<f64>, Vec<f64>, &str)> {
-        Ok((self.time_s.to_vec(), self.mps.to_vec(), self.grade.to_vec(), self.road_type.to_vec(), &self.name))
-    }
-
-    #[classmethod]
-    #[pyo3(name = "from_csv_file")]
-    pub fn from_csv_file_py(_cls: &PyType, pathstr: String) -> anyhow::Result<Self> {
-        Self::from_csv_file(&pathstr)
-    }
-
-    pub fn to_rust(&self) -> anyhow::Result<Self> {
-        Ok(self.clone())
-    }
-
-    /// Return a HashMap representing the cycle
-    pub fn get_cyc_dict(&self) -> anyhow::Result<HashMap<String, Vec<f64>>> {
-        let dict: HashMap<String, Vec<f64>> = HashMap::from([
-            ("time_s".to_string(), self.time_s.to_vec()),
-            ("mps".to_string(), self.mps.to_vec()),
-            ("grade".to_string(), self.grade.to_vec()),
-            ("road_type".to_string(), self.road_type.to_vec()),
-        ]);
-        Ok(dict)
-    }
-
-    #[pyo3(name = "modify_by_const_jerk_trajectory")]
-    pub fn modify_by_const_jerk_trajectory_py(
-        &mut self,
-        idx: usize,
-        n: usize,
-        jerk_m_per_s3: f64,
-        accel0_m_per_s2: f64,
-    ) -> PyResult<f64> {
-        Ok(self.modify_by_const_jerk_trajectory(idx, n, jerk_m_per_s3, accel0_m_per_s2))
-    }
-
-    #[pyo3(name = "modify_with_braking_trajectory")]
-    pub fn modify_with_braking_trajectory_py(
-        &mut self,
-        brake_accel_m_per_s2: f64,
-        idx: usize,
-        dts_m: Option<f64>
-    ) -> PyResult<(f64, usize)> {
-        Ok(self.modify_with_braking_trajectory(brake_accel_m_per_s2, idx, dts_m))
-    }
-
-    #[pyo3(name = "calc_distance_to_next_stop_from")]
-    pub fn calc_distance_to_next_stop_from_py(&self, distance_m: f64) -> PyResult<f64> {
-        Ok(self.calc_distance_to_next_stop_from(distance_m, None))
-    }
-
-    #[pyo3(name = "average_grade_over_range")]
-    pub fn average_grade_over_range_py(
-        &self,
-        distance_start_m: f64,
-        delta_distance_m: f64,
-    ) -> PyResult<f64> {
-        Ok(self.average_grade_over_range(distance_start_m, delta_distance_m, None))
-    }
-
-    #[pyo3(name = "build_cache")]
-    pub fn build_cache_py(&self) -> PyResult<RustCycleCache> {
-        Ok(self.build_cache())
-    }
-
-    #[pyo3(name = "dt_s_at_i")]
-    pub fn dt_s_at_i_py(&self, i: usize) -> PyResult<f64> {
-        if i == 0 {
-            Ok(0.0)
+        // ### Build roadway power lookup table
+        // self.max_roadway_chg_kw = Array1::from_vec(vec![0.0, 0.0, 0.0, 0.0, 0.0, 0.0]);
+        // self.charging_on = false;
+
+        // # Checking if a vehicle has any hybrid components
+        if (self.ess_max_kwh == 0.0) || (self.ess_max_kw == 0.0) || (self.mc_max_kw == 0.0) {
+            self.no_elec_sys = true;
         } else {
-            Ok(self.dt_s_at_i(i))
+            self.no_elec_sys = false;
         }
-    }
-
-    #[getter]
-    pub fn get_mph(&self) -> PyResult<Vec<f64>> {
-        Ok((&self.mps * crate::params::MPH_PER_MPS).to_vec())
-    }
-    #[setter]
-    pub fn set_mph(&mut self, new_value: Vec<f64>) -> PyResult<()> {
-        self.mps = Array::from_vec(new_value) / MPH_PER_MPS;
-        Ok(())
-    }
-    #[getter]
-    /// array of time steps
-    pub fn get_dt_s(&self) -> PyResult<Vec<f64>> {
-        Ok(self.dt_s().to_vec())
-    }
-    #[getter]
-    /// cycle length
-    pub fn get_len(&self) -> PyResult<usize> {
-        Ok(self.len())
-    }
-    #[getter]
-    /// distance for each time step based on final speed
-    pub fn get_dist_m(&self) -> PyResult<Vec<f64>> {
-        Ok(self.dist_m().to_vec())
-    }
-    #[getter]
-    pub fn get_delta_elev_m(&self) -> PyResult<Vec<f64>> {
-        Ok(self.delta_elev_m().to_vec())
-    }
-)]
-/// Struct for containing:
-/// * time_s, cycle time, $s$
-/// * mps, vehicle speed, $\frac{m}{s}$
-/// * grade, road grade/slope, $\frac{rise}{run}$
-/// * road_type, $kW$
-/// * legacy, will likely change to road charging capacity
-///    * Another sublist.
-pub struct RustCycle {
-    /// array of time [s]
-    #[serde(alias = "cycSecs")]
-    pub time_s: Array1<f64>,
-    /// array of speed [m/s]
-    #[serde(alias = "cycMps")]
-    pub mps: Array1<f64>,
-    /// array of grade [rise/run]
-    #[serde(alias = "cycGrade")]
-    pub grade: Array1<f64>,
-    /// array of max possible charge rate from roadway
-    #[serde(alias = "cycRoadType")]
-    pub road_type: Array1<f64>,
-    pub name: String,
-    #[serde(skip)]
-    pub orphaned: bool,
-}
 
-/// pure Rust methods that need to be separate due to pymethods incompatibility
-impl RustCycle {
-    pub fn new(
-        time_s: Vec<f64>,
-        mps: Vec<f64>,
-        grade: Vec<f64>,
-        road_type: Vec<f64>,
-        name: String,
-    ) -> Self {
-        let time_s = Array::from_vec(time_s);
-        let mps = Array::from_vec(mps);
-        let grade = Array::from_vec(grade);
-        let road_type = Array::from_vec(road_type);
-        Self {
-            time_s,
-            mps,
-            grade,
-            road_type,
-            name,
-            orphaned: false,
+        // # Checking if aux loads go through an alternator
+        if self.no_elec_sys || (self.mc_max_kw <= self.aux_kw) || self.force_aux_on_fc {
+            self.no_elec_aux = true;
+        } else {
+            self.no_elec_aux = false;
         }
-    }
 
-    pub fn build_cache(&self) -> RustCycleCache {
-        RustCycleCache::new(&self)
-    }
+        self.fc_perc_out_array = FC_PERC_OUT_ARRAY.clone().to_vec();
 
-    pub fn push(&mut self, cyc_elem: RustCycleElement) {
-        self.time_s
-            .append(Axis(0), array![cyc_elem.time_s].view())
-            .unwrap();
-        self.mps
-            .append(Axis(0), array![cyc_elem.mps].view())
-            .unwrap();
-        self.grade
-            .append(Axis(0), array![cyc_elem.grade].view())
-            .unwrap();
-        self.road_type
-            .append(Axis(0), array![cyc_elem.road_type].view())
-            .unwrap();
-    }
-
-    #[allow(clippy::len_without_is_empty)]
-    pub fn len(&self) -> usize {
-        self.time_s.len()
-    }
-
-    pub fn test_cyc() -> Self {
-        let time_s = Array1::<f64>::range(0.0, 10.0, 1.0).to_vec();
-        let speed_mps = Array1::<f64>::range(0.0, 10.0, 1.0).to_vec();
-        let grade = Array::zeros(10).to_vec();
-        let road_type = Array::zeros(10).to_vec();
-        let name = String::from("test");
-        Self::new(time_s, speed_mps, grade, road_type, name)
-    }
-
-    /// Returns the average grade over the given range of distances
-    /// - distance_start_m: non-negative-number, the distance at start of evaluation area (m)
-    /// - delta_distance_m: non-negative-number, the distance traveled from distance_start_m (m)
-    /// RETURN: number, the average grade (rise over run) over the given distance range
-    /// Note: grade is assumed to be constant from just after the previous sample point
-    /// until the current sample point. That is, grade[i] applies over the range of
-    /// distances, d, from (d[i - 1], d[i]]
-    pub fn average_grade_over_range(
-        &self,
-        distance_start_m: f64,
-        delta_distance_m: f64,
-        cache: Option<&RustCycleCache>,
-    ) -> f64 {
-        let tol = 1e-6;
-        match &cache {
-            Some(rcc) => {
-                if rcc.grade_all_zero {
+        // # discrete array of possible engine power outputs
+        self.input_kw_out_array = self.fc_pwr_out_perc.clone() * self.fc_max_kw;
+        // # Relatively continuous array of possible engine power outputs
+        self.fc_kw_out_array = self
+            .fc_perc_out_array
+            .iter()
+            .map(|n| n * self.fc_max_kw)
+            .collect();
+        // # Creates relatively continuous array for fc_eff
+        if self.fc_eff_array.is_empty() {
+            self.fc_eff_array = self
+                .fc_perc_out_array
+                .iter()
+                .map(|x: &f64| -> f64 {
+                    interpolate(
+                        x,
+                        &Array1::from(self.fc_pwr_out_perc.to_vec()),
+                        &self.fc_eff_map,
+                        false,
+                    )
+                })
+                .collect();
+        }
+        //self.modern_max = MODERN_MAX;
+
+        // NOTE: unused because the first part of if/else commented below is unused
+        let modern_diff = self.modern_max - arrmax(&LARGE_BASELINE_EFF);
+        let large_baseline_eff_adj: Vec<f64> =
+            LARGE_BASELINE_EFF.iter().map(|x| x + modern_diff).collect();
+        let mc_kw_adj_perc = max(
+            0.0,
+            min(
+                (self.mc_max_kw - self.small_motor_power_kw)
+                    / (self.large_motor_power_kw - self.small_motor_power_kw),
+                1.0,
+            ),
+        );
+
+        // NOTE: it should not be possible to have `None in self.mc_eff_map` in Rust (although NaN is possible...).
+        //       if we want to express that mc_eff_map should be calculated in some cases, but not others,
+        //       we may need some sort of option type ?
+        //if None in self.mc_eff_map:
+        //    self.mc_eff_array = mc_kw_adj_perc * large_baseline_eff_adj + \
+        //            (1 - mc_kw_adj_perc) * self.small_baseline_eff
+        //    self.mc_eff_map = self.mc_eff_array
+        //else:
+        //    self.mc_eff_array = self.mc_eff_map
+        if self.mc_eff_map == Array1::<f64>::zeros(LARGE_BASELINE_EFF.len()) {
+            self.mc_eff_map = large_baseline_eff_adj
+                .iter()
+                .zip(SMALL_BASELINE_EFF.iter())
+                .map(|(&x, &y)| mc_kw_adj_perc * x + (1.0 - mc_kw_adj_perc) * y)
+                .collect();
+        }
+        self.mc_eff_array = self.mc_eff_map.clone();
+        // println!("{:?}",self.mc_eff_map);
+        // self.mc_eff_array = mc_kw_adj_perc * large_baseline_eff_adj
+        //     + (1.0 - mc_kw_adj_perc) * self.small_baseline_eff.clone();
+        // self.mc_eff_map = self.mc_eff_array.clone();
+
+        self.mc_perc_out_array = MC_PERC_OUT_ARRAY.clone().to_vec();
+
+        self.mc_kw_out_array =
+            (Array::linspace(0.0, 1.0, self.mc_perc_out_array.len()) * self.mc_max_kw).to_vec();
+
+        self.mc_full_eff_array = self
+            .mc_perc_out_array
+            .iter()
+            .enumerate()
+            .map(|(idx, &x): (usize, &f64)| -> f64 {
+                if idx == 0 {
                     0.0
-                } else if delta_distance_m <= tol {
-                    rcc.interp_grade(distance_start_m)
                 } else {
-                    let e0 = rcc.interp_elevation(distance_start_m);
-                    let e1 = rcc.interp_elevation(distance_start_m + delta_distance_m);
-                    ((e1 - e0) / delta_distance_m).asin().tan()
+                    interpolate(&x, &self.mc_pwr_out_perc, &self.mc_eff_array, false)
                 }
-            }
-            None => {
-                let grade_all_zero = {
-                    let mut all0 = true;
-                    for idx in 0..self.len() {
-                        if self.grade[idx] != 0.0 {
-                            all0 = false;
-                            break;
-                        }
-                    }
-                    all0
-                };
-                if grade_all_zero {
-                    return 0.0;
+            })
+            .collect();
+
+        self.mc_kw_in_array = [0.0; 101]
+            .iter()
+            .enumerate()
+            .map(|(idx, _)| {
+                if idx == 0 {
+                    0.0
                 } else {
-                    let delta_dists = trapz_step_distances(&self);
-                    let trapz_distances_m = ndarrcumsum(&delta_dists);
-                    if delta_distance_m <= tol {
-                        if distance_start_m <= trapz_distances_m[0] {
-                            return self.grade[0];
-                        }
-                        let max_idx = self.len() - 1;
-                        if distance_start_m > trapz_distances_m[max_idx] {
-                            return self.grade[max_idx];
-                        }
-                        for idx in 1..self.time_s.len() {
-                            if distance_start_m > trapz_distances_m[idx - 1]
-                                && distance_start_m <= trapz_distances_m[idx]
-                            {
-                                return self.grade[idx];
-                            }
-                        }
-                        self.grade[max_idx]
-                    } else {
-                        // NOTE: we use the following instead of delta_elev_m in order to use
-                        // more precise trapezoidal distance and elevation at sample points.
-                        // This also uses the fully accurate trig functions in case we have large slope angles.
-                        let trapz_elevations_m = ndarrcumsum(
-                            &(self.grade.mapv(|g| g.atan().cos()) * delta_dists * &self.grade),
-                        );
-                        let e0 = interpolate(
-                            &distance_start_m,
-                            &trapz_distances_m,
-                            &trapz_elevations_m,
-                            false,
-                        );
-                        let e1 = interpolate(
-                            &(distance_start_m + delta_distance_m),
-                            &trapz_distances_m,
-                            &trapz_elevations_m,
-                            false,
-                        );
-                        ((e1 - e0) / delta_distance_m).asin().tan()
-                    }
+                    self.mc_kw_out_array[idx] / self.mc_full_eff_array[idx]
                 }
-            }
-        }
-    }
+            })
+            .collect();
 
-    /// Calculate the distance to next stop from `distance_m`
-    /// - distance_m: non-negative-number, the current distance from start (m)
-    /// RETURN: returns the distance to the next stop from distance_m
-    /// NOTE: distance may be negative if we're beyond the last stop
-    pub fn calc_distance_to_next_stop_from(
-        &self,
-        distance_m: f64,
-        cache: Option<&RustCycleCache>,
-    ) -> f64 {
-        let tol: f64 = 1e-6;
-        match cache {
-            Some(rcc) => {
-                for (&dist, &v) in rcc.trapz_distances_m.iter().zip(self.mps.iter()) {
-                    if (v < tol) && (dist > (distance_m + tol)) {
-                        return dist - distance_m;
-                    }
-                }
-                rcc.trapz_distances_m.last().unwrap() - distance_m
-            }
-            None => {
-                let ds = ndarrcumsum(&trapz_step_distances(self));
-                for (&dist, &v) in ds.iter().zip(self.mps.iter()) {
-                    if (v < tol) && (dist > (distance_m + tol)) {
-                        return dist - distance_m;
-                    }
-                }
-                ds.last().unwrap() - distance_m
-            }
-        }
-    }
+        self.mc_max_elec_in_kw = arrmax(&self.mc_kw_in_array);
 
-    /// Modifies the cycle using the given constant-jerk trajectory parameters
-    /// - idx: non-negative integer, the point in the cycle to initiate
-    ///   modification (note: THIS point is modified since trajectory should be
-    ///   calculated from idx-1)
-    /// - n: non-negative integer, the number of steps ahead
-    /// - jerk_m__s3: number, the "Jerk" associated with the trajectory (m/s3)
-    /// - accel0_m__s2: number, the initial acceleration (m/s2)
-    /// NOTE:
-    /// - modifies cyc in place to hit any critical rendezvous_points by a trajectory adjustment
-    /// - CAUTION: NOT ROBUST AGAINST VARIABLE DURATION TIME-STEPS
-    /// RETURN: Number, final modified speed (m/s)
-    pub fn modify_by_const_jerk_trajectory(
-        &mut self,
-        i: usize,
-        n: usize,
-        jerk_m_per_s3: f64,
-        accel0_m_per_s2: f64,
-    ) -> f64 {
-        if n == 0 {
-            return 0.0;
-        }
-        let num_samples = self.mps.len();
-        if i >= num_samples {
-            if num_samples > 0 {
-                return self.mps[num_samples - 1];
-            }
-            return 0.0;
-        }
-        let v0 = self.mps[i - 1];
-        let dt = self.dt_s_at_i(i);
-        let mut v = v0;
-        for ni in 1..(n + 1) {
-            let idx_to_set = (i - 1) + ni;
-            if idx_to_set >= num_samples {
-                break;
-            }
-            v = speed_for_constant_jerk(ni, v0, accel0_m_per_s2, jerk_m_per_s3, dt);
-            self.mps[idx_to_set] = max(v, 0.0);
-        }
-        v
-    }
+        #[cfg(feature = "pyo3")]
+        if let Some(new_fc_peak) = self.fc_peak_eff_override {
+            self.set_fc_peak_eff(new_fc_peak);
+            self.fc_peak_eff_override = None;
+        }
+        #[cfg(feature = "pyo3")]
+        if let Some(new_mc_peak) = self.mc_peak_eff_override {
+            self.set_mc_peak_eff(new_mc_peak);
+            self.mc_peak_eff_override = None;
+        }
+
+        // check that efficiencies are not violating the first law of thermo
+        assert!(
+            arrmin(&self.fc_eff_array) >= 0.0,
+            "min MC eff < 0 is not allowed"
+        );
+        assert!(self.fc_peak_eff() < 1.0, "fcPeakEff >= 1 is not allowed.");
+        assert!(
+            arrmin(&self.mc_full_eff_array) >= 0.0,
+            "min MC eff < 0 is not allowed"
+        );
+        assert!(self.mc_peak_eff() < 1.0, "mcPeakEff >= 1 is not allowed.");
 
-    /// Add a braking trajectory that would cover the same distance as the given constant brake deceleration
-    /// - brake_accel_m__s2: negative number, the braking acceleration (m/s2)
-    /// - idx: non-negative integer, the index where to initiate the stop trajectory, start of the step (i in FASTSim)
-    /// - dts_m: None | float: if given, this is the desired distance-to-stop in meters. If not given, it is
-    ///     calculated based on braking deceleration.
-    /// RETURN: (non-negative-number, positive-integer)
-    /// - the final speed of the modified trajectory (m/s)
-    /// - the number of time-steps required to complete the braking maneuver
-    /// NOTE:
-    /// - modifies the cycle in place for the braking trajectory
-    pub fn modify_with_braking_trajectory(
-        &mut self,
-        brake_accel_m_per_s2: f64,
-        i: usize,
-        dts_m: Option<f64>,
-    ) -> (f64, usize) {
-        assert!(brake_accel_m_per_s2 < 0.0);
-        if i >= self.time_s.len() {
-            return (*self.mps.last().unwrap(), 0);
-        }
-        let v0 = self.mps[i - 1];
-        let dt = self.dt_s_at_i(i);
-        // distance-to-stop (m)
-        let dts_m = match dts_m {
-            Some(value) => {
-                if value > 0.0 {
-                    value
-                } else {
-                    -0.5 * v0 * v0 / brake_accel_m_per_s2
-                }
-            }
-            None => -0.5 * v0 * v0 / brake_accel_m_per_s2,
-        };
-        if dts_m <= 0.0 {
-            return (v0, 0);
-        }
-        // time-to-stop (s)
-        let tts_s = -v0 / brake_accel_m_per_s2;
-        // number of steps to take
-        let n: usize = (tts_s / dt).round() as usize;
-        let n: usize = if n < 2 { 2 } else { n }; // need at least 2 steps
-        let (jerk_m_per_s3, accel_m_per_s2) =
-            calc_constant_jerk_trajectory(n, 0.0, v0, dts_m, 0.0, dt);
-        (
-            self.modify_by_const_jerk_trajectory(i, n, jerk_m_per_s3, accel_m_per_s2),
-            n,
-        )
-    }
-
-    /// rust-internal time steps
-    pub fn dt_s(&self) -> Array1<f64> {
-        diff(&self.time_s)
-    }
-
-    /// rust-internal time steps at i
-    pub fn dt_s_at_i(&self, i: usize) -> f64 {
-        self.time_s[i] - self.time_s[i - 1]
-    }
-
-    /// distance covered in each time step
-    pub fn dist_m(&self) -> Array1<f64> {
-        &self.mps * self.dt_s()
-    }
-
-    /// get mph from self.mps
-    pub fn mph_at_i(&self, i: usize) -> f64 {
-        self.mps[i] * MPH_PER_MPS
-    }
-
-    /// Load cycle from csv file
-    pub fn from_csv_file(pathstr: &str) -> Result<Self, anyhow::Error> {
-        let pathbuf = PathBuf::from(&pathstr);
-
-        // create empty cycle to be populated
-        let mut cyc = Self::default();
-
-        // unwrap is ok because if statement checks existence
-        let file = File::open(&pathbuf).unwrap();
-        let name = String::from(pathbuf.file_stem().unwrap().to_str().unwrap());
-        cyc.name = name;
-        let mut rdr = csv::ReaderBuilder::new()
-            .has_headers(true)
-            .from_reader(file);
-        for result in rdr.deserialize() {
-            // TODO: make this more elegant than unwrap
-            let cyc_elem: RustCycleElement = result?;
-            cyc.push(cyc_elem);
-        }
+        self.set_veh_mass();
 
-        Ok(cyc)
+        Ok(())
     }
 
-    /// elevation change w.r.t. to initial
-    pub fn delta_elev_m(&self) -> Array1<f64> {
-        ndarrcumsum(&(self.dist_m() * self.grade.clone()))
-    }
-
-    pub fn from_file(filename: &str) -> Result<Self, anyhow::Error> {
-        // check if the extension is csv, and if it is, then call Self::from_csv_file
-        let pathbuf = PathBuf::from(filename);
-        let file = File::open(filename)?;
-        let extension = pathbuf.extension().unwrap().to_str().unwrap();
-        match extension {
-            "yaml" => Ok(serde_yaml::from_reader(file)?),
-            "json" => Ok(serde_json::from_reader(file)?),
-            "csv" => Ok(Self::from_csv_file(filename)?),
-            _ => Err(anyhow!("Unsupported file extension {}", extension)),
-        }
+    pub fn mock_vehicle() -> Self {
+        let mut v = Self {
+            scenario_name: String::from("2016 FORD Escape 4cyl 2WD"),
+            selection: 5,
+            veh_year: 2016,
+            veh_pt_type: String::from("Conv"),
+            drag_coef: 0.355,
+            frontal_area_m2: 3.066,
+            glider_kg: 1359.166,
+            veh_cg_m: 0.53,
+            drive_axle_weight_frac: 0.59,
+            wheel_base_m: 2.6,
+            cargo_kg: 136.0,
+            veh_override_kg: None,
+            comp_mass_multiplier: 1.4,
+            fs_max_kw: 2000.0,
+            fs_secs_to_peak_pwr: 1.0,
+            fs_kwh: 504.0,
+            fs_kwh_per_kg: 9.89,
+            fc_max_kw: 125.0,
+            fc_pwr_out_perc: array![
+                0.0, 0.005, 0.015, 0.04, 0.06, 0.1, 0.14, 0.2, 0.4, 0.6, 0.8, 1.0,
+            ],
+            fc_eff_map: array![
+                0.1, 0.12, 0.16, 0.22, 0.28, 0.33, 0.35, 0.36, 0.35, 0.34, 0.32, 0.3,
+            ],
+            fc_peak_eff_override: Default::default(),
+            fc_eff_type: String::from("SI"),
+            fc_sec_to_peak_pwr: 6.0,
+            fc_base_kg: 61.0,
+            fc_kw_per_kg: 2.13,
+            min_fc_time_on: 30.0,
+            idle_fc_kw: 2.5,
+            mc_max_kw: 0.0,
+            mc_peak_eff_override: Default::default(),
+            mc_pwr_out_perc: array![0.0, 0.02, 0.04, 0.06, 0.08, 0.1, 0.2, 0.4, 0.6, 0.8, 1.0],
+            mc_eff_map: array![0.12, 0.16, 0.21, 0.29, 0.35, 0.42, 0.75, 0.92, 0.93, 0.93, 0.92,],
+            mc_sec_to_peak_pwr: 4.0,
+            mc_pe_kg_per_kw: 0.833,
+            mc_pe_base_kg: 21.6,
+            small_motor_power_kw: 7.5,
+            large_motor_power_kw: 75.0,
+            modern_max: MODERN_MAX,
+            charging_on: false,
+            max_roadway_chg_kw: Array1::<f64>::from_vec(vec![0.0, 0.0, 0.0, 0.0, 0.0, 0.0]),
+            ess_max_kw: 0.0,
+            ess_max_kwh: 0.0,
+            ess_kg_per_kwh: 8.0,
+            ess_base_kg: 75.0,
+            ess_round_trip_eff: 0.97,
+            ess_life_coef_a: 110.0,
+            ess_life_coef_b: -0.6811,
+            min_soc: 0.4,
+            max_soc: 0.8,
+            ess_dischg_to_fc_max_eff_perc: 0.0,
+            ess_chg_to_fc_max_eff_perc: 0.0,
+            wheel_inertia_kg_m2: 0.815,
+            num_wheels: 4.0,
+            wheel_rr_coef: 0.006,
+            wheel_radius_m: 0.336,
+            wheel_coef_of_fric: 0.7,
+            max_accel_buffer_mph: 60.0,
+            max_accel_buffer_perc_of_useable_soc: 0.2,
+            perc_high_acc_buf: 0.0,
+            mph_fc_on: 30.0,
+            kw_demand_fc_on: 100.0,
+            max_regen: 0.98,
+            stop_start: false,
+            force_aux_on_fc: true,
+            alt_eff: 1.0,
+            chg_eff: 0.86,
+            aux_kw: 0.7,
+            trans_kg: 114.0,
+            trans_eff: 0.92,
+            ess_to_fuel_ok_error: 0.005,
+            val_udds_mpgge: 23.0,
+            val_hwy_mpgge: 32.0,
+            val_comb_mpgge: 26.0,
+            val_udds_kwh_per_mile: f64::NAN,
+            val_hwy_kwh_per_mile: f64::NAN,
+            val_comb_kwh_per_mile: f64::NAN,
+            val_cd_range_mi: f64::NAN,
+            val_const65_mph_kwh_per_mile: f64::NAN,
+            val_const60_mph_kwh_per_mile: f64::NAN,
+            val_const55_mph_kwh_per_mile: f64::NAN,
+            val_const45_mph_kwh_per_mile: f64::NAN,
+            val_unadj_udds_kwh_per_mile: f64::NAN,
+            val_unadj_hwy_kwh_per_mile: f64::NAN,
+            val0_to60_mph: 9.9,
+            val_ess_life_miles: f64::NAN,
+            val_range_miles: f64::NAN,
+            val_veh_base_cost: f64::NAN,
+            val_msrp: f64::NAN,
+            props: RustPhysicalProperties::default(),
+            regen_a: 500.0,
+            regen_b: 0.99,
+            orphaned: Default::default(),
+            // fields that get overriden by `set_derived`
+            no_elec_sys: Default::default(),
+            no_elec_aux: Default::default(),
+            fc_perc_out_array: Default::default(),
+            input_kw_out_array: Default::default(),
+            fc_kw_out_array: Default::default(),
+            fc_eff_array: Default::default(),
+            mc_eff_array: Default::default(),
+            mc_perc_out_array: Default::default(),
+            mc_kw_out_array: Default::default(),
+            mc_full_eff_array: Default::default(),
+            mc_kw_in_array: Default::default(),
+            mc_max_elec_in_kw: Default::default(),
+            ess_mass_kg: Default::default(),
+            mc_mass_kg: Default::default(),
+            fc_mass_kg: Default::default(),
+            fs_mass_kg: Default::default(),
+            veh_kg: Default::default(),
+            max_trac_mps2: Default::default(),
+        };
+        v.set_derived().unwrap();
+        v
     }
 
-    // load a cycle from a string representation of a csv file
-    pub fn from_csv_string(data: &str, name: String) -> Result<Self, anyhow::Error> {
-        let mut cyc = Self::default();
-
-        cyc.name = name;
-        let mut rdr = csv::ReaderBuilder::new()
-            .has_headers(true)
-            .from_reader(data.as_bytes());
-        for result in rdr.deserialize() {
-            let cyc_elem: RustCycleElement = result?;
-            cyc.push(cyc_elem);
-        }
-
-        Ok(cyc)
+    #[allow(clippy::should_implement_trait)]
+    pub fn from_str(filename: &str) -> Result<Self, anyhow::Error> {
+        let mut veh_res: Result<RustVehicle, anyhow::Error> = Ok(serde_json::from_str(filename)?);
+        veh_res.as_mut().unwrap().set_derived()?;
+        veh_res
     }
 }
 
-pub struct PassingInfo {
-    /// True if first cycle passes the second
-    pub has_collision: bool,
-    /// the index where first cycle passes the second
-    pub idx: usize,
-    /// the number of time-steps until idx from i
-    pub num_steps: usize,
-    /// the starting distance of the first cycle at i
-    pub start_distance_m: f64,
-    /// the distance (m) traveled of the second cycle when first passes
-    pub distance_m: f64,
-    /// the starting speed (m/s) of the first cycle at i
-    pub start_speed_m_per_s: f64,
-    /// the speed (m/s) of the second cycle when first passes
-    pub speed_m_per_s: f64,
-    /// the time step duration throught the passing investigation
-    pub time_step_duration_s: f64,
-}
-
-/// Reports back information of the first point where cyc passes cyc0, starting at
-/// step i until the next stop of cyc.
-/// - cyc: fastsim.Cycle, the proposed cycle of the vehicle under simulation
-/// - cyc0: fastsim.Cycle, the reference/lead vehicle/shadow cycle to compare with
-/// - i: int, the time-step index to consider
-/// - dist_tol_m: float, the distance tolerance away from lead vehicle to be seen as
-///     "deviated" from the reference/shadow trace (m)
-/// RETURNS: PassingInfo
-pub fn detect_passing(
-    cyc: &RustCycle,
-    cyc0: &RustCycle,
-    i: usize,
-    dist_tol_m: Option<f64>,
-) -> PassingInfo {
-    if i >= cyc.time_s.len() {
-        return PassingInfo {
-            has_collision: false,
-            idx: 0,
-            num_steps: 0,
-            start_distance_m: 0.0,
-            distance_m: 0.0,
-            start_speed_m_per_s: 0.0,
-            speed_m_per_s: 0.0,
-            time_step_duration_s: 1.0,
-        };
-    }
-    let zero_speed_tol_m_per_s = 1e-6;
-    let dist_tol_m = dist_tol_m.unwrap_or(0.1);
-    let mut v0: f64 = cyc.mps[i - 1];
-    let d0: f64 = trapz_step_start_distance(cyc, i);
-    let mut v0_lv: f64 = cyc0.mps[i - 1];
-    let d0_lv: f64 = trapz_step_start_distance(cyc0, i);
-    let mut d = d0;
-    let mut d_lv = d0_lv;
-    let mut rendezvous_idx: Option<usize> = None;
-    let mut rendezvous_num_steps: usize = 0;
-    let mut rendezvous_distance_m: f64 = 0.0;
-    let mut rendezvous_speed_m_per_s: f64 = 0.0;
-    for di in 0..(cyc.mps.len() - i) {
-        let idx = i + di;
-        let v = cyc.mps[idx];
-        let v_lv = cyc0.mps[idx];
-        let vavg = (v + v0) * 0.5;
-        let vavg_lv = (v_lv + v0_lv) * 0.5;
-        let dd = vavg * cyc.dt_s_at_i(idx);
-        let dd_lv = vavg_lv * cyc0.dt_s_at_i(idx);
-        d += dd;
-        d_lv += dd_lv;
-        let dtlv = d_lv - d;
-        v0 = v;
-        v0_lv = v_lv;
-        if di > 0 && dtlv < -dist_tol_m {
-            rendezvous_idx = Some(idx);
-            rendezvous_num_steps = di + 1;
-            rendezvous_distance_m = d_lv;
-            rendezvous_speed_m_per_s = v_lv;
-            break;
-        }
-        if v <= zero_speed_tol_m_per_s {
-            break;
-        }
-    }
-    PassingInfo {
-        has_collision: rendezvous_idx.is_some(),
-        idx: rendezvous_idx.unwrap_or(0),
-        num_steps: rendezvous_num_steps,
-        start_distance_m: d0,
-        distance_m: rendezvous_distance_m,
-        start_speed_m_per_s: cyc.mps[i - 1],
-        speed_m_per_s: rendezvous_speed_m_per_s,
-        time_step_duration_s: cyc.dt_s_at_i(i),
+impl SerdeAPI for RustVehicle {
+    fn init(&mut self) -> anyhow::Result<()> {
+        self.set_derived()?;
+        Ok(())
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use validator::ValidationErrors;
 
     #[test]
-    fn test_dist() {
-        let cyc = RustCycle::test_cyc();
-        assert_eq!(cyc.dist_m().sum(), 45.0);
+    fn test_set_derived_via_new() {
+        let veh = RustVehicle::mock_vehicle();
+        assert!(veh.veh_kg > 0.0);
     }
 
     #[test]
-    fn test_average_speeds_and_distances() {
-        let time_s = vec![0.0, 10.0, 30.0, 34.0, 40.0];
-        let speed_mps = vec![0.0, 10.0, 10.0, 0.0, 0.0];
-        let grade = Array::zeros(5).to_vec();
-        let road_type = Array::zeros(5).to_vec();
-        let name = String::from("test");
-        let cyc = RustCycle::new(time_s, speed_mps, grade, road_type, name);
-        let avg_mps = average_step_speeds(&cyc);
-        let expected_avg_mps = Array::from_vec(vec![0.0, 5.0, 10.0, 5.0, 0.0]);
-        assert_eq!(expected_avg_mps.len(), avg_mps.len());
-        for (expected, actual) in expected_avg_mps.iter().zip(avg_mps.iter()) {
-            assert_eq!(expected, actual);
-        }
-        let dist_m = trapz_step_distances(&cyc);
-        let expected_dist_m = Array::from_vec(vec![0.0, 50.0, 200.0, 20.0, 0.0]);
-        assert_eq!(expected_dist_m.len(), dist_m.len());
-        for (expected, actual) in expected_dist_m.iter().zip(dist_m.iter()) {
-            assert_eq!(expected, actual);
-        }
+    fn test_veh_kg_override() {
+        let mut veh_file = resources_path();
+        veh_file.push("vehdb/test_overrides.yaml");
+        let veh = RustVehicle::from_file(veh_file.as_os_str().to_str().unwrap()).unwrap();
+        assert!(veh.veh_kg == veh.veh_override_kg.unwrap());
+        // test input validation by providing bad inputs, then checking
+        // the produced error for the offending field names
     }
 
     #[test]
-    fn test_loading_a_cycle_from_the_filesystem() {
-        let pathstr = String::from("../../fastsim/resources/cycles/udds.csv");
-        let expected_udds_length: usize = 1370;
-        let cyc = RustCycle::from_csv_file(&pathstr).unwrap();
-        assert_eq!(cyc.name, String::from("udds"));
-        let num_entries = cyc.time_s.len();
-        assert!(num_entries > 0);
-        assert_eq!(num_entries, cyc.time_s.len());
-        assert_eq!(num_entries, cyc.mps.len());
-        assert_eq!(num_entries, cyc.grade.len());
-        assert_eq!(num_entries, cyc.road_type.len());
-        assert_eq!(num_entries, expected_udds_length);
+    fn test_input_validation() {
+        // set up vehicle input parameters
+        let scenario_name = String::from("2016 FORD Escape 4cyl 2WD");
+        let selection: u32 = 5;
+        let veh_year: u32 = 2016;
+        let veh_pt_type = String::from("whoops"); // bad input
+        let drag_coef: f64 = 0.355;
+        let frontal_area_m2: f64 = 3.066;
+        let glider_kg: f64 = -50.0; // bad input
+        let veh_cg_m: f64 = 0.53;
+        let drive_axle_weight_frac: f64 = 0.59;
+        let wheel_base_m: f64 = 2.6;
+        let cargo_kg: f64 = 136.0;
+        let veh_override_kg: Option<f64> = None;
+        let comp_mass_multiplier: f64 = 1.4;
+        let fs_max_kw: f64 = 2000.0;
+        let fs_secs_to_peak_pwr: f64 = 1.0;
+        let fs_kwh: f64 = 504.0;
+        let fs_kwh_per_kg: f64 = 9.89;
+        let fc_max_kw: f64 = -60.0; // bad input
+        let fc_pwr_out_perc: Vec<f64> = vec![
+            0.0, 0.005, 0.015, 0.04, 0.06, 0.1, 0.14, 0.2, 0.4, 0.6, 0.8, 1.0,
+        ];
+        let fc_eff_type: String = String::from("SI");
+        let fc_sec_to_peak_pwr: f64 = 6.0;
+        let fc_base_kg: f64 = 61.0;
+        let fc_kw_per_kg: f64 = 2.13;
+        let min_fc_time_on: f64 = 30.0;
+        let idle_fc_kw: f64 = 2.5;
+        let mc_max_kw: f64 = 0.0;
+        let mc_sec_to_peak_pwr: f64 = 4.0;
+        let mc_pe_kg_per_kw: f64 = 0.833;
+        let mc_pe_base_kg: f64 = 21.6;
+        let ess_max_kw: f64 = 0.0;
+        let ess_max_kwh: f64 = 0.0;
+        let ess_kg_per_kwh: f64 = 8.0;
+        let ess_base_kg: f64 = 75.0;
+        let ess_round_trip_eff: f64 = 0.97;
+        let ess_life_coef_a: f64 = 110.0;
+        let ess_life_coef_b: f64 = -0.6811;
+        let min_soc: f64 = -0.5; // bad input
+        let max_soc: f64 = 1.5; // bad input
+        let ess_dischg_to_fc_max_eff_perc: f64 = 0.0;
+        let ess_chg_to_fc_max_eff_perc: f64 = 0.0;
+        let wheel_inertia_kg_m2: f64 = 0.815;
+        let num_wheels: f64 = 4.0;
+        let wheel_rr_coef: f64 = 0.006;
+        let wheel_radius_m: f64 = 0.336;
+        let wheel_coef_of_fric: f64 = 0.7;
+        let max_accel_buffer_mph: f64 = 60.0;
+        let max_accel_buffer_perc_of_useable_soc: f64 = 0.2;
+        let perc_high_acc_buf: f64 = 0.0;
+        let mph_fc_on: f64 = 30.0;
+        let kw_demand_fc_on: f64 = 100.0;
+        let max_regen: f64 = 0.98;
+        let stop_start: bool = false;
+        let force_aux_on_fc: bool = true;
+        let alt_eff: f64 = 1.0;
+        let chg_eff: f64 = 0.86;
+        let aux_kw: f64 = 0.7;
+        let trans_kg: f64 = 114.0;
+        let trans_eff: f64 = 0.92;
+        let ess_to_fuel_ok_error: f64 = 0.005;
+        let val_udds_mpgge: f64 = 23.0;
+        let val_hwy_mpgge: f64 = 32.0;
+        let val_comb_mpgge: f64 = 26.0;
+        let val_udds_kwh_per_mile: f64 = f64::NAN;
+        let val_hwy_kwh_per_mile: f64 = f64::NAN;
+        let val_comb_kwh_per_mile: f64 = f64::NAN;
+        let val_cd_range_mi: f64 = f64::NAN;
+        let val_const65_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const60_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const55_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_const45_mph_kwh_per_mile: f64 = f64::NAN;
+        let val_unadj_udds_kwh_per_mile: f64 = f64::NAN;
+        let val_unadj_hwy_kwh_per_mile: f64 = f64::NAN;
+        let val0_to60_mph: f64 = 9.9;
+        let val_ess_life_miles: f64 = f64::NAN;
+        let val_range_miles: f64 = f64::NAN;
+        let val_veh_base_cost: f64 = f64::NAN;
+        let val_msrp: f64 = f64::NAN;
+        let props = RustPhysicalProperties::default();
+        let regen_a: f64 = 500.0;
+        let regen_b: f64 = 0.99;
+        let fc_peak_eff_override: Option<f64> = None;
+        let mc_peak_eff_override: Option<f64> = Some(-0.50); // bad input
+        let small_motor_power_kw = 7.5;
+        let large_motor_power_kw = 75.0;
+        let fc_perc_out_array = FC_PERC_OUT_ARRAY.clone().to_vec();
+        let mc_eff_map = Array1::<f64>::zeros(LARGE_BASELINE_EFF.len());
+        let mc_kw_out_array =
+            (Array::linspace(0.0, 1.0, MC_PERC_OUT_ARRAY.len()) * mc_max_kw).to_vec();
+        let mc_perc_out_array = MC_PERC_OUT_ARRAY.clone().to_vec();
+        let mc_pwr_out_perc = array![0.0, 0.02, 0.04, 0.06, 0.08, 0.1, 0.2, 0.4, 0.6, 0.8, 1.0];
+        let mc_full_eff_array: Vec<f64> = mc_perc_out_array
+            .iter()
+            .enumerate()
+            .map(|(idx, &x): (usize, &f64)| -> f64 {
+                if idx == 0 {
+                    0.0
+                } else {
+                    interpolate(&x, &mc_pwr_out_perc, &mc_eff_map.clone(), false)
+                }
+            })
+            .collect();
+        let mc_kw_in_array: Vec<f64> = [0.0; 101]
+            .iter()
+            .enumerate()
+            .map(|(idx, _)| {
+                if idx == 0 {
+                    0.0
+                } else {
+                    mc_kw_out_array[idx] / mc_full_eff_array[idx]
+                }
+            })
+            .collect();
+        let mc_max_elec_in_kw = arrmax(&mc_kw_in_array);
+
+        // instantiate vehicle result
+        let mut veh = RustVehicle {
+            small_motor_power_kw,
+            large_motor_power_kw,
+            fc_perc_out_array: FC_PERC_OUT_ARRAY.clone().to_vec(),
+            charging_on: Default::default(),
+            no_elec_sys: Default::default(),
+            no_elec_aux: Default::default(),
+            max_roadway_chg_kw: Default::default(),
+            input_kw_out_array: Array1::from_vec(fc_pwr_out_perc.clone()) * fc_max_kw,
+            fc_kw_out_array: fc_perc_out_array.iter().map(|n| n * fc_max_kw).collect(),
+            fc_eff_array: fc_perc_out_array
+                .iter()
+                .map(|x: &f64| -> f64 {
+                    interpolate(
+                        x,
+                        &Array1::from(fc_pwr_out_perc.to_vec()),
+                        &array![
+                            0.10, 0.12, 0.16, 0.22, 0.28, 0.33, 0.35, 0.36, 0.35, 0.34, 0.32, 0.30
+                        ],
+                        false,
+                    )
+                })
+                .collect(),
+            modern_max: MODERN_MAX,
+            mc_eff_array: mc_eff_map,
+            mc_kw_in_array: [0.0; 101]
+                .iter()
+                .enumerate()
+                .map(|(idx, _)| {
+                    if idx == 0 {
+                        0.0
+                    } else {
+                        mc_kw_out_array[idx] / mc_full_eff_array[idx]
+                    }
+                })
+                .collect(),
+            mc_kw_out_array,
+            mc_max_elec_in_kw,
+            mc_full_eff_array,
+            // these get calculated in `se
+            veh_kg: Default::default(),
+            max_trac_mps2: Default::default(),
+            ess_mass_kg: Default::default(),
+            mc_mass_kg: Default::default(),
+            fc_mass_kg: Default::default(),
+            fs_mass_kg: Default::default(),
+            mc_perc_out_array,
+            orphaned: Default::default(),
+            scenario_name,
+            selection,
+            veh_year,
+            veh_pt_type, // bad input
+            drag_coef,
+            frontal_area_m2,
+            glider_kg, // bad input
+            veh_cg_m,
+            drive_axle_weight_frac,
+            wheel_base_m,
+            cargo_kg,
+            veh_override_kg,
+            comp_mass_multiplier,
+            fs_max_kw,
+            fs_secs_to_peak_pwr,
+            fs_kwh,
+            fs_kwh_per_kg,
+            fc_max_kw, // bad input
+            fc_pwr_out_perc: array![
+                0.0, 0.005, 0.015, 0.04, 0.06, 0.1, 0.14, 0.2, 0.4, 0.6, 0.8, 1.0,
+            ],
+            fc_eff_map: array![
+                0.1, 0.12, 0.16, 0.22, 0.28, 0.33, 0.35, 0.36, 0.35, 0.34, 0.32, 0.3,
+            ],
+            fc_eff_type,
+            fc_sec_to_peak_pwr,
+            fc_base_kg,
+            fc_kw_per_kg,
+            min_fc_time_on,
+            idle_fc_kw,
+            mc_max_kw,
+            mc_pwr_out_perc,
+            mc_eff_map: array![0.12, 0.16, 0.21, 0.29, 0.35, 0.42, 0.75, 0.92, 0.93, 0.93, 0.92],
+            mc_sec_to_peak_pwr,
+            mc_pe_kg_per_kw,
+            mc_pe_base_kg,
+            ess_max_kw,
+            ess_max_kwh,
+            ess_kg_per_kwh,
+            ess_base_kg,
+            ess_round_trip_eff,
+            ess_life_coef_a,
+            ess_life_coef_b,
+            min_soc, // bad input
+            max_soc, // bad input
+            ess_dischg_to_fc_max_eff_perc,
+            ess_chg_to_fc_max_eff_perc,
+            wheel_inertia_kg_m2,
+            num_wheels,
+            wheel_rr_coef,
+            wheel_radius_m,
+            wheel_coef_of_fric,
+            max_accel_buffer_mph,
+            max_accel_buffer_perc_of_useable_soc,
+            perc_high_acc_buf,
+            mph_fc_on,
+            kw_demand_fc_on,
+            max_regen,
+            stop_start,
+            force_aux_on_fc,
+            alt_eff,
+            chg_eff,
+            aux_kw,
+            trans_kg,
+            trans_eff,
+            ess_to_fuel_ok_error,
+            val_udds_mpgge,
+            val_hwy_mpgge,
+            val_comb_mpgge,
+            val_udds_kwh_per_mile,
+            val_hwy_kwh_per_mile,
+            val_comb_kwh_per_mile,
+            val_cd_range_mi,
+            val_const65_mph_kwh_per_mile,
+            val_const60_mph_kwh_per_mile,
+            val_const55_mph_kwh_per_mile,
+            val_const45_mph_kwh_per_mile,
+            val_unadj_udds_kwh_per_mile,
+            val_unadj_hwy_kwh_per_mile,
+            val0_to60_mph,
+            val_ess_life_miles,
+            val_range_miles,
+            val_veh_base_cost,
+            val_msrp,
+            props,
+            regen_a,
+            regen_b,
+            fc_peak_eff_override,
+            mc_peak_eff_override, // bad input
+        };
+
+        let validation_result = veh.set_derived();
+
+        // hard-coded fields where bad inputs were provided above
+        let bad_fields = [
+            "veh_pt_type",
+            "glider_kg",
+            "fc_max_kw",
+            "min_soc",
+            "max_soc",
+            "mc_peak_eff_override",
+        ];
+        // downcast anyhow::error back into validator::ValidationErrors
+        // this test will fail on the unwrap() if the error is not downcastable to ValidationErrors
+        // e.g. if the error was not from input validation
+        let validation_errs = validation_result
+            .unwrap_err()
+            .downcast::<ValidationErrors>()
+            .unwrap();
+        let validation_errs_hashmap = validation_errs.errors();
+        // assert that specified bad fields were caught
+        assert!(validation_errs_hashmap
+            .keys()
+            .all(|key| bad_fields.contains(key)));
+        assert!(validation_errs_hashmap.len() == bad_fields.len());
     }
 }
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/html/docs-header.html` & `fastsim-2.1.0/rust/fastsim-core/src/html/docs-header.html`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/lib.rs` & `fastsim-2.1.0/rust/fastsim-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/macros.rs` & `fastsim-2.1.0/rust/fastsim-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/params.rs` & `fastsim-2.1.0/rust/fastsim-core/src/params.rs`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     pub kwh_per_gge: f64,           // = 33.7 # kWh per gallon of gasoline
     pub fuel_rho_kg__L: f64, // = 0.75 # gasoline density in kg/L https://inchem.org/documents/icsc/icsc/eics1400.htm
     pub fuel_afr_stoich: f64, // = 14.7 # gasoline stoichiometric air-fuel ratio https://en.wikipedia.org/wiki/Air%E2%80%93fuel_ratio
     #[serde(skip)]
     pub orphaned: bool,
 }
 
+impl SerdeAPI for RustPhysicalProperties {}
+
 impl Default for RustPhysicalProperties {
     fn default() -> Self {
         let air_density_kg_per_m3: f64 = 1.2;
         let a_grav_mps2: f64 = 9.81;
         let kwh_per_gge: f64 = 33.7;
         #[allow(non_snake_case)]
         let fuel_rho_kg__L: f64 = 0.75;
@@ -145,17 +147,18 @@
     pub hwy_intercept: f64,
     #[serde(rename = "Highway Slope")]
     pub hwy_slope: f64,
 }
 
 impl Default for RustLongParams {
     fn default() -> Self {
-        let long_params_str: &str = include_str!("../../../fastsim/resources/longparams.json");
+        let long_params_str: &str =
+            include_str!("../../../python/fastsim/resources/longparams.json");
         let long_params: Self = from_str(long_params_str).unwrap();
-        return long_params;
+        long_params
     }
 }
 
 #[cfg(test)]
 mod params_test {
     use super::*;
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/simdrive/cyc_mods.rs` & `fastsim-2.1.0/rust/fastsim-core/src/simdrive/cyc_mods.rs`

 * *Files identical despite different names*

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/simdrive/simdrive_impl.rs` & `fastsim-2.1.0/rust/fastsim-core/src/simdrive/simdrive_impl.rs`

 * *Files 0% similar despite different names*

```diff
@@ -438,15 +438,15 @@
                         );
                     }
                     init_soc
                 } else if self.veh.veh_pt_type == PHEV || self.veh.veh_pt_type == BEV {
                     // If EV, initializing initial SOC to maximum SOC.
                     self.veh.max_soc
                 } else {
-                    panic!("Failed to properly initialize SOC.");
+                    bail!("Failed to properly initialize SOC.");
                 }
             }
         };
 
         self.walk(init_soc, aux_in_kw_override)?;
 
         self.set_post_scalars()?;
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/simdrive.rs` & `fastsim-2.1.0/rust/fastsim-core/src/simdrive.rs`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,16 @@
     pub idm_v_desired_in_m_per_s_by_distance_m: Option<Vec<(f64, f64)>>,
     // Other, Misc.
     pub max_epa_adj: f64,
     #[serde(skip)]
     pub orphaned: bool,
 }
 
+impl SerdeAPI for RustSimDriveParams {}
+
 impl Default for RustSimDriveParams {
     fn default() -> Self {
         // if True, accuracy will be favored over performance for grade per step estimates
         // Specifically, for performance, grade for a step will be assumed to be the grade
         // looked up at step start distance. For accuracy, the actual elevations will be
         // used. This distinciton only makes a difference for CAV maneuvers.
         let favor_grade_accuracy = true;
@@ -416,14 +418,20 @@
 
     #[getter]
     pub fn get_fs_cumu_mj_out_ach(&self) -> PyResult<Pyo3ArrayF64> {
         Ok(
             Pyo3ArrayF64::new(ndarrcumsum(&(self.fs_kw_out_ach.clone() * self.cyc.dt_s() * 1e-3)))
         )
     }
+    #[getter]
+    pub fn get_fc_cumu_mj_out_ach(&self) -> PyResult<Pyo3ArrayF64> {
+        Ok(
+            Pyo3ArrayF64::new(ndarrcumsum(&(self.fc_kw_out_ach.clone() * self.cyc.dt_s() * 1e-3)))
+        )
+    }
 )]
 pub struct RustSimDrive {
     pub hev_sim_count: usize,
     #[api(has_orphaned)]
     pub veh: RustVehicle,
     #[api(has_orphaned)]
     pub cyc: RustCycle,
@@ -552,14 +560,16 @@
     pub orphaned: bool,
     pub coast_delay_index: Array1<i32>,
     pub idm_target_speed_m_per_s: Array1<f64>,
     #[serde(skip)]
     pub cyc0_cache: RustCycleCache,
 }
 
+impl SerdeAPI for RustSimDrive {}
+
 // #[cfg(test)]
 // mod tests {
 //     use super::*;
 
 //     #[test]
 //     fn test_walk() {
 //         // CYCLE
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/simdrivelabel.rs` & `fastsim-2.1.0/rust/fastsim-core/src/simdrivelabel.rs`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     }
 }
 
 pub fn get_label_fe(
     veh: &vehicle::RustVehicle,
     full_detail: Option<bool>,
     verbose: Option<bool>,
-) -> Result<(LabelFe, Option<HashMap<&str, RustSimDrive>>), anyhow::Error> {
+) -> anyhow::Result<(LabelFe, Option<HashMap<&str, RustSimDrive>>)> {
     // Generates label fuel economy (FE) values for a provided vehicle.
     //
     // Arguments:
     // ----------
     // veh : vehicle::RustVehicle
     // full_detail : boolean, default False
     //     If True, sim_drive objects for each cycle are also returned.
@@ -190,14 +190,16 @@
     let udds_filestring = include_str!(concat!(
         "..",
         main_separator!(),
         "..",
         main_separator!(),
         "..",
         main_separator!(),
+        "python",
+        main_separator!(),
         "fastsim",
         main_separator!(),
         "resources",
         main_separator!(),
         "cycles",
         main_separator!(),
         "udds.csv"
@@ -205,14 +207,16 @@
     let hwy_filestring = include_str!(concat!(
         "..",
         main_separator!(),
         "..",
         main_separator!(),
         "..",
         main_separator!(),
+        "python",
+        main_separator!(),
         "fastsim",
         main_separator!(),
         "resources",
         main_separator!(),
         "cycles",
         main_separator!(),
         "hwfet.csv"
@@ -229,19 +233,17 @@
 
     // run simdrive for non-phev powertrains
     sd.insert("udds", RustSimDrive::new(cyc["udds"].clone(), veh.clone()));
     sd.insert("hwy", RustSimDrive::new(cyc["hwy"].clone(), veh.clone()));
 
     for (k, val) in sd.iter_mut() {
         val.sim_drive(None, None)?;
-        let key = String::from(k.clone());
+        let key = String::from(*k);
         let trace_miss_speed_mph = val.trace_miss_speed_mps * MPH_PER_MPS;
-        if (key == String::from("udds") || key == String::from("hwy"))
-            && trace_miss_speed_mph > max_trace_miss_in_mph
-        {
+        if (key == *"udds" || key == *"hwy") && trace_miss_speed_mph > max_trace_miss_in_mph {
             max_trace_miss_in_mph = trace_miss_speed_mph;
         }
     }
     out.trace_miss_speed_mph = max_trace_miss_in_mph;
 
     // find year-based adjustment parameters
     let adj_params: &AdjCoef = if veh.veh_year < 2017 {
@@ -318,17 +320,17 @@
                         * props.kwh_per_gge
                         * (1. - sim_params.max_epa_adj),
                 )) * props.kwh_per_gge
                     / CHG_EFF;
             out.adj_comb_kwh_per_mi =
                 0.55 * out.adj_udds_kwh_per_mi + 0.45 * out.adj_hwy_kwh_per_mi;
 
-            out.adj_udds_kwh_per_mi = out.adj_udds_kwh_per_mi * CHG_EFF;
-            out.adj_hwy_kwh_per_mi = out.adj_hwy_kwh_per_mi * CHG_EFF;
-            out.adj_comb_kwh_per_mi = out.adj_comb_kwh_per_mi * CHG_EFF;
+            out.adj_udds_kwh_per_mi *= CHG_EFF;
+            out.adj_hwy_kwh_per_mi *= CHG_EFF;
+            out.adj_comb_kwh_per_mi *= CHG_EFF;
 
             // range for combined city/highway
             out.net_range_miles = veh.ess_max_kwh / out.adj_comb_ess_kwh_per_mi;
         }
 
         // utility factor (percent driving in PHEV charge depletion mode)
         out.uf = 0.;
@@ -395,22 +397,22 @@
     sd.insert("accel", sd_accel);
 
     // success Boolean -- did all of the tests work(e.g. met trace within ~2 mph)?
     out.res_found = String::from("model needs to be implemented for this"); // this may need fancier logic than just always being true
 
     if full_detail.unwrap_or(false) && verbose.unwrap_or(false) {
         println!("{:#?}", out);
-        return Ok((out, Some(sd)));
+        Ok((out, Some(sd)))
     } else if full_detail.unwrap_or(false) {
-        return Ok((out, Some(sd)));
+        Ok((out, Some(sd)))
     } else if verbose.unwrap_or(false) {
         println!("{:#?}", out);
-        return Ok((out, None));
+        Ok((out, None))
     } else {
-        return Ok((out, None));
+        Ok((out, None))
     }
 }
 
 pub fn get_label_fe_phev(
     veh: &vehicle::RustVehicle,
     sd: &mut HashMap<&str, RustSimDrive>,
     long_params: &RustLongParams,
@@ -426,25 +428,26 @@
     // sd : RustSimDrive objects to use for label fe calculations
     // long_params : Struct for longparams.json values
     // adj_params: Adjusted coefficients from longparams.json
     // sim_params : RustSimDriveParams
     // props : RustPhysicalProperties
     //
     // Returns label fuel economy values for PHEV as a struct.
-    let mut phev_calcs: LabelFePHEV = LabelFePHEV::default();
-
-    phev_calcs.regen_soc_buffer = min(
-        ((0.5 * veh.veh_kg * ((60. * (1. / MPH_PER_MPS)).powi(2)))
-            * (1. / 3600.)
-            * (1. / 1000.)
-            * veh.max_regen
-            * veh.mc_peak_eff())
-            / veh.ess_max_kwh,
-        (veh.max_soc - veh.min_soc) / 2.0,
-    );
+    let mut phev_calcs = LabelFePHEV {
+        regen_soc_buffer: min(
+            ((0.5 * veh.veh_kg * ((60. * (1. / MPH_PER_MPS)).powi(2)))
+                * (1. / 3600.)
+                * (1. / 1000.)
+                * veh.max_regen
+                * veh.mc_peak_eff())
+                / veh.ess_max_kwh,
+            (veh.max_soc - veh.min_soc) / 2.0,
+        ),
+        ..LabelFePHEV::default()
+    };
 
     // charge sustaining behavior
     for (key, sd_val) in sd.iter_mut() {
         // do PHEV soc iteration
         // This runs 1 cycle starting at max SOC then runs 1 cycle starting at min SOC.
         // By assuming that the battery SOC depletion per mile is constant across cycles,
         // the first cycle can be extrapolated until charge sustaining kicks in.
@@ -574,26 +577,25 @@
                 1.0 / (adj_params.city_intercept
                     + (adj_params.city_slope
                         / (sd_val.dist_mi.sum() / (phev_calc.cs_fs_kwh / props.kwh_per_gge)))),
                 sd_val.dist_mi.sum() / (phev_calc.cs_fs_kwh / props.kwh_per_gge)
                     * (1.0 - sim_params.max_epa_adj),
             ));
 
-            for c in 0..phev_calc.lab_iter_kwh_per_mi.len() {
-                if phev_calc.lab_iter_kwh_per_mi[c] == 0.0 {
+            for (c, lab_iter_kwh_per_mi) in phev_calc.lab_iter_kwh_per_mi.iter().enumerate() {
+                if *lab_iter_kwh_per_mi == 0.0 {
                     adj_iter_kwh_per_mi_vals[c] = 0.0;
                 } else {
                     adj_iter_kwh_per_mi_vals[c] =
                         (1.0 / max(
                             1.0 / (adj_params.city_intercept
                                 + (adj_params.city_slope
-                                    / ((1.0 / phev_calc.lab_iter_kwh_per_mi[c])
-                                        * props.kwh_per_gge))),
+                                    / ((1.0 / lab_iter_kwh_per_mi) * props.kwh_per_gge))),
                             (1.0 - sim_params.max_epa_adj)
-                                * ((1.0 / phev_calc.lab_iter_kwh_per_mi[c]) * props.kwh_per_gge),
+                                * ((1.0 / lab_iter_kwh_per_mi) * props.kwh_per_gge),
                         )) * props.kwh_per_gge;
                 }
             }
         } else {
             adj_iter_mpgge_vals.push(max(
                 1.0 / (adj_params.hwy_intercept
                     + (adj_params.hwy_slope
@@ -605,26 +607,25 @@
                 1.0 / (adj_params.hwy_intercept
                     + (adj_params.hwy_slope
                         / (sd_val.dist_mi.sum() / (phev_calc.cs_fs_kwh / props.kwh_per_gge)))),
                 sd_val.dist_mi.sum() / (phev_calc.cs_fs_kwh / props.kwh_per_gge)
                     * (1.0 - sim_params.max_epa_adj),
             ));
 
-            for c in 0..phev_calc.lab_iter_kwh_per_mi.len() {
-                if phev_calc.lab_iter_kwh_per_mi[c] == 0.0 {
+            for (c, lab_iter_kwh_per_mi) in phev_calc.lab_iter_kwh_per_mi.iter().enumerate() {
+                if *lab_iter_kwh_per_mi == 0.0 {
                     adj_iter_kwh_per_mi_vals[c] = 0.0;
                 } else {
                     adj_iter_kwh_per_mi_vals[c] =
                         (1.0 / max(
                             1.0 / (adj_params.hwy_intercept
                                 + (adj_params.hwy_slope
-                                    / ((1.0 / phev_calc.lab_iter_kwh_per_mi[c])
-                                        * props.kwh_per_gge))),
+                                    / ((1.0 / lab_iter_kwh_per_mi) * props.kwh_per_gge))),
                             (1.0 - sim_params.max_epa_adj)
-                                * ((1.0 / phev_calc.lab_iter_kwh_per_mi[c]) * props.kwh_per_gge),
+                                * ((1.0 / lab_iter_kwh_per_mi) * props.kwh_per_gge),
                         )) * props.kwh_per_gge;
                 }
             }
         }
         phev_calc.adj_iter_mpgge = Array::from(adj_iter_mpgge_vals);
         phev_calc.adj_iter_kwh_per_mi = Array::from(adj_iter_kwh_per_mi_vals);
 
@@ -699,29 +700,29 @@
         match *key {
             "udds" => phev_calcs.udds = phev_calc.clone(),
             "hwy" => phev_calcs.hwy = phev_calc.clone(),
             &_ => return Err(anyhow!("No field for cycle {}", key)),
         };
     }
 
-    return Ok(phev_calcs);
+    Ok(phev_calcs)
 }
 
 #[cfg(test)]
 mod simdrivelabel_tests {
     use super::*;
 
     #[test]
     fn test_get_label_fe_conv() {
         let veh: vehicle::RustVehicle = vehicle::RustVehicle::mock_vehicle();
         let (mut label_fe, _) = get_label_fe(&veh, None, None).unwrap();
         // For some reason, RustVehicle::mock_vehicle() != RustVehicle::mock_vehicle()
         // Therefore, veh field in both structs replaced with Default for comparison purposes
         label_fe.veh = vehicle::RustVehicle::default();
-        println!("Calculated net accel: {}", label_fe.net_accel);
+        // println!("Calculated net accel: {}", label_fe.net_accel);
 
         let label_fe_truth: LabelFe = LabelFe {
             veh: vehicle::RustVehicle::default(),
             adj_params: RustLongParams::default().ld_fe_adj_coef.adj_coef_map["2008"].clone(),
             lab_udds_mpgge: 32.47503766676829,
             lab_hwy_mpgge: 42.265348793379445,
             lab_comb_mpgge: 36.25407690819302,
@@ -744,118 +745,166 @@
             phev_calcs: None,
             adj_cs_comb_mpgge: None,
             adj_cd_comb_mpgge: None,
             net_phev_cd_miles: None,
             trace_miss_speed_mph: 0.0,
         };
 
-        println!(
-            "Percent diff to Python calc: {:.3}%",
-            100. * (label_fe_truth.net_accel - label_fe.net_accel) / label_fe_truth.net_accel
-        );
+        // println!(
+        //     "Percent diff to Python calc: {:.3}%",
+        //     100. * (label_fe_truth.net_accel - label_fe.net_accel) / label_fe_truth.net_accel
+        // );
 
         assert!(label_fe.approx_eq(&label_fe_truth, 1e-10));
     }
 
     #[test]
     fn test_get_label_fe_phev() {
-        let veh: vehicle::RustVehicle = vehicle::RustVehicle::new(
-            String::from("2016 Chevrolet Volt"),
-            13,
-            2016,
-            String::from("PHEV"),
-            0.3,
-            2.565,
-            950.564,
-            0.53,
-            0.59,
-            2.6,
-            136.0,
-            None,
-            1.4,
-            2000.0,
-            1.0,
-            297.0,
-            9.89,
-            75.0,
-            vec![
+        let mut veh = vehicle::RustVehicle {
+            props: RustPhysicalProperties {
+                air_density_kg_per_m3: 1.2,
+                a_grav_mps2: 9.81,
+                kwh_per_gge: 33.7,
+                fuel_rho_kg__L: 0.75,
+                fuel_afr_stoich: 14.7,
+                orphaned: false,
+            },
+            veh_kg: Default::default(),
+            scenario_name: "2016 Chevrolet Volt".into(),
+            selection: 13,
+            veh_year: 2016,
+            veh_pt_type: "PHEV".into(),
+            drag_coef: 0.3,
+            frontal_area_m2: 2.565,
+            glider_kg: 950.564,
+            veh_cg_m: 0.53,
+            drive_axle_weight_frac: 0.59,
+            wheel_base_m: 2.6,
+            cargo_kg: 136.0,
+            veh_override_kg: None,
+            comp_mass_multiplier: 1.4,
+            fs_max_kw: 2000.0,
+            fs_secs_to_peak_pwr: 1.0,
+            fs_kwh: 297.0,
+            fs_kwh_per_kg: 9.89,
+            fc_max_kw: 75.0,
+            fc_pwr_out_perc: Array1::from(vec![
                 0.0, 0.005, 0.015, 0.04, 0.06, 0.1, 0.14, 0.2, 0.4, 0.6, 0.8, 1.0,
-            ],
-            vec![
+            ]),
+            fc_eff_map: Array1::from(vec![
                 0.1, 0.12, 0.16, 0.22, 0.28, 0.33, 0.35, 0.36, 0.35, 0.34, 0.32, 0.3,
-            ],
-            String::from("SI"),
-            6.0,
-            61.0,
-            2.13,
-            30.0,
-            1.5,
-            111.0,
-            vec![0., 0.02, 0.04, 0.06, 0.08, 0.1, 0.2, 0.4, 0.6, 0.8, 1.],
-            Some(vec![
+            ]),
+            fc_eff_type: "SI".into(),
+            fc_sec_to_peak_pwr: 6.0,
+            fc_base_kg: 61.0,
+            fc_kw_per_kg: 2.13,
+            min_fc_time_on: 30.0,
+            idle_fc_kw: 1.5,
+            mc_max_kw: 111.0,
+            mc_pwr_out_perc: Array1::from(vec![
+                0.0, 0.02, 0.04, 0.06, 0.08, 0.1, 0.2, 0.4, 0.6, 0.8, 1.0,
+            ]),
+            mc_eff_map: Array1::from(vec![
                 0.84, 0.86, 0.88, 0.9, 0.91, 0.92, 0.94, 0.95, 0.95, 0.94, 0.93,
             ]),
-            3.0,
-            0.833,
-            21.6,
-            115.0,
-            18.4,
-            8.0,
-            75.0,
-            0.97,
-            110.0,
-            -0.6811,
-            0.15,
-            0.9,
-            1.0,
-            0.0,
-            0.815,
-            4.0,
-            0.007,
-            0.336,
-            0.7,
-            60.0,
-            0.2,
-            0.0,
-            85.0,
-            120.0,
-            0.98,
-            false,
-            false,
-            1.0,
-            0.86,
-            0.3,
-            114.0,
-            0.98,
-            0.005,
-            f64::NAN,
-            f64::NAN,
-            42.0,
-            f64::NAN,
-            f64::NAN,
-            0.31,
-            53.0,
-            f64::NAN,
-            f64::NAN,
-            f64::NAN,
-            f64::NAN,
-            f64::NAN,
-            f64::NAN,
-            8.4,
-            120000.0,
-            f64::NAN,
-            17000.0,
-            33170.0,
-            RustPhysicalProperties::default(),
-            500.0,
-            0.99,
-            None,
-            None,
-        )
-        .unwrap();
+            mc_sec_to_peak_pwr: 3.0,
+            mc_pe_kg_per_kw: 0.833,
+            mc_pe_base_kg: 21.6,
+            ess_max_kw: 115.0,
+            ess_max_kwh: 18.4,
+            ess_kg_per_kwh: 8.0,
+            ess_base_kg: 75.0,
+            ess_round_trip_eff: 0.97,
+            ess_life_coef_a: 110.0,
+            ess_life_coef_b: -0.6811,
+            min_soc: 0.15,
+            max_soc: 0.9,
+            ess_dischg_to_fc_max_eff_perc: 1.0,
+            ess_chg_to_fc_max_eff_perc: 0.0,
+            wheel_inertia_kg_m2: 0.815,
+            num_wheels: 4.0,
+            wheel_rr_coef: 0.007,
+            wheel_radius_m: 0.336,
+            wheel_coef_of_fric: 0.7,
+            max_accel_buffer_mph: 60.0,
+            max_accel_buffer_perc_of_useable_soc: 0.2,
+            perc_high_acc_buf: 0.0,
+            mph_fc_on: 85.0,
+            kw_demand_fc_on: 120.0,
+            max_regen: 0.98,
+            stop_start: false,
+            force_aux_on_fc: false,
+            alt_eff: 1.0,
+            chg_eff: 0.86,
+            aux_kw: 0.3,
+            trans_kg: 114.0,
+            trans_eff: 0.98,
+            ess_to_fuel_ok_error: 0.005,
+            small_motor_power_kw: 7.5,
+            large_motor_power_kw: 75.0,
+            fc_perc_out_array: FC_PERC_OUT_ARRAY.into(),
+            mc_kw_out_array: Default::default(),
+            mc_max_elec_in_kw: Default::default(),
+            mc_full_eff_array: Default::default(),
+            max_trac_mps2: Default::default(),
+            ess_mass_kg: Default::default(),
+            mc_mass_kg: Default::default(),
+            fc_mass_kg: Default::default(),
+            fs_mass_kg: Default::default(),
+            mc_perc_out_array: Default::default(),
+            regen_a: 500.0,
+            regen_b: 0.99,
+            charging_on: false,
+            no_elec_sys: false,
+            no_elec_aux: false,
+            max_roadway_chg_kw: Array1::from(vec![0.0, 0.0, 0.0, 0.0, 0.0, 0.0]),
+            input_kw_out_array: Array1::from(vec![
+                0.0,
+                0.375,
+                1.125,
+                3.0,
+                4.5,
+                7.5,
+                10.500000000000002,
+                15.0,
+                30.0,
+                45.0,
+                60.0,
+                75.0,
+            ]),
+            fc_kw_out_array: Default::default(),
+            fc_eff_array: Default::default(),
+            modern_max: 0.95,
+            mc_eff_array: Array1::from(vec![
+                0.84, 0.86, 0.88, 0.9, 0.91, 0.92, 0.94, 0.95, 0.95, 0.94, 0.93,
+            ]),
+            mc_kw_in_array: Default::default(),
+            val_udds_mpgge: f64::NAN,
+            val_hwy_mpgge: f64::NAN,
+            val_comb_mpgge: 42.0,
+            val_udds_kwh_per_mile: f64::NAN,
+            val_hwy_kwh_per_mile: f64::NAN,
+            val_comb_kwh_per_mile: 0.31,
+            val_cd_range_mi: 53.0,
+            val_const65_mph_kwh_per_mile: f64::NAN,
+            val_const60_mph_kwh_per_mile: f64::NAN,
+            val_const55_mph_kwh_per_mile: f64::NAN,
+            val_const45_mph_kwh_per_mile: f64::NAN,
+            val_unadj_udds_kwh_per_mile: f64::NAN,
+            val_unadj_hwy_kwh_per_mile: f64::NAN,
+            val0_to60_mph: 8.4,
+            val_ess_life_miles: 120000.0,
+            val_range_miles: f64::NAN,
+            val_veh_base_cost: 17000.0,
+            val_msrp: 33170.0,
+            fc_peak_eff_override: None,
+            mc_peak_eff_override: None,
+            orphaned: false,
+        };
+        veh.set_derived().unwrap();
 
         let (mut label_fe, _) = get_label_fe(&veh, None, None).unwrap();
         // For some reason, RustVehicle::mock_vehicle() != RustVehicle::mock_vehicle()
         // Therefore, veh field in both structs replaced with Default for comparison purposes
         label_fe.veh = vehicle::RustVehicle::default();
         // TODO: Figure out why net_accel values are different
         println!("Calculated net accel: {}", label_fe.net_accel);
@@ -1062,10 +1111,19 @@
             phev_calcs: Some(phev_calcs),
             adj_cs_comb_mpgge: Some(45.06826741586106),
             adj_cd_comb_mpgge: Some(2293.5675017498143),
             net_phev_cd_miles: Some(57.04992781503185),
             trace_miss_speed_mph: 0.0,
         };
 
-        assert!(label_fe.approx_eq(&label_fe_truth, 1e-8));
+        let tol = 1e-8;
+        assert!(label_fe.veh.approx_eq(&label_fe_truth.veh, tol));
+        assert!(
+            label_fe
+                .phev_calcs
+                .approx_eq(&label_fe_truth.phev_calcs, tol),
+            "label_fe.phev_calcs: {:?}",
+            &label_fe.phev_calcs
+        );
+        assert!(label_fe.approx_eq(&label_fe_truth, tol));
     }
 }
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/thermal.rs` & `fastsim-2.1.0/rust/fastsim-core/src/thermal.rs`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,16 @@
     pub state: ThermalState,
     pub history: ThermalStateHistoryVec,
     pub hvac_model_history: HVACModelHistoryVec,
     #[api(skip_get, skip_set)]
     amb_te_deg_c: Option<Array1<f64>>,
 }
 
+impl SerdeAPI for SimDriveHot {}
+
 impl SimDriveHot {
     pub fn new(
         cyc: cycle::RustCycle,
         veh: vehicle::RustVehicle,
         vehthrm: VehicleThermal,
         init_state: Option<ThermalState>,
         amb_te_deg_c: Option<Array1<f64>>,
@@ -296,15 +298,15 @@
                     init_soc
                 } else if self.sd.veh.veh_pt_type == vehicle::PHEV
                     || self.sd.veh.veh_pt_type == vehicle::BEV
                 {
                     // If EV, initializing initial SOC to maximum SOC.
                     self.sd.veh.max_soc
                 } else {
-                    panic!("Failed to properly initialize SOC.");
+                    bail!("Failed to properly initialize SOC.");
                 }
             }
         };
 
         self.walk(init_soc, aux_in_kw_override);
 
         self.set_post_scalars()?;
@@ -1095,14 +1097,16 @@
 
     /// ambient temperature
     pub amb_te_deg_c: f64,
     #[serde(skip)]
     pub orphaned: bool,
 }
 
+impl SerdeAPI for ThermalState {}
+
 impl ThermalState {
     pub fn new(
         amb_te_deg_c: Option<f64>,
         fc_te_deg_c_init: Option<f64>,
         cab_te_deg_c_init: Option<f64>,
         exhport_te_deg_c_init: Option<f64>,
         cat_te_deg_c_init: Option<f64>,
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/traits.rs` & `fastsim-2.1.0/rust/fastsim-core/src/traits.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,103 @@
 use crate::imports::*;
 use std::collections::HashMap;
 
 pub trait SerdeAPI: Serialize + for<'a> Deserialize<'a> {
-    fn to_file(&self, filename: &str) -> anyhow::Result<()> {
+    /// runs any initialization steps that might be needed
+    fn init(&mut self) -> anyhow::Result<()> {
+        Ok(())
+    }
+
+    #[allow(clippy::wrong_self_convention)]
+    /// Save current data structure to file. Method adaptively calls serialization methods
+    /// dependent on the suffix of the file given as str.
+    ///
+    /// # Argument:
+    ///
+    /// * `filename`: a `str` storing the targeted file name. Currently `.json` and `.yaml` suffixes are
+    /// supported
+    ///
+    /// # Returns:
+    ///
+    /// A Rust Result
+    fn to_file(&self, filename: &str) -> Result<(), anyhow::Error> {
         let file = PathBuf::from(filename);
         match file.extension().unwrap().to_str().unwrap() {
             "json" => serde_json::to_writer(&File::create(file)?, self)?,
             "yaml" => serde_yaml::to_writer(&File::create(file)?, self)?,
             _ => serde_json::to_writer(&File::create(file)?, self)?,
         };
         Ok(())
     }
 
+    /// Read from file and return instantiated struct. Method adaptively calls deserialization
+    /// methods dependent on the suffix of the file name given as str.
+    /// Function returns a dynamic Error Result if it fails.
+    ///
+    /// # Argument:
+    ///
+    /// * `filename`: a `str` storing the targeted file name. Currently `.json` and `.yaml` suffixes are
+    /// supported
+    ///
+    /// # Returns:
+    ///
+    /// A Rust Result wrapping data structure if method is called successfully; otherwise a dynamic
+    /// Error.
     fn from_file(filename: &str) -> Result<Self, anyhow::Error>
     where
         Self: std::marker::Sized,
         for<'de> Self: Deserialize<'de>,
     {
         let extension = Path::new(filename)
             .extension()
             .and_then(OsStr::to_str)
             .unwrap_or("");
 
         let file = File::open(filename)?;
-        match extension {
-            "yaml" => Ok(serde_yaml::from_reader(file)?),
-            "json" => Ok(serde_json::from_reader(file)?),
-            _ => Err(anyhow!("Unsupported file extension {}", extension)),
-        }
+        // deserialized file
+        let mut file_de: Self = match extension {
+            "yaml" => serde_yaml::from_reader(file)?,
+            "json" => serde_json::from_reader(file)?,
+            _ => bail!("Unsupported file extension {}", extension),
+        };
+        file_de.init()?;
+        Ok(file_de)
     }
 
     /// json serialization method.
     fn to_json(&self) -> String {
         serde_json::to_string(&self).unwrap()
     }
 
     /// json deserialization method.
-    fn from_json(json_str: &str) -> Result<Self, anyhow::Error>
-    where
-        Self: Sized,
-    {
+    fn from_json(json_str: &str) -> Result<Self, anyhow::Error> {
         Ok(serde_json::from_str(json_str)?)
     }
 
     /// yaml serialization method.
     fn to_yaml(&self) -> String {
         serde_yaml::to_string(&self).unwrap()
     }
 
     /// yaml deserialization method.
-    fn from_yaml(yaml_str: &str) -> Result<Self, anyhow::Error>
-    where
-        Self: Sized,
-    {
+    fn from_yaml(yaml_str: &str) -> Result<Self, anyhow::Error> {
         Ok(serde_yaml::from_str(yaml_str)?)
     }
 
     /// bincode serialization method.
     fn to_bincode(&self) -> Vec<u8> {
         serialize(&self).unwrap()
     }
 
     /// bincode deserialization method.
-    fn from_bincode(encoded: &[u8]) -> Result<Self, anyhow::Error>
-    where
-        Self: Sized,
-    {
+    fn from_bincode(encoded: &[u8]) -> Result<Self, anyhow::Error> {
         Ok(deserialize(encoded)?)
     }
 }
 
-impl<T> SerdeAPI for T where T: Serialize + for<'a> Deserialize<'a> {}
-
 pub trait ApproxEq<Rhs = Self> {
     fn approx_eq(&self, other: &Rhs, tol: f64) -> bool;
 }
 
 macro_rules! impl_approx_eq_for_strict_eq_types {
     ($($strict_eq_type: ty),*) => {
         $(
@@ -119,32 +141,31 @@
 }
 
 impl<T> ApproxEq for Array1<T>
 where
     T: ApproxEq + std::clone::Clone,
 {
     fn approx_eq(&self, other: &Array1<T>, tol: f64) -> bool {
-        return self.to_vec().approx_eq(&other.to_vec(), tol);
+        self.to_vec().approx_eq(&other.to_vec(), tol)
     }
 }
 
 impl<T> ApproxEq for Option<T>
 where
     T: ApproxEq,
 {
     fn approx_eq(&self, other: &Option<T>, tol: f64) -> bool {
         if self.is_none() && other.is_none() {
-            return true;
+            true
         } else if self.is_some() && other.is_some() {
-            return self
-                .as_ref()
+            self.as_ref()
                 .unwrap()
-                .approx_eq(&other.as_ref().unwrap(), tol);
+                .approx_eq(other.as_ref().unwrap(), tol)
         } else {
-            return false;
+            false
         }
     }
 }
 
 impl<K, V, S> ApproxEq for HashMap<K, V, S>
 where
     K: Eq + std::hash::Hash,
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/utils.rs` & `fastsim-2.1.0/rust/fastsim-core/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 use std::collections::HashSet;
 
 use crate::imports::*;
 #[cfg(feature = "pyo3")]
 use crate::pyo3imports::*;
 
+#[cfg(test)]
+pub fn resources_path() -> PathBuf {
+    let pb = PathBuf::from("../../python/fastsim/resources");
+    assert!(pb.exists());
+    pb
+}
+
 /// Error message for when user attempts to set value in a nested struct.
 pub const NESTED_STRUCT_ERR: &str = "Setting field value on nested struct not allowed.
 Assign nested struct to own variable, run the `reset_orphaned` method, and then 
 modify field value. Then set the nested struct back inside containing struct.";
 
 pub fn diff(x: &Array1<f64>) -> Array1<f64> {
     concatenate(
@@ -216,34 +223,40 @@
     use proc_macros::add_pyo3_api;
 
     use super::*;
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
     #[derive(Default, Serialize, Deserialize, Clone, PartialEq, Eq)]
     pub struct Pyo3ArrayU32(Array1<u32>);
+    impl SerdeAPI for Pyo3ArrayU32 {}
 
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
     #[derive(Default, Serialize, Deserialize, Clone, PartialEq, Eq)]
     pub struct Pyo3ArrayI32(Array1<i32>);
+    impl SerdeAPI for Pyo3ArrayI32 {}
 
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
     #[derive(Default, Serialize, Deserialize, Clone, PartialEq)]
     pub struct Pyo3ArrayF64(Array1<f64>);
+    impl SerdeAPI for Pyo3ArrayF64 {}
 
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
     #[derive(Default, Serialize, Deserialize, Clone, PartialEq, Eq)]
     pub struct Pyo3ArrayBool(Array1<bool>);
+    impl SerdeAPI for Pyo3ArrayBool {}
 
     /// Helper struct to allow Rust to return a Python class that will indicate to the user that it's a clone.  
     #[add_pyo3_api]
     #[derive(Default, Serialize, Deserialize, Clone, PartialEq)]
     pub struct Pyo3VecF64(Vec<f64>);
+
+    impl SerdeAPI for Pyo3VecF64 {}
 }
 
 #[cfg(feature = "pyo3")]
 pub use array_wrappers::*;
 
 #[cfg(test)]
 mod tests {
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/vehicle_thermal.rs` & `fastsim-2.1.0/rust/fastsim-core/src/vehicle_thermal.rs`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,25 @@
 impl Default for FcModelTypes {
     fn default() -> Self {
         FcModelTypes::Internal(FcTempEffModel::default(), FcTempEffComponent::default())
     }
 }
 
 /// Which commponent temperature affects FC efficency
-#[derive(Debug, Clone, Deserialize, Serialize, PartialEq, Eq)]
+#[derive(Default, Debug, Clone, Deserialize, Serialize, PartialEq, Eq)]
 pub enum FcTempEffComponent {
     /// FC efficiency is purely dependent on cat temp
     Catalyst,
     /// FC efficency is dependent on both cat and FC temp
     CatAndFC,
     /// FC efficiency is dependent on FC temp only
+    #[default]
     FuelConverter,
 }
 
-impl Default for FcTempEffComponent {
-    fn default() -> Self {
-        FcTempEffComponent::FuelConverter
-    }
-}
-
 /// Model variants for how FC efficiency depends on temperature
 #[derive(Debug, Clone, Deserialize, Serialize, PartialEq)]
 pub enum FcTempEffModel {
     /// Linear temperature dependence
     Linear(FcTempEffModelLinear),
     /// Exponential temperature dependence
     Exponential(FcTempEffModelExponential),
@@ -131,14 +126,16 @@
     pub pwr_max_aux_load_for_cooling_kw: f64,
     /// coefficient of performance of vapor compression cycle
     pub cop: f64,
     #[serde(skip)]
     orphaned: bool,
 }
 
+impl SerdeAPI for HVACModel {}
+
 impl Default for HVACModel {
     fn default() -> Self {
         Self {
             te_set_deg_c: 22.0,
             p_cntrl_kw_per_deg_c: 0.1,
             i_cntrl_kw_per_deg_c_scnds: 0.01,
             d_cntrl_kj_per_deg_c: 0.1,
@@ -161,28 +158,23 @@
 pub enum CabinHvacModelTypes {
     /// HVAC is modeled natively
     Internal(HVACModel),
     External,
 }
 
 /// Whether compontent thermal model is handled by FASTSim
-#[derive(Debug, Clone, Deserialize, Serialize, PartialEq, Eq)]
+#[derive(Debug, Default, Clone, Deserialize, Serialize, PartialEq, Eq)]
 pub enum ComponentModelTypes {
     /// Component temperature is handled inside FASTSim
+    #[default]
     Internal,
     /// Component temperature will be overriden by wrapper code
     External,
 }
 
-impl Default for ComponentModelTypes {
-    fn default() -> Self {
-        ComponentModelTypes::Internal
-    }
-}
-
 #[cfg_attr(feature = "pyo3", pyfunction)]
 /// Given Reynolds number `re`, return C and m to calculate Nusselt number for
 /// sphere, from Incropera's Intro to Heat Transfer, 5th Ed., eq. 7.44
 pub fn get_sphere_conv_params(re: f64) -> (f64, f64) {
     let (c, m) = if re < 4.0 {
         (0.989, 0.330)
     } else if re < 40.0 {
@@ -228,20 +220,20 @@
 
     pub fn set_fc_model_internal_exponential(
         &mut self,
         offset: f64,
         lag: f64,
         minimum: f64,
         fc_temp_eff_component: String
-    ) -> PyResult<()>{
+    ) -> anyhow::Result<()>{
         let fc_temp_eff_comp = match fc_temp_eff_component.as_str() {
             "FuelConverter" => FcTempEffComponent::FuelConverter,
             "Catalyst" => FcTempEffComponent::Catalyst,
             "CatAndFC" => FcTempEffComponent::CatAndFC,
-            _ => panic!("Invalid option for fc_temp_eff_component.")
+            _ => bail!("Invalid option for fc_temp_eff_component.")
         };
 
         Ok(check_orphaned_and_set!(
             self,
             fc_model,
             FcModelTypes::Internal(
                 FcTempEffModel::Exponential(
@@ -441,14 +433,16 @@
     pub cat_fc_eta_coeff: f64,
 
     /// for pyo3 api
     #[serde(skip)]
     pub orphaned: bool,
 }
 
+impl SerdeAPI for VehicleThermal {}
+
 impl Default for VehicleThermal {
     fn default() -> Self {
         VehicleThermal {
             fc_c_kj__k: 150.0,
             fc_l: 1.0,
             fc_htc_to_amb_stop: 50.0,
             fc_coeff_from_comb: 1e-4,
```

### Comparing `fastsim-2.0.22/rust/fastsim-core/src/vehicle_utils.rs` & `fastsim-2.1.0/rust/fastsim-core/src/vehicle_utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 #[cfg(feature = "pyo3")]
 use crate::pyo3imports::*;
 use crate::simdrive::RustSimDrive;
 use crate::vehicle::RustVehicle;
 
 #[allow(non_snake_case)]
 #[cfg_attr(feature = "pyo3", pyfunction)]
+#[allow(clippy::too_many_arguments)]
 pub fn abc_to_drag_coeffs(
     veh: &mut RustVehicle,
     a_lbf: f64,
     b_lbf__mph: f64,
     c_lbf__mph2: f64,
     custom_rho: Option<bool>,
     custom_rho_temp_degC: Option<f64>,
@@ -74,15 +75,15 @@
 
     let drag_coef: f64;
     let wheel_rr_coef: f64;
 
     if simdrive_optimize.unwrap_or(true) {
         let cost: GetError = GetError {
             cycle: &cyc,
-            vehicle: &veh,
+            vehicle: veh,
             dyno_func_lb: &dyno_func_lb,
         };
         let solver: NelderMead<Array1<f64>, f64> =
             NelderMead::new(vec![array![0.0, 0.0], array![0.5, 0.0], array![0.5, 0.1]]);
         let res: OptimizationResult<_, _, _> = Executor::new(cost, solver)
             .configure(|state| state.max_iters(100))
             .run()
@@ -94,15 +95,15 @@
         drag_coef = c_newton__mps2 / (0.5 * veh.frontal_area_m2 * cur_ambient_air_density_kg__m3);
         wheel_rr_coef = a_newton / veh.veh_kg / props.a_grav_mps2;
     }
 
     veh.drag_coef = drag_coef;
     veh.wheel_rr_coef = wheel_rr_coef;
 
-    return (drag_coef, wheel_rr_coef);
+    (drag_coef, wheel_rr_coef)
 }
 
 pub fn get_error_val(model: Array1<f64>, test: Array1<f64>, time_steps: Array1<f64>) -> f64 {
     // Returns time-averaged error for model and test signal.
     // Arguments:
     // ----------
     // model: array of values for signal from model
@@ -154,33 +155,32 @@
         let mut sd_coast: RustSimDrive = RustSimDrive::new(self.cycle.clone(), veh);
         sd_coast.impose_coast = Array::from_vec(vec![true; sd_coast.impose_coast.len()]);
         let _sim_drive_result: Result<_, _> = sd_coast.sim_drive(None, None);
 
         let cutoff_vec: Vec<usize> = sd_coast
             .mps_ach
             .indexed_iter()
-            .filter_map(|(index, &item)| (item < 0.1).then(|| index))
+            .filter_map(|(index, &item)| (item < 0.1).then_some(index))
             .collect();
-        let cutoff: usize;
-        if cutoff_vec.len() == 0 {
-            cutoff = sd_coast.mps_ach.len();
+        let cutoff: usize = if cutoff_vec.is_empty() {
+            sd_coast.mps_ach.len()
         } else {
-            cutoff = cutoff_vec[0];
-        }
+            cutoff_vec[0]
+        };
 
-        return Ok(get_error_val(
+        Ok(get_error_val(
             (Array::from_vec(vec![1000.0; sd_coast.mps_ach.len()])
                 * (sd_coast.drag_kw + sd_coast.rr_kw)
                 / sd_coast.mps_ach)
                 .slice_move(s![0..cutoff]),
             (sd_coast.mph_ach.map(|x| dyno_func_lb.eval(*x))
                 * Array::from_vec(vec![super::params::N_PER_LBF; sd_coast.mph_ach.len()]))
             .slice_move(s![0..cutoff]),
             cyc.time_s.slice_move(s![0..cutoff]),
-        ));
+        ))
     }
 }
 
 #[cfg(test)]
 mod vehicle_utils_tests {
     use super::*;
```

### Comparing `fastsim-2.0.22/rust/fastsim-py/src/lib.rs` & `fastsim-2.1.0/rust/fastsim-py/src/lib.rs`

 * *Files identical despite different names*

