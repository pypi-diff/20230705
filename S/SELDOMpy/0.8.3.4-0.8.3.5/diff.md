# Comparing `tmp/SELDOMpy-0.8.3.4.tar.gz` & `tmp/SELDOMpy-0.8.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.8.3.4.tar", last modified: Tue Jul  4 16:31:16 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.8.3.5.tar", last modified: Wed Jul  5 08:35:09 2023, max compression
```

## Comparing `SELDOMpy-0.8.3.4.tar` & `SELDOMpy-0.8.3.5.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.826997 SELDOMpy-0.8.3.4/
--rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.8.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0      229 2023-07-04 16:03:59.000000 SELDOMpy-0.8.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      603 2023-07-04 16:31:16.826997 SELDOMpy-0.8.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.8.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.190012 SELDOMpy-0.8.3.4/SELDOMpy/
--rw-rw-rw-   0        0        0      390 2023-07-04 08:20:50.000000 SELDOMpy-0.8.3.4/SELDOMpy/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.8.3.4/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1288 2023-07-04 08:20:50.000000 SELDOMpy-0.8.3.4/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.8.3.4/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.4/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.8.3.4/SELDOMpy/getRandomLBODEmodel.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.075997 SELDOMpy-0.8.3.4/SELDOMpy/include/
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.521997 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.078027 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.644026 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.657993 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.743026 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
--rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.4/SELDOMpy/optimization.py
--rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.8.3.4/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.4/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.4/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.4/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.816998 SELDOMpy-0.8.3.4/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/CNOStructure.h
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bandpre_impl.h
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bbdpre_impl.h
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_diag_impl.h
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_direct_impl.h
--rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_impl.h
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spils_impl.h
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/fnvector_serial.h
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/hill_function.c
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-04 16:31:16.194997 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0      603 2023-07-04 16:31:15.000000 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5566 2023-07-04 16:31:15.000000 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 16:31:15.000000 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-04 16:31:15.000000 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-04 16:31:15.000000 SELDOMpy-0.8.3.4/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-04 16:31:16.827997 SELDOMpy-0.8.3.4/setup.cfg
--rw-rw-rw-   0        0        0     4676 2023-07-04 16:31:10.000000 SELDOMpy-0.8.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.671424 SELDOMpy-0.8.3.5/
+-rw-rw-rw-   0        0        0     1077 2023-06-28 13:23:52.000000 SELDOMpy-0.8.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      229 2023-07-04 16:03:59.000000 SELDOMpy-0.8.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      603 2023-07-05 08:35:09.671424 SELDOMpy-0.8.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-28 07:06:15.000000 SELDOMpy-0.8.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:08.877446 SELDOMpy-0.8.3.5/SELDOMpy/
+-rw-rw-rw-   0        0        0      390 2023-07-04 08:20:50.000000 SELDOMpy-0.8.3.5/SELDOMpy/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.8.3.5/SELDOMpy/buildmim.py
+-rw-rw-rw-   0        0        0     1288 2023-07-04 08:20:50.000000 SELDOMpy-0.8.3.5/SELDOMpy/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.8.3.5/SELDOMpy/gen_exps.py
+-rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.5/SELDOMpy/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.8.3.5/SELDOMpy/getRandomLBODEmodel.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:08.710393 SELDOMpy-0.8.3.5/SELDOMpy/include/
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.372405 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/
+-rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
+-rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_model.h
+-rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
+-rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_problem.h
+-rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/amigoJAC.h
+-rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/amigoRHS.h
+-rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/amigoSensRHS.h
+-rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/simulate_amigo_model.h
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:08.712394 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.501425 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/
+-rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
+-rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
+-rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
+-rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
+-rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
+-rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
+-rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
+-rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
+-rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
+-rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
+-rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
+-rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.513438 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/nvector/
+-rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.590425 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/
+-rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
+-rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
+-rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
+-rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
+-rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
+-rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
+-rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
+-rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
+-rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
+-rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
+-rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
+-rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
+-rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
+-rw-rw-rw-   0        0        0     2460 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.5/SELDOMpy/optimization.py
+-rw-rw-rw-   0        0        0     1438 2023-06-23 11:21:41.000000 SELDOMpy-0.8.3.5/SELDOMpy/plot_results.py
+-rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.5/SELDOMpy/reduce_fun.py
+-rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.5/SELDOMpy/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.8.3.5/SELDOMpy/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:09.664427 SELDOMpy-0.8.3.5/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/CNOStructure.h
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bandpre_impl.h
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bbdpre_impl.h
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_diag_impl.h
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_direct_impl.h
+-rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_impl.h
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spils_impl.h
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/fnvector_serial.h
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/hill_function.c
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-05 08:35:08.890426 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-07-05 08:35:07.000000 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5566 2023-07-05 08:35:08.000000 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:35:07.000000 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-05 08:35:07.000000 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-05 08:35:07.000000 SELDOMpy-0.8.3.5/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-05 08:35:09.672425 SELDOMpy-0.8.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     4676 2023-07-05 08:34:41.000000 SELDOMpy-0.8.3.5/setup.py
```

### Comparing `SELDOMpy-0.8.3.4/LICENSE.txt` & `SELDOMpy-0.8.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/PKG-INFO` & `SELDOMpy-0.8.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.8.3.4
+Version: 0.8.3.5
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/buildmim.py` & `SELDOMpy-0.8.3.5/SELDOMpy/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/extras.py` & `SELDOMpy-0.8.3.5/SELDOMpy/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/gen_exps.py` & `SELDOMpy-0.8.3.5/SELDOMpy/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.8.3.5/SELDOMpy/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.8.3.5/SELDOMpy/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_model.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_model.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_amigo/AMIGO_problem.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_amigo/AMIGO_problem.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_band.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_config.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_math.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/include/include_cvodes/sundials/sundials_types.h` & `SELDOMpy-0.8.3.5/SELDOMpy/include/include_cvodes/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/optimization.py` & `SELDOMpy-0.8.3.5/SELDOMpy/optimization.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/plot_results.py` & `SELDOMpy-0.8.3.5/SELDOMpy/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.8.3.5/SELDOMpy/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.8.3.5/SELDOMpy/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.8.3.5/SELDOMpy/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/CNOStructure.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/CNOStructure.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bandpre_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_bbdpre_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_diag_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_direct_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_spils_impl.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/dhc.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/findStates.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/fnvector_serial.h` & `SELDOMpy-0.8.3.5/SELDOMpy/src/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.8.3.5/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.8.3.5/SELDOMpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.8.3.4
+Version: 0.8.3.5
 Summary: hardware acceleration
 Home-page: https://github.com/voxy/accel.git
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `SELDOMpy-0.8.3.4/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.8.3.5/SELDOMpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.3.4/setup.py` & `SELDOMpy-0.8.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 extra_link_args = ["-shared", "-lxilinxopencl", "-lpthread", "-lrt",
                    "-L/opt/Xilinx/SDx/2017.1.op/runtime/lib/x86_64", "-lstdc++", ]
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version='0.8.3.4',
+    version='0.8.3.5',
     description=DESCRIPTION,
     long_description=long_description,
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     packages=find_packages(exclude=('tests',)),
     ext_modules=[Extension(
```

