# Comparing `tmp/struphy-2.0.0.tar.gz` & `tmp/struphy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struphy-2.0.0.tar", last modified: Fri Jun  2 10:34:40 2023, max compression
+gzip compressed data, was "struphy-2.0.1.tar", last modified: Wed Jul  5 18:44:37 2023, max compression
```

## Comparing `struphy-2.0.0.tar` & `struphy-2.0.1.tar`

### file list

```diff
@@ -1,362 +1,365 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.615116 struphy-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-05-24 14:21:27.000000 struphy-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7601 2023-06-02 10:34:40.615116 struphy-2.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5143 2023-05-25 12:17:28.000000 struphy-2.0.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-06-02 07:48:31.000000 struphy-2.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-02 10:34:40.615116 struphy-2.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.431117 struphy-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.439117 struphy-2.0.0/src/struphy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.451117 struphy-2.0.0/src/struphy/b_splines/
--rw-rw-rw-   0 root         (0) root         (0)     1621 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/Bspline.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4670 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    14007 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    27508 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    20754 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines.py
--rw-rw-rw-   0 root         (0) root         (0)    20660 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)     6303 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines_kernels_particles.py
--rw-rw-rw-   0 root         (0) root         (0)     6384 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/compile_struphy.mk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/console/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/compile.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/example.py
--rw-rw-rw-   0 root         (0) root         (0)    18252 2023-05-30 13:00:48.000000 struphy-2.0.0/src/struphy/console/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/pproc.py
--rw-rw-rw-   0 root         (0) root         (0)     5507 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     6986 2023-06-01 11:22:35.000000 struphy-2.0.0/src/struphy/console/run.py
--rw-rw-rw-   0 root         (0) root         (0)     4416 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/console/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/diagnostics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13919 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/diagnostics/continuous_spectra.py
--rw-rw-rw-   0 root         (0) root         (0)    19187 2023-05-30 06:30:19.000000 struphy-2.0.0/src/struphy/diagnostics/diagn_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/diagnostics/paraview/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13277 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/mesh_creator.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/vtk_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/dispersion_relations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/dispersion_relations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32608 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/dispersion_relations/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/dispersion_relations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.459117 struphy-2.0.0/src/struphy/eigenvalue_solvers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5540 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/derivatives.py
--rw-rw-rw-   0 root         (0) root         (0)     5212 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_2d.py
--rw-rw-rw-   0 root         (0) root         (0)     7722 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    23321 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global.py
--rw-rw-rw-   0 root         (0) root         (0)    34110 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.459117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/
--rw-rw-rw-   0 root         (0) root         (0)    32233 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15856 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)     8521 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7080 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)    20929 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)    11250 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py
--rw-rw-rw-   0 root         (0) root         (0)    21155 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)     9994 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py
--rw-rw-rw-   0 root         (0) root         (0)     8890 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py
--rw-rw-rw-   0 root         (0) root         (0)    32983 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py
--rwxrwxrwx   0 root         (0) root         (0)     9189 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/emw_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     3606 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    11738 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py
--rw-rw-rw-   0 root         (0) root         (0)     3432 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    17672 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    17438 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    16554 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18026 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py
--rw-rw-rw-   0 root         (0) root         (0)    14698 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)    25326 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)    46819 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    27140 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)   139137 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py
--rw-rw-rw-   0 root         (0) root         (0)   146225 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.467117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10395 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py
--rw-rw-rw-   0 root         (0) root         (0)    22026 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py
--rw-rw-rw-   0 root         (0) root         (0)   144069 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py
--rw-rw-rw-   0 root         (0) root         (0)    72812 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.467117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    94136 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)    26256 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py
--rw-rw-rw-   0 root         (0) root         (0)    33024 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py
--rw-rw-rw-   0 root         (0) root         (0)   129589 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)     8106 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    19797 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    21575 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_3d.py
--rw-rw-rw-   0 root         (0) root         (0)     9590 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py
--rw-rw-rw-   0 root         (0) root         (0)    45855 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    70280 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators_core.py
--rw-rw-rw-   0 root         (0) root         (0)    86755 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/projectors_global.py
--rw-rw-rw-   0 root         (0) root         (0)    93476 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/spline_space.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/examples/
--rw-rw-rw-   0 root         (0) root         (0)     7775 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/TAE_tokamak.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_draw_parallel.py
--rw-rw-rw-   0 root         (0) root         (0)     5860 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_cylinder.py
--rw-rw-rw-   0 root         (0) root         (0)     6072 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_slab.py
--rw-rw-rw-   0 root         (0) root         (0)     8292 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_sendrecv.py
--rw-rw-rw-   0 root         (0) root         (0)     6905 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/gc_orbits_tokamak.py
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/examples/linearextendedmhd.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhd.py
--rw-rw-rw-   0 root         (0) root         (0)     3953 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhdvlasov_cc.py
--rw-rw-rw-   0 root         (0) root         (0)     3953 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhdvlasov_pc.py
--rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/maxwell.py
--rw-rw-rw-   0 root         (0) root         (0)     6873 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/orbits_tokamak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/electric_equil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/analytical.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20147 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.519117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/
--rw-rw-rw-   0 root         (0) root         (0)  8579339 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9280 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py
--rw-rw-rw-   0 root         (0) root         (0)    56499 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/equils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.523117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.435117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.523117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    65028 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7253 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.527117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/
--rw-rw-rw-   0 root         (0) root         (0)    89724 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.531117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/
--rw-rw-rw-   0 root         (0) root         (0)   161316 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-rw-   0 root         (0) root         (0)     7249 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/vtk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/vmec/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/vmec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/geometry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68581 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/base.py
--rw-rw-rw-   0 root         (0) root         (0)    25913 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/geometry/domains.py
--rw-rw-rw-   0 root         (0) root         (0)     3359 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/geometry/map_coef/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/map_coef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26068 2023-05-25 08:07:41.000000 struphy-2.0.0/src/struphy/geometry/map_eval.py
--rw-rw-rw-   0 root         (0) root         (0)    33123 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/mappings_fast.py
--rw-rw-rw-   0 root         (0) root         (0)    16513 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/transform.py
--rw-rw-rw-   0 root         (0) root         (0)     8862 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/initial/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3897 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)     7822 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8005 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/initial/eigenfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)     4104 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/initialize.py
--rw-rw-rw-   0 root         (0) root         (0)     4294 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/perturbations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.547117 struphy-2.0.0/src/struphy/io/batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/batch_cobra.sh
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_016.sh
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_032.sh
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_064.sh
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_128.sh
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_256.sh
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_512.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.547117 struphy-2.0.0/src/struphy/io/inp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.559117 struphy-2.0.0/src/struphy/io/inp/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_TAE_tokamak.yml
--rw-rw-rw-   0 root         (0) root         (0)     4989 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
--rw-rw-rw-   0 root         (0) root         (0)     5470 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
--rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
--rw-rw-rw-   0 root         (0) root         (0)     3537 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linearextendedmhd.yml
--rw-rw-rw-   0 root         (0) root         (0)     2981 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linearmhd.yml
--rwxrwxrwx   0 root         (0) root         (0)     4791 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
--rwxrwxrwx   0 root         (0) root         (0)     6403 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
--rwxrwxrwx   0 root         (0) root         (0)     2049 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_maxwell.yml
--rw-rw-rw-   0 root         (0) root         (0)     4849 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_orbits_tokamak.yml
--rwxrwxrwx   0 root         (0) root         (0)    22014 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/parameters.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/io/inp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6000 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
--rwxrwxrwx   0 root         (0) root         (0)     5493 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml
--rw-rw-rw-   0 root         (0) root         (0)     7714 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybrid_fA.yml
--rw-rw-rw-   0 root         (0) root         (0)     5423 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
--rw-rw-rw-   0 root         (0) root         (0)     5596 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
--rw-rw-rw-   0 root         (0) root         (0)     5356 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
--rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd.yml
--rw-rw-rw-   0 root         (0) root         (0)     3447 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd_gvec.yml
--rwxrwxrwx   0 root         (0) root         (0)     5592 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml
--rwxrwxrwx   0 root         (0) root         (0)     2240 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_1.yml
--rwxrwxrwx   0 root         (0) root         (0)     2316 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_2.yml
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/strscl.yml
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_1.yml
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_2.yml
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_3.yml
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_4.yml
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_5.yml
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_6.yml
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_7.yml
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_8.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/io/out/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/out/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/kinetic_background/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/analytical.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/background_eval.py
--rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/f0_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    10095 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/moments_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.587116 struphy-2.0.0/src/struphy/linear_algebra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5790 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/linear_algebra/core.py
--rw-rw-rw-   0 root         (0) root         (0)    21910 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/iterative_solvers.py
--rw-rw-rw-   0 root         (0) root         (0)    12463 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/linalg_kron.py
--rw-rw-rw-   0 root         (0) root         (0)     5299 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/schur_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     8558 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/stencil_dot_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    14375 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/stencil_transpose_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.591117 struphy-2.0.0/src/struphy/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35985 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)    17825 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/models/fluid.py
--rw-rw-rw-   0 root         (0) root         (0)    41877 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/hybrid.py
--rw-rw-rw-   0 root         (0) root         (0)    27537 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/kinetic.py
--rw-rw-rw-   0 root         (0) root         (0)     9164 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/models/main.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/models/output_handling.py
--rw-rw-rw-   0 root         (0) root         (0)    11468 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/toy.py
--rw-rw-rw-   0 root         (0) root         (0)    13506 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/models/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.595116 struphy-2.0.0/src/struphy/pic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   132313 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/accum_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    20171 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/filler_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)   247659 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/mat_vec_filler.py
--rw-rw-rw-   0 root         (0) root         (0)    33953 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/particles.py
--rw-rw-rw-   0 root         (0) root         (0)    18057 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/particles_to_grid.py
--rw-rw-rw-   0 root         (0) root         (0)    10146 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/pusher.py
--rw-rw-rw-   0 root         (0) root         (0)   184071 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/pusher_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    21310 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/pusher_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     8535 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/sampling.py
--rw-rw-rw-   0 root         (0) root         (0)    14923 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/sobol_seq.py
--rw-rw-rw-   0 root         (0) root         (0)     5608 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)    74158 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/pic/utilities_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/polar/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16532 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/basic.py
--rw-rw-rw-   0 root         (0) root         (0)    52606 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/polar/extraction_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    32352 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/linear_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/post_processing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/post_processing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6362 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/post_processing/cprofile_analyser.py
--rw-rw-rw-   0 root         (0) root         (0)    18854 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/post_processing/post_processing_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/post_processing/pproc_struphy.py
--rw-rw-rw-   0 root         (0) root         (0)     5300 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/post_processing/profile_struphy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/propagators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3393 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/base.py
--rw-rw-rw-   0 root         (0) root         (0)    60910 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/propagators/propagators_coupling.py
--rw-rw-rw-   0 root         (0) root         (0)    64079 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/propagators_fields.py
--rw-rw-rw-   0 root         (0) root         (0)    43013 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/propagators/propagators_markers.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/solvers.py
--rw-rw-rw-   0 root         (0) root         (0)  1335528 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac-0.1-py3-none-any.whl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.603116 struphy-2.0.0/src/struphy/psydac_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/banded_to_stencil_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    19977 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/basis_projection_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    43532 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/psydac_api/basis_projection_ops.py
--rw-rw-rw-   0 root         (0) root         (0)    22585 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    22918 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/linear_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    46576 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/mass.py
--rw-rw-rw-   0 root         (0) root         (0)    15604 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/mass_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    15886 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/preconditioner.py
--rw-rw-rw-   0 root         (0) root         (0)    19799 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/projectors.py
--rw-rw-rw-   0 root         (0) root         (0)    35047 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/psydac_derham.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/quadrature_evaluation_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    14732 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5381 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/utilities_kernels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.603116 struphy-2.0.0/src/struphy/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.607116 struphy-2.0.0/src/struphy/tests/tests_mpi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29086 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_accumulation.py
--rw-rw-rw-   0 root         (0) root         (0)    24190 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_basis_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_draw_parallel.py
--rw-rw-rw-   0 root         (0) root         (0)    16166 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)     6548 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_iterative_solvers.py
--rw-rw-rw-   0 root         (0) root         (0)    37762 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_mass_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    16313 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_mat_vec_filler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.611116 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19425 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py
--rw-rw-rw-   0 root         (0) root         (0)    51404 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    22396 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    14116 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py
--rw-rw-rw-   0 root         (0) root         (0)    11123 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py
--rw-rw-rw-   0 root         (0) root         (0)    64611 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py
--rw-rw-rw-   0 root         (0) root         (0)    17908 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    14178 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py
--rw-rw-rw-   0 root         (0) root         (0)    33254 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_polar.py
--rw-rw-rw-   0 root         (0) root         (0)    14324 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_basics.py
--rw-rw-rw-   0 root         (0) root         (0)     8477 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_derham.py
--rw-rw-rw-   0 root         (0) root         (0)    31560 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pushers.py
--rw-rw-rw-   0 root         (0) root         (0)    11285 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)     6583 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.615116 struphy-2.0.0/src/struphy/tests/tests_serial/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7092 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_bsplines_kernels.py
--rw-rw-rw-   0 root         (0) root         (0)    38312 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_gvec_equil.py
--rw-rw-rw-   0 root         (0) root         (0)    45727 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_polar_splines.py
--rw-rw-rw-   0 root         (0) root         (0)    33620 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_mhd_equils.py
--rw-rw-rw-   0 root         (0) root         (0)     6283 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
--rw-rw-rw-   0 root         (0) root         (0)    28774 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_projectors_global.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_prop_solvers.py
--rw-rw-rw-   0 root         (0) root         (0)    20678 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_basis_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     6177 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_linear_operators.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     2924 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_spline_space_1d.py
--rw-rw-rw-   0 root         (0) root         (0)    23198 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py
--rw-rw-rw-   0 root         (0) root         (0)    23652 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_GVEC.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_codes.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_cprofiler.py
--rw-rw-rw-   0 root         (0) root         (0)    19344 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_divB.py
--rw-rw-rw-   0 root         (0) root         (0)    10695 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_filler_kernel.py
--rw-rw-rw-   0 root         (0) root         (0)    12684 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mappings.py
--rw-rw-rw-   0 root         (0) root         (0)    16292 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mhd_equil.py
--rw-rw-rw-   0 root         (0) root         (0)    15899 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_paraview.py
--rw-rw-rw-   0 root         (0) root         (0)   277942 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py
--rw-rw-rw-   0 root         (0) root         (0)     3530 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_preconditioner.py
--rw-rw-rw-   0 root         (0) root         (0)    32930 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py
--rw-rw-rw-   0 root         (0) root         (0)    15913 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8515 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    10294 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_template_gvec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.447117 struphy-2.0.0/src/struphy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7601 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15465 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.556247 struphy-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-06-21 05:54:37.000000 struphy-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7600 2023-07-05 18:44:37.556247 struphy-2.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5142 2023-07-04 15:04:56.000000 struphy-2.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-05 14:52:10.000000 struphy-2.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-05 18:44:37.556247 struphy-2.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.480248 struphy-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.488247 struphy-2.0.1/src/struphy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.492247 struphy-2.0.1/src/struphy/b_splines/
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/Bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/b_splines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14007 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    27508 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    20754 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bsplines.py
+-rw-rw-rw-   0 root         (0) root         (0)    20660 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bsplines_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/b_splines/bsplines_kernels_particles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6405 2023-07-03 14:56:04.000000 struphy-2.0.1/src/struphy/compile_struphy.mk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.492247 struphy-2.0.1/src/struphy/console/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/console/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/compile.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    18437 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/console/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/pproc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5507 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6986 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-06-27 05:19:41.000000 struphy-2.0.1/src/struphy/console/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/console/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.492247 struphy-2.0.1/src/struphy/diagnostics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/diagnostics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/diagnostics/console_diagn.py
+-rw-rw-rw-   0 root         (0) root         (0)    13915 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/diagnostics/continuous_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)    12255 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/diagnostics/diagn_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.492247 struphy-2.0.1/src/struphy/diagnostics/paraview/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/diagnostics/paraview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13277 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/diagnostics/paraview/mesh_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/diagnostics/paraview/vtk_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.492247 struphy-2.0.1/src/struphy/dispersion_relations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/dispersion_relations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38252 2023-06-27 05:19:41.000000 struphy-2.0.1/src/struphy/dispersion_relations/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/dispersion_relations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.496247 struphy-2.0.1/src/struphy/eigenvalue_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5540 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/derivatives.py
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)     7722 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    23321 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)    34110 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.500247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/
+-rw-rw-rw-   0 root         (0) root         (0)    32233 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.500247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15856 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.500247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7080 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20929 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11250 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21155 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9994 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8890 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py
+-rw-rw-rw-   0 root         (0) root         (0)    32983 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py
+-rwxrwxrwx   0 root         (0) root         (0)     9189 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/emw_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    11738 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3432 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    17672 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    17438 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    16554 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.504247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18026 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)    14698 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    25326 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    46819 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    27140 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)   139137 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py
+-rw-rw-rw-   0 root         (0) root         (0)   146225 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.504247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.504247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10395 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    22026 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py
+-rw-rw-rw-   0 root         (0) root         (0)   144069 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    72812 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.504247 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94136 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    26256 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py
+-rw-rw-rw-   0 root         (0) root         (0)    33024 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py
+-rw-rw-rw-   0 root         (0) root         (0)   129589 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    19797 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    21575 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)     9549 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py
+-rw-rw-rw-   0 root         (0) root         (0)    45855 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    70280 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_operators_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    86755 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)    93476 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/eigenvalue_solvers/spline_space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.508247 struphy-2.0.1/src/struphy/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     7828 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/TAE_tokamak.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/_draw_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/_mhd_eigenvalues_cylinder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/_mhd_eigenvalues_slab.py
+-rw-rw-rw-   0 root         (0) root         (0)     8292 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/_sendrecv.py
+-rw-rw-rw-   0 root         (0) root         (0)     6993 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/gc_orbits_tokamak.py
+-rw-rw-rw-   0 root         (0) root         (0)     6901 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/linearextendedmhd.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/linearmhd.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/linearmhdvlasov_cc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/linearmhdvlasov_pc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/maxwell.py
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/examples/orbits_tokamak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.508247 struphy-2.0.1/src/struphy/fields_background/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.508247 struphy-2.0.1/src/struphy/fields_background/electric_equil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/electric_equil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/electric_equil/analytical.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/electric_equil/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.508247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22702 2023-06-26 08:31:22.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.508247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/data/
+-rw-rw-rw-   0 root         (0) root         (0)  8579339 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9280 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py
+-rw-rw-rw-   0 root         (0) root         (0)    67736 2023-06-26 08:31:22.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/equils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.480248 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    65028 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7253 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    89724 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)   161316 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/output/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/output/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/output/vtk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/output/vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/fields_background/mhd_equil/vmec/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/fields_background/mhd_equil/vmec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.520247 struphy-2.0.1/src/struphy/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68667 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/geometry/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    40248 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/geometry/domains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3359 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/geometry/kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.524247 struphy-2.0.1/src/struphy/geometry/map_coef/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/geometry/map_coef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26156 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/geometry/map_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)    32046 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/geometry/mappings_fast.py
+-rw-rw-rw-   0 root         (0) root         (0)    16513 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/geometry/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8862 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/geometry/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.524247 struphy-2.0.1/src/struphy/initial/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/initial/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3897 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/initial/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     7822 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/initial/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8005 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/initial/eigenfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/initial/initialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4294 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/initial/perturbations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.524247 struphy-2.0.1/src/struphy/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.524247 struphy-2.0.1/src/struphy/io/batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/batch_cobra.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_016.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_032.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_064.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_128.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_256.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/batch/p_512.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.524247 struphy-2.0.1/src/struphy/io/inp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/inp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.528247 struphy-2.0.1/src/struphy/io/inp/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/inp/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4815 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_TAE_tokamak.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5522 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5308 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-06-28 09:15:27.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_linearextendedmhd.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_linearmhd.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
+-rwxrwxrwx   0 root         (0) root         (0)     5788 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_linvlasovmaxwell_streaming_weibel.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6194 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_maxwell.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/examples/params_orbits_tokamak.yml
+-rw-rw-rw-   0 root         (0) root         (0)    12847 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/io/inp/parameters.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.532247 struphy-2.0.1/src/struphy/io/inp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/inp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
+-rwxrwxrwx   0 root         (0) root         (0)     3405 2023-06-27 05:19:41.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_coldplasma.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5551 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7776 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_hybrid_fA.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5649 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_linearmhd.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_linearmhd_gvec.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2023-07-04 15:04:56.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2240 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_maxwell_1.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/params_maxwell_2.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/strscl.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_1.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_2.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_3.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_4.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_5.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_6.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_7.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/io/inp/tests/wkscl_8.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.532247 struphy-2.0.1/src/struphy/io/out/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/io/out/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.532247 struphy-2.0.1/src/struphy/kinetic_background/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/kinetic_background/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/kinetic_background/background_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)     3629 2023-07-04 09:33:29.000000 struphy-2.0.1/src/struphy/kinetic_background/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/kinetic_background/f0_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    21280 2023-07-05 07:28:59.000000 struphy-2.0.1/src/struphy/kinetic_background/maxwellians.py
+-rw-rw-rw-   0 root         (0) root         (0)    10095 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/kinetic_background/moments_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.532247 struphy-2.0.1/src/struphy/linear_algebra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/linear_algebra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7557 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    21910 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/iterative_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12463 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/linalg_kron.py
+-rw-rw-rw-   0 root         (0) root         (0)     5299 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/schur_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     8558 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/stencil_dot_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    14375 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/linear_algebra/stencil_transpose_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.536247 struphy-2.0.1/src/struphy/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38411 2023-07-05 11:29:36.000000 struphy-2.0.1/src/struphy/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    18000 2023-06-27 05:19:41.000000 struphy-2.0.1/src/struphy/models/fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)    42265 2023-07-04 09:33:29.000000 struphy-2.0.1/src/struphy/models/hybrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    31429 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/models/kinetic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9070 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/models/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/models/output_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)    13944 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/models/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    13090 2023-06-26 08:31:22.000000 struphy-2.0.1/src/struphy/models/toy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.540247 struphy-2.0.1/src/struphy/pic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/pic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   138355 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/pic/accum_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    20171 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/filler_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)   247659 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/mat_vec_filler.py
+-rw-rw-rw-   0 root         (0) root         (0)    39865 2023-07-05 11:29:36.000000 struphy-2.0.1/src/struphy/pic/particles.py
+-rw-rw-rw-   0 root         (0) root         (0)    18056 2023-07-04 09:50:44.000000 struphy-2.0.1/src/struphy/pic/particles_to_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    15007 2023-07-05 14:52:10.000000 struphy-2.0.1/src/struphy/pic/pusher.py
+-rw-rw-rw-   0 root         (0) root         (0)   204819 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/pic/pusher_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    21310 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/pusher_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8535 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/sampling.py
+-rw-rw-rw-   0 root         (0) root         (0)    14923 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/sobol_seq.py
+-rw-rw-rw-   0 root         (0) root         (0)     5608 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/pic/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)   104291 2023-06-26 08:31:22.000000 struphy-2.0.1/src/struphy/pic/utilities_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.540247 struphy-2.0.1/src/struphy/polar/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/polar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16532 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/polar/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    52606 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/polar/extraction_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    32352 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/polar/linear_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.540247 struphy-2.0.1/src/struphy/post_processing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/post_processing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6362 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/post_processing/cprofile_analyser.py
+-rw-rw-rw-   0 root         (0) root         (0)    18853 2023-07-04 09:33:29.000000 struphy-2.0.1/src/struphy/post_processing/post_processing_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/post_processing/pproc_struphy.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/post_processing/profile_struphy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.540247 struphy-2.0.1/src/struphy/propagators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/propagators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-05 14:52:10.000000 struphy-2.0.1/src/struphy/propagators/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    62012 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/propagators/propagators_coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)    71738 2023-07-04 09:33:29.000000 struphy-2.0.1/src/struphy/propagators/propagators_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    45141 2023-07-04 09:33:29.000000 struphy-2.0.1/src/struphy/propagators/propagators_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/propagators/solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)  1335528 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac-0.1-py3-none-any.whl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.544247 struphy-2.0.1/src/struphy/psydac_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/psydac_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/banded_to_stencil_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    19977 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/basis_projection_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    43809 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/basis_projection_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    22797 2023-07-03 14:23:35.000000 struphy-2.0.1/src/struphy/psydac_api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22918 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    50895 2023-06-28 09:15:27.000000 struphy-2.0.1/src/struphy/psydac_api/mass.py
+-rw-rw-rw-   0 root         (0) root         (0)    15604 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/mass_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/preconditioner.py
+-rw-rw-rw-   0 root         (0) root         (0)    19799 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/projectors.py
+-rw-rw-rw-   0 root         (0) root         (0)    35047 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/psydac_derham.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/quadrature_evaluation_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    14732 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/psydac_api/utilities_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.544247 struphy-2.0.1/src/struphy/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.548247 struphy-2.0.1/src/struphy/tests/tests_mpi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30505 2023-07-05 11:29:36.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_accumulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    24182 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_basis_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2023-07-05 11:29:36.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_draw_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)    16166 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6544 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_iterative_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    37746 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_mass_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    16313 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_mat_vec_filler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.548247 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19425 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    51404 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    22396 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14116 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py
+-rw-rw-rw-   0 root         (0) root         (0)    11123 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py
+-rw-rw-rw-   0 root         (0) root         (0)    64611 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py
+-rw-rw-rw-   0 root         (0) root         (0)    17908 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14178 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    33254 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_polar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-07-04 12:08:43.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_prop_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14324 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_psydac_basics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8477 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_psydac_derham.py
+-rw-rw-rw-   0 root         (0) root         (0)    31868 2023-07-05 11:29:36.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_pushers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11285 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.556247 struphy-2.0.1/src/struphy/tests/tests_serial/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 18:44:25.000000 struphy-2.0.1/src/struphy/tests/tests_serial/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7092 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_bsplines_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    38312 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_gvec_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    45719 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_legacy_polar_splines.py
+-rw-rw-rw-   0 root         (0) root         (0)    34306 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_mhd_equils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    28774 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)    20676 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_basis_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/test_spline_space_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    23196 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    23652 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_GVEC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_cprofiler.py
+-rw-rw-rw-   0 root         (0) root         (0)    19344 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_divB.py
+-rw-rw-rw-   0 root         (0) root         (0)    10695 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_filler_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    12684 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mappings.py
+-rw-rw-rw-   0 root         (0) root         (0)    16292 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mhd_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    15899 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_paraview.py
+-rw-rw-rw-   0 root         (0) root         (0)   277942 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py
+-rw-rw-rw-   0 root         (0) root         (0)     3530 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_preconditioner.py
+-rw-rw-rw-   0 root         (0) root         (0)    32928 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)    15913 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8515 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10294 2023-06-21 05:54:37.000000 struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_template_gvec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:44:37.488247 struphy-2.0.1/src/struphy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7600 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15601 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 18:44:37.000000 struphy-2.0.1/src/struphy.egg-info/top_level.txt
```

### Comparing `struphy-2.0.0/LICENSE` & `struphy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/PKG-INFO` & `struphy-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struphy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Multi-model plasma physics package
 Author: Max Planck Institute for Plasma Physics
 Author-email: stefan.possanner@ipp.mpg.de, florian.holderied@ipp.mpg.de
 License: Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and 
         associated documentation files (the "Software"), to deal in the Software without restriction, 
@@ -42,19 +42,19 @@
 # STRUPHY - STRUcture-Preserving HYbrid codes
 
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
-## What you can do with struphy
+## What you can do with Struphy
 
 * Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
 * Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html#module-struphy.fields_background.mhd_equil.equils) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
 * Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
 * Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
 * Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
 * [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
     * model equations
     * domains (geometry)
     * MHD equilibria
@@ -70,24 +70,23 @@
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [Struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
 
 ## Tutorials
 
-* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+* [Tutorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
 
-* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
-of field/fluid and kinetic variables.
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Data generated by Struphy simulations, post processing and simple plotting of variables.
 
-* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
@@ -106,10 +105,10 @@
 In addition, we ask you to cite the following reference in scientific publications which contain results obtained with
 this software and developments:
 
 F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", J. Comp. Phys. 433 (2021) 110143
 
 ## Contact
 
-* Florian Holderied [floho@ipp.mpg.de](floho@ipp.mpg.de)
 * Stefan Possanner [spossann@ipp.mpg.de](spossann@ipp.mpg.de)
+* Eric Sonnendrücker [spossann@ipp.mpg.de](eric.sonnendruecker@ipp.mpg.de)
 * Xin Wang [xin.wang@ipp.mpg.de](xin.wang@ipp.mpg.de)
```

### Comparing `struphy-2.0.0/README.md` & `struphy-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # STRUPHY - STRUcture-Preserving HYbrid codes
 
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
-## What you can do with struphy
+## What you can do with Struphy
 
 * Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
 * Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html#module-struphy.fields_background.mhd_equil.equils) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
 * Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
 * Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
 * Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
 * [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
     * model equations
     * domains (geometry)
     * MHD equilibria
@@ -29,24 +29,23 @@
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [Struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
 
 ## Tutorials
 
-* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+* [Tutorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
 
-* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
-of field/fluid and kinetic variables.
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Data generated by Struphy simulations, post processing and simple plotting of variables.
 
-* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
@@ -65,10 +64,10 @@
 In addition, we ask you to cite the following reference in scientific publications which contain results obtained with
 this software and developments:
 
 F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", J. Comp. Phys. 433 (2021) 110143
 
 ## Contact
 
-* Florian Holderied [floho@ipp.mpg.de](floho@ipp.mpg.de)
 * Stefan Possanner [spossann@ipp.mpg.de](spossann@ipp.mpg.de)
+* Eric Sonnendrücker [spossann@ipp.mpg.de](eric.sonnendruecker@ipp.mpg.de)
 * Xin Wang [xin.wang@ipp.mpg.de](xin.wang@ipp.mpg.de)
```

### Comparing `struphy-2.0.0/pyproject.toml` & `struphy-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "struphy"
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.md"
 requires-python = ">=3.7, <3.11"
 license = {file = "LICENSE"}
 authors = [
   { name = "Max Planck Institute for Plasma Physics"},
   { email = "stefan.possanner@ipp.mpg.de"},
   { email = "florian.holderied@ipp.mpg.de"}
```

### Comparing `struphy-2.0.0/src/struphy/b_splines/Bspline.py` & `struphy-2.0.1/src/struphy/b_splines/Bspline.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_1d.py` & `struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_2d.py` & `struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_3d.py` & `struphy-2.0.1/src/struphy/b_splines/bspline_evaluation_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bsplines.py` & `struphy-2.0.1/src/struphy/b_splines/bsplines.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bsplines_kernels.py` & `struphy-2.0.1/src/struphy/b_splines/bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/b_splines/bsplines_kernels_particles.py` & `struphy-2.0.1/src/struphy/b_splines/bsplines_kernels_particles.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/compile_struphy.mk` & `struphy-2.0.1/src/struphy/compile_struphy.mk`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 psydac_path := $(shell $(PYTHON) -c "import psydac as _; print(_.__path__[0])")
 struphy_path := $(shell $(PYTHON) -c "import struphy as _; print(_.__path__[0])")
 
 # Arguments to this script are: 
 # flags
 # flags_openmp_pic
 # flags_openmp_mhd
-FLAGS            := --libdir $(LIBDIR) $(flags)
+FLAGS            := --libdir $(LIBDIR) $(flags) --conda-warnings off
 FLAGS_openmp_pic := $(flags_openmp_pic)
 FLAGS_openmp_mhd := $(flags_openmp_mhd)
 
 #--------------------------------------
 # SOURCE FILES PSYDAC
 #--------------------------------------
```

### Comparing `struphy-2.0.0/src/struphy/console/compile.py` & `struphy-2.0.1/src/struphy/console/compile.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/console/example.py` & `struphy-2.0.1/src/struphy/console/example.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/console/main.py` & `struphy-2.0.1/src/struphy/console/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def struphy():
     '''
     Struphy main executable. Performs argument parsing and sub-command call.
     '''
 
-    import os
+    import os, shutil
     import inspect
     import argparse
     from struphy.models import fluid, kinetic, hybrid, toy
     from struphy.console.compile import struphy_compile
     from struphy.console.run import struphy_run
     from struphy.console.units import struphy_units
     from struphy.console.profile import struphy_profile
@@ -57,24 +57,24 @@
     parser.add_argument('-v', '--version', action='version',
                         version=version_message)
     parser.add_argument('-p', '--path', action='version',
                         version=path_message, help='default installations and i/o paths')
     parser.add_argument('--set-io',
                         type=str,
                         metavar='PATH',
-                        help='set PATH to default I/O folder and copy templates there (type "." to use current working directory)',)
+                        help='make PATH the new default I/O folder and copy templates there (type "." to use current working directory)',)
 
     # create sub-commands and save name of sub-command into variable "command"
     subparsers = parser.add_subparsers(title='available commands',
                                        metavar='COMMAND',
                                        dest='command')
 
     # 1. "compile" sub-command
     parser_compile = subparsers.add_parser('compile',
-                                           help='compile computational kernels, install psydac',
+                                           help='compile computational kernels, install psydac (on first call only)',
                                            description='Compile Struphy kernels using pyccel, https://github.com/pyccel/pyccel.')
 
     parser_compile.add_argument('--no-openmp',
                                 help='compile without OpenMP',
                                 action='store_true')
 
     parser_compile.add_argument('-d', '--delete',
@@ -221,15 +221,15 @@
                               choices=list_models,
                               metavar='model',
                               help=model_message,)
 
     parser_units.add_argument('-i', '--input',
                               type=str,
                               metavar='FILE',
-                              help='parameter file (.yml) relative to <install_path>/struphy/io/inp/ (default=parameters.yml)',
+                              help='parameter file (.yml) relative to current I/O path (default=parameters.yml)',
                               default='parameters.yml',)
 
     parser_units.add_argument('--input-abs',
                               type=str,
                               metavar='FILE',
                               help='parameter file (.yml), absolute path',)
 
@@ -270,15 +270,15 @@
         'pproc',
         help='post process data of a finished Struphy run',
         description='Post-process data of a finished Struphy run to prepare for diagnostics.')
 
     parser_pproc.add_argument('-d', '--dirr',
                               type=str,
                               metavar='DIR',
-                              help='simulation output folder to post-process relative to <install_path>/struphy/io/out/ (default=sim_1)',
+                              help='simulation output folder to post-process relative to current I/O path (default=sim_1)',
                               default='sim_1',)
 
     parser_pproc.add_argument('--dir-abs',
                               type=str,
                               metavar='DIR',
                               help='simulation output folder to post-process, absolute path',)
 
@@ -381,14 +381,18 @@
             pass
 
         from distutils.dir_util import copy_tree
         copy_tree(os.path.join(libpath, 'io/inp/'),
                   os.path.join(io_dir, 'inp/'))
         copy_tree(os.path.join(libpath, 'io/batch/'),
                   os.path.join(io_dir, 'batch/'))
+        
+        # remove tests and examples input folders
+        shutil.rmtree(os.path.join(io_dir, 'inp/tests/'))
+        shutil.rmtree(os.path.join(io_dir, 'inp/examples/'))
 
         print(f'New default I/O path has been set:')
         import subprocess
         subprocess.run(['struphy', '-p'])
 
         exit()
```

### Comparing `struphy-2.0.0/src/struphy/console/pproc.py` & `struphy-2.0.1/src/struphy/console/pproc.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/console/profile.py` & `struphy-2.0.1/src/struphy/console/profile.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/console/run.py` & `struphy-2.0.1/src/struphy/console/run.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/console/units.py` & `struphy-2.0.1/src/struphy/console/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,12 @@
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     # load model class
     objs = [fluid, kinetic, hybrid, toy]
     for obj in objs:
         try:
             model_class = getattr(obj, model)
-        except:
+        except AttributeError:
             pass
 
     # print units
     model_class.model_units(params, verbose=True)
```

### Comparing `struphy-2.0.0/src/struphy/diagnostics/continuous_spectra.py` & `struphy-2.0.1/src/struphy/diagnostics/continuous_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     n_tor = int(os.path.split(spec_path)[-1][-6:-4])
     
     # load parameter file
     with open(os.path.join(input_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
        
     # create domain and MHD equilibrium
-    from struphy.models.utilities import setup_domain_mhd
+    from struphy.models.setup import setup_domain_mhd
     
     domain, mhd_equil = setup_domain_mhd(params)
        
     # get MHD equilibrium parameters
     params_mhd = params['mhd_equilibrium'][params['mhd_equilibrium']['type']]
     
     # set up spline spaces
```

### Comparing `struphy-2.0.0/src/struphy/diagnostics/diagn_tools.py` & `struphy-2.0.1/src/struphy/post_processing/post_processing_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,507 +1,557 @@
-#!/usr/bin/env python3
-import matplotlib.pyplot as plt
 import numpy as np
-from scipy.fft import fftfreq, fftn
-import matplotlib.colors as colors
-import argparse
-import pickle
+
 import os
+import shutil
 import h5py
 import yaml
 
-import struphy
-from struphy.dispersion_relations import analytic
+from struphy.psydac_api.psydac_derham import Derham
+from struphy.psydac_api.fields import Field
+from struphy.kinetic_background import maxwellians
+from struphy.models.setup import setup_domain_mhd
 
+from tqdm import tqdm
 
-def main():
-    """
-    TODO
+
+def create_femfields(path, step=1):
     """
+    Creates instances of struphy.psydac_api.fields.Field from distributed Struphy data.
 
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter)
+    Parameters
+    ----------
+    path : str
+        Absolute path of simulation output folder.
 
-    parser.add_argument('actions', nargs='+', type=str, default=[None],
-                        help='''which actions to perform:\
-                            \n - fourier_1d   : performs Fourier analysis of the fields and plots the results\
-                            \n - plot_scalars : plots the scalar quantities that were saved during the simulation\
-                            \n - plot_distr   : plots the distribution function and delta-f (if available)\
-                            \n                  set points for slicing with options below (default is middle of the space)''')
-    parser.add_argument('-f', nargs=1, type=str, default=['sim_1'],
-                        help='in which folder the simulation data has been stored')
-    parser.add_argument('-scalars', nargs='+', action='append', default=[[]],
-                        help='(for plot_scalars) which quantities to plot')
-    parser.add_argument('--log', action='store_true',
-                        help='(for plot_scalars) if logarithmic y-axis should be used')
-    parser.add_argument('-t', nargs=1, type=float, default=[0.],
-                        help='(for plot_distr) at which time to plot the distribution function')
-    parser.add_argument('-e1', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which position in eta1 direction to plot')
-    parser.add_argument('-e2', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which position in eta2 direction to plot')
-    parser.add_argument('-e3', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which position in eta3 direction to plot')
-    parser.add_argument('-v1', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which point in v1 direction to plot')
-    parser.add_argument('-v2', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which point in v2 direction to plot')
-    parser.add_argument('-v3', nargs=1, type=float, default=[None],
-                        help='(for plot_distr) at which point in v3 direction to plot')
-
-    args = parser.parse_args()
-    actions = args.actions
-    foldername = args.f[0]
-    time = args.t[0]
-    do_log = args.log
-    scalars_plot = args.scalars[0]
-    
-    libpath = struphy.__path__[0]
-    with open(os.path.join(libpath, 'io_path.txt')) as f:
-        io_path = f.readlines()[0]
-        
-    path = os.path.join(io_path, 'io/out', foldername)
+    step : int, optional
+        Whether to create FEM fields at every time step (step=1, default), every second time step (step=2), etc. 
 
-    grid_slices = {'e': {'e1': args.e1[0], 'e2': args.e2[0], 'e3': args.e3[0]},
-                   'v': {'v1': args.v1[0], 'v2': args.v2[0], 'v3': args.v3[0]}}
+    Returns
+    -------
+    fields : dict
+        Nested dictionary holding struphy.psydac_api.field.Field: fields[t][name] contains the Field with the name "name" in the hdf5 file at time t.
 
-    # code name
-    with open(path + '/meta.txt', 'r') as f:
+    space_ids : dict
+        The space IDs of the fields (H1, Hcurl, Hdiv, L2 or H1vec). space_ids[name] contains the space ID of the field with the name "name".
+
+    model : str
+        From which model in struphy/models the data has been obtained.
+    """
+
+    # get model name and # of MPI processes from meta.txt file
+    with open(os.path.join(path, 'meta.txt'), 'r') as f:
         lines = f.readlines()
 
-    code = lines[3].split()[-1]
+    model = lines[3].split()[-1]
+    nproc = lines[4].split()[-1]
+
+    # create Derham sequence from grid parameters
+    with open(os.path.join(path, 'parameters.yml'), 'r') as f:
+        params = yaml.load(f, Loader=yaml.FullLoader)
+
+    derham = Derham(params['grid']['Nel'],
+                    params['grid']['p'],
+                    params['grid']['spl_kind'])
 
-    # Get fields
+    # get fields names, space IDs and time grid from 0-th rank hdf5 file
     file = h5py.File(os.path.join(path, 'data/', 'data_proc0.hdf5'), 'r')
-    field_names = list(file['feec'].keys())
-    saved_scalars = file['scalar']
-    saved_time = file['time']['value'][:]
-
-    # read in parameters
-    with open(path + '/parameters.yml') as file:
-        params = yaml.load(file, Loader=yaml.FullLoader)
-
-    if 'fourier_1d' in actions:
-        assert os.path.exists(os.path.join(path, 'post_processing', 'fields_data')), \
-            'For Fourier analysis needs fields in the model.'
-
-        point_data_log = []
-        # load data dicts for e_field
-        for k in range(len(field_names)):
-            with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_log.bin'), 'rb') as handle:
-                point_data_log += [pickle.load(handle)]
-
-        point_data_phys = []
-        for k in range(len(field_names)):
-            with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_phy.bin'), 'rb') as handle:
-                point_data_phys += [pickle.load(handle)]
-
-        # load grids
-        with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_log.bin'), 'rb') as handle:
-            grids = pickle.load(handle)
-
-        with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_phy.bin'), 'rb') as handle:
-            grids_mapped = pickle.load(handle)
-
-        if code == 'LinearMHD':
-            equil_type = params['mhd_equilibrium']['name']
-
-            if equil_type == 'HomogenSlab':
-                B0x = params['mhd_equilibrium']['HomogenSlab']['B0x']
-                B0y = params['mhd_equilibrium']['HomogenSlab']['B0y']
-                B0z = params['mhd_equilibrium']['HomogenSlab']['B0z']
-
-                p0 = (2*params['mhd_equilibrium']['HomogenSlab']
-                      ['beta']/100)/(B0x**2 + B0y**2 + B0z**2)
-                n0 = params['mhd_equilibrium']['HomogenSlab']['n0']
 
-                gamma = 5/3
+    space_ids = {}
 
-            else:
-                raise NotImplementedError(
-                    f'Dispersion relations for MHD equilibrium of type {equil_type} has not been implemented yet!')
+    for field_name, dset in file['feec'].items():
+        space_ids[field_name] = dset.attrs['space_id']
 
-            disp_params = {'B0x': B0x, 'B0y': B0y, 'B0z': B0z,
-                           'p0': p0, 'n0': n0, 'gamma': gamma}
+    t_grid = file['time/value'][::step].copy()
 
-            # fft in (t, z) of first component of u_field on physical grid
-            fourier_1d(point_data_log[3], field_names[3], code, grids,
-                       grids_mapped=grids_mapped, component=0, slice_at=[0, 0, None],
-                       do_plot=True, disp_name='Mhd1D', disp_params=disp_params,
-                       save_plot=True, save_name=os.path.join(path, code + '_' + field_names[3]))
-
-            # fft in (t, z) of pressure on physical grid
-            fourier_1d(point_data_log[2], field_names[2], code, grids,
-                       grids_mapped=grids_mapped, component=0, slice_at=[0, 0, None],
-                       do_plot=True, disp_name='Mhd1D', disp_params=disp_params,
-                       save_plot=True, save_name=os.path.join(path, code + '_' + field_names[2]))
-
-        elif code == 'Maxwell':
-            # fft in (t, z) of first component of e_field on physical grid
-            fourier_1d(point_data_log[1], field_names[1], code, grids,
-                       grids_mapped=grids_mapped, component=0, slice_at=[0, 0, None],
-                       do_plot=True, disp_name='Maxwell1D',
-                       save_plot=True, save_name=os.path.join(path, code + '_' + field_names[1]))
+    file.close()
 
-        else:
-            raise NotImplementedError(
-                f'1D Fourier analysis is not yet implemented for the model {code}')
+    # create one FemField for each snapshot
+    fields = {}
+    for t in t_grid:
+        fields[t] = {}
+        for field_name, ID in space_ids.items():
+            fields[t][field_name] = Field(field_name, ID, derham)
 
-    if 'plot_scalars' in actions:
-        plot_scalars(saved_time,
-                     saved_scalars,
-                     scalars_plot=scalars_plot,
-                     do_log=do_log,
-                     save_plot=True,
-                     savename=os.path.join(path, code))
-
-    if 'plot_distr' in actions:
-        for species in params['kinetic'].keys():
-            time_idx = np.argmin(np.abs(time - saved_time))
-            plot_distr_fun(path=os.path.join(path, 'post_processing', 'kinetic_data', species),
-                           time_idx=time_idx,
-                           grid_slices=grid_slices,
-                           save_plot=True, savepath=path)
+    # get hdf5 data
+    for rank in range(int(nproc)):
 
-    file.close()
+        # open hdf5 file
+        file = h5py.File(os.path.join(
+            path, 'data/', 'data_proc' + str(rank) + '.hdf5'), 'r')
 
+        for field_name, dset in tqdm(file['feec'].items()):
 
-def fourier_1d(values, name, code, grids,
-               grids_mapped=None, component=0, slice_at=[None, 0, 0],
-               do_plot=False, disp_name=None, disp_params={},
-               save_plot=False, save_name=None, file_format='png'):
-    """
-    Perform fft in space-time, (t, x) -> (omega, k), where x can be a logical or physical coordinate.
-    Returns values if plot=False.
+            # get global start indices, end indices and pads
+            gl_s = dset.attrs['starts']
+            gl_e = dset.attrs['ends']
+            pads = dset.attrs['pads']
 
-    Parameters
-    ----------
-        values : dict
-            Dictionary holding values of a B-spline FemField on the grid as 3d np.arrays:
-            values[n] contains the values at time step n, where n = 0:Nt-1:step with 0<step.
+            assert gl_s.shape == (3,) or gl_s.shape == (3, 3)
+            assert gl_e.shape == (3,) or gl_e.shape == (3, 3)
+            assert pads.shape == (3,) or pads.shape == (3, 3)
 
-        name : str
-            Name of the FemField. 
+            # loop over time
+            for n, t in enumerate(t_grid):
 
-        code : str
-            From which code the data has been obtained.
+                # scalar field
+                if gl_s.shape == (3,):
 
-        grids : 3-list
-            1d logical grids in each eta-direction with Nel[i]*npts_per_cell[i] + 1 entries in each direction. 
+                    s1, s2, s3 = gl_s
+                    e1, e2, e3 = gl_e
+                    p1, p2, p3 = pads
+
+                    data = dset[n*step, p1:-p1, p2:-p2, p3:-p3].copy()
+
+                    fields[t][field_name].vector[s1:e1 +
+                                                 1, s2:e2 + 1, s3:e3 + 1] = data
+                    # update after each data addition, can be made more efficient
+                    fields[t][field_name].vector.update_ghost_regions()
+
+                # vector-valued field
+                else:
+                    for comp in range(3):
 
-        grids_mapped : 3-list
-            Mapped grids obtained by domain(). If None, the fft is performed on the logical grids.
+                        s1, s2, s3 = gl_s[comp]
+                        e1, e2, e3 = gl_e[comp]
+                        p1, p2, p3 = pads[comp]
 
-        component : int
-            Which component of a FemField to consider; is 0 for 0-and 3-forms, is in {0, 1, 2} for 1- and 2-forms.
+                        data = dset[str(comp + 1)][n * step,
+                                                   p1:-p1,
+                                                   p2:-p2,
+                                                   p3:-p3].copy()
 
-        slice_at : 3-list
-            At which indices i, j the 1d slice data (t, eta)_(i, j) should be obtained. 
-            One entry must be "None"; this is the direction of the fft. 
-            Default: [None, 0, 0] performs the eta1-fft at (eta2[0], eta3[0]). 
+                        fields[t][field_name].vector[comp][s1:e1 + 1,
+                                                           s2:e2 + 1,
+                                                           s3:e3 + 1] = data
+                    # update after each data addition, can be made more efficient
+                    fields[t][field_name].vector.update_ghost_regions()
 
-        do_plot : boolean
-            Plot result if True, otherwise return things.
+        file.close()
 
-        disp_name : str
-            The name of the dispersion relation class in struphy.dispersion_relations.analytic to be used for analytic comparison.
+    print('Creation of PSYDAC FemFields done.')
 
-        disp_params : dict
-            Parameters needed for analytical dispersion relation, see struphy.dispersion_relations.analytic.
+    return fields, space_ids, model
+
+
+def eval_femfields(path, fields, space_ids, celldivide=[1, 1, 1]):
+    """
+    Evaluate FEM fields obtained from create_femfields. 
+
+    Parameters
+    ----------
+    path : str
+        Absolute path of simulation output folder.
 
-        save_plot : boolean
-            Save figure if True. Then a path has to be given.
+    fields : dict
+        Obtained from struphy.diagnostics.post_processing.create_femfields.
 
-        save_name : str
-            Name under which the plot of the result should be saved.
+    space_ids : dict
+        Obtained from struphy.diagnostics.post_processing.create_femfields.
 
-        file_format : str
-            Type of file which the plot of the result should be saved.
+    celldivide : list of ints, optional
+        Grid refinement in each eta direction.
 
     Returns
     -------
-        omega : np.array
-            1d array of angular frequency.
+    point_data_log : dict
+        Nested dictionary holding values of FemFields on the grid as list of 3d np.arrays:
+        point_data_log[name][t] contains the values of the field with name "name" in fields[t].keys() at time t.
 
-        kvec : np.array
-            1d array of wave vector.
+    point_data_phy : dict
+        Pushed-forward point_data_log obtained by domain.push().
 
-        dispersion : np.array
-            2d array of shape (omega.size, kvce.size) holding the fft.
+    grids_log : 3-list
+        1d logical grids in each eta-direction with Nel[i]*cell_divide[i] + 1 entries in each direction.  
+
+    grids_phy : 3-list
+        Mapped (physical) grids obtained by domain(*grids_log).
     """
 
-    print(f'code: {code}')
+    assert isinstance(fields, dict)
+    assert isinstance(space_ids, dict)
 
-    keys = list(values.keys())
+    # domain object according to parameter file and grids
+    with open(os.path.join(path, 'parameters.yml'), 'r') as f:
+        params = yaml.load(f, Loader=yaml.FullLoader)
 
-    # check uniform grid in time
-    dt = keys[1] - keys[0]
-    print(f'time step: {dt}')
-    assert np.all([np.abs(y - x - dt) < 1e-12 for x,
-                  y in zip(keys[:-1], keys[1:])])
-
-    # create 4d np.array with shape (time, eta1, eta2, eta3)
-    dim_t = len(keys)
-    dim_eta = values[keys[0]][component].shape
-
-    temp = np.zeros((dim_t, *dim_eta))
-
-    for n, (time, snapshot) in enumerate(values.items()):
-        temp[n, :, :, :] = snapshot[component]
-
-    # Extract 2d data (t, eta) for fft
-    if slice_at[0] == None:
-
-        data = temp[:, :, slice_at[1], slice_at[2]]
-        grid = grids[0]
-        if grids_mapped is not None:
-            grid = grids_mapped[0][:, slice_at[1], slice_at[2]]
-
-    elif slice_at[1] == None:
-
-        data = temp[:, slice_at[0], :, slice_at[2]]
-        grid = grids[1]
-        if grids_mapped is not None:
-            grid = grids_mapped[1][slice_at[0], :, slice_at[2]]
-
-    elif slice_at[2] == None:
-
-        data = temp[:, slice_at[0], slice_at[1], :]
-        grid = grids[2].flatten()
-        if grids_mapped is not None:
-            grid = grids_mapped[2][slice_at[0], slice_at[1], :]
-
-    else:
-        AssertionError('One entry of slice_at must be "None".')
-
-    # extract uniform grid in space
-    Nt = data.shape[0]
-    Nx = grid.size
-    dx = grid[1] - grid[0]
-    print(f'space step: {dx}')
-    assert np.allclose(grid[1:] - grid[:-1], dx*np.ones_like(grid[:-1]))
-
-    dispersion = (2./Nt)*(2./Nx)*np.abs(fftn(data))[:Nt//2, :Nx//2]
-    kvec = 2*np.pi*fftfreq(Nx, dx)[:Nx//2]
-    omega = 2*np.pi*fftfreq(Nt, dt)[:Nt//2]
-
-    if do_plot:
-        _, ax = plt.subplots(1, 1, figsize=(10, 10))
-        colormap = 'plasma'
-        K, W = np.meshgrid(kvec, omega)
-        lvls = np.logspace(-15, -1, 27)
-        disp_plot = ax.contourf(K, W, dispersion**2 / (dispersion**2).max(),
-                                cmap=colormap, norm=colors.LogNorm(), levels=lvls)
-        plt.colorbar(ticks=[1e-12, 1e-9, 1e-6, 1e-3],
-                     mappable=disp_plot, format='%.0e')
-        title = name + ' component ' + \
-            str(component + 1) + ' from code: ' + code
-        ax.set_title(title)
-        ax.set_xlabel('$k$ [a.u.]')
-        ax.set_ylabel('$\omega$ [a.u.]')
-
-        # analytic solution:
-        disp_class = getattr(analytic, disp_name)
-        disp = disp_class(**disp_params)
-
-        kpara = kvec
-
-        branches = disp(kpara)
-        set_min = 0.
-        set_max = 0.
-        for key, branch in branches.items():
-            vals = np.real(branch)
-            ax.plot(kvec, vals, '--', label=key)
-            tmp = np.min(vals)
-            if tmp < set_min:
-                set_min = tmp
-            tmp = np.max(vals)
-            if tmp > set_max:
-                set_max = tmp
-
-        ax.legend()
-        ax.set_xlim(0, kvec[-1])
-        ax.set_ylim(set_min*1.1, set_max*1.1)
-
-        if save_plot:
-            assert save_name is not None, 'When wanting to save the plot a path has to be given!'
-            plt.savefig(save_name + '.' + file_format)
-        else:
-            plt.show()
+    domain = setup_domain_mhd(params)[0]
+
+    # create logical and physical grids
+    assert isinstance(celldivide, list)
+    assert len(celldivide) == 3
+
+    Nel = params['grid']['Nel']
+
+    grids_log = [np.linspace(0., 1., Nel_i * n_i + 1)
+                 for Nel_i, n_i in zip(Nel, celldivide)]
+    grids_phy = [domain(*grids_log)[0],
+                 domain(*grids_log)[1],
+                 domain(*grids_log)[2]]
+
+    # evaluate fields at evaluation grid and push-forward
+    point_data_log = {}
+    point_data_phy = {}
+
+    # one dict for each field
+    for name in space_ids:
+        point_data_log[name] = {}
+        point_data_phy[name] = {}
+
+    # time loop
+    print('Evaluating fields ...')
+    for t in tqdm(fields):
 
-    else:
-        return kvec, omega, dispersion
+        # field loop
+        for name, field in fields[t].items():
 
+            # space ID
+            space_id = space_ids[name]
+
+            # field evaluation
+            temp_val = field(*grids_log)
+
+            point_data_log[name][t] = []
+            point_data_phy[name][t] = []
+
+            # scalar spaces
+            if isinstance(temp_val, np.ndarray):
+
+                point_data_log[name][t].append(temp_val)
+
+                # push-forward
+                if space_id == 'H1':
+                    point_data_phy[name][t].append(domain.push(
+                        temp_val, *grids_log, kind='0_form'))
+                elif space_id == 'L2':
+                    point_data_phy[name][t].append(domain.push(
+                        temp_val, *grids_log, kind='3_form'))
+
+            # vector-valued spaces
+            else:
 
-def plot_scalars(time, scalar_quantities, scalars_plot=[], do_log=False, save_plot=False, savename=None, file_format='png'):
+                for j in range(3):
+
+                    point_data_log[name][t].append(temp_val[j])
+
+                    # push-forward
+                    if space_id == 'Hcurl':
+                        point_data_phy[name][t].append(domain.push(
+                            temp_val, *grids_log, kind='1_form')[j])
+                    elif space_id == 'Hdiv':
+                        point_data_phy[name][t].append(domain.push(
+                            temp_val, *grids_log, kind='2_form')[j])
+                    elif space_id == 'H1vec':
+                        point_data_phy[name][t].append(domain.push(
+                            temp_val, *grids_log, kind='vector')[j])
+
+    return point_data_log, point_data_phy, grids_log, grids_phy
+
+
+def create_vtk(path, grids_phy, point_data_phy):
     """
-    Plot the scalar quantities and the relative error in the total energy for a simulation.
+    Creates structured virtual toolkit files (.vts) for Paraview from evaluated field data.
 
     Parameters
     ----------
-    scalar_quantities : dict
-        HDF5 dictionary dataset containing the scalar quantities that were saved during the simulation
+    path : str
+        Absolute path of where to store the .vts files. Will then be in path/vtk/step_<step>.vts.
+
+    grids_phy : 3-list
+        Mapped (physical) grids obtained from struphy.diagnostics.post_processing.eval_femfields.
 
-    scalars_plot : list
-        list of names of scalars that should be plotted. If empty then all are plotted
+    point_data_phy : dict
+        Pushed-forward field data obtained from struphy.diagnostics.post_processing.eval_femfields.
+    """
 
-    do_log : boolean
-        Do a logarithmic plot in the y-axis if True.
+    from pyevtk.hl import gridToVTK
 
-    save_plot : boolean
-        Save figure if True. Then a path has to be given.
+    # directory for vtk files
+    path_vtk = os.path.join(path, 'vtk')
 
-    savename : str
-        Name under which the plot of the result should be saved.
+    try:
+        os.mkdir(path_vtk)
+    except:
+        shutil.rmtree(path_vtk)
+        os.mkdir(path_vtk)
 
-    file_format : str
-        Type of file which the plot of the result should be saved.
-    """
+    # field names
+    names = list(point_data_phy.keys())
 
-    if 'en_tot' in scalar_quantities.keys():
-        en_tot = scalar_quantities['en_tot'][:]
+    # time loop
+    tgrid = list(point_data_phy[names[0]].keys())
 
-        plt.figure('en_tot')
-        if do_log:
-            plt.semilogy(time, en_tot)
-        else:
-            plt.plot(time, en_tot)
+    nt = len(tgrid) - 1
+    log_nt = int(np.log10(nt)) + 1
 
-        if save_plot:
-            assert savename is not None, 'When wanting to save the plot a path has to be given!'
-            plt.savefig(savename + '_en_tot' + '.' + file_format)
-        else:
-            plt.show()
+    print('Creating vtk ...')
+    for n, t in enumerate(tqdm(tgrid)):
 
-        plt.figure('en_tot_rel_err')
-        plt.plot(time[1:], np.divide(
-            np.abs(en_tot[1:] - en_tot[0]), en_tot[0]))
-
-        if save_plot:
-            assert savename is not None, 'When wanting to save the plot a path has to be given!'
-            plt.savefig(savename + '_en_tot_rel_err' + '.' + file_format)
-        else:
-            plt.show()
+        point_data_n = {}
 
-    plt.figure('scalars')
-    if len(scalars_plot) == 0:
-        for key, quantity in scalar_quantities.items():
-            if key not in ['time', 'en_tot']:
-                if do_log:
-                    plt.semilogy(time, quantity[:], label=key)
-                else:
-                    plt.plot(time, quantity[:], label=key)
-    else:
-        for key in scalars_plot:
-            if do_log:
-                plt.semilogy(time, scalar_quantities[key][:], label=key)
-            else:
-                plt.plot(time, scalar_quantities[key][:], label=key)
+        for name in names:
 
-    plt.legend()
-    plt.xlabel('time')
+            points_list = point_data_phy[name][t]
 
-    if save_plot:
-        assert savename is not None, 'When wanting to save the plot a path has to be given!'
-        plt.savefig(savename + '_scalars' + '.' + file_format)
-    else:
-        plt.show()
+            # scalar
+            if len(points_list) == 1:
+                point_data_n[name] = points_list[0]
 
+            # vector
+            else:
+                for j in range(3):
+                    point_data_n[name + f'_{j + 1}'] = points_list[j]
+
+        gridToVTK(os.path.join(path_vtk, 'step_{0:0{1}d}'.format(n, log_nt)),
+                  *grids_phy, pointData=point_data_n)
 
-def plot_distr_fun(path, time_idx, grid_slices, save_plot=False, savepath=None, file_format='png'):
+
+def post_process_markers(path_in, path_out, species, step=1):
     """
-    Plot the binned distribution function at given slices of the phase space.
+    Computes the Cartesian (x, y, z) coordinates of saved markers during a simulation and writes them
+    to text files that can be imported to e.g. Paraview (one text file for each time step saved as
+    "<name_of_species>_<time_step>.txt" in a directory "kinetic_data/<name_of_species>/orbits/").
 
     Parameters
     ----------
-    path : str
-        Path to the kinetic data of the species.
+    path_in : str
+        Absolute path of simulation output folder.
+
+    path_out : str
+        Absolute path of where to store the .txt files. Will be in path_out/orbits. 
+
+    species : str
+        Name of the species for which the post processing should be performed.
+
+    step : int, optional
+        Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc. 
+    """
+
+    # get # of MPI processes from meta.txt file
+    with open(os.path.join(path_in, 'meta.txt'), 'r') as f:
+        lines = f.readlines()
+
+    nproc = lines[4].split()[-1]
+
+    # create domain for calculating markers' physical coordinates
+    with open(os.path.join(path_in, 'parameters.yml'), 'r') as f:
+        params = yaml.load(f, Loader=yaml.FullLoader)
+
+    domain = setup_domain_mhd(params)[0]
+
+    # open hdf5 files and get names and number of saved markers of kinetic species
+    files = [h5py.File(os.path.join(
+        path_in, 'data/', f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
+
+    n_IDs = files[0]['kinetic/' + species + '/markers'].shape[1]
 
-    time : float
-        at which point in time to plot
+    # directory for .txt files
+    path_orbits = os.path.join(path_out, 'orbits')
 
-    grid_slices : dict
-        dictionary with keys e and v that hold dictionaries with directions and values
-        that indicate which slices of the data should be plotted
+    try:
+        os.mkdir(path_orbits)
+    except:
+        shutil.rmtree(path_orbits)
+        os.mkdir(path_orbits)
 
-    save_plot : boolean
-        Save figure if True. Then a path has to be given.
+    t_grid = files[0]['time/value'][::step]
 
-    savepath : str
-        Path under which the plot of the result should be saved.
+    nt = len(t_grid) - 1
+    log_nt = int(np.log10(nt)) + 1
 
-    file_format : str
-        Type of file which the plot of the result should be saved.
+    print('Evaluation of marker orbits for ' + str(species))
+
+    # loop over time grid
+    for n, _ in enumerate(tqdm(t_grid)):
+
+        # create text file for this time step and this species
+        with open(os.path.join(path_orbits, species + '_{0:0{1}d}.txt'.format(n, log_nt)), 'w') as f_out:
+
+            # find markers with right IDs by looping over all hdf5 files and all saved markers
+            for ID in range(n_IDs):
+
+                break_flag = False
+                for m in range(n_IDs):
+                    for file in files:
+                        marker = file['kinetic/' +
+                                      species + '/markers'][n*step, m, :]
+
+                        if marker[-1] == ID:
+
+                            # compute x, y, z coordinates and write to .txt file
+                            X = domain(marker[0], marker[1], marker[2])
+
+                            write_string = '{0:0{1}d}'.format(int(ID), 2)
+                            write_string += ',' + str(X[0])
+                            write_string += ',' + str(X[1])
+                            write_string += ',' + str(X[2])
+
+                            if int(ID) < n_IDs - 1:
+                                write_string += '\n'
+
+                            f_out.write(write_string)
+                            break_flag = True
+                            break
+
+                    if break_flag:
+                        break
+
+    # close hdf5 files
+    for file in files:
+        file.close()
+
+
+def post_process_f(path_in, path_out, species, step=1, marker_type='full_f'):
     """
+    Computes and saves distribution function of saved binning data during a simulation
+    (saved as f_<slice>.npy in a directory "kinetic_data/<name_of_species>/distribution_function/").
 
-    species = str(path.split('/')[-1])
-    path = os.path.join(path, 'distribution_function')
+    Parameters
+    ----------
+    path_in : str
+        Absolute path of simulation output folder.
 
-    # make empty dictionaries
-    f = {'e': None, 'v': None}
-    delta_f = {'e': None, 'v': None}
-    grids = {'e': [], 'v': []}
-
-    # Loop over files and load distribution function data
-    for filename in os.listdir(path):
-        filepath = os.path.join(path, filename)
-
-        # load full distribution functions and compute inds_to_names and names_to_inds
-        if filename[:3] == 'f_e':
-            f['e'] = np.load(filepath)
-            for comp in filename.split('_')[1:]:
-                comp = comp.split('.')[0]
-                grids['e'] += [np.load(os.path.join(path, 'grid_' + comp + '.npy'))]
-        elif filename[:3] == 'f_v':
-            f['v'] = np.load(filepath)
-            for comp in filename.split('_')[1:]:
-                comp = comp.split('.')[0]
-                grids['v'] += [np.load(os.path.join(path, 'grid_' + comp + '.npy'))]
-
-        # load delta f
-        elif filename[:9] == 'delta_f_e':
-            delta_f['e'] = np.load(filepath)
-        elif filename[:9] == 'delta_f_v':
-            delta_f['v'] = np.load(filepath)
-
-    for typ in ['e', 'v']:
-        for k in range(f[typ].ndim - 1):
-
-            f_slicing = [0] * f[typ].ndim
-            f_slicing[k + 1] = slice(None)
-            # plot delta_f
-            if delta_f[typ] is not None:
-                plt.figure('delta_f')
-                plt.plot(grids[typ][k], delta_f[typ][tuple(f_slicing)].squeeze())
-                plt.xlabel(typ + str(k + 1))
-                plt.ylabel(r'$\delta f$')
-                print(f'Created plot for delta_f in {typ + str(k + 1)}')
-
-                if save_plot:
-                    assert savepath is not None, 'When wanting to save the plot a path has to be given!'
-                    savename = os.path.join(savepath, species + '_delta_f_'
-                                            + typ + str(k + 1) + '.' + file_format)
-                    plt.savefig(savename)
-                else:
-                    plt.show()
-                plt.close()
+    path_out : str
+        Absolute path of where to store the .txt files. Will be in path_out/orbits. 
 
-            # plot full f
-            if f[typ] is not None:
-                plt.figure('f')
-                plt.plot(grids[typ][k], f[typ][tuple(f_slicing)].squeeze())
-                plt.xlabel(typ + str(k + 1))
-                plt.ylabel(r'$f$')
-                print(f'Created plot for f in {typ + str(k + 1)}')
-
-                if save_plot:
-                    assert savepath is not None, 'When wanting to save the plot a path has to be given!'
-                    savename = os.path.join(savepath, species + '_f_'
-                                            + typ + str(k + 1) + '.' + file_format)
-                    plt.savefig(savename)
-                else:
-                    plt.show()
-                plt.close()
+    species : str
+        Name of the species for which the post processing should be performed.
+
+    step : int, optional
+        Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc.
+
+    marker_type : str
+        Which type of markers were simulated.
+    """
+
+    # get model name and # of MPI processes from meta.txt file
+    with open(os.path.join(path_in, 'meta.txt'), 'r') as f:
+        lines = f.readlines()
+
+    model = lines[3].split()[-1]
+    nproc = lines[4].split()[-1]
+
+    # load parameters
+    with open(os.path.join(path_in, 'parameters.yml'), 'r') as f:
+        params = yaml.load(f, Loader=yaml.FullLoader)
+
+    # open hdf5 files
+    files = [h5py.File(os.path.join(
+        path_in, 'data/', f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
+
+    # directory for .npy files
+    path_distr = os.path.join(path_out, 'distribution_function')
+
+    try:
+        os.mkdir(path_distr)
+    except:
+        shutil.rmtree(path_distr)
+        os.mkdir(path_distr)
+
+    print('Evaluation of distribution functions for ' + str(species))
+
+    # Create grids
+    for slice_name, dset in tqdm(files[0]['kinetic/' + species + '/f'].items()):
+
+        # create a new folder for each slice
+        path_slice = os.path.join(path_distr, slice_name)
+        os.mkdir(path_slice)
 
+        # Find out all names of slices
+        slice_names = slice_name.split('_')
+
+        # save grid
+        for n_gr, (_, grid) in enumerate(files[0]['kinetic/' + species + '/f/' + slice_name].attrs.items()):
+            grid_path = os.path.join(
+                path_slice, 'grid_' + slice_names[n_gr] + '.npy')
+            np.save(grid_path, grid[:])
+
+    # compute distribution function (and delta f)
+    for k, (slice_name, dset) in enumerate(tqdm(files[0]['kinetic/' + species + '/f'].items())):
+
+        # path to folder of slice
+        path_slice = os.path.join(path_distr, slice_name)
+
+        # Find out all names of slices
+        slice_names = slice_name.split('_')
+
+        # load data
+        data = dset[::step].copy()
+        for rank in range(1, int(nproc)):
+            data += files[rank]['kinetic/' +
+                                species + '/f/' + slice_name][::step]
+
+        assert marker_type in ['full_f', 'control_variate', 'delta_f'], \
+            f'Got unexpected marker type: {marker_type}'
+
+        if marker_type == 'full_f':
+            # save distribution function
+            np.save(os.path.join(path_slice, 'f_binned.npy'), data)
+
+        else:
+            fun_name = params['kinetic'][species]['background']['type']
+            bckgr_params = params['kinetic'][species]['background']
+
+            # Get background function
+            if fun_name in bckgr_params.keys():
+                f_bckgr = getattr(maxwellians, fun_name)(
+                    **bckgr_params[fun_name])
+            else:
+                f_bckgr = getattr(maxwellians, fun_name)()
+
+            # load all grids of the variables of f
+            grid_tot = []
+            for coord in ['e', 'v']:
+                for comp in range(1, 4):
+                    current_slice = coord + str(comp)
+                    filename = os.path.join(
+                        path_slice, 'grid_' + current_slice + '.npy')
+
+                    # check if file exists and is in slice_name
+                    if os.path.exists(filename) and current_slice in slice_names:
+                        grid_tot += [np.load(filename)]
+
+                    # otherwise evaluate at zero 
+                    else:
+                        if coord == 'e':
+                            grid_tot += [np.zeros(1)]
+                        elif coord == 'v':
+                            grid_tot += [np.zeros(1)]
+
+            grid_eval = np.meshgrid(*grid_tot, indexing='ij')
+
+            data_bckgr = f_bckgr(*grid_eval).squeeze()
+
+            if marker_type == 'control_variate':
+                data_delta_f = data
+
+            elif marker_type == 'delta_f':
+
+                # Linearized Vlasov-Maxwell system
+                if model == "LinearVlasovMaxwell":
+                    assert fun_name == 'Maxwellian6DUniform', \
+                        'The linearized Vlasov-Maxwell is only implemented for a uniform Maxwellian background!'
+
+                    # h = f_1 / sqrt{f_0}
+                    data_delta_f = np.multiply(data,
+                                               np.sqrt(data_bckgr[tuple([None])]))  # add extra axis at beginning
+
+                # Vlasov-Maxwell system with Delta-f
+                elif model == "DeltaFVlasovMaxwell":
+                    assert fun_name == 'Maxwellian6DUniform', \
+                        'The Vlasov-Maxwell system with Delta-f is only implemented for a uniform Maxwellian background!'
+
+                    # h = f_0 - (f_0 + f_1) * ln(f_0)
+                    data_delta_f = data_bckgr[tuple([None])] - \
+                        np.multiply(data_bckgr[tuple([None])] + data,
+                                    np.log(data_bckgr[tuple([None])]))
+
+                else:
+                    raise NotImplementedError(
+                        f'Post-processing for the model {model} with {marker_type} has not been implemented yet!')
 
-if __name__ == '__main__':
-    main()
+            # save distribution function
+            np.save(os.path.join(path_slice, 'delta_f_binned.npy'), data_delta_f)
+            np.save(os.path.join(path_slice, 'f_binned.npy'), data_delta_f + data_bckgr)
+
+    # close hdf5 files
+    for file in files:
+        file.close()
```

### Comparing `struphy-2.0.0/src/struphy/diagnostics/paraview/mesh_creator.py` & `struphy-2.0.1/src/struphy/diagnostics/paraview/mesh_creator.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/diagnostics/paraview/vtk_writer.py` & `struphy-2.0.1/src/struphy/diagnostics/paraview/vtk_writer.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/dispersion_relations/analytic.py` & `struphy-2.0.1/src/struphy/dispersion_relations/analytic.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import numpy as np
 from scipy.optimize import fsolve
 
 from struphy.dispersion_relations.base import DispersionRelations1D, ContinuousSpectra1D, Zplasma
+from struphy.fields_background.mhd_equil.equils import set_defaults
 
 
 class Maxwell1D(DispersionRelations1D):
     r"""
     Dispersion relation for Maxwell's equation in vacuum in Struphy units (see ``Maxwell`` in :ref:`models`):
 
     .. math::
 
         \omega^2 = k^2 \,.
     """
 
-    def __init__(self, **params):
+    def __init__(self):
         super().__init__('light wave')
 
     def __call__(self, k):
         """
         The evaluation of all branches of the 1d dispersion relation.
 
         Parameters
         ----------
         k : array_like
             Evaluation wave numbers.
 
         Returns
         -------
         omegas : dict
-            A dictionary with key=branch_name and value=omega(k) (complex ndarray).
+            A dictionary with key=branch_name and value=omega(k) (complex numpy.ndarray).
         """
 
         # One complex array for each branch
         tmps = []
         for n in range(self.nbranches):
             tmps += [np.zeros_like(k, dtype=complex)]
 
@@ -56,44 +57,75 @@
     .. math::
 
         \textnormal{shear Alfvén}:\quad &\omega^2 = c_\textnormal{A}^2 k^2\frac{B_{0z}^2}{|\mathbf B_0|^2}\,,
 
         \textnormal{fast (+) and slow (-) magnetosonic}:\quad &\omega^2 =\frac{1}{2}(c_\textnormal{S}^2+c_\textnormal{A}^2)k^2(1\pm\sqrt{1-\delta}\,)\,,\quad\delta=\frac{4B_{0z}^2c_\textnormal{S}^2c_\textnormal{A}^2}{(c_\textnormal{S}^2+c_\textnormal{A}^2)^2|\mathbf B_0|^2}\,,
 
     where :math:`c_\textnormal{A}^2=|\mathbf B_0|^2/n_0` is the Alfvén velocity and :math:`c_\textnormal{S}^2=\gamma\,p_0/n_0` is the speed of sound.
+
+    Parameters
+    ----------
+    **params
+        Keyword arguments that characterize the dispersion relation.
+            * B0x : float  
+                x-component of magnetic field (default: 0.).
+            * B0y : float  
+                y-component of magnetic field (default: 0.).
+            * B0z : float  
+                z-component of magnetic field (default: 1.).
+            * p0 : float
+                Plasma pressure (default: 0.5).
+            * n0 : float 
+                Ion number density (default: 1.).
+            * gamma : float 
+                Adiabatic index (default: 5/3).
     """
 
     def __init__(self, **params):
-        super().__init__('shear Alfvén', 'slow magnetosonic', 'fast magnetosonic', **params)
+
+        # set default parameters
+        params_default = {'B0x': 0.,
+                          'B0y': 0.,
+                          'B0z': 1.,
+                          'p0': 0.5,
+                          'n0': 1.0,
+                          'gamma': 5/3}
+
+        params_all = set_defaults(params, params_default)
+
+        super().__init__('shear Alfvén', 'slow magnetosonic',
+                         'fast magnetosonic', **params_all)
 
     def __call__(self, k):
         """
         The evaluation of all branches of the 1d dispersion relation.
 
         Parameters
         ----------
         k : array_like
             Evaluation wave numbers.
 
         Returns
         -------
         omegas : dict
-            A dictionary with key=branch_name and value=omega(k) (complex ndarray).
+            A dictionary with key=branch_name and value=omega(k) (complex numpy.ndarray).
         """
 
         # One complex array for each branch
         tmps = []
         for n in range(self.nbranches):
             tmps += [np.zeros_like(k, dtype=complex)]
 
         ########### Model specific part ##############################
 
         # Alfvén velocity and speed of sound
-        cA = np.sqrt((self.params['B0x']**2 + self.params['B0y']
-                     ** 2 + self.params['B0z']**2)/self.params['n0'])
+        cA = np.sqrt((self.params['B0x']**2 +
+                      self.params['B0y']**2 +
+                      self.params['B0z']**2)/self.params['n0'])
+
         cS = np.sqrt(self.params['gamma']*self.params['p0']/self.params['n0'])
 
         # shear Alfvén branch
         tmps[0][:] = cA * k * self.params['B0z'] / \
             np.sqrt(self.params['B0x']**2 +
                     self.params['B0y']**2 + self.params['B0z']**2)
 
@@ -125,15 +157,16 @@
 
         \textnormal{fast (+) and slow (-) magnetosonic}:\quad &\omega^2 =\frac{1}{2}(c_\textnormal{S}^2+c_\textnormal{A}^2)k^2(1\pm\sqrt{1-\delta}\,)\,,\quad\delta=\frac{4B_{0z}^2c_\textnormal{S}^2c_\textnormal{A}^2}{(c_\textnormal{S}^2+c_\textnormal{A}^2)^2|\mathbf B_0|^2}\,,
 
     where :math:`c_\textnormal{A}^2=|\mathbf B_0|^2/n_0` is the Alfvén velocity and :math:`c_\textnormal{S}^2=\gamma\,p_0/n_0` is the speed of sound.
     """
 
     def __init__(self, **params):
-        super().__init__('fast magnetosonic', 'slow magnetosonic','compression Alfvén','shear Alfvén', **params)
+        super().__init__('fast magnetosonic', 'slow magnetosonic',
+                         'compression Alfvén', 'shear Alfvén', **params)
 
     def __call__(self, k):
         """
         The evaluation of all branches of the 1d dispersion relation.
 
         Parameters
         ----------
@@ -149,161 +182,179 @@
         # One complex array for each branch
         tmps = []
         for n in range(self.nbranches):
             tmps += [np.zeros_like(k, dtype=complex)]
 
         ########### Model specific part ##############################
 
-        #Quantities related with backgorund magnetic field
+        # Quantities related with backgorund magnetic field
         B0x = self.params['B0x']
         B0y = self.params['B0y']
         B0z = self.params['B0z']
         B0n = np.sqrt(B0x**2.0 + B0y**2.0 + B0z**2.0)
-        
-        #Cos(theta)
+
+        # Cos(theta)
         cos = B0z/B0n
-        
-        #Background number density
+
+        # Background number density
         n0 = self.params['n0']
-        
-        #Background pressures
+
+        # Background pressures
         pi0 = self.params['p0']
         pe0 = self.params['p0']
         gamma = self.params['gamma']
-        
-        #Basic units of magnetic field and time
+
+        # Basic units of magnetic field and time
         Bu = self.params['Bu']
         tu = self.params['tu']
-        
+
         # compute coupling parameter kappa
         ee = 1.602176634e-19  # elementary charge (C)
         mH = 1.67262192369e-27  # proton mass (kg)
         Ab = self.params['A']
         Zb = self.params['Z']
-        
+
         omega_ch = (Zb*ee*Bu)/(Ab*mH)
         kappa = omega_ch*tu/(2.0 * np.pi)
 
         if abs(kappa - 1) < 1e-6:
             kappa = 1.
-        
-        # Alfvén velocity 
+
+        # Alfvén velocity
         cA = B0n/np.sqrt(n0)
-        
-        #We will need some auxiliary arrays to compute the las three waves
+
+        # We will need some auxiliary arrays to compute the las three waves
         bs = np.zeros_like(k, dtype=complex)
-        bs[:] = - k**2.0 *(cA**2.0)*(cos**2.0*(1.0+ k**2.0 * kappa**2.0/n0) + 1.0 + (gamma/B0n**2.0)*(pi0+pe0) )
+        bs[:] = - k**2.0 * (cA**2.0)*(cos**2.0*(1.0 + k**2.0 *
+                                                kappa**2.0/n0) + 1.0 + (gamma/B0n**2.0)*(pi0+pe0))
 
         cs = np.zeros_like(k, dtype=complex)
-        cs[:] = k**4.0 * cos**2.0 * cA**4.0 * (1.0 + (pi0+pe0)*(gamma/B0n**2.0)*(2.0 + k**2.0 * kappa**2.0 / n0) )
+        cs[:] = k**4.0 * cos**2.0 * cA**4.0 * \
+            (1.0 + (pi0+pe0)*(gamma/B0n**2.0)*(2.0 + k**2.0 * kappa**2.0 / n0))
 
         ds = np.zeros_like(k, dtype=complex)
         ds[:] = -k**6.0 * (B0n**4.0 / n0**3.0) * gamma * (pi0 + pe0) * cos**4.0
 
         D0s = np.zeros_like(k, dtype=complex)
         D0s[:] = bs**2.0 - 3.0*cs
 
         D1s = np.zeros_like(k, dtype=complex)
-        D1s[:] = 2.0* bs**3.0 - 9.0*bs*cs + 27.0*ds
+        D1s[:] = 2.0 * bs**3.0 - 9.0*bs*cs + 27.0*ds
 
         Ccs = np.zeros_like(k, dtype=complex)
-        Ccs[:] = ( (D1s + (D1s**2.0 - 4.0*D0s**3.0 )**(1.0/2.0) )/2.0 )**(1.0/3.0)
+        Ccs[:] = ((D1s + (D1s**2.0 - 4.0*D0s**3.0)**(1.0/2.0))/2.0)**(1.0/3.0)
 
-        #Finally we need a special complex number
+        # Finally we need a special complex number
         SHI = (-1.0 + (-3.0)**(1.0/2.0))*0.5
-        
+
         # fast magnetosonic branch
-        tmps[0][:] = (B0n*kappa*cos/n0)*k**2.0 
-        
+        tmps[0][:] = (B0n*kappa*cos/n0)*k**2.0
+
         # slow magnetosonic
-        tmps[1][:] = ( (-1.0/3.0)*(bs + Ccs + D0s/Ccs) )**(1.0/2.0) 
-        
+        tmps[1][:] = ((-1.0/3.0)*(bs + Ccs + D0s/Ccs))**(1.0/2.0)
+
         # compression Alfvén branch
-        tmps[2][:] = ( (-1.0/3.0)*(bs + SHI*Ccs + D0s/(SHI*Ccs) ) )**(1.0/2.0) 
-        
+        tmps[2][:] = ((-1.0/3.0)*(bs + SHI*Ccs + D0s/(SHI*Ccs)))**(1.0/2.0)
+
         # shear Alfvén branch
-        tmps[3][:] = ( (-1.0/3.0)*(bs + SHI*SHI*Ccs + D0s/(SHI*SHI*Ccs) ) )**(1.0/2.0)
+        tmps[3][:] = ((-1.0/3.0)*(bs + SHI*SHI*Ccs +
+                      D0s/(SHI*SHI*Ccs)))**(1.0/2.0)
 
         ##############################################################
 
         # fill output dictionary
         omegas = {}
         for name, tmp in zip(self.branches, tmps):
             omegas[name] = tmp
 
         return omegas
 
 
 class ColdPlasma1D(DispersionRelations1D):
-    r'''Dispersion relation for cold plasma model :math:`(\alpha,\mathbf B_0)`
+    r'''Dispersion relation for cold plasma model for homogeneous background :math:`(n_0,\mathbf B_0)`
     and wave propagation along z-axis :math:`(\mathbf k = k \mathbf e_z)` in Struphy units
     (see ``ColdPlasma`` in :ref:`models`):
-    
+
     .. math::
-    
-        \left[ \left( \omega^2 - |k|^2 \right) \mathbb I + \mathbf k \otimes \mathbf k + i \omega \alpha \sigma_c \right] \mathbf E = 0\,,
 
-    where :math:`\left( \omega^2 - |k|^2 \right) \mathbb I + \mathbf k \otimes \mathbf k + i \omega \alpha \sigma_c = \varepsilon`
-    is the dielectric tensor, :math:`\alpha` is the plasma frequency in units of the electron cyclotron frequency
-    and :math:`\sigma_c = \left( \mathbb I - i Q / \omega \right)^{-1} i \alpha / \omega`,
+        \left[ \left( \omega^2 - |k|^2 \right) \mathbb I + \mathbf k \otimes \mathbf k + i \frac{\omega \alpha}{\varepsilon_c} \sigma_c \right] \mathbf E = 0\,,
+
+    where :math:`\left( \omega^2 - |k|^2 \right) \mathbb I + \mathbf k \otimes \mathbf k + i \frac{\omega \alpha}{\varepsilon_c} \sigma_c = \epsilon`
+    is the dielectric tensor, :math:`\alpha` is the plasma frequency in units of the electron cyclotron frequency, 
+    :math:`1/\varepsilon_c` is the electron cyclotron frequency in struphy units,
+    and :math:`\sigma_c = \left( \mathbb I - i Q / \varepsilon_c \omega \right)^{-1} i \alpha n_0 / \varepsilon_c \omega`,
     with :math:`Q` being an operator which, if applied to vector :math:`\mathbf v`, returns :math:`\mathbf v \times \mathbf B_0`.
     '''
 
     def __init__(self, **params):
-        super().__init__('ion-cyclotron wave', 'electron-cyclotron wave', 'L-wave', 'R-wave', **params)
 
-    def __call__(self, kvec, kperp=None):
-        
+        # set default parameters
+        params_default = {'B0x': 0.,
+                          'B0y': 0.,
+                          'B0z': 1.,
+                          'n0': 1.,
+                          'alpha': 1.,
+                          'epsilon': 1.}
+
+        params_all = set_defaults(params, params_default)
+
+        super().__init__('ion-cyclotron wave',
+                         'electron-cyclotron wave', 'L-wave', 'R-wave', **params)
+
+    def __call__(self, kvec):
+
         # One complex array for each branch
         tmps = []
         for n in range(self.nbranches):
             tmps += [np.zeros_like(kvec, dtype=complex)]
 
         ########### Model specific part ##############################
 
-        # squared B modulus
-        B2 = self.params['B0x']**2 + self.params['B0y']**2 + self.params['B0z']**2
-        # squared Bz modulus
-        Bz2 = self.params['B0z']**2
-        # squared k modulus
-        k2vec = kvec**2
-        # alpha squared
+        # angle between k and magnetic field
+        if self.params['B0z'] == 0:
+            theta = np.pi/2
+        else:
+            theta = np.arctan(
+                np.sqrt(self.params['B0x']**2 + self.params['B0y']**2) / self.params['B0z'])
+        print(theta)
+        cos2 = np.cos(theta)**2
+
+        neq = self.params['n0']
+
+        # powers of parameters
+        B2 = self.params['B0x']**2 + \
+            self.params['B0y']**2 + self.params['B0z']**2
         alpha2 = self.params['alpha']**2
+        alpha4 = self.params['alpha']**4
+        alpha6 = self.params['alpha']**6
+        eps2 = self.params['epsilon']**2
+        eps4 = self.params['epsilon']**4
+        eps6 = self.params['epsilon']**6
+        k2vec = kvec**2
 
         for n, k2 in enumerate(k2vec):
             # polynomial coefficients in order of increasing degree
             # 0th degree
-            a = - k2**2 * Bz2 * alpha2
-            # 1st degree
-            b = 0
-            # 2nd degree
-            c = k2**2 * B2 + k2**2 * alpha2 + k2 * B2 * alpha2 + k2 * Bz2 * alpha2 + alpha2**3
-            # 3rd degree
-            d = 0
-            # 4th degree
-            e = -1 * (k2**2 + 2 * k2 * B2 + 4 * alpha2 * k2 + alpha2 * B2 + 3 * alpha2**2)
-            # 5th degree
-            f = 0
-            # 6th degree
-            g = B2 + 3 * alpha2
-            # 7th degree
-            h = 0
-            # 8th degree
-            i = -1 
-
-            # R-wave cut frequency in terms of the electron-cyclotron one
-            Rcut = 0.5 * (np.sqrt(1 + 4 * alpha2) + 1)
+            a = B2*k2**2*neq*alpha2*eps2*cos2
+            # 1st degree in omega^2
+            b = -neq**3 * alpha6 - B2*k2*neq*alpha2*eps2 - 2*k2*neq**2*alpha4*eps2 - \
+                B2*k2*neq*alpha2*eps2*cos2 - B2*k2**2*eps4 - k2**2*neq*alpha2*eps4
+            # 2nc degree in omega^2
+            c = B2*neq*alpha2*eps2 + 3*neq**2*alpha4*eps2 + 2 * \
+                B2*k2*eps4 + 4*k2*neq*alpha2*eps4 + k2**2*eps6
+            # 3rd degree in omega^2
+            d = -B2*eps4 - 3*neq*alpha2*eps4 - 2*k2*eps6
+            # 4th degree in omega^2
+            e = eps6
 
             # determinant in polynomial form
-            det = np.polynomial.Polynomial([a, b, c, d, e, f, g, h, i], domain=[0, 10 * Rcut])
+            det = np.polynomial.Polynomial([a, b, c, d, e])
 
             # solutions
-            sol = det.roots()
-            # we want only positive omegas
-            sol = sol[sol >= 0]
+            sol = np.sqrt(np.abs(det.roots()))
             # Ion-cyclotron branch
             tmps[0][n] = sol[0]
             # Electron-cyclotron branch
             tmps[1][n] = sol[1]
             # L-branch
             tmps[2][n] = sol[2]
             # R- branch
@@ -313,15 +364,15 @@
 
         # fill output dictionary
         dict_disp = {}
         for name, tmp in zip(self.branches, tmps):
             dict_disp[name] = tmp
 
         return dict_disp
-    
+
 
 class CurrentCoupling6DParallel(DispersionRelations1D):
     r"""
     Dispersion relation for linearized hybrid MHD-Vlasov model (current coupling scheme) in Struphy units for homogeneous background :math:`(n_0=1,p_0,\mathbf B_0=B_0\mathbf e_z)`, wave propagation along z-axis and EP distribution function
 
     .. math::
 
@@ -336,27 +387,67 @@
     and standard sound waves
 
     .. math::
 
         \omega^2=\gamma p_0 k^2\,,
 
     where :math:`\xi^\pm=(\omega-kv_0\pm Z_\textnormal{h}B_0\kappa/A_\textnormal{h})/kv_\textnormal{th}` and :math:`Z(\xi)=\sqrt{\pi}\exp(-\xi^2)[i-\textnormal{erfi}(\xi)]` is the plasma dispersion function.
+
+    Parameters
+    ----------
+    **params
+        Keyword arguments that characterize the dispersion relation.
+            * B0 : float  
+                Magnetic field strength (default: 1.).
+            * p0 : float
+                Plasma pressure (default: 0.5).
+            * gamma : float 
+                Adiabatic index (default: 5/3).
+            * Ab : int 
+                Bulk species mass number (default: 1).
+            * Ah : int 
+                Energetic species mass number (default: 1).
+            * Zh : int 
+                Energetic species charge number (default: 1).
+            * vth : float 
+                Energetic species thermal velocity (default: 1.).
+            * v0 : float 
+                Energetic species shift of Maxwellian (default: 2.).
+            * nuh : float 
+                Ratio of energetic/bulk number densities (default: 0.5).
+            * nb : float
+                Bulk species number density in units of 1e20 / m^3 (default: 0.0005185219355).
     """
 
     def __init__(self, **params):
-        super().__init__('shear_Alfvén_R', 'shear_Alfvén_L', 'sound', **params)
+
+        # set default parameters
+        params_default = {'B0': 1.,
+                          'p0': 0.5,
+                          'gamma': 5/3,
+                          'Ab': 1,
+                          'Ah': 1,
+                          'Zh': 1,
+                          'vth': 1.,
+                          'v0': 2.,
+                          'nuh': 0.05,
+                          'nb': 0.0005185219355}
+
+        params_all = set_defaults(params, params_default)
+
+        super().__init__('shear_Alfvén_R', 'shear_Alfvén_L', 'sound', **params_all)
 
         # some constants
         mp = 1.672621924e-27
         mu = 1.256637062e-6
         ee = 1.602176634e-19
 
         # calculate coupling parameter alpha_c from bulk number density and mass number
         self._kappa = ee * \
-            np.sqrt(mu*self.params['Ab']*self.params['nb']*1e19/mp)
+            np.sqrt(mu*self.params['Ab']*self.params['nb']*1e20/mp)
 
     def __call__(self, k, method='newton', tol=1e-10, max_it=100):
         """
         Solves the dispersion relation for given wave numbers.
 
         Parameters
         ----------
@@ -371,15 +462,15 @@
 
         max_it : int, optional
             Maximum number of iterations in case of Newton solver.
 
         Returns
         -------
         omegas : dict
-            A dictionary with key=branch_name and value=omega(k) (complex ndarray).
+            A dictionary with key=branch_name and value=omega(k) (complex numpy.ndarray).
         """
 
         # One complex array for each branch
         tmps = []
         for _ in range(self.nbranches):
             tmps += [np.zeros_like(k, dtype=complex)]
 
@@ -517,15 +608,15 @@
             out += nuh*Zh**2*B0**2 / \
                 (Ah*Ab)*self._kappa**2/(k*vth) * \
                 (Zplasma(xi, 0) + (w - k*v0)*Zplasma(xi, 1)*xip)
 
         return np.real(out), np.imag(out)
 
 
-class PC_LinMHD_6d_full1D(DispersionRelations1D):
+class PressureCouplingFull6DParallel(DispersionRelations1D):
     r'''Dispersion relation for linear MHD equations coupled to the Vlasov equation with Full Pressure Coupling scheme
     for homogeneous background :math:`(n_0,p_0,\mathbf B_0)`, wave propagation along z-axis in Struphy units and space-homogeneous shifted Maxwellian energetic particles distribution :math:`f_h = f_{h,0} + \tilde{f_h}` 
     where :math:`f_{h,0}(v_{\parallel}, v_{\perp}) = n_0 \frac{1}{\sqrt{\pi}} \frac{1}{\hat{v_{\parallel}}} e^{- (v_{\parallel} - u_0)^2 / \hat{v}^2_{\parallel} } \frac{1}{\pi} \frac{1}{\hat{v^2_{\perp}}} e^{- v^2_{\perp} / \hat{v}^2_{\perp}}`
     here, :math:`u_0` is a velocity shift in the parallel direction (see ``PC_LinMHD_6d_full`` in :ref:`models`):
 
     :math:`\textnormal{shear Alfvén (R) and (L) wave}` :
 
@@ -798,30 +889,61 @@
     The continuous spectra are then given by
 
     .. math::
 
         \textnormal{shear Alfvén}:\quad & \omega^2(x)=\frac{B_{0z}(x)^2}{n_0(x)}\frac{1}{R_0^2}\left(n+\frac{m}{q(x)}\right)^2\,
 
         \textnormal{slow sound}:\quad & \omega^2(x)=\frac{\gamma p_0(x)B_{0z}(x)^2}{n_0(x)\,[\gamma p_0(x) + B_{0y}(x)^2 + B_{0z}(x)^2]}\frac{1}{R_0^2}\left(n+\frac{m}{q(x)}\right)^2\,.
+
+    Parameters
+    ----------
+    **params
+        Keyword arguments that characterize the dispersion relation.
+            * a : float 
+                "Minor" radius (must be compatible with :math:`L_x=a` and :math:`L_y=2\pi a`, default: 1.).
+            * R0 : float
+                "Major" radius (must be compatible with :math:`L_z=2\pi R_0`, default: 3.).
+            * gamma : float 
+                Adiabatic index (default: 5/3).
+            * Bz : callable
+                Profile of axial magnetic field Bz=Bz(x) (default: 1. - 0*x).
+            * p : callable
+                Pressure profile p=p(x) (default: 0.5 - 0*x).
+            * rho : callable
+                Profile of mass density rho=rho(x) (default: 1. - 0*x).
+            * q : callable
+                Safety factor profile q=q(x) (default: 1.1 + 0.7*x**2).
     """
 
     def __init__(self, **params):
-        super().__init__('shear_Alfvén', 'slow_sound', **params)
+
+        # set default parameters
+        params_default = {'a': 1.,
+                          'R0': 3.,
+                          'gamma': 5/3,
+                          'Bz': lambda x: 1. - 0*x,
+                          'p': lambda x: 0.5 - 0*x,
+                          'rho': lambda x: 1. - 0*x,
+                          'q': lambda x: 1.1 + 0.7*x**2}
+
+        params_all = set_defaults(params, params_default)
+
+        super().__init__('shear_Alfvén', 'slow_sound', **params_all)
 
     def __call__(self, x, m, n):
         """ 
         The calculation of all continuous spectra.
 
         Parameters
         ----------
         x : array_like
             The x points at which the continuous spectra shall be evaluated.
 
         m, n : int
-            Mode numbers in y- and z-direction.
+            Mode numbers in y- (m) and z- (n) direction.
 
         Returns
         -------
         specs : dict
             A dictionary with key=branch_name and value=omega(x) (ndarray).
         """
 
@@ -877,30 +999,58 @@
     The continuous spectra are then given by
 
     .. math::
 
         \textnormal{shear Alfvén}:\quad & \omega^2(r)=\frac{B_{0z}(r)^2}{n_0(r)}\frac{1}{R_0^2}\left(n+\frac{m}{q(r)}\right)^2\,
 
         \textnormal{slow sound}:\quad & \omega^2(r)=\frac{\gamma p_0(r)B_{0z}(r)^2}{n_0(r)\,[\gamma p_0(r) + B_{0\theta}(r)^2 + B_{0z}(r)^2]}\frac{1}{R_0^2}\left(n+\frac{m}{q(r)}\right)^2\,.
+
+    Parameters
+    ----------
+    **params
+        Keyword arguments that characterize the dispersion relation.
+            * R0 : float
+                "Major" radius (must be compatible with :math:`L_z=2\pi R_0`, default: 3.).
+            * gamma : float 
+                Adiabatic index (default: 5/3).
+            * Bz : callable
+                Profile of axial magnetic field Bz=Bz(x) (default: 1. - 0*r).
+            * p : callable
+                Pressure profile p=p(x) (default: 0.5 - 0*r).
+            * rho : callable
+                Profile of mass density rho=rho(x) (default: 1. - 0*r).
+            * q : callable
+                Safety factor profile q=q(x) (default: 1.1 + 0.7*r**2).
     """
 
     def __init__(self, **params):
-        super().__init__('shear_Alfvén', 'slow_sound', **params)
+
+        # set default parameters
+        params_default = {'R0': 3.,
+                          'gamma': 5/3,
+                          'Bz': lambda r: 1. - 0*r,
+                          'p': lambda r: 0.5 - 0*r,
+                          'rho': lambda r: 1. - 0*r,
+                          'q': lambda r: 1.1 + 0.7*r**2}
+
+        params_all = set_defaults(params, params_default)
+
+        super().__init__('shear_Alfvén', 'slow_sound', **params_all)
 
     def __call__(self, r, m, n):
         """ 
         The evaluation of all continuous spectra.
 
         Parameters
         ----------
         r : array_like
             The radial points at which the continuous spectra shall be evaluated.
 
         m, n : int
-            Mode numbers in theta- and z-direction.
+            Mode numbers in theta- (m) and z- (n) direction.
 
         Returns
         -------
         specs : dict
             A dictionary with key=branch_name and value=omega(r) (ndarray).
         """
```

### Comparing `struphy-2.0.0/src/struphy/dispersion_relations/base.py` & `struphy-2.0.1/src/struphy/dispersion_relations/base.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/derivatives.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/derivatives.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_2d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_3d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/emw_operators.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/emw_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_1d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_2d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_3d.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mass_matrices_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,26 +175,26 @@
     parser.add_argument('n_tor', 
                         type=int, 
                         help='the toroidal mode number')
     
     parser.add_argument('-i', '--input',
                         type=str,
                         metavar='FILE',
-                        help='parameter file (.yml) relative to <install_path>/struphy/io/inp/ (default=parameters.yml)',
+                        help='parameter file (.yml) in current I/O path (default=parameters.yml)',
                         default='parameters.yml')
 
     parser.add_argument('--input-abs',
                         type=str,
                         metavar='FILE',
                         help='parameter file (.yml), absolute path')
 
     parser.add_argument('-o', '--output',
                         type=str,
                         metavar='DIR',
-                        help='output directory relative to <install_path>/struphy/io/out/ (default=sim_1)',
+                        help='output directory relative to current I/O path (default=sim_1)',
                         default='sim_1')
 
     parser.add_argument('--output-abs',
                         type=str,
                         metavar='DIR',
                         help='output directory, absolute path')    
 
@@ -227,15 +227,15 @@
         shutil.copy2(input_abs, os.path.join(output_abs, 'parameters.yml'))
     
     # load parameter file
     with open(input_abs) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
         
     # create domain and MHD equilibrium
-    from struphy.models.utilities import setup_domain_mhd
+    from struphy.models.setup import setup_domain_mhd
     
     domain, mhd_equil = setup_domain_mhd(params)
        
     # load grid parameters
     num_params = {'Nel'     : params['grid']['Nel'][:2],
                   'p'       : params['grid']['p'][:2],
                   'spl_kind': params['grid']['spl_kind'][:2],
```

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                         type=int, 
                         help='toroidal mode number',
                         required=True)
     
     parser.add_argument('-i', '--input',
                         type=str,
                         metavar='DIR',
-                        help='directory with eigenspectrum (.npy), relative to <install_path>/struphy/io/out/ (default=sim_1)',
+                        help='directory with eigenspectrum (.npy), relative to current I/O path (default=sim_1)',
                         default='sim_1')
 
     parser.add_argument('--input-abs',
                         type=str,
                         metavar='DIR',
                         help='directory with eigenspectrum (.npy) file, absolute path')
```

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators_core.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/mhd_operators_core.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/projectors_global.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/eigenvalue_solvers/spline_space.py` & `struphy-2.0.1/src/struphy/eigenvalue_solvers/spline_space.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/examples/TAE_tokamak.py` & `struphy-2.0.1/src/struphy/examples/TAE_tokamak.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,25 @@
         io_path = f.readlines()[0]
 
     # name of simulation output folder
     out_name = 'sim_example_TAE_tokamak'
     
     # run MHD eigenvalue solver
     subprocess.run(['python3',
-                    'eigenvalue_solvers/mhd_axisymmetric_main.py',
+                    os.path.join(libpath, 'eigenvalue_solvers/mhd_axisymmetric_main.py'),
                     '-1',
-                    '-i'
-                    'examples/params_TAE_tokamak.yml',
-                    '-o'
-                    'sim_example_TAE_tokamak'], 
-                    check=True, cwd=libpath)
+                    '--input-abs',
+                    os.path.join(libpath, 'io/inp/examples/params_TAE_tokamak.yml'),
+                    '-o',
+                    out_name], 
+                    check=True)
     
     # make the .npy eigenspectrum smaller (just for testing)
     subprocess.run(['python3',
-                    'eigenvalue_solvers/mhd_axisymmetric_pproc.py',
+                    os.path.join(libpath, 'eigenvalue_solvers/mhd_axisymmetric_pproc.py'),
                     '-n',
                     '-1',
                     '-i',
                     out_name,
                     '0.1',
                     '0.2'], 
                     check=True, cwd=libpath)
@@ -69,15 +69,15 @@
     """
     
     import os, yaml, h5py, pickle
     
     import numpy as np
     import matplotlib.pyplot as plt
 
-    from struphy.models.utilities import setup_domain_mhd
+    from struphy.models.setup import setup_domain_mhd
     from struphy.diagnostics.continuous_spectra import get_mhd_continua_2d
     from struphy.dispersion_relations.analytic import MhdContinousSpectraCylinder
     from struphy.eigenvalue_solvers.spline_space import Spline_space_1d, Tensor_spline_space
     
     import struphy
 
     libpath = struphy.__path__[0]
```

### Comparing `struphy-2.0.0/src/struphy/examples/_draw_parallel.py` & `struphy-2.0.1/src/struphy/examples/_draw_parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     loading_type = 'pseudo_random'
     loading_params = {'type': loading_type, 'seed': 1234,
                       'moments': [0., 0., 0., 1., 1., 1.]}
 
     marker_params = {'ppc': 10, 'eps': .25, 'loading': loading_params}
 
     # create domain
-    dom_type = 'HollowTorusStraightFieldLine'
+    dom_type = 'HollowTorus'
     domain_class = getattr(domains, dom_type)
-    domain = domain_class()
+    domain = domain_class(sfl=True)
 
     # create de rham object
     derham = Derham(Nel, p, spl_kind, comm=comm)
 
     if rank == 0:
         print()
         print('Domain decomposition according to : ')
```

### Comparing `struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_cylinder.py` & `struphy-2.0.1/src/struphy/examples/_mhd_eigenvalues_cylinder.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_slab.py` & `struphy-2.0.1/src/struphy/examples/_mhd_eigenvalues_slab.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/examples/_sendrecv.py` & `struphy-2.0.1/src/struphy/examples/_sendrecv.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/examples/gc_orbits_tokamak.py` & `struphy-2.0.1/src/struphy/examples/gc_orbits_tokamak.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_gc_orbits_tokamak'  
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
                     'DriftKinetic',
                     '-i',
-                    'examples/params_gc_orbits_tokamak.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_gc_orbits_tokamak.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -38,15 +41,15 @@
     
     import os, yaml, h5py
     from tqdm import tqdm
     
     import numpy as np
     import matplotlib.pyplot as plt
     
-    from struphy.models.utilities import setup_domain_mhd
+    from struphy.models.setup import setup_domain_mhd
     from struphy.fields_background.mhd_equil.equils import EQDSKequilibrium
     
     import struphy
     libpath = struphy.__path__[0]
     
     with open(os.path.join(libpath, 'io_path.txt')) as f:
         io_path = f.readlines()[0]
```

### Comparing `struphy-2.0.0/src/struphy/examples/linearextendedmhd.py` & `struphy-2.0.1/src/struphy/examples/linearextendedmhd.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_linearextendedmhd'
     
     # run the model (could also call main() directly, but to enable parallel runs, use Struphy's command line interface)
     subprocess.run(['struphy', 
                     'run', 
                     'LinearExtendedMHD',
                     '-i',
-                    'examples/params_linearextendedmhd.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_linearextendedmhd.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -40,16 +43,19 @@
     
     from struphy.diagnostics.diagn_tools import fourier_1d
     
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     out_name = 'sim_example_linearextendedmhd'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    out_path = os.path.join(io_path, 'io/out', out_name)
     
     # read in parameters for analytical dispersion relation
     with open(os.path.join(out_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     
     # parameters for dispersion relation
@@ -61,15 +67,15 @@
     nu = params['units']['n']
     mH = 1.67262192369e-27  # proton mass (kg)
     MU = 1.25663706212e-6 #vacuum permeability (N / A^2)
     A = params['fluid']['mhd']['phys_params']['A']
     Z = params['fluid']['mhd']['phys_params']['Z']
     tu= (xu/Bu) * (MU*mH*A*nu)**(0.5) *(10.0**10.0)
     p0 = (2*params['mhd_equilibrium']['HomogenSlab']
-          ['beta']/100)/(B0x**2 + B0y**2 + B0z**2)
+          ['beta'])/(B0x**2 + B0y**2 + B0z**2)
     n0 = params['mhd_equilibrium']['HomogenSlab']['n0']
 
     disp_params = {'B0x': B0x, 
                    'B0y': B0y,
                    'B0z': B0z, 
                    'p0': p0, 
                    'n0': n0,
```

### Comparing `struphy-2.0.0/src/struphy/examples/linearmhd.py` & `struphy-2.0.1/src/struphy/examples/linearmhd.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_linearmhd'
     
     # run the model (could also call main() directly, but to enable parallel runs, use Struphy's command line interface)
     subprocess.run(['struphy', 
                     'run', 
                     'LinearMHD',
                     '-i',
-                    'examples/params_linearmhd.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_linearmhd.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -56,15 +59,15 @@
 
     # parameters for dispersion relation
     B0x = params['mhd_equilibrium']['HomogenSlab']['B0x']
     B0y = params['mhd_equilibrium']['HomogenSlab']['B0y']
     B0z = params['mhd_equilibrium']['HomogenSlab']['B0z']
 
     p0 = (2*params['mhd_equilibrium']['HomogenSlab']
-          ['beta']/100)/(B0x**2 + B0y**2 + B0z**2)
+          ['beta'])/(B0x**2 + B0y**2 + B0z**2)
     n0 = params['mhd_equilibrium']['HomogenSlab']['n0']
 
     disp_params = {'B0x': B0x, 
                    'B0y': B0y,
                    'B0z': B0z, 
                    'p0': p0, 
                    'n0': n0,
```

### Comparing `struphy-2.0.0/src/struphy/examples/linearmhdvlasov_cc.py` & `struphy-2.0.1/src/struphy/examples/linearmhdvlasov_cc.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_linearmhdvlasovcc'
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
                     'LinearMHDVlasovCC',
                     '-i',
-                    'examples/params_hybridmhdvlasovcc.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_hybridmhdvlasovcc.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -93,15 +96,15 @@
     plt.text(15, 2.5e-2, 'analytical growth')
     plt.arrow(51, 2.8e-2, 7., 0., head_width=.01, head_length=.5000)
     plt.text(15, 2e-3, 'linear phase')
     plt.text(80, 1e-4, 'nonlinear phase')
 
     plt.subplot(1, 2, 2)
     plt.plot(vz, f[0], label='$t=0$')
-    plt.plot(vz, f[100], label='$t=60$')
+    plt.plot(vz, f[300], label='$t=60$')
     plt.xlabel('$v_z$')
     plt.ylabel('$f_{v_z}$')
     plt.title('EP distribution function')
     plt.text(3.5, 0.03, 'resonance velocity')
     plt.arrow(3.3, 0.03, -0.5, 0., head_width=.002, head_length=.15)
     plt.legend(loc='upper left')
```

### Comparing `struphy-2.0.0/src/struphy/examples/linearmhdvlasov_pc.py` & `struphy-2.0.1/src/struphy/examples/linearmhdvlasov_pc.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_linearmhdvlasovpc'
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
                     'LinearMHDVlasovPC',
                     '-i',
-                    'examples/params_hybridmhdvlasovpc.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_hybridmhdvlasovpc.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
```

### Comparing `struphy-2.0.0/src/struphy/examples/maxwell.py` & `struphy-2.0.1/src/struphy/examples/maxwell.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
        
     # name of simulation output folder
     out_name = 'sim_example_maxwell'
     
     # run the model (could also call main() directly, but to enable parallel runs, use Struphy's command line interface)
     subprocess.run(['struphy', 
                     'run', 
                     'Maxwell',
-                    '-i',
-                    'examples/params_maxwell.yml',
+                    '--input-abs',
+                    os.path.join(libpath, 'io/inp/examples/params_maxwell.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
```

### Comparing `struphy-2.0.0/src/struphy/examples/orbits_tokamak.py` & `struphy-2.0.1/src/struphy/examples/orbits_tokamak.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,28 @@
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
-    import subprocess
+    import os, subprocess
+    import struphy
+    
+    libpath = struphy.__path__[0]
     
     # name of simulation output folder
     out_name = 'sim_example_orbits_tokamak' 
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
                     'Vlasov',
                     '-i',
-                    'examples/params_orbits_tokamak.yml',
+                    os.path.join(libpath, 'io/inp/examples/params_orbits_tokamak.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -38,15 +41,15 @@
     
     import os, yaml, h5py
     from tqdm import tqdm
     
     import numpy as np
     import matplotlib.pyplot as plt
     
-    from struphy.models.utilities import setup_domain_mhd
+    from struphy.models.setup import setup_domain_mhd
     from struphy.fields_background.mhd_equil.equils import EQDSKequilibrium
     
     import struphy
     libpath = struphy.__path__[0]
     
     with open(os.path.join(libpath, 'io_path.txt')) as f:
         io_path = f.readlines()[0]
```

### Comparing `struphy-2.0.0/src/struphy/fields_background/electric_equil/analytical.py` & `struphy-2.0.1/src/struphy/fields_background/electric_equil/analytical.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/electric_equil/base.py` & `struphy-2.0.1/src/struphy/fields_background/electric_equil/base.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/base.py` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from matplotlib import pyplot as plt
 from pyevtk.hl import gridToVTK
 
 
 class MHDequilibrium(metaclass=ABCMeta):
     """
     Base class for Struphy MHD equilibria.
-    The callables B, J, p and n have to be provided through the child classes `CartesianMHDequilibrium` or `LogicalMHDequilibrium`.
+    The callables B, J, p and n have to be provided through the child classes `CartesianMHDequilibrium`, `LogicalMHDequilibrium`
+    or `AxisymmMHDequilibrium`.
     The base class provides transformations of callables to different representations or coordinates.
     For logical equilibria, the methods b2, j2, p0 and n0 are overidden by the child class.   
     """    
 
     def absB0(self, *etas, squeeze_out=True):
         """ 0-form absolute value of equilibrium magnetic field on logical cube [0, 1]^3.
         """
@@ -59,14 +60,39 @@
         """ Unit vector Cartesian components of equilibrium magnetic field evaluated on logical cube [0, 1]^3. Returns also (x,y,z).
         """
         b, xyz = self.b_cart(*etas, squeeze_out=squeeze_out)
         absB = self.absB0(*etas, squeeze_out=squeeze_out)
         out = np.array([b[0]/absB, b[1]/absB, b[2]/absB], dtype=float)
         return out, xyz
 
+    def a1(self, *etas, squeeze_out=True):
+        """ 1-form components of equilibrium vector potential on logical cube [0, 1]^3.
+        """
+        avail_list = ['HomogenSlab']
+        assert self.__class__.__name__ in avail_list, f'Vector potential currently available only for {avail_list}, but mhd_equil is "{self.mhd_equil.__class__.__name__}".'
+        
+        return self.domain.transform(self.a2(*etas, squeeze_out=False), *etas, kind='2_to_1', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
+
+    def a2(self, *etas, squeeze_out=True):
+        """ 2-form components of equilibrium vector potential on logical cube [0, 1]^3.
+        """
+        avail_list = ['HomogenSlab']
+        assert self.__class__.__name__ in avail_list, f'Vector potential currently available only for {avail_list}, but mhd_equil is "{self.mhd_equil.__class__.__name__}".'
+        
+        xyz = self.domain(*etas, squeeze_out=False)
+        return self.domain.pull(self.a_xyz(xyz[0], xyz[1], xyz[2]), *etas, kind='2_form', squeeze_out=squeeze_out)
+    
+    def av(self, *etas, squeeze_out=True):
+        """ Contra-variant components of equilibrium vector potneital on logical cube [0, 1]^3.
+        """
+        avail_list = ['HomogenSlab']
+        assert self.__class__.__name__ in avail_list, f'Vector potential currently available only for {avail_list}, but mhd_equil is "{self.mhd_equil.__class__.__name__}".'
+        
+        return self.domain.transform(self.a2(*etas, squeeze_out=False), *etas, kind='2_to_v', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
+    
     def j1(self, *etas, squeeze_out=True):
         """ 1-form components of equilibrium current on logical cube [0, 1]^3.
         """
         return self.domain.transform(self.j2(*etas, squeeze_out=False), *etas, kind='2_to_1', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
 
     def j2(self, *etas, squeeze_out=True):
         """ 2-form components of equilibrium current on logical cube [0, 1]^3.
@@ -115,23 +141,50 @@
         return self.b1(*etas, squeeze_out=squeeze_out)[0]
 
     def b1_2(self, *etas, squeeze_out=True):
         return self.b1(*etas, squeeze_out=squeeze_out)[1]
 
     def b1_3(self, *etas, squeeze_out=True):
         return self.b1(*etas, squeeze_out=squeeze_out)[2]
+    
+    def a1_1(self, *etas, squeeze_out=True):
+        return self.a1(*etas, squeeze_out=squeeze_out)[0]
+
+    def a1_2(self, *etas, squeeze_out=True):
+        return self.a1(*etas, squeeze_out=squeeze_out)[1]
+
+    def a1_3(self, *etas, squeeze_out=True):
+        return self.a1(*etas, squeeze_out=squeeze_out)[2]
 
     def b2_1(self, *etas, squeeze_out=True):
         return self.b2(*etas, squeeze_out=squeeze_out)[0]
 
     def b2_2(self, *etas, squeeze_out=True):
         return self.b2(*etas, squeeze_out=squeeze_out)[1]
 
     def b2_3(self, *etas, squeeze_out=True):
         return self.b2(*etas, squeeze_out=squeeze_out)[2]
+    
+    def a2_1(self, *etas, squeeze_out=True):
+        return self.a2(*etas, squeeze_out=squeeze_out)[0]
+
+    def a2_2(self, *etas, squeeze_out=True):
+        return self.a2(*etas, squeeze_out=squeeze_out)[1]
+
+    def a2_3(self, *etas, squeeze_out=True):
+        return self.a2(*etas, squeeze_out=squeeze_out)[2]
+    
+    def av_1(self, *etas, squeeze_out=True):
+        return self.av(*etas, squeeze_out=squeeze_out)[0]
+
+    def av_2(self, *etas, squeeze_out=True):
+        return self.av(*etas, squeeze_out=squeeze_out)[1]
+
+    def av_3(self, *etas, squeeze_out=True):
+        return self.av(*etas, squeeze_out=squeeze_out)[2]
 
     def unit_b1_1(self, *etas, squeeze_out=True):
         return self.unit_b1(*etas, squeeze_out=squeeze_out)[0]
 
     def unit_b1_2(self, *etas, squeeze_out=True):
         return self.unit_b1(*etas, squeeze_out=squeeze_out)[1]
```

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/equils.py` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/equils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,206 +1,273 @@
 import numpy as np
 
 from struphy.fields_background.mhd_equil.base import CartesianMHDequilibrium, LogicalMHDequilibrium, AxisymmMHDequilibrium
 
 
 class HomogenSlab(CartesianMHDequilibrium):
     r"""
-    Homogeneous MHD equilibrium in slab geometry.
+    Homogeneous MHD equilibrium:
 
     .. math::
 
         \mathbf B &= B_{0x}\,\mathbf e_x + B_{0y}\,\mathbf e_y + B_{0z}\,\mathbf e_z = const.\,,
-        
+
         p &= \beta \frac{|\mathbf B|^2}{2}=const.\,,
-        
+
         n &= n_0 = const.\,.
+        
+    Units are those defned in the parameter file (:code:`struphy units -h`).
 
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-
-            * B0x  : magnetic field in x-direction
-            * B0y  : magnetic field in y-direction
-            * B0z  : magnetic field in z-direction
-            * beta : plasma beta in % (ratio kinetic/magnetic pressure)
-            * n0   : number density            
+        Keyword arguments that characterize the MHD equilibrium.
+            * B0x : float  
+                x-component of magnetic field (default: 0.).
+            * B0y : float  
+                y-component of magnetic field (default: 0.).
+            * B0z : float  
+                z-component of magnetic field (default: 1.).
+            * beta : float
+                Plasma beta (ratio of kinematic pressure to B^2/(2*mu0), default: 0.1).
+            * n0 : float 
+                Ion number density (default: 1.).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : HomogenSlab
+            HomogenSlab :
+                B0x  : 0. # magnetic field in x
+                B0y  : 0. # magnetic field in y
+                B0z  : 1. # magnetic field in z
+                beta : .1 # plasma beta = p*(2*mu_0)/B^2
+                n0   : 1. # number density     
     """
 
     def __init__(self, **params):
 
         params_default = {'B0x': 0.,
                           'B0y': 0.,
                           'B0z': 1.,
-                          'beta': 100.,
+                          'beta': .1,
                           'n0': 1.}
 
         self._params = set_defaults(params, params_default)
 
     @property
     def params(self):
         """ Parameters dictionary.
         """
         return self._params
 
     # ===============================================================
     #                  profiles on physical domain
     # ===============================================================
 
-    # equilibrium magnetic field
+    # equilibrium magnetic field (curl of equilibrium vector potential)
     def b_xyz(self, x, y, z):
         """ Magnetic field.
         """
         bx = self.params['B0x'] - 0*x
         by = self.params['B0y'] - 0*x
         bz = self.params['B0z'] - 0*x
 
         return bx, by, bz
 
+    #equilibrium vector potential
+    def a_xyz(self, x, y, z):
+        """ Vector potential.
+        """
+        bx = self.params['B0x'] - 0*x
+        by = self.params['B0y'] - 0*x
+        bz = self.params['B0z'] - 0*x
+
+        ax = by*z
+        ay = bz*x
+        az = bx*y 
+        
+        return ax, ay, az
+    
     # equilibrium current (curl of equilibrium magnetic field)
     def j_xyz(self, x, y, z):
         """ Current density.
         """
         jx = 0*x
         jy = 0*x
         jz = 0*x
 
         return jx, jy, jz
 
     # equilibrium pressure
     def p_xyz(self, x, y, z):
-        """ Pressure.
+        """ Plasma pressure.
         """
-        pp = self.params['beta']/200*(self.params['B0x']**2 +
-                                      self.params['B0y']**2 + self.params['B0z']**2) - 0*x
+        pp = self.params['beta'] * (self.params['B0x']**2 +
+                                    self.params['B0y']**2 + self.params['B0z']**2) / 2. - 0*x
 
         return pp
 
     # equilibrium number density
     def n_xyz(self, x, y, z):
         """ Number density.
         """
         nn = self.params['n0'] - 0*x
 
         return nn
 
 
 class ShearedSlab(CartesianMHDequilibrium):
     r"""
-    Sheared slab MHD equilibrium in a cube with side lengths :math:`L_x=a,\,L_y=2\pi a,\,L_z=2\pi R_0`. Profiles depend on :math:`x` solely. 
+    Sheared slab MHD equilibrium in a cube with side lengths :math:`L_x=a,\,L_y=2\pi a,\,L_z=2\pi R_0`. Profiles depend on :math:`x` solely: 
 
     .. math::
 
         \mathbf B(x) &= B_{0} \left( \mathbf e_z + \frac{a}{q(x)R_0}\mathbf e_y\right)\,,\qquad q(x) = q_0 + ( q_1 - q_0 )\frac{x^2}{a^2}\,,
 
         p(x) &= \beta\frac{B_{0}^2}{2} \left( 1 + \frac{a^2}{q(x)^2 R_0^2} \right) + B_{0}^2 \frac{a^2}{R_0^2} \left( \frac{1}{q_0^2} - \frac{1}{q(x)^2} \right)\,,
 
         n(x) &= n_a + ( 1 - n_a ) \left( 1 - \left(\frac{x}{a}\right)^{n_1} \right)^{n_2} \,.
 
+    Units are those defned in the parameter file (:code:`struphy units -h`).
+
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-
-            * a    : "minor" radius (Lx = a, Ly = 2*pi*a)
-            * R0   : "major" radius (Lz = 2*pi*R0)
-            * B0   : magnetic field in z-direction
-            * q0   : safety factor at x=0
-            * q1   : safety factor at x=a
-            * n1   : 1st shape factor for number density profile 
-            * n2   : 2nd shape factor for number density profile 
-            * na   : number density at x=a
-            * beta : plasma beta in % at x=0 (ratio of kinetic pressure to magnetic pressure)            
+        Keyword arguments that characterize the MHD equilibrium. 
+            * a : float 
+                "Minor" radius (must be compatible with :math:`L_x=a` and :math:`L_y=2\pi a`, default: 1.).
+            * R0 : float
+                "Major" radius (must be compatible with :math:`L_z=2\pi R_0`, default: 3.).
+            * B0 : float
+                z-component of magnetic field (constant) (default: 1.).
+            * q0 : float
+                Safety factor at x=0 (default: 1.05).
+            * q1 : float
+                Safety factor at x=a (default: 1.80).
+            * n1 : float
+                1st shape factor for ion number density profile (default: 0.).
+            * n2 : float
+                2nd shape factor for ion number density profile (default: 0.). 
+            * na : float
+                Ion number density at x=a (default: 1.).
+            * beta : float
+                Plasma beta (ratio of kinematic pressure to B^2/(2*mu0), default: 0.1).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : ShearedSlab
+            ShearedSlab :
+                a    : 1.   # minor radius (Lx=a, Ly=2*pi*a) 
+                R0   : 3.   # major radius (Lz=2*pi*R0)
+                B0   : 1.   # magnetic field in z-direction    
+                q0   : 1.05 # safety factor at x = 0
+                q1   : 1.80 # safety factor at x = a
+                n1   : 0.   # 1st shape factor for ion number density profile
+                n2   : 0.   # 2nd shape factor for ion number density profile
+                na   : 1.   # number density at r=a
+                beta : .1   # plasma beta = p*(2*mu_0)/B^2
     """
 
     def __init__(self, **params):
 
         params_default = {'a': 1.,
                           'R0': 3.,
                           'B0': 1.,
                           'q0': 1.05,
                           'q1': 1.80,
                           'n1': 0.,
                           'n2': 0.,
                           'na': 1.,
-                          'beta': 10.}
+                          'beta': .1}
 
         self._params = set_defaults(params, params_default)
 
     @property
     def params(self):
         """ Parameters dictionary.
         """
         return self._params
 
     # ===============================================================
     #             profiles for a sheared slab geometry
     # ===============================================================
 
-    def nx(self, x):
-        """ Radial (x) number density profile.
+    def q_x(self, x, der=0):
+        """ Safety factor profile q = q(x) (or its first derivative if der=1).
         """
-        nout = (1 - self.params['na'])*(1 - (x/self.params['a']) **
-                                        self.params['n1'])**self.params['n2'] + self.params['na']
 
-        return nout
-
-    def q(self, x):
-        """ Radial (x) safety factor profile.
-        """
-        qout = self.params['q0'] + (self.params['q1'] -
-                                    self.params['q0'])*(x/self.params['a'])**2
+        assert der >= 0 and der <= 1, 'Only first derivative available!'
 
-        return qout
+        if self.params['q0'] == 'inf' and self.params['q1'] == 'inf':
+            if der == 0:
+                qout = 101. - 0*x
+            else:
+                qout = 0*x
 
-    def q_p(self, x):
-        """ Radial (x) derivative of safety factor profile.
-        """
-        qout = 2*(self.params['q1'] - self.params['q0'])*x/self.params['a']**2
+        else:
+            if der == 0:
+                qout = self.params['q0'] + (self.params['q1'] -
+                                            self.params['q0'])*(x/self.params['a'])**2
+            else:
+                qout = 2*(self.params['q1'] -
+                          self.params['q0'])*x/self.params['a']**2
 
         return qout
 
-    def px(self, x):
-        """ Radial pressure profile.
+    def p_x(self, x):
+        """ Pressure profile p = p(x).
         """
-        q = self.q(x)
+        q = self.q_x(x)
 
         eps = self.params['a']/self.params['R0']
 
-        if np.all(q >= 100.) or np.all(q == 0.):
-            pout = self.params['B0']**2*self.params['beta']/200 - 0*x
+        if np.all(q >= 100.):
+            pout = self.params['B0']**2*self.params['beta'] / 2. - 0*x
         else:
-            pout = self.params['B0']**2*self.params['beta']/200*(
+            pout = self.params['B0']**2*self.params['beta'] / 2. *(
                 1 + eps**2/q**2) + self.params['B0']**2*eps**2*(1/self.params['q0']**2 - 1/q**2)
 
         return pout
 
+    def n_x(self, x):
+        """ Ion number density profile n = n(x).
+        """
+        nout = (1 - self.params['na'])*(1 - (x/self.params['a']) **
+                                        self.params['n1'])**self.params['n2'] + self.params['na']
+
+        return nout
+
     def plot_profiles(self, n_pts=501):
         """ Plots radial profiles.
         """
 
         import matplotlib.pyplot as plt
 
         x = np.linspace(0., self.params['a'], n_pts)
 
         fig, ax = plt.subplots(1, 3)
 
         fig.set_figheight(3)
         fig.set_figwidth(12)
 
-        ax[0].plot(x, self.q(x))
+        ax[0].plot(x, self.q_x(x))
         ax[0].set_xlabel('x')
         ax[0].set_ylabel('q')
 
-        ax[1].plot(x, self.px(x))
+        ax[1].plot(x, self.p_x(x))
         ax[1].set_xlabel('x')
         ax[1].set_ylabel('p')
 
-        ax[2].plot(x, self.nx(x))
+        ax[2].plot(x, self.n_x(x))
         ax[2].set_xlabel('x')
         ax[2].set_ylabel('n')
 
         plt.subplots_adjust(wspace=0.4)
 
         plt.show()
 
@@ -210,116 +277,142 @@
 
     # equilibrium magnetic field
     def b_xyz(self, x, y, z):
         """ Magnetic field.
         """
         bx = 0*x
 
-        q = self.q(x)
+        q = self.q_x(x)
         eps = self.params['a']/self.params['R0']
         if np.all(q >= 100.):
             by = 0*x
             bz = self.params['B0'] - 0*x
-        elif np.all(q == 0.):
-            by = self.params['B0'] - 0*x
-            bz = 0*x
         else:
             by = self.params['B0']*eps/q
             bz = self.params['B0'] - 0*x
 
         return bx, by, bz
 
     # equilibrium current (curl of equilibrium magnetic field)
     def j_xyz(self, x, y, z):
         """ Current density.
         """
         jx = 0*x
         jy = 0*x
 
-        q = self.q(x)
+        q = self.q_x(x)
         eps = self.params['a']/self.params['R0']
         if np.all(q >= 100.):
             jz = 0*x
-        elif np.all(q == 0.):
-            jz = 0*x
         else:
-            jz = -self.params['B0']*eps*self.q_p(x)/q**2
+            jz = -self.params['B0']*eps*self.q_x(x, der=1)/q**2
 
         return jx, jy, jz
 
     # equilibrium pressure
     def p_xyz(self, x, y, z):
         """ Pressure.
         """
-        pp = self.px(x)
+        pp = self.p_x(x)
 
         return pp
 
     # equilibrium number density
     def n_xyz(self, x, y, z):
         """ Number density.
         """
-        nn = self.nx(x)
+        nn = self.n_x(x)
 
         return nn
 
 
 class ScrewPinch(CartesianMHDequilibrium):
     r"""
-    Straight tokamak (screw pinch) MHD equilibrium for a cylinder or radius :math:`a` and length :math:`L_z=2\pi R_0`.
+    Straight tokamak (screw pinch) MHD equilibrium for a cylindrical geometry of radius :math:`a` and length :math:`L_z=2\pi R_0`.
 
     The profiles in cylindrical coordinates :math:`(r, \theta, z)` with transformation formulae 
 
     .. math::
 
-        x &= r\cos(\theta)\,,
+        x &= r\cos\theta\,,
+
+        y &= r\sin\theta\,,
 
-        y &= r\sin(\theta)\,,
+        z &= z\,,
 
     are:
 
     .. math::
 
         \mathbf B(r) &= B_{0}\left( \mathbf e_z + \frac{r}{q(r) R_0}\mathbf e_\theta \right)\,,\qquad q(r) = q_0 + ( q_1 - q_0 )\frac{r^2}{a^2}\,,
 
         p(r) &= \left\{\begin{aligned}
-        &\frac{B_{0}^2 a^2 q_0}{ 2 R_0^2(q_1 - q_0) } \left( \frac{1}{q(r)^2} - \frac{1}{q_1^2} \right) \quad &&\textnormal{if}\quad q_1\neq q_0\,, 
+        &\frac{B_{0}^2 a^2 q_0}{ 2 R_0^2(q_1 - q_0) } \left( \frac{1}{q(r)^2} - \frac{1}{q_1^2} \right) \quad &&\textnormal{if}\quad q_1\neq q_0\neq\infty\,, 
+
+        &\frac{B_{0}^2 a^2}{R_0^2q_0^2} \left(1 - \frac{r^2}{a^2} \right) \quad &&\textnormal{if}\quad q_1= q_0\neq\infty\,, 
 
-        &\beta\frac{B_{0}^2}{2} \quad &&\textnormal{else}\,,
+        &\beta\frac{B_{0}^2}{2} \quad &&\textnormal{if}\quad q_0= q_1=\infty\,, 
         \end{aligned}\right.
 
         n(r) &= n_a + ( 1 - n_a )\left( 1 - \left(\frac{r}{a}\right)^{n_1} \right)^{n_2}\,.
+        
+    Units are those defned in the parameter file (:code:`struphy units -h`).
 
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-
-            * a    : minor radius (radius of cylinder)
-            * R0   : major radius (Lz = 2*pi*R0)
-            * B0   : magnetic field in z-direction
-            * q0   : safety factor at r=0
-            * q1   : safety factor at r=a
-            * n1   : 1st shape factor for number density profile 
-            * n2   : 2nd shape factor for number density profile 
-            * na   : number density at r=a
-            * beta : plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)  
+        Keyword arguments that characterize the MHD equilibrium.
+            * a : float 
+                "Minor" radius (radius of cylinder, default: 1.).
+            * R0 : float 
+                "Major" radius (must be compatible with :math:`L_z=2\pi R_0`, default: 5.).
+            * B0 : float
+                z-component of magnetic field (constant) (default: 1.).
+            * q0 : float, str
+                Safety factor at r=0 (use the string "inf" for infinity, default: 1.05).
+            * q1 : float, str
+                Safety factor at r=a (use the string "inf" for infinity, default: 1.80).
+            * n1 : float
+                1st shape factor for ion number density profile (default: 0.).
+            * n2 : float
+                2nd shape factor for ion number density profile (default: 0.). 
+            * na : float
+                Ion nnumber density at r=a (default: 1.).
+            * beta : float
+                Plasma beta for :math:`q_0=q_1=\infty` (ratio of kinematic pressure to B^2/(2*mu0), default: 0.1).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : ScrewPinch
+            ScrewPinch :
+                a    : 1.   # minor radius (radius of cylinder)
+                R0   : 3.   # major radius (length of pinch Lz=2*pi*R0)
+                B0   : 1.   # magnetic field in z-direction
+                q0   : 1.05 # safety factor at r=0
+                q1   : 1.80 # safety factor at r=a
+                n1   : 0.   # 1st shape factor for ion number density profile 
+                n2   : 0.   # 2nd shape factor for ion number density profile 
+                na   : 1.   # ion number density at r=a
+                beta : 0.1  # plasma beta = p*(2*mu_0)/B^2 for q0=q1=inf (pure axial field).
     """
 
     def __init__(self, **params):
 
         params_default = {'a': 1.,
                           'R0': 5.,
                           'B0': 1.,
                           'q0': 1.05,
                           'q1': 1.80,
                           'n1': 0.,
                           'n2': 0.,
                           'na': 1.,
-                          'beta': 10.}
+                          'beta': .1}
 
         self._params = set_defaults(params, params_default)
 
         # inverse cylindrical coordinate transformation (x, y, z) --> (r, theta, phi)
         self.r = lambda x, y, z: np.sqrt(x**2 + y**2)
         self.theta = lambda x, y, z: np.arctan2(y, x)
         self.z = lambda x, y, z: 1*z
@@ -330,74 +423,90 @@
         """
         return self._params
 
     # ===============================================================
     #           profiles for a straight tokamak equilibrium
     # ===============================================================
 
-    def nr(self, r):
-        """ Radial number density profile.
+    def q_r(self, r, der=0):
+        """ Radial safety factor profile q = q(r) (and first derivative).
         """
-        nout = (1 - self.params['na'])*(1 - (r/self.params['a']) **
-                                        self.params['n1'])**self.params['n2'] + self.params['na']
 
-        return nout
-
-    def q(self, r):
-        """ Radial safety factor profile.
-        """
-        qout = self.params['q0'] + (self.params['q1'] -
-                                    self.params['q0'])*(r/self.params['a'])**2
+        assert der >= 0 and der <= 1, 'Only first derivative available!'
 
-        return qout
+        if self.params['q0'] == 'inf' and self.params['q1'] == 'inf':
+            if der == 0:
+                qout = 101. - 0*r
+            else:
+                qout = 0*r
 
-    def q_p(self, r):
-        """ Radial derivative of safety factor profile.
-        """
-        qout = 2*(self.params['q1'] - self.params['q0'])*r/self.params['a']**2
+        else:
+            if der == 0:
+                qout = self.params['q0'] + (self.params['q1'] -
+                                            self.params['q0'])*(r/self.params['a'])**2
+            else:
+                qout = 2*(self.params['q1'] -
+                          self.params['q0'])*r/self.params['a']**2
 
         return qout
 
-    def pr(self, r):
-        """ Radial pressure profile.
+    def p_r(self, r):
+        """ Radial pressure profile p = p(r).
         """
         eps = self.params['a']/self.params['R0']
 
-        if self.params['q0'] == self.params['q1']:
-            pout = self.params['B0']**2*self.params['beta']/200 - 0*r
+        q0 = self.params['q0']
+        q1 = self.params['q1']
+        B0 = self.params['B0']
+
+        if q0 == 'inf' and q1 == 'inf':
+            pout = B0**2 * self.params['beta'] / 2. - 0*r
+
         else:
-            pout = self.params['B0']**2*eps**2*self.params['q0']/(
-                2*(self.params['q1'] - self.params['q0']))*(1/self.q(r)**2 - 1/self.params['q1']**2)
+
+            if q0 == q1:
+                pout = (B0**2*eps**2/q0**2)*(1 - r**2/self.params['a']**2)
+            else:
+                pout = B0**2*eps**2*q0/(2*(q1 - q0)) * \
+                    (1/self.q_r(r)**2 - 1/q1**2)
 
         return pout
 
+    def n_r(self, r):
+        """ Radial ion number density profile n = n(r).
+        """
+        nout = (1 - self.params['na'])*(1 - (r/self.params['a']) **
+                                        self.params['n1'])**self.params['n2'] + self.params['na']
+
+        return nout
+
     def plot_profiles(self, n_pts=501):
         """ Plots radial profiles.
         """
 
         import matplotlib.pyplot as plt
 
         r = np.linspace(0., self.params['a'], n_pts)
 
         fig, ax = plt.subplots(1, 3)
 
         fig.set_figheight(3)
         fig.set_figwidth(12)
 
-        ax[0].plot(r, self.q(r))
+        ax[0].plot(r, self.q_r(r))
         ax[0].set_xlabel('r')
         ax[0].set_ylabel('q')
 
         ax[0].plot(r, np.ones(r.size), 'k--')
 
-        ax[1].plot(r, self.pr(r))
+        ax[1].plot(r, self.p_r(r))
         ax[1].set_xlabel('r')
         ax[1].set_ylabel('p')
 
-        ax[2].plot(r, self.nr(r))
+        ax[2].plot(r, self.n_r(r))
         ax[2].set_xlabel('r')
         ax[2].set_ylabel('n')
 
         plt.subplots_adjust(wspace=0.4)
 
         plt.show()
 
@@ -407,15 +516,15 @@
 
     # equilibrium magnetic field
     def b_xyz(self, x, y, z):
         """ Magnetic field.
         """
         r = self.r(x, y, z)
         theta = self.theta(x, y, z)
-        q = self.q(r)
+        q = self.q_r(r)
         # azimuthal component
         if np.all(q >= 100.):
             b_theta = 0*r
         else:
             b_theta = self.params['B0']*r/(self.params['R0']*q)
         # cartesian x-component
         bx = -b_theta*np.sin(theta)
@@ -428,114 +537,153 @@
     def j_xyz(self, x, y, z):
         """ Current density.
         """
         jx = 0*x
         jy = 0*x
 
         r = self.r(x, y, z)
-        q = self.q(r)
-        q_p = self.q_p(r)
+        q = self.q_r(r)
+        q_p = self.q_r(r, der=1)
         if np.all(q >= 100.):
             jz = 0*x
         else:
             jz = self.params['B0']/(self.params['R0']*q**2)*(2*q - r*q_p)
 
         return jx, jy, jz
 
     # equilibrium pressure
     def p_xyz(self, x, y, z):
         """ Pressure.
         """
-        pp = self.pr(self.r(x, y, z))
+        pp = self.p_r(self.r(x, y, z))
 
         return pp
 
     # equilibrium number density
     def n_xyz(self, x, y, z):
         """ Number density.
         """
-        nn = self.nr(self.r(x, y, z))
+        nn = self.n_r(self.r(x, y, z))
 
         return nn
 
 
 class AdhocTorus(AxisymmMHDequilibrium):
     r"""
     Ad hoc tokamak MHD equilibrium with circular concentric flux surfaces.
-    
+
     For a cylindrical coordinate system :math:`(R, \phi, Z)` with transformation formulae
-    
+
     .. math::
 
         x &= R\cos(\phi)\,,     &&R = \sqrt{x^2 + y^2}\,,
 
         y &= R\sin(\phi)\,,  &&\phi = \arctan(y/x)\,,
 
         z &= Z\,,               &&Z = z\,,
-        
+
     the magnetic field is given by
-    
+
     .. math::
-    
+
         \mathbf B = \nabla\psi\times\nabla\phi+g\nabla\phi\,,
-        
+
     where :math:`g=g(R, Z)=-B_0R_0=const.` is the toroidal field function, :math:`R_0` the major radius of the torus and :math:`B_0` the on-axis magnetic field. The ad hoc poloidal flux function :math:`\psi=\psi(r)` is the solution of
-    
+
     .. math::
-    
+
         \frac{\textnormal{d}\psi}{\textnormal{d}r}=\frac{B_0r}{q(r)\sqrt{1 - r^2/R_0^2}}\,,\qquad r=\sqrt{Z^2+(R-R_0)^2}\,,
-        
+
     for some given safety factor profile. Two profiles in terms of the on-axis :math:`q_0\equiv q(r=0)` and edge :math:`q_1\equiv q(r=a)` safety factor values are available (:math:`a` is the minor radius of the torus):
-    
+
     .. math::
-    
+
         q(r) &= \left\{\begin{aligned}
         &q_0 + ( q_1 - q_0 )\frac{r^2}{a^2} \quad &&\textnormal{if} \quad q_\textnormal{kind}=0\,,
 
         &\frac{q_0}{1-\left(1-\frac{r^2}{a^2}\right)^{\frac{q_1}{q_0}}}\frac{r^2}{a^2} \quad &&\textnormal{if} \quad q_\textnormal{kind}=1\,.
         \end{aligned}\right.
 
     The pressure profile
-    
+
     .. math::
-    
+
         p^\prime(r) &= -\frac{B_0^2}{R_0^2}\frac{r\left[2q(r)-rq^\prime(r)\right]}{q(r)^3} \quad &&\textnormal{if} \quad p_\textnormal{kind}=0\,,
-        
+
         p(r) &= \beta \frac{B_{0}^2}{2} \left( 1 - p_1 \frac{r^2}{a^2} - p_2 \frac{r^4}{a^4} \right) \quad &&\textnormal{if} \quad p_\textnormal{kind}=1\,,
-    
+
     is either the exact solution of the MHD equilibrium condition in the cylindrical limit (:math:`p_\textnormal{kind}=0`) or an monotonically decreasing adhoc profile for some given on-axis plasma beta (:math:`p_\textnormal{kind}=1`). Finally, the number density profile is chosen as
 
     .. math::
 
         n(r) = n_a + ( 1 - n_a ) \left( 1 - \left(\frac{r}{a}\right)^{n_1} \right)^{n_2}\,.
+        
+    Units are those defned in the parameter file (:code:`struphy units -h`).
 
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-        
-            * a       : minor radius of torus
-            * R0      : major radius of torus
-            * B0      : on-axis toroidal magnetic field
-            * q_kind  : which safety factor profile (0: parabolic, 1: alternative)
-            * q0      : safety factor at r=0
-            * q1      : safety factor at r=a
-            * n1      : 1st shape factor for number density profile 
-            * n2      : 2nd shape factor for number density profile 
-            * na      : number density at r=a
-            * p_kind  : kind of pressure profile (0 : exact solution in cylindrical limit, 1 : ad hoc)
-            * p1      : 1st shape factor for ad hoc pressure profile
-            * p2      : 2nd shape factor for ad hoc pressure profile
-            * beta    : on-axis plasma beta in % (ratio of kinetic pressure to magnetic pressure)
-            * psi_k   : spline degree to be used for interpolation of poloidal flux function (if q_kind = 1)
-            * psi_nel : number of cells to be used for interpolation of poloidal flux function (if q_kind = 1)
+        Keyword arguments that characterize the MHD equilibrium.
+            * a : float
+                Minor radius of torus (default: 1.).
+            * R0 : float
+                Major radius of torus (default: 10.).
+            * B0 : float
+                On-axis (r=0) toroidal magnetic field (default: 3.).
+            * q_kind : int 
+                Which safety factor profile, see docstring (0 or 1, default: 0).
+            * q0 : float
+                Safety factor at r=0 (default: 1.71).
+            * q1 : float
+                Safety factor at r=a (default: 1.87).
+            * n1 : float
+                1st shape factor for ion number density profile (default: 0.).
+            * n2 : float
+                2nd shape factor for ion number density profile (default: 0.).
+            * na : float
+                Ion number density at r=a (default: 1.).
+            * p_kind : int 
+                Kind of pressure profile, see docstring (0 or 1, default: 1).
+            * p1 : float
+                1st shape factor for ad hoc pressure profile (default: 0.).
+            * p2 : float
+                2nd shape factor for ad hoc pressure profile (default: 0.).
+            * beta : float
+                On-axis (r=0) plasma beta if p_kind=1 (ratio of kinematic pressure to B^2/(2*mu0), default: 0.179).
+            * psi_k : int
+                Spline degree to be used for interpolation of poloidal flux function (if q_kind=1, default=3).
+            * psi_nel : int
+                Number of cells to be used for interpolation of poloidal flux function (if q_kind=1, default=50).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : AdhocTorus
+            AdhocTorus :
+                a       : 1.   # minor radius
+                R0      : 3.   # major radius
+                B0      : 1.   # on-axis toroidal magnetic field
+                q_kind  : 0    # which profile (0 : parabolic, 1 : other, see documentation)
+                q0      : 1.05 # safety factor at r=0
+                q1      : 1.80 # safety factor at r=a
+                n1      : 0.   # 1st shape factor for number density profile 
+                n2      : 0.   # 2nd shape factor for number density profile 
+                na      : 1.   # number density at r=a
+                p_kind  : 1    # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
+                p1      : .1   # 1st shape factor for ad hoc pressure profile
+                p2      : .1   # 2nd shape factor for ad hoc pressure profile
+                beta    : .01  # plasma beta = p*(2*mu_0)/B^2 for flat safety factor 
+                psi_k   : 3    # spline degree to be used for interpolation of poloidal flux function (only needed if q_kind=1)
+                psi_nel : 50   # number of cells to be used for interpolation of poloidal flux function (only needed if q_kind=1)
     """
 
     def __init__(self, **params):
-        
+
         from scipy.interpolate import UnivariateSpline
         from scipy.integrate import quad
 
         # parameters
         params_default = {'a': 1.,
                           'R0': 10.,
                           'B0': 3.,
@@ -553,52 +701,55 @@
                           'psi_nel': 50}
 
         self._params = set_defaults(params, params_default)
 
         # plasma boundary contour
         ths = np.linspace(0., 2*np.pi, 201)
 
-        self._rbs = self.params['R0']*(1 + self.params['a']/self.params['R0']*np.cos(ths))
+        self._rbs = self.params['R0'] * \
+            (1 + self.params['a']/self.params['R0']*np.cos(ths))
         self._zbs = self.params['a']*np.sin(ths)
 
         # set on-axis and boundary fluxes
         if self.params['q_kind'] == 0:
-            
+
             self._psi0 = self.psi(self.params['R0'], 0.)
             self._psi1 = self.psi(self.params['R0'] + self.params['a'], 0.)
-            
+
             self._psi_i = None
             self._p_i = None
-            
+
         else:
-            
+
             r_i = np.linspace(0., self.params['a'], self.params['psi_nel'] + 1)
-            
+
             def dpsi_dr(r):
                 return self.params['B0']*r/(self.q_r(r)*np.sqrt(1 - r**2/self.params['R0']**2))
-            
+
             psis = np.zeros_like(r_i)
-            
+
             for i, rr in enumerate(r_i):
                 psis[i] = quad(dpsi_dr, 0., rr)[0]
-            
-            self._psi_i = UnivariateSpline(r_i, psis, k=self.params['psi_k'], s=0., ext=3)
-            
+
+            self._psi_i = UnivariateSpline(
+                r_i, psis, k=self.params['psi_k'], s=0., ext=3)
+
             self._psi0 = 0.
             self._psi1 = self.psi(self.params['R0'] + self.params['a'], 0.)
-            
+
             def dp_dr(r):
                 return -(self.params['B0']**2*r)/(self.params['R0']**2*self.q_r(r)**3)*(2*self.q_r(r) - r*self.q_r(r, der=1))
-            
+
             ps = np.zeros_like(r_i)
-            
+
             for i, rr in enumerate(r_i):
                 ps[i] = quad(dp_dr, 0., rr)[0]
-            
-            self._p_i = UnivariateSpline(r_i, ps - ps[-1], k=self.params['psi_k'], s=0., ext=3)  
+
+            self._p_i = UnivariateSpline(
+                r_i, ps - ps[-1], k=self.params['psi_k'], s=0., ext=3)
 
     @property
     def params(self):
         """ Parameters dictionary.
         """
         return self._params
 
@@ -609,17 +760,17 @@
         return self._rbs
 
     @property
     def boundary_pts_Z(self):
         """ Z-coordinates of plasma boundary contour.
         """
         return self._zbs
-    
+
     # ===============================================================
-    #           abstract properties 
+    #           abstract properties
     # ===============================================================
 
     @property
     def psi_range(self):
         """ Psi on-axis and at plasma boundary.
         """
         return [self._psi0, self._psi1]
@@ -633,20 +784,20 @@
     # ===============================================================
     #           radial profiles for an ad hoc tokamak equilibrium
     # ===============================================================
 
     def psi_r(self, r, der=0):
         """ Ad hoc poloidal flux function psi = psi(r).
         """
-        
+
         assert der >= 0 and der <= 2, 'Only first and second derivative available!'
 
         # parabolic profile (analytical)
         if self.params['q_kind'] == 0:
-        
+
             eps = self.params['a']/self.params['R0']
 
             q0 = self.params['q0']
             q1 = self.params['q1']
             dq = q1 - q0
 
             # geometric correction factor and its first derivative
@@ -665,49 +816,49 @@
                     np.sqrt(dq*q0*eps**2 + dq**2)
                 out *= np.arctanh(np.sqrt((dq - dq*(r/self.params['R0'])
                                   ** 2)/(q0*eps**2 + dq)))
             elif der == 1:
                 out = self.params['B0']*r/q_bar_0
             elif der == 2:
                 out = self.params['B0']*(q_bar_0 - r*q_bar_1)/q_bar_0**2
-                
+
         # alternative profile (interpolated)
         else:
-            
+
             out = self._psi_i(r, nu=der)
 
             # remove all "dimensions" for point-wise evaluation
             if isinstance(r, (int, float)):
                 assert out.ndim == 0
                 out = out.item()
 
         return out
-    
+
     def q_r(self, r, der=0):
         """ Radial safety factor profile q = q(r) (and first derivative).
         """
-        
+
         assert der >= 0 and der <= 1, 'Only first derivative available!'
-        
+
         q0 = self.params['q0']
         q1 = self.params['q1']
-        
+
         a = self.params['a']
-        
+
         # parabolic profile
         if self.params['q_kind'] == 0:
-        
+
             if der == 0:
                 qout = q0 + (q1 - q0)*(r/a)**2
             else:
                 qout = 2*(q1 - q0)*r/a**2
-                
+
         # alternative profile
         else:
-            
+
             # int/float input
             if isinstance(r, (int, float)):
                 if r == 0:
                     if der == 0:
                         qout = 1*q0
                     else:
                         qout = 0*r
@@ -717,16 +868,17 @@
                             qout = 1*q0
                         else:
                             qout = q1*(r/a)**2/(1 - (1 - (r/a)**2)**(q1/q0))
                     else:
                         if self.params['q0'] == self.params['q1']:
                             qout = 0*r
                         else:
-                            qout = (2*r*q1/a**2)*(1 - (1 - (r/a)**2)**(q1/q0) - (r/a)**2*(q1/q0)*(1 - (r/a)**2)**(q1/q0 - 1))/(1 - (1 - (r/a)**2)**(q1/q0))**2
-                    
+                            qout = (2*r*q1/a**2)*(1 - (1 - (r/a)**2)**(q1/q0) - (r/a)**2*(q1/q0)
+                                                  * (1 - (r/a)**2)**(q1/q0 - 1))/(1 - (1 - (r/a)**2)**(q1/q0))**2
+
             # vector input
             else:
                 sh = r.shape
 
                 r_flat = r.flatten()
 
                 r_zeros = np.where(r_flat == 0.)[0]
@@ -735,62 +887,65 @@
                 qout = np.zeros(r_flat.size, dtype=float)
 
                 if der == 0:
                     if self.params['q0'] == self.params['q1']:
                         qout[:] = 1*q0
                     else:
                         qout[r_zeros] = 1*q0
-                        qout[r_nzero] = q1*(r_flat[r_nzero]/a)**2/(1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0))
+                        qout[r_nzero] = q1*(r_flat[r_nzero]/a)**2 / \
+                            (1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0))
                 else:
                     if self.params['q0'] == self.params['q1']:
                         qout[:] = 0.
                     else:
                         qout[r_zeros] = 0*r_zeros
-                        qout[r_nzero] = (2*r_flat[r_nzero]*q1/a**2)*(1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0) - (r_flat[r_nzero]/a)**2*(q1/q0)*(1 - (r_flat[r_nzero]/a)**2)**(q1/q0 - 1))/(1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0))**2
+                        qout[r_nzero] = (2*r_flat[r_nzero]*q1/a**2)*(1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0) - (r_flat[r_nzero]/a)**2*(
+                            q1/q0)*(1 - (r_flat[r_nzero]/a)**2)**(q1/q0 - 1))/(1 - (1 - (r_flat[r_nzero]/a)**2)**(q1/q0))**2
 
                 qout = qout.reshape(sh).copy()
 
         return qout
-    
+
     def p_r(self, r):
         """ Radial pressure profile p = p(r).
         """
-        
+
         eps = self.params['a']/self.params['R0']
 
         # profile in cylindrical limit
         if self.params['p_kind'] == 0:
-            
+
             # parabolic q-profile
             if self.params['q_kind'] == 0:
-                
+
                 if self.params['q0'] == self.params['q1']:
-                    pout = self.params['B0']**2*self.params['a']**2/(self.params['R0']**2*self.params['q0']**2)*(1 - r**2/self.params['a']**2)
+                    pout = self.params['B0']**2*self.params['a']**2/(
+                        self.params['R0']**2*self.params['q0']**2)*(1 - r**2/self.params['a']**2)
                 else:
                     pout = self.params['B0']**2*eps**2*self.params['q0']/(
                         2*(self.params['q1'] - self.params['q0']))*(1/self.q_r(r)**2 - 1/self.params['q1']**2)
-                    
+
             # alternative profile
             else:
-                
+
                 pout = self._p_i(r)
 
                 # remove all "dimensions" for point-wise evaluation
                 if isinstance(r, (int, float)):
                     assert pout.ndim == 0
                     pout = pout.item()
 
         # ad-hoc profile
         else:
 
-            pout = self.params['B0']**2*self.params['beta']/200*(
+            pout = self.params['B0']**2 * self.params['beta'] / 2. * (
                 1 - self.params['p1']*r**2/self.params['a']**2 - self.params['p2']*r**4/self.params['a']**4)
 
         return pout
-    
+
     def n_r(self, r):
         """ Radial number density profile n = n(r).
         """
         nout = (1 - self.params['na'])*(1 - (r/self.params['a']) **
                                         self.params['n1'])**self.params['n2'] + self.params['na']
 
         return nout
@@ -807,15 +962,15 @@
 
         fig.set_figheight(5)
         fig.set_figwidth(6)
 
         ax[0, 0].plot(r, self.psi_r(r))
         ax[0, 0].set_xlabel('$r$')
         ax[0, 0].set_ylabel('$\psi$')
-        
+
         ax[0, 1].plot(r, self.q_r(r))
         ax[0, 1].set_xlabel('$r$')
         ax[0, 1].set_ylabel('$q$')
 
         ax[1, 0].plot(r, self.p_r(r))
         ax[1, 0].set_xlabel('$r$')
         ax[1, 0].set_ylabel('$p$')
@@ -893,85 +1048,122 @@
         """ Number density n = n(x, y, z).
         """
         r = np.sqrt((np.sqrt(x**2 + y**2) - self._params['R0'])**2 + z**2)
 
         nn = self.n_r(r)
 
         return nn
-    
+
 
 class AdhocTorusQPsi(AxisymmMHDequilibrium):
     r"""
     Ad hoc tokamak MHD equilibrium with circular concentric flux surfaces.
-    
+
     For a cylindrical coordinate system :math:`(R, \phi, Z)` with transformation formulae
-    
+
     .. math::
 
         x &= R\cos(\phi)\,,     &&R = \sqrt{x^2 + y^2}\,,
 
         y &= R\sin(\phi)\,,  &&\phi = \arctan(y/x)\,,
 
         z &= Z\,,               &&Z = z\,,
-        
+
     the magnetic field is given by
-    
+
     .. math::
-    
+
         \mathbf B = \nabla\psi\times\nabla\phi+g\nabla\phi\,,
-        
+
     where :math:`g=g(R, Z)=-B_0R_0=const.` is the toroidal field function, :math:`R_0` the major radius of the torus and :math:`B_0` the on-axis magnetic field. The ad hoc poloidal flux function :math:`\psi=\psi(r)` is the solution of
-    
+
     .. math::
-    
+
         \frac{\textnormal{d}\psi}{\textnormal{d}r}=\frac{B_0r}{q(\psi(r))\sqrt{1 - r^2/R_0^2}}\,,\qquad r=\sqrt{Z^2+(R-R_0)^2}\,,
-        
+
     for a safety factor profile
-    
+
     .. math::
-    
+
         q(\psi) &= q_0 + \psi_{\textnormal{norm}}\left[ q_1-q_0+(q_1^\prime-q_1+q_0)\frac{(1-\psi_s)(\psi_{\textnormal{norm}}-1)}{\psi_{\textnormal{norm}}-\psi_s} \right]\,,
-        
+
         \psi_{\textnormal{norm}} &= \frac{\psi-\psi(0)}{\psi(a)-\psi(0)}\,,
-        
+
         \psi_s &= (q_1^\prime-q_1+q_0)/(q_0^\prime+q_1^\prime-2q_1+2q_0)\,,
 
     where :math:`a` is the minor radius of the torus.
-    
+
     The pressure and number density profiles are chosen as
 
     .. math::
 
         p(\psi) &= \frac{\beta B_0^2}{2}\exp\left(-\frac{\psi_{\textnormal{norm}}}{p_1}\right)\,,
 
         n(\psi) &= n_a + ( 1 - n_a ) \left( 1 - \psi_{\textnormal{norm}}^{n_1} \right)^{n_2}\,.
+        
+    Units are those defned in the parameter file (:code:`struphy units -h`).
 
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-        
-            * a       : minor radius of torus
-            * R0      : major radius of torus
-            * B0      : on-axis toroidal magnetic field
-            * q0      : safety factor at r=0
-            * q1      : safety factor at r=a
-            * q0p     : derivative of safety factor at r=0 (w.r.t. poloidal flux function)
-            * q1p     : derivative of safety factor at r=a (w.r.t. poloidal flux function)
-            * n1      : 1st shape factor for number density profile 
-            * n2      : 2nd shape factor for number density profile 
-            * na      : number density at r=a
-            * beta    : on-axis plasma beta in % (ratio of kinetic pressure to magnetic pressure)   
-            * p1      : shape factor of pressure profile
-            * psi_k   : spline degree to be used for interpolation of poloidal flux function
-            * psi_nel : number of cells to be used for interpolation of poloidal flux function
+        Keyword arguments that characterize the MHD equilibrium.
+            * a : float
+                Minor radius of torus (default: 0.361925).
+            * R0 : float
+                Major radius of torus (default: 1.).
+            * B0 : float
+                On-axis (r=0) toroidal magnetic field (default: 1.).
+            * q0 : float
+                Safety factor at r=0 (default: 0.6).
+            * q1 : float
+                Safety factor at r=a (default: 2.5).
+            * q0p : float
+                Derivative of safety factor at r=0 (w.r.t. poloidal flux function, default: 0.78).
+            * q1p : float
+                Derivative of safety factor at r=a (w.r.t. poloidal flux function, default: 5.00).
+            * n1 : float
+                1st shape factor for ion number density profile (default: 0.).
+            * n2 : float
+                2nd shape factor for ion number density profile (default: 0.).
+            * na : float
+                Ion number density at r=a (default: 1.).
+            * beta : float
+                On-axis (r=0) plasma beta (ratio of kinematic pressure to B^2/(2*mu0), default: 0.1).
+            * p1 : float
+                Shape factor for pressure profile, see docstring (default: 0.25).
+            * psi_k : int
+                Spline degree to be used for interpolation of poloidal flux function (default=3).
+            * psi_nel : int
+                Number of cells to be used for interpolation of poloidal flux function (default=50).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : AdhocTorusQPsi
+            AdhocTorusQPsi :
+                a       : 0.361925 # minor radius
+                R0      : 1.   # major radius
+                B0      : 1.   # on-axis toroidal magnetic field
+                q0      : 0.6  # safety factor at r=0
+                q1      : 2.5  # safety factor at r=a
+                q0p     : 0.78 # derivative of safety factor at r=0 (w.r.t. to poloidal flux function)
+                q1p     : 5.00 # derivative of safety factor at r=a (w.r.t. to poloidal flux function)
+                n1      : 0.   # shape factor for number density profile 
+                n2      : 0.   # shape factor for number density profile 
+                na      : 1.   # number density at r=a
+                beta    : .1   # plasma beta = p*(2*mu_0)/B^2 for flat safety factor
+                p1      : 0.25 # shape factor of pressure profile
+                psi_k   : 3    # spline degree to be used for interpolation of poloidal flux function
+                psi_nel : 50   # number of cells to be used for interpolation of poloidal flux functionq_kind=1)
     """
-    
+
     def __init__(self, **params):
-        
+
         from scipy.optimize import fsolve
         from scipy.integrate import odeint
         from scipy.interpolate import UnivariateSpline
 
         # parameters
         params_default = {'a': 0.361925,
                           'R0': 1.,
@@ -985,60 +1177,62 @@
                           'na': 1.,
                           'beta': 4.,
                           'p1': 0.25,
                           'psi_k': 3,
                           'psi_nel': 50}
 
         self._params = set_defaults(params, params_default)
-        
+
         # plasma boundary contour
         ths = np.linspace(0., 2*np.pi, 201)
 
-        self._rbs = self.params['R0']*(1 + self.params['a']/self.params['R0']*np.cos(ths))
+        self._rbs = self.params['R0'] * \
+            (1 + self.params['a']/self.params['R0']*np.cos(ths))
         self._zbs = self.params['a']*np.sin(ths)
-        
+
         # on-axis flux (arbitrary value)
         self._psi0 = -10.
-        
+
         # poloidal flux function differential equation: dpsi_dr(r) = B0*r/(q(psi(r))*sqrt(1 - r**2/R0**2))
         def dpsi_dr(psi, r, psi1):
-            
+
             q0 = self.params['q0']
             q1 = self.params['q1']
 
             q0p = self.params['q0p']
             q1p = self.params['q1p']
-            
+
             B0 = self.params['B0']
             R0 = self.params['R0']
 
             psi_norm = (psi - self._psi0)/(psi1 - self._psi0)
             psi_s = (q1p - q1 + q0)/(q0p + q1p - 2*q1 + 2*q0)
 
-            q = q0 + psi_norm*(q1 - q0 + (q1p - q1 + q0)*(1 - psi_s)*(psi_norm - 1)/(psi_norm - psi_s))
-            
+            q = q0 + psi_norm*(q1 - q0 + (q1p - q1 + q0) *
+                               (1 - psi_s)*(psi_norm - 1)/(psi_norm - psi_s))
+
             out = B0*r/(q*np.sqrt(1 - r**2/R0**2))
-            
+
             return out
-        
+
         # solve differential equation and fix boundary flux
         r_i = np.linspace(0., self.params['a'], self.params['psi_nel'] + 1)
-        
+
         def fun(psi1):
-            
+
             out = odeint(dpsi_dr, self._psi0, r_i, args=(psi1,)).flatten()
-            
+
             return out[-1] - psi1
-        
+
         self._psi1 = fsolve(fun, -9.5)[0]
-        
+
         # interpolate flux function
         self._psi_i = UnivariateSpline(r_i, odeint(dpsi_dr, self._psi0, r_i, args=(self._psi1,)).flatten(),
                                        k=self.params['psi_k'], s=0., ext=3)
-        
+
     @property
     def params(self):
         """ Parameters dictionary describing the equilibrium.
         """
         return self._params
 
     @property
@@ -1048,15 +1242,15 @@
         return self._rbs
 
     @property
     def boundary_pts_Z(self):
         """ Z-coordinates of plasma boundary contour.
         """
         return self._zbs
-    
+
     # ===============================================================
     #           abstract properties
     # ===============================================================
 
     @property
     def psi_range(self):
         """ Psi on-axis and at plasma boundary.
@@ -1072,78 +1266,82 @@
     # ===============================================================
     #       1d profiles for an ad hoc tokamak equilibrium
     # ===============================================================
 
     def psi_r(self, r, der=0):
         """ Ad hoc poloidal flux function psi = psi(r).
         """
-        
+
         assert der >= 0 and der <= 2, 'Only first and second derivatives available!'
 
         out = self._psi_i(r, nu=der)
 
         # remove all "dimensions" for point-wise evaluation
         if isinstance(r, (int, float)):
             assert out.ndim == 0
             out = out.item()
 
         return out
-    
+
     def q_psi(self, psi):
         """ Safety factor profile q = q(psi).
         """
-        
+
         q0 = self.params['q0']
         q1 = self.params['q1']
 
         q0p = self.params['q0p']
         q1p = self.params['q1p']
 
         psi_s = (q1p - q1 + q0)/(q0p + q1p - 2*q1 + 2*q0)
-        
+
         psi_norm = (psi - self._psi0)/(self._psi1 - self._psi0)
 
-        q = q0 + psi_norm*(q1 - q0 + (q1p - q1 + q0)*(1 - psi_s)*(psi_norm - 1)/(psi_norm - psi_s))
-        
+        q = q0 + psi_norm*(q1 - q0 + (q1p - q1 + q0)*(1 - psi_s)
+                           * (psi_norm - 1)/(psi_norm - psi_s))
+
         return q
-    
+
     def p_psi(self, psi, der=0):
         """ Pressure profile p = p(psi).
         """
-        
+
         assert der >= 0 and der <= 1, 'Only first derivative available!'
-        
-        beta, p1, B0 = self.params['beta'], self.params['p1'], self.params['B0'] 
-        
+
+        beta, p1, B0 = self.params['beta'], self.params['p1'], self.params['B0']
+
         psi_norm = (psi - self._psi0)/(self._psi1 - self._psi0)
-        
+
         if der == 0:
-            out = self.params['beta']*self.params['B0']**2/200*np.exp(-psi_norm/p1)
+            out = self.params['beta'] * \
+                self.params['B0']**2 / 2. * np.exp(-psi_norm/p1)
         else:
-            out = -self.params['beta']*self.params['B0']**2/200*np.exp(-psi_norm/p1)/(p1*(self._psi1 - self._psi0))
+            out = -self.params['beta']*self.params['B0']**2 / 2. * \
+                np.exp(-psi_norm/p1)/(p1*(self._psi1 - self._psi0))
 
         return out
-    
+
     def n_psi(self, psi, der=0):
         """ Number density profile n = n(psi).
         """
-        
+
         assert der >= 0 and der <= 1, 'Only first derivative available!'
 
         n1, n2, na = self.params['n1'], self.params['n2'], self.params['na']
 
         psi_norm = (psi - self._psi0)/(self._psi1 - self._psi0)
 
         if der == 0:
             out = (1 - na)*(1 - psi_norm**n1)**n2 + na
         else:
-            out = -(1 - na)*n1*n2/(self._psi1 - self._psi0)*(1 - psi_norm**n1)**(n2 - 1)*psi_norm**(n1 - 1)
+            out = -(1 - na)*n1*n2/(self._psi1 - self._psi0) * \
+                (1 - psi_norm**n1)**(n2 - 1)*psi_norm**(n1 - 1)
 
         return out
-    
+
     def plot_profiles(self, n_pts=501):
         """ Plots 1d profiles.
         """
 
         import matplotlib.pyplot as plt
 
         r = np.linspace(0., self.params['a'], n_pts)
@@ -1153,35 +1351,35 @@
 
         fig.set_figheight(5)
         fig.set_figwidth(6)
 
         ax[0, 0].plot(r, self.psi_r(r))
         ax[0, 0].set_xlabel('$r$')
         ax[0, 0].set_ylabel('$\psi$')
-        
+
         ax[0, 1].plot(psi, self.q_psi(psi))
         ax[0, 1].set_xlabel('$\psi$')
         ax[0, 1].set_ylabel('$q$')
 
         ax[1, 0].plot(psi, self.p_psi(psi))
         ax[1, 0].set_xlabel('$\psi$')
         ax[1, 0].set_ylabel('$p$')
-        
+
         ax[1, 1].plot(psi, self.n_psi(psi))
         ax[1, 1].set_xlabel('$\psi$')
         ax[1, 1].set_ylabel('$n$')
 
         plt.subplots_adjust(wspace=0.4, hspace=0.4)
 
         plt.show()
-    
+
     # ===============================================================
     #           abstract methods
     # ===============================================================
-    
+
     def psi(self, R, Z, dR=0, dZ=0):
         """ Poloidal flux function psi = psi(R, Z).
         """
 
         r = np.sqrt(Z**2 + (R - self.params['R0'])**2)
 
         if dR == 0 and dZ == 0:
@@ -1243,48 +1441,78 @@
 
 class EQDSKequilibrium(AxisymmMHDequilibrium):
     """
     Interface to `EQDSK file format <https://w3.pppl.gov/ntcc/TORAY/G_EQDSK.pdf>`_.
 
     Parameters
     ----------
+    units : dict
+        All Struphy units. If None, no rescaling of EQDSK output is performed.
+    
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-        
-            * rel_path : str
-                Whether file is relative to "<struphy_path>/fields_background/mhd_equil/gvec", or is an absolute path.
+        Keyword arguments that characterize the MHD equilibrium.
+            * rel_path : bool
+                Whether file is relative to "<struphy_path>/fields_background/mhd_equil/eqdsk/data/", or is an absolute path (default: True).
             * file : str
-                Path to eqdsk file.
+                Path to eqdsk file (default: "AUGNLED_g031213.00830.high").
             * data_type : int
-                0: there is no space between data, 1: there is space between data.
+                0: there is no space between data, 1: there is space between data (default: 0).
             * p_for_psi : list[int]
-                Spline degrees in (R, Z) directions used for interpolation of psi data.
+                Spline degrees in (R, Z) directions used for interpolation of psi data (default: [3, 3]).
             * psi_resolution : list[float]
-                Resolution of psi data in (R, Z) directions in %, e.g. [50., 50.] uses every second psi data point.
+                Resolution of psi data in (R, Z) directions in %, e.g. [50., 50.] uses every second psi data point (default: [25., 6.25]).
             * p_for_flux : int
-                Spline degree in psi direction used for interpolation of 1d functions that depend on psi: f=f(psi).
+                Spline degree in psi direction used for interpolation of 1d functions that depend on psi: f=f(psi) (default: 3).
             * flux_resolution : float
-                Resolution of 1d f=f(psi) data in %, e.g. 25. uses every forth data point.
+                Resolution of 1d f=f(psi) data in %, e.g. 25. uses every forth data point (default: 50.).
             * n1 : float
-                1st shape factor for number density profile n = n(psi).
+                1st shape factor for ion number density profile n = n(psi) (default: 0.).
             * n2 : float
-                2nd shape factor for number density profile n = n(psi).
+                2nd shape factor for ion number density profile n = n(psi) (default: 0.).
             * na : float
-                Number density at plasma boundary.
+                Ion number density at plasma boundary (default: 1.).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : EQDSKequilibrium
+            EQDSKequilibrium :
+                rel_path        : True # whether eqdsk file path relative to "<struphy_path>/fields_background/mhd_equil/eqdsk/data/", or the absolute path
+                file            : 'AUGNLED_g031213.00830.high' # path to eqdsk file
+                data_type       : 0 # 0: there is no space between data, 1: there is space between data
+                p_for_psi       : [3, 3]      # spline degrees used in interpolation of poloidal flux function grid data
+                psi_resolution  : [25., 6.25] # resolution used in interpolation of poloidal flux function grid data in %, i.e. [100., 100.] uses all grid points
+                p_for_flux      : 3   # spline degree used in interpolation of 1d functions f=f(psi) (e.g. toroidal field function)
+                flux_resolution : 50. # resolution used in interpolation of of 1d functions f=f(psi) in %
+                n1              : 0.  # 1st shape factor for number density profile n(psi) = (1-na)*(1 - psi_norm^n1)^n2 + na
+                n2              : 0.  # 2nd shape factor for number density profile n(psi) = (1-na)*(1 - psi_norm^n1)^n2 + na
+                na              : 1.  # number density at last closed flux surface
     """
 
-    def __init__(self, **params):
+    def __init__(self, units=None, **params):
 
         from scipy.interpolate import UnivariateSpline, RectBivariateSpline
         from scipy.optimize import minimize
 
         from struphy.fields_background.mhd_equil.eqdsk import readeqdsk
 
         import struphy
 
+        # no rescaling if units are not provided
+        if units is None:
+            units = {}
+            units['x'] = 1.
+            units['B'] = 1.
+            units['p'] = 1 / 1.25663706212e-6
+            print('\n+++WARNING+++: "units" was passed as None, no rescaling performed in EQDSK output.')
+
+        self._units = units
+
         params_default = {'rel_path': True,
                           'file': 'AUGNLED_g031213.00830.high',
                           'data_type': 0,
                           'p_for_psi': [3, 3],
                           'psi_resolution': [25., 6.25],
                           'p_for_flux': 3,
                           'flux_resolution': 50.,
@@ -1340,15 +1568,15 @@
         # Z of limiter contour in meter
         self._zlims = eqdsk.data['zlim'][0]
 
         assert g_profile.size == p_profile.size
         assert g_profile.size == q_profile.size
         assert psi.shape == (nR, nZ)
 
-        # normalize pressure profile to pressure unit 1 Tesla/mu_0
+        # normalize pressure profile to pressure unit 1 Tesla^2/mu_0
         p_profile *= 1.25663706212e-6
 
         # spline interpolation of smoothed flux function
         self._r_range = [rleft, rleft + rdim]
         self._z_range = [zmid - zdim/2, zmid + zdim/2]
 
         R = np.linspace(self._r_range[0], self._r_range[1], nR)
@@ -1378,14 +1606,20 @@
                                      k=self._params['p_for_flux'], s=0., ext=3)
         self._p_i = UnivariateSpline(flux_grid[::smooth_step], p_profile[::smooth_step],
                                      k=self._params['p_for_flux'], s=0., ext=3)
         self._q_i = UnivariateSpline(flux_grid[::smooth_step], q_profile[::smooth_step],
                                      k=self._params['p_for_flux'], s=0., ext=3)
 
     @property
+    def units(self):
+        """ All Struphy units.
+        """
+        return self._units
+
+    @property
     def params(self):
         """ Parameters describing the equilibrium.
         """
         return self._params
 
     @property
     def boundary_pts_R(self):
@@ -1450,15 +1684,15 @@
 
         # remove all "dimensions" for point-wise evaluation
         if isinstance(psi, (int, float)):
             assert out.ndim == 0
             out = out.item()
 
         return out
-    
+
     def g_psi(self, psi, der=0):
         """ Toroidal field function g = g(psi).
         """
         out = self._g_i(psi, nu=der)
 
         # remove all "dimensions" for point-wise evaluation
         if isinstance(psi, (int, float)):
@@ -1480,15 +1714,15 @@
         return out
 
     def n_psi(self, psi, der=0):
         """ Number density profile n = n(psi).
         """
 
         assert der >= 0 and der <= 1, 'Only first derivative available!'
-        
+
         n1, n2, na = self._params['n1'], self._params['n2'], self._params['na']
 
         psi_norm = (psi - self._psi0)/(self._psi1 - self._psi0)
 
         if der == 0:
             out = (1 - na)*(1 - psi_norm**n1)**n2 + na
         else:
@@ -1498,25 +1732,28 @@
         return out
 
     # ===============================================================
     #           abstract methods
     # ===============================================================
 
     def psi(self, R, Z, dR=0, dZ=0):
-        """ Poloidal flux function psi = psi(R, Z).
+        """ Poloidal flux function psi = psi(R, Z) in units T*m^2.
         """
 
         is_float = all(isinstance(v, (int, float)) for v in [R, Z])
 
         out = self._psi_i(R, Z, dx=dR, dy=dZ, grid=False)
 
         # remove all "dimensions" for point-wise evaluation
         if is_float:
             assert out.ndim == 0
             out = out.item()
+            
+        # rescale to Struphy units
+        out /= self.units['B'] * self.units['x']**2
 
         return out
 
     def g_tor(self, R, Z, dR=0, dZ=0):
         """ Toroidal field function g = g(R, Z).
         """
 
@@ -1524,63 +1761,84 @@
             out = self.g_psi(self.psi(R, Z, dR=0, dZ=0), der=0)
         elif dR == 1 and dZ == 0:
             out = self.g_psi(self.psi(R, Z, dR=0, dZ=0), der=1) * \
                 self.psi(R, Z, dR=1, dZ=0)
         elif dR == 0 and dZ == 1:
             out = self.g_psi(self.psi(R, Z, dR=0, dZ=0), der=1) * \
                 self.psi(R, Z, dR=0, dZ=1)
+                
+        # rescale to Struphy units
+        out /= self.units['B'] * self.units['x']
 
         return out
 
     def p_xyz(self, x, y, z):
-        """ Pressure p = p(x, y, z).
+        """ Pressure p = p(x, y, z) in units 1 Tesla^2/mu_0.
         """
-        
+
         R = np.sqrt(x**2 + y**2)
         Z = 1*z
 
         out = self.p_psi(self.psi(R, Z))
+        
+        # rescale to Struphy units
+        out /= 1.25663706212e-6 * self.units['p']
 
         return out
 
     def n_xyz(self, x, y, z):
-        """ Number density in physical space.
+        """ Number density in physical space. Units from parameter file. 
         """
-        
+
         R = np.sqrt(x**2 + y**2)
         Z = 1*z
 
         out = self.n_psi(self.psi(R, Z))
 
         return out
 
 
 class GVECequilibrium(LogicalMHDequilibrium):
-    '''Interface to `gvec_to_python <https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python>`_.
+    """
+    Interface to `gvec_to_python <https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python>`_.
 
     Parameters
     ----------
     **params
-        Parameters that characterize the MHD equilibrium. Possible keys are
-
-        * rel_path : str
-            Whether dat_file (json_file) are relative to "<struphy_path>/fields_background/mhd_equil/gvec", or are absolute paths.
-        * dat_file : str
-            Path to .dat file.    
-        * json_file : str
-            Path to .json file.
-        * use_pest : bool
-            Whether to use straigh-field line coordinates (PEST).
-        * use_nfp : bool
-            Whether the field periods of the stellarator should be used in the mapping, i.e. phi = 2*pi*eta3 / nfp (piece of cake).
-        * Nel : tuple[int]
-            Number of cells in each direction used for interpolation of the mapping.   
-        * p : tuple[int]
-            Spline degree in each direction used for interpolation of the mapping.
-    '''
+        Keyword arguments that characterize the MHD equilibrium.
+            * rel_path : bool
+                Whether dat_file (json_file) are relative to "<struphy_path>/fields_background/mhd_equil/gvec", or are absolute paths (default: True).
+            * dat_file : str
+                Path to .dat file (default: "/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat").    
+            * json_file : str
+                Path to .json file (default: None).
+            * use_pest : bool
+                Whether to use straigh-field line coordinates (PEST) (default: False).
+            * use_nfp : bool
+                Whether the field periods of the stellarator should be used in the mapping, i.e. phi = 2*pi*eta3 / nfp (piece of cake) (default: True).
+            * Nel : tuple[int]
+                Number of cells in each direction used for interpolation of the mapping (default: (16, 16, 16)).   
+            * p : tuple[int]
+                Spline degree in each direction used for interpolation of the mapping (default: (3, 3, 3)).
+
+    Note
+    ----
+    In the parameter .yml, use the following in the section `mhd_equilibrium`::
+
+        mhd_equilibrium :
+            type : GVECequilibrium
+            GVECequilibrium : 
+                rel_path : True # whether file path is relative to "<struphy_path>/fields_background/mhd_equil/gvec", or the absolute path
+                dat_file : '/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat' # path to gvec .dat output file 
+                json_file : null # give directly the parsed json file, if it exists (then dat_file is not used)
+                use_pest : False # whether to use straight-field line coordinates (PEST)
+                use_nfp : True # whether to use the field periods of the stellarator in the mapping, i.e. phi = 2*pi*eta3 / nfp (piece of cake).
+                Nel : [32, 32, 32] # number of cells in each direction used for interpolation of the mapping.
+                p : [3, 3, 3] # spline degree in each direction used for interpolation of the mapping.
+    """
 
     def __init__(self, show=False, **params):
 
         from struphy.geometry.base import interp_mapping
         from struphy.geometry.domains import Spline
 
         from gvec_to_python.reader.gvec_reader import create_GVEC_json
```

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini` & `struphy-2.0.1/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/geometry/base.py` & `struphy-2.0.1/src/struphy/geometry/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,14 +597,15 @@
 
             # remove holes
             out = out[:, :, :n_inside]
 
             if transposed:
                 out = np.transpose(out, axes=(1, 0, 2))
 
+            # change size of "out" depending on which metric coeff has been evaluated
             if which == 0 or which == -1:
                 out = out[:, 0, :]
                 if change_out_order:
                     out = np.transpose(out, axes=(1, 0))
             elif which == 2:
                 out = out[0, 0, :]
             else:
```

### Comparing `struphy-2.0.0/src/struphy/geometry/kernels.py` & `struphy-2.0.1/src/struphy/geometry/kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/geometry/map_eval.py` & `struphy-2.0.1/src/struphy/geometry/map_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,15 @@
         maps.hollow_cyl(eta1, eta2, eta3,
                         params[0], params[1], params[2], f_out)
     elif kind_map == 21:
         maps.powered_ellipse(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], f_out)
     elif kind_map == 22:
         maps.hollow_torus(eta1, eta2, eta3,
-                          params[0], params[1], params[2], params[3], f_out)
-    elif kind_map == 23:
-        maps.hollow_torus_straight_field_line(eta1, eta2, eta3,
-                          params[0], params[1], params[2], params[3], f_out)
+                          params[0], params[1], params[2], params[3], params[4], f_out)
     elif kind_map == 30:
         maps.shafranov_shift(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], f_out)
     elif kind_map == 31:
         maps.shafranov_sqrt(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], f_out)
     elif kind_map == 32:
@@ -150,18 +147,15 @@
     elif kind_map == 20:
         maps.hollow_cyl_df(eta1, eta2, params[0], params[1], params[2], df_out)
     elif kind_map == 21:
         maps.powered_ellipse_df(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], df_out)
     elif kind_map == 22:
         maps.hollow_torus_df(
-            eta1, eta2, eta3, params[0], params[1], params[2], params[3], df_out)
-    elif kind_map == 23:
-        maps.hollow_torus_straight_field_line_df(
-            eta1, eta2, eta3, params[0], params[1], params[2], params[3], df_out)
+            eta1, eta2, eta3, params[0], params[1], params[2], params[3], params[4], df_out)
     elif kind_map == 30:
         maps.shafranov_shift_df(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], df_out)
     elif kind_map == 31:
         maps.shafranov_sqrt_df(
             eta1, eta2, eta3, params[0], params[1], params[2], params[3], df_out)
     elif kind_map == 32:
@@ -305,16 +299,14 @@
     elif kind_map == 21:
         dfinv_out[0, 2] = 0.
         dfinv_out[1, 2] = 0.
         dfinv_out[2, 0] = 0.
         dfinv_out[2, 1] = 0.
     elif kind_map == 22:
         dfinv_out[2, 2] = 0.
-    elif kind_map == 23:
-        dfinv_out[2, 2] = 0.
     elif kind_map == 30:
         dfinv_out[0, 2] = 0.
         dfinv_out[1, 2] = 0.
         dfinv_out[2, 0] = 0.
         dfinv_out[2, 1] = 0.
     elif kind_map == 31:
         dfinv_out[0, 2] = 0.
@@ -416,25 +408,31 @@
         g_out[2, 1] = 0.
     elif kind_map == 21:
         g_out[0, 2] = 0.
         g_out[1, 2] = 0.
         g_out[2, 0] = 0.
         g_out[2, 1] = 0.
     elif kind_map == 22:
-        g_out[0, 1] = 0.
-        g_out[0, 2] = 0.
-        g_out[1, 0] = 0.
-        g_out[1, 2] = 0.
-        g_out[2, 0] = 0.
-        g_out[2, 1] = 0.
-    elif kind_map == 23:
-        g_out[0, 2] = 0.
-        g_out[1, 2] = 0.
-        g_out[2, 0] = 0.
-        g_out[2, 1] = 0.
+        
+        # straight field line coordinates
+        if params[3] == 1.:
+            g_out[0, 2] = 0.
+            g_out[1, 2] = 0.
+            g_out[2, 0] = 0.
+            g_out[2, 1] = 0.
+        
+        # equal angle coordinates 
+        else:
+            g_out[0, 1] = 0.
+            g_out[0, 2] = 0.
+            g_out[1, 0] = 0.
+            g_out[1, 2] = 0.
+            g_out[2, 0] = 0.
+            g_out[2, 1] = 0.
+    
     elif kind_map == 30:
         g_out[0, 2] = 0.
         g_out[1, 2] = 0.
         g_out[2, 0] = 0.
         g_out[2, 1] = 0.
     elif kind_map == 31:
         g_out[0, 2] = 0.
@@ -533,25 +531,31 @@
         ginv_out[2, 1] = 0.
     elif kind_map == 21:
         ginv_out[0, 2] = 0.
         ginv_out[1, 2] = 0.
         ginv_out[2, 0] = 0.
         ginv_out[2, 1] = 0.
     elif kind_map == 22:
-        ginv_out[0, 1] = 0.
-        ginv_out[0, 2] = 0.
-        ginv_out[1, 0] = 0.
-        ginv_out[1, 2] = 0.
-        ginv_out[2, 0] = 0.
-        ginv_out[2, 1] = 0.
-    elif kind_map == 23:
-        ginv_out[0, 2] = 0.
-        ginv_out[1, 2] = 0.
-        ginv_out[2, 0] = 0.
-        ginv_out[2, 1] = 0.
+        
+        # straight field line coordinates
+        if params[3] == 1.:
+            ginv_out[0, 2] = 0.
+            ginv_out[1, 2] = 0.
+            ginv_out[2, 0] = 0.
+            ginv_out[2, 1] = 0.
+            
+        # equal angle coordinates
+        else:    
+            ginv_out[0, 1] = 0.
+            ginv_out[0, 2] = 0.
+            ginv_out[1, 0] = 0.
+            ginv_out[1, 2] = 0.
+            ginv_out[2, 0] = 0.
+            ginv_out[2, 1] = 0.
+            
     elif kind_map == 30:
         ginv_out[0, 2] = 0.
         ginv_out[1, 2] = 0.
         ginv_out[2, 0] = 0.
         ginv_out[2, 1] = 0.
     elif kind_map == 31:
         ginv_out[0, 2] = 0.
@@ -741,14 +745,19 @@
         Control points of (F_x, F_y, F_z) in case of an IGA mapping.
 
     mat_f : float[:,:,:]
         Output values.
         
     remove_outside : bool
         Whether to remove values that originate from markers outside of [0, 1]^d.
+        
+    Returns
+    -------
+    counter : int
+        How many markers have been treated (not been skipped).
     """
 
     np = shape(markers)[0]
     counter = 0
 
     for i in range(np):
```

### Comparing `struphy-2.0.0/src/struphy/geometry/mappings_fast.py` & `struphy-2.0.1/src/struphy/geometry/mappings_fast.py`

 * *Files 7% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         f_out[1] = cy[0, 0]
 
 @stack_array('b1', 'b2', 'der1', 'der2')
 def spline_2d_straight_df(eta1: float, eta2: float,
                           t1: 'float[:]', t2: 'float[:]', p: 'int[:]',
                           ind1: 'int[:,:]', ind2: 'int[:,:]',
                           cx: 'float[:,:]', cy: 'float[:,:]',
-                          lz: 'float',
+                          lz: float,
                           df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.spline_2d_straight`.
     """
 
     # mapping spans
     span1 = bsp.find_span(t1, p[0], eta1)
@@ -334,17 +334,17 @@
         df_out[1, 1] = 0.
 
     if eta1 == 0. and cy[0, 0] == cy[0, 1]:
         df_out[2, 1] = 0.
         
 @pure
 def cuboid(eta1: float, eta2: float, eta3: float,
-           l1: 'float', r1: 'float',
-           l2: 'float', r2: 'float',
-           l3: 'float', r3: 'float',
+           l1: float, r1: float,
+           l2: float, r2: float,
+           l3: float, r3: float,
            f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
     
         F_x &= l_1 + (r_1 - l_1)\,\eta_1\,, 
@@ -376,17 +376,17 @@
 
     # value =  begin + (end - begin) * eta
     f_out[0] = l1 + (r1 - l1) * eta1
     f_out[1] = l2 + (r2 - l2) * eta2
     f_out[2] = l3 + (r3 - l3) * eta3
 
 @pure
-def cuboid_df(l1: 'float', r1: 'float',
-              l2: 'float', r2: 'float',
-              l3: 'float', r3: 'float',
+def cuboid_df(l1: float, r1: float,
+              l2: float, r2: float,
+              l3: float, r3: float,
               df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.cuboid`.
     """
         
     df_out[0, 0] = r1 - l1
     df_out[0, 1] = 0.
@@ -396,15 +396,15 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = r3 - l3
 
 @pure
 def orthogonal(eta1: float, eta2: float, eta3: float,
-               lx: 'float', ly: 'float', alpha: 'float', lz: 'float',
+               lx: float, ly: float, alpha: float, lz: float,
                f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
 
         F_x &= L_x\,\left[\,\eta_1 + \\alpha\sin(2\pi\,\eta_1)\,\\right]\,, 
@@ -442,15 +442,15 @@
 
     f_out[0] = lx * (eta1 + alpha * sin(2*pi*eta1))
     f_out[1] = ly * (eta2 + alpha * sin(2*pi*eta2))
     f_out[2] = lz * eta3
 
 @pure
 def orthogonal_df(eta1: float, eta2: float,
-                  lx: 'float', ly: 'float', alpha: 'float', lz: 'float',
+                  lx: float, ly: float, alpha: float, lz: float,
                   df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.orthogonal`.
     """
 
     df_out[0, 0] = lx * (1 + alpha * cos(2*pi*eta1) * 2*pi)
     df_out[0, 1] = 0.
@@ -460,15 +460,15 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def colella(eta1: float, eta2: float, eta3: float,
-            lx: 'float', ly: 'float', alpha: 'float', lz: 'float',
+            lx: float, ly: float, alpha: float, lz: float,
             f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
     
         F_x &= L_x\,\left[\,\eta_1 + \\alpha\sin(2\pi\,\eta_1)\sin(2\pi\,\eta_2)\,\\right]\,, 
@@ -506,15 +506,15 @@
 
     f_out[0] = lx * (eta1 + alpha * sin(2*pi*eta1) * sin(2*pi*eta2))
     f_out[1] = ly * (eta2 + alpha * sin(2*pi*eta1) * sin(2*pi*eta2))
     f_out[2] = lz * eta3
 
 @pure
 def colella_df(eta1: float, eta2: float,
-               lx: 'float', ly: 'float', alpha: 'float', lz: 'float',
+               lx: float, ly: float, alpha: float, lz: float,
                df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.colella`.
     """
 
     df_out[0, 0] = lx * (1 + alpha * cos(2*pi*eta1) * sin(2*pi*eta2) * 2*pi)
     df_out[0, 1] = lx * alpha * sin(2*pi*eta1) * cos(2*pi*eta2) * 2*pi
@@ -524,15 +524,15 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def hollow_cyl(eta1: float, eta2: float, eta3: float,
-               a1: 'float', a2: 'float', lz: 'float',
+               a1: float, a2: float, lz: float,
                f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
 
         F_x &= \left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(2\pi\,\eta_2)\,, 
@@ -569,15 +569,15 @@
 
     f_out[0] = (a1 + eta1 * da) * cos(2*pi*eta2)
     f_out[1] = (a1 + eta1 * da) * sin(2*pi*eta2)
     f_out[2] = lz * eta3
 
 @pure
 def hollow_cyl_df(eta1: float, eta2: float, 
-                  a1: 'float', a2: 'float', lz: 'float', 
+                  a1: float, a2: float, lz: float, 
                   df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.hollow_cyl`.
     """
 
     da = a2 - a1
 
@@ -589,16 +589,16 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def powered_ellipse(eta1: float, eta2: float, eta3: float,
-                    rx: 'float', ry: 'float',
-                    lz: 'float', s: 'float',
+                    rx: float, ry: float,
+                    lz: float, s: float,
                     f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
         F_x &= r_x\,\eta_1^s\cos(2\pi\,\eta_2)\,, 
 
@@ -632,16 +632,16 @@
 
     f_out[0] = (eta1**s) * rx * cos(2*pi*eta2)
     f_out[1] = (eta1**s) * ry * sin(2*pi*eta2)
     f_out[2] = (eta3 * lz)
 
 @pure
 def powered_ellipse_df(eta1: float, eta2: float, eta3: float,
-                       rx: 'float', ry: 'float',
-                       lz: 'float', s: 'float',
+                       rx: float, ry: float,
+                       lz: float, s: float,
                        df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.powered_ellipse`.
     """
 
     df_out[0, 0] = (eta1**(s-1)) * rx * cos(2*pi*eta2)
     df_out[0, 1] = -2*pi * (eta1**s) * rx * sin(2*pi*eta2)
@@ -651,27 +651,27 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def hollow_torus(eta1: float, eta2: float, eta3: float,
-                 a1: 'float', a2: 'float', r0: 'float',
+                 a1: float, a2: float, r0: float, sfl: float,
                  tor_period: float,
                  f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
 
-        F_x &= \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(2\pi\,\eta_2)+R_0\\rbrace\cos(2\pi\,\eta_3)\,, 
+        F_x &= \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(\theta(\eta_1,\eta_2))+R_0\\rbrace\cos(2\pi\,\eta_3)\,, 
 
-        F_y &= - \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(2\pi\,\eta_2)+R_0\\rbrace\sin(2\pi\,\eta_3) \,, 
+        F_y &= \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(\theta(\eta_1,\eta_2))+R_0\\rbrace\sin(2\pi\,\eta_3) \,, 
 
-        F_z &= \,\,\,\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\sin(2\pi\,\eta_2)\,.
+        F_z &= \,\,\,\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\sin(\theta(\eta_1,\eta_2)) \,,
 
     Note
     ----
         Example with paramters :math:`a_1=0.2\,,a_2=1` and :math:`R_0=3`:
 
         .. image:: ../pics/mappings/hollow_torus.png
 
@@ -684,142 +684,107 @@
             Inner radius.
 
         a2 : float
             Outer radius.
 
         r0 : float
             Major radius.
+            
+        sfl : float
+            Whether to use straight field line angular parametrization (yes: 1., no: 0.).
 
         tor_period : int
             Toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
 
         f_out : array[float]
             Output: (x, y, z) = F(eta1, eta2, eta3).
     '''
 
-    da = a2 - a1
+    # straight field lines coordinates
+    if sfl == 1.:
+        
+        da = a2 - a1
+    
+        r = (a1 + eta1 * da)
+        theta = 2*arctan( sqrt( (1 + r/r0) / (1 - r/r0) ) * tan(pi*eta2))
+
+        f_out[0] = (r * cos(theta) + r0) * cos(2*pi*eta3 / tor_period)
+        f_out[1] = (r * cos(theta) + r0) * (-1) * sin(2*pi*eta3 / tor_period)
+        f_out[2] = r * sin(theta)
+    
+    # equal angle coordinates
+    else:
+    
+        da = a2 - a1
 
-    f_out[0] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * cos(2*pi*eta3 / tor_period)
-    f_out[1] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * (-1) * sin(2*pi*eta3 / tor_period)
-    f_out[2] = (a1 + eta1 * da) * sin(2*pi*eta2) 
+        f_out[0] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * cos(2*pi*eta3 / tor_period)
+        f_out[1] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * (-1) * sin(2*pi*eta3 / tor_period)
+        f_out[2] = (a1 + eta1 * da) * sin(2*pi*eta2) 
 
 @pure
 def hollow_torus_df(eta1: float, eta2: float, eta3: float,
-                    a1: 'float', a2: 'float', r0: 'float',
+                    a1: float, a2: float, r0: float, sfl: float,
                     tor_period: float,
                     df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.hollow_torus`.
     """
+    
+    # straight field lines coordinates
+    if sfl == 1.:
+        
+        da = a2 - a1
+    
+        r = (a1 + da*eta1)
 
-    da = a2 - a1
-
-    df_out[0, 0] = da * cos(2*pi*eta2) * cos(2*pi*eta3 / tor_period)
-    df_out[0, 1] = -2*pi * (a1 + eta1 * da) * sin(2*pi*eta2) * cos(2*pi*eta3 / tor_period)
-    df_out[0, 2] = -2*pi / tor_period * ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * sin(2*pi*eta3 / tor_period) 
-    df_out[1, 0] = da * cos(2*pi*eta2) * (-1) * sin(2*pi*eta3 / tor_period)
-    df_out[1, 1] = -2*pi * (a1 + eta1 * da) * sin(2*pi*eta2) * (-1) * sin(2*pi*eta3 / tor_period)
-    df_out[1, 2] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * (-1) * cos(2*pi*eta3 / tor_period) * 2*pi / tor_period
-    df_out[2, 0] = da * sin(2*pi*eta2)
-    df_out[2, 1] = (a1 + eta1 * da) * cos(2*pi*eta2) * 2*pi
-    df_out[2, 2] = 0.
-     
-@pure
-def hollow_torus_straight_field_line(eta1: float, eta2: float, eta3: float,
-                 a1: 'float', a2: 'float', r0: 'float',
-                 tor_period: float,
-                 f_out: 'float[:]'):
-    '''
-    Point-wise evaluation of
-
-    .. math::
-
-        F_x &= \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(\theta(\eta_1,\eta_2))+R_0\\rbrace\cos(2\pi\,\eta_3)\,, 
-
-        F_y &= \lbrace\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\cos(\theta(\eta_1,\eta_2))+R_0\\rbrace\sin(2\pi\,\eta_3) \,, 
-
-        F_z &= \,\,\,\left[\,a_1 + (a_2-a_1)\,\eta_1\,\\right]\sin(\theta(\eta_1,\eta_2)) \,,
-
-    Note
-    ----
-        No example plot yet.
-
-    Parameters
-    ----------
-        eta1, eta2, eta3 : float
-            Logical coordinate in [0, 1].
-
-        a1 : float
-            Inner radius.
+        eps = r/r0
+        eps_p = da/r0
 
-        a2 : float
-            Outer radius.
+        tpe = tan(pi*eta2)
+        tpe_p = pi/cos(pi*eta2)**2
 
-        r0 : float
-            Major radius.
+        g = sqrt((1 + eps)/(1 - eps))
+        g_p = 1/(2*g) * (eps_p*(1 - eps) + (1 + eps)*eps_p)/(1 - eps)**2
 
-        tor_period : int
-            Toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
+        theta = 2*arctan(g*tpe)
 
-        f_out : array[float]
-            Output: (x, y, z) = F(eta1, eta2, eta3).
-    '''
+        dtheta_deta1 = 2/(1 + (g*tpe)**2)*g_p*tpe
+        dtheta_deta2 = 2/(1 + (g*tpe)**2)*g*tpe_p
 
-    da = a2 - a1
-    
-    r = (a1 + eta1 * da)
-    theta = 2*arctan( sqrt( (1 + r/r0) / (1 - r/r0) ) * tan(pi*eta2))
+        df_out[0, 0] = (da * cos(theta) - r * sin(theta) * dtheta_deta1) * cos(2*pi*eta3 / tor_period)
+        df_out[0, 1] = -r * sin(theta) * dtheta_deta2 * cos(2*pi*eta3 / tor_period)
+        df_out[0, 2] = -2*pi / tor_period * (r * cos(theta) + r0) * sin(2*pi*eta3 / tor_period)
 
-    f_out[0] = (r * cos(theta) + r0) * cos(2*pi*eta3 / tor_period)
-    f_out[1] = (r * cos(theta) + r0) * (-1) * sin(2*pi*eta3 / tor_period)
-    f_out[2] = r * sin(theta) 
-       
-@pure
-def hollow_torus_straight_field_line_df(eta1: float, eta2: float, eta3: float,
-                    a1: 'float', a2: 'float', r0: 'float',
-                    tor_period: float,
-                    df_out: 'float[:,:]'):
-    """
-    Jacobian matrix for :meth:`struphy.geometry.mappings_fast.hollow_torus_straight_field_line`.
-    """
+        df_out[1, 0] = (da * cos(theta) - r * sin(theta) * dtheta_deta1) * (-1) * sin(2*pi*eta3 / tor_period)
+        df_out[1, 1] = -r * sin(theta) * dtheta_deta2 * (-1) * sin(2*pi*eta3 / tor_period)
+        df_out[1, 2] = 2*pi / tor_period * (r * cos(theta) + r0) * (-1) * cos(2*pi*eta3 / tor_period)
 
-    da = a2 - a1
-    
-    r = (a1 + da*eta1)
-    
-    eps = r/r0
-    eps_p = da/r0
-    
-    tpe = tan(pi*eta2)
-    tpe_p = pi/cos(pi*eta2)**2
-    
-    g = sqrt((1 + eps)/(1 - eps))
-    g_p = 1/(2*g) * (eps_p*(1 - eps) + (1 + eps)*eps_p)/(1 - eps)**2
-    
-    theta = 2*arctan(g*tpe)
-    
-    dtheta_deta1 = 2/(1 + (g*tpe)**2)*g_p*tpe
-    dtheta_deta2 = 2/(1 + (g*tpe)**2)*g*tpe_p
+        df_out[2, 0] = (da * sin(theta) + r * cos(theta) * dtheta_deta1)
+        df_out[2, 1] = r * cos(theta) * dtheta_deta2
+        df_out[2, 2] = 0.
+        
+    # equal angle coordinates
+    else:
 
-    df_out[0, 0] = (da * cos(theta) - r * sin(theta) * dtheta_deta1) * cos(2*pi*eta3 / tor_period)
-    df_out[0, 1] = -r * sin(theta) * dtheta_deta2 * cos(2*pi*eta3 / tor_period)
-    df_out[0, 2] = -2*pi / tor_period * (r * cos(theta) + r0) * sin(2*pi*eta3 / tor_period)
-    
-    df_out[1, 0] = (da * cos(theta) - r * sin(theta) * dtheta_deta1) * (-1) * sin(2*pi*eta3 / tor_period)
-    df_out[1, 1] = -r * sin(theta) * dtheta_deta2 * (-1) * sin(2*pi*eta3 / tor_period)
-    df_out[1, 2] = 2*pi / tor_period * (r * cos(theta) + r0) * (-1) * cos(2*pi*eta3 / tor_period)
+        da = a2 - a1
 
-    df_out[2, 0] = (da * sin(theta) + r * cos(theta) * dtheta_deta1)
-    df_out[2, 1] = r * cos(theta) * dtheta_deta2
-    df_out[2, 2] = 0.
+        df_out[0, 0] = da * cos(2*pi*eta2) * cos(2*pi*eta3 / tor_period)
+        df_out[0, 1] = -2*pi * (a1 + eta1 * da) * sin(2*pi*eta2) * cos(2*pi*eta3 / tor_period)
+        df_out[0, 2] = -2*pi / tor_period * ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * sin(2*pi*eta3 / tor_period) 
+        df_out[1, 0] = da * cos(2*pi*eta2) * (-1) * sin(2*pi*eta3 / tor_period)
+        df_out[1, 1] = -2*pi * (a1 + eta1 * da) * sin(2*pi*eta2) * (-1) * sin(2*pi*eta3 / tor_period)
+        df_out[1, 2] = ((a1 + eta1 * da) * cos(2*pi*eta2) + r0) * (-1) * cos(2*pi*eta3 / tor_period) * 2*pi / tor_period
+        df_out[2, 0] = da * sin(2*pi*eta2)
+        df_out[2, 1] = (a1 + eta1 * da) * cos(2*pi*eta2) * 2*pi
+        df_out[2, 2] = 0.
 
 @pure
 def shafranov_shift(eta1: float, eta2: float, eta3: float,
-                    rx: 'float', ry: 'float',
-                    lz: 'float', de: 'float',
+                    rx: float, ry: float,
+                    lz: float, de: float,
                     f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
 
         F_x &= r_x\,\eta_1\cos(2\pi\,\eta_2)+(1-\eta_1^2)r_x\Delta\,, 
@@ -854,16 +819,16 @@
 
     f_out[0] = (eta1 * rx) * cos(2*pi*eta2) + (1-eta1**2) * rx * de
     f_out[1] = (eta1 * ry) * sin(2*pi*eta2)
     f_out[2] = (eta3 * lz)
 
 @pure
 def shafranov_shift_df(eta1: float, eta2: float, eta3: float,
-                       rx: 'float', ry: 'float',
-                       lz: 'float', de: 'float',
+                       rx: float, ry: float,
+                       lz: float, de: float,
                        df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.shafranov_shift`.
     """
 
     df_out[0, 0] = rx * cos(2*pi*eta2) - 2 * eta1 * rx * de
     df_out[0, 1] = -2*pi * (eta1 * rx) * sin(2*pi*eta2)
@@ -873,16 +838,16 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def shafranov_sqrt(eta1: float, eta2: float, eta3: float,
-                   rx: 'float', ry: 'float',
-                   lz: 'float', de: 'float',
+                   rx: float, ry: float,
+                   lz: float, de: float,
                    f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
 
         F_x &= r_x\,\eta_1\cos(2\pi\,\eta_2)+(1-\sqrt \eta_1)r_x\Delta\,, 
@@ -915,16 +880,16 @@
 
     f_out[0] = (eta1 * rx) * cos(2*pi*eta2) + (1-sqrt(eta1)) * rx * de
     f_out[1] = (eta1 * ry) * sin(2*pi*eta2)
     f_out[2] = (eta3 * lz)
 
 @pure
 def shafranov_sqrt_df(eta1: float, eta2: float, eta3: float,
-                      rx: 'float', ry: 'float',
-                      lz: 'float', de: 'float',
+                      rx: float, ry: float,
+                      lz: float, de: float,
                       df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.shafranov_sqrt`.
     """
 
     df_out[0, 0] = rx * cos(2*pi*eta2) - 0.5 / sqrt(eta1) * rx * de
     df_out[0, 1] = -2*pi * (eta1 * rx) * sin(2*pi*eta2)
@@ -934,16 +899,16 @@
     df_out[1, 2] = 0.
     df_out[2, 0] = 0.
     df_out[2, 1] = 0.
     df_out[2, 2] = lz
 
 @pure
 def shafranov_dshaped(eta1: float, eta2: float, eta3: float,
-                      r0: 'float', lz: 'float',
-                      dx: 'float', dy: 'float', dg: 'float', eg: 'float', kg: 'float',
+                      r0: float, lz: float,
+                      dx: float, dy: float, dg: float, eg: float, kg: float,
                       f_out: 'float[:]'):
     '''
     Point-wise evaluation of
 
     .. math::
     
         x &= R_0\left[1 + (1 - \eta_1^2)\Delta_x + \eta_1\epsilon\cos(2\pi\,\eta_2 + \\arcsin(\delta)\eta_1\sin(2\pi\,\eta_2)) \\right]\,, 
@@ -991,16 +956,16 @@
     f_out[0] = r0 * (1 + (1 - eta1**2) * dx + eg *
                           eta1 * cos(2*pi*eta2 + arcsin(dg)*eta1*sin(2*pi*eta2)))
     f_out[1] = r0 * ((1 - eta1**2) * dy + eg * kg * eta1 * sin(2*pi*eta2))
     f_out[2] = (eta3 * lz)
 
 @pure
 def shafranov_dshaped_df(eta1: float, eta2: float, eta3: float,
-                         r0: 'float', lz: 'float',
-                         dx: 'float', dy: 'float', dg: 'float', eg: 'float', kg: 'float',
+                         r0: float, lz: float,
+                         dx: float, dy: float, dg: float, eg: float, kg: float,
                          df_out: 'float[:,:]'):
     """
     Jacobian matrix for :meth:`struphy.geometry.mappings_fast.shafranov_dshaped`.
     """
 
     df_out[0, 0] = r0 * (- 2 * dx * eta1 - eg * eta1 * sin(2*pi*eta2) * arcsin(dg) * sin(eta1 * sin(2*pi*eta2) * arcsin(dg) + 2*pi*eta2) + eg * cos(eta1 * sin(2*pi*eta2) * arcsin(dg) + 2*pi*eta2))
     df_out[0, 1] = - r0 * eg * eta1 * (2*pi*eta1 * cos(2*pi*eta2) * arcsin(dg) + 2*pi) * sin(eta1 * sin(2*pi*eta2) * arcsin(dg) + 2*pi*eta2)
```

### Comparing `struphy-2.0.0/src/struphy/geometry/transform.py` & `struphy-2.0.1/src/struphy/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/geometry/utilities.py` & `struphy-2.0.1/src/struphy/geometry/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/initial/analytic.py` & `struphy-2.0.1/src/struphy/initial/analytic.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/initial/base.py` & `struphy-2.0.1/src/struphy/initial/base.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/initial/eigenfunctions.py` & `struphy-2.0.1/src/struphy/initial/eigenfunctions.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/initial/initialize.py` & `struphy-2.0.1/src/struphy/initial/initialize.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/initial/perturbations.py` & `struphy-2.0.1/src/struphy/initial/perturbations.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/batch_cobra.sh` & `struphy-2.0.1/src/struphy/io/batch/batch_cobra.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_016.sh` & `struphy-2.0.1/src/struphy/io/batch/p_016.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_032.sh` & `struphy-2.0.1/src/struphy/io/batch/p_032.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_064.sh` & `struphy-2.0.1/src/struphy/io/batch/p_064.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_128.sh` & `struphy-2.0.1/src/struphy/io/batch/p_128.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_256.sh` & `struphy-2.0.1/src/struphy/io/batch/p_256.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/batch/p_512.sh` & `struphy-2.0.1/src/struphy/io/batch/p_512.sh`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_TAE_tokamak.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_TAE_tokamak.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 time : 
     dt         : 0.02  # time step
     Tend       : 20. # simulation time interval is [0, Tend]
     split_algo : Strang # LieTrotter | Strang
 
 geometry : 
-    type : HollowTorusStraightFieldLine # mapping F (possible types seen below)  
-    HollowTorusStraightFieldLine :
-        a1       : 0.1 # inner radius
-        a2       : 1.0 # minor radius
-        R0       : 5.0 # major radius
+    type : HollowTorus # mapping F (possible types seen below)  
+    HollowTorus :
+        a1  : 0.1 # inner radius
+        a2  : 1.0 # minor radius
+        R0  : 5.0 # major radius
+        sfl : True # straight field line coordinates?
         tor_period : 2 # toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
             
 mhd_equilibrium : 
     type : AdhocTorus # (possible choices seen below)
     AdhocTorus :
         a       : 1. # minor radius
         R0      : 5. # major radius
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 units : # units not stated here can be viewed via "struphy units -h"
     x  : 1. # length scale unit in m
     B  : 1. # magnetic field unit in T
     n  : 1. # number density unit in 10^20 m^(-3)
 
 time :
-    dt         : 0.2  # time step
+    dt         : 0.1  # time step
     Tend       : 100. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Tokamak # mapping F (possible types seen below)
     Tokamak :
         Nel        : [28, 72] # number of poloidal grid cells, >p
@@ -57,23 +57,24 @@
             Np      : 4 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : 2.0 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1608 # seed for random number generator
                 moments : [0., 0., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
                 initial : [[.501, 0.001, 0.001,  1.935 , -1.72], # counter-passing particle
                            [.501, 0.001, 0.001, -1.935 , -1.72], # co-passing particle
                            [.501, 0.001, 0.001,  0.4515, -1.72], # counter-trapped particle
                            [.501, 0.001, 0.001, -0.6665, -1.72]] # co-trapped particle
 
         init :
             type : Maxwellian5DUniform
             Maxwellian5DUniform:
                 n : 0.05
         save_data :
             n_markers : 4 # number of markers to be save during simulation
         push_algos :
             integrator : implicit # explicit or implicit
-            method : discrete_gradients # possible choices: discrete_gradients, discrete_gradients_faster, forward_euler, heun2, rk2, heun3, rk4
-            maxiter : 10
-            tol : 1.e-15
+            method : discrete_gradients_Itoh_Newton # possible choices: discrete_gradients, discrete_gradients_faster, discrete_gradients_Itoh_Newton, forward_euler, heun2, rk2, heun3, rk4
+            maxiter : 5
+            tol : 1.e-10
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
             ppc     : 800 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
                 u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [6, 6, 6] # quadrature points per grid cell
     nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
-units : # units not stated here can be viewed via "struphy units -h"
-    x : 1. # length scale unit in m
-    B : 1. # magnetic field unit in T
-    n : 0.0005185219355 # number density unit in 10^20 m^(-3)
-
-time :
-    dt         : 0.2  # time step
-    Tend       : 120. # simulation time interval is [0, Tend]
+units :
+    x  : 1. # length scale unit in m
+    B  : 1. # magnetic field unit in T
+    n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
+
+time : 
+    dt         : 0.1  # time step
+    Tend       : .5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
@@ -30,15 +30,15 @@
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
         B0z  : 1. # magnetic field in z
-        beta : 0. # plasma beta = 2*p*mu_0/B^2
+        beta : 0.1 # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
 em_fields :
     init :
         type : null # initial conditions (possible types seen below)
 
 fluid :
@@ -80,14 +80,15 @@
             ppc     : 800 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
                 u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_linearextendedmhd.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_linearextendedmhd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 units : # units not stated here can be viewed via "struphy units -h"
     x      : 1. # length scale unit in m
     B      : 1. # magnetic field unit in T
     n      : 1. # number density unit in 10^20 m^(-3)
 
 time :
-    dt         : 0.01 # time step
+    dt         : 0.0001 # time step
     Tend       : 18. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1 : 0. # start of interval in eta1
@@ -65,15 +65,15 @@
         maxiter : 3000
         info : False
         verbose : False
     solver_2 :
         type : PBiConjugateGradientStab
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
-        maxiter : 3000
+        maxiter : 30000
         info : False
         verbose : False
     solver_3 :
         type : PBiConjugateGradientStab
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_linearmhd.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_linearmhd.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,119 +1,140 @@
+# Landau damping with the following initial distribution function
+# 
+#     f(t=0,x,v) = 1 / [(2*pi)^(3/2) * sigma^3] \
+#                   * exp(- (v1^2 + v2^2 + v3^2) / (2 * sigma^2)) \
+#                   * (1 + alpha * cos(kx))
+# 
+# With parameters sigma = 1, k = 0.5, and alpha = 0.5.
+# 
+# The magnetic field is initialized as zero: B(t=0,x) = 0
+# and the electric field obtained from solving the Poisson equation.
+
 grid :
-    Nel      : [2, 2, 64] # number of grid cells, >p
-    p        : [1, 1, 3]  # spline degree
+    Nel      : [128, 2, 2] # number of grid cells, >p
+    p        : [3, 1, 1]  # spline degree
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [2, 2, 2] # quadrature points per grid cell
     nq_pr    : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
 units :
-    x   : 1. # length scale unit in m
+    x   : 0.0017045090240267625 # c * m_e / e
     B   : 1. # magnetic field unit in T
-    n   : 1. # bulk number density unit in 1 x 10^20 m^(-3)
+    n   : 0.09719853837468743 # eps_0 / m_e / 1e20 # bulk number density unit in 1 x 10^20 m^(-3)
 
 time :
-    dt         : 0.01 # time step
-    Tend       : 30. # simulation time interval is [0, Tend]
+    dt         : 0.05 # time step
+    Tend       : 50. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
-        l1       : 0. # start of interval in eta1
-        r1       : 2. # end of interval in eta1, r1>l1
-        l2       : 0. # start of interval in eta2
-        r2       : 2. # end of interval in eta2, r2>l2
-        l3       : 0. # start of interval in eta3
-        r3       : 20. # end of interval in eta3, r3>l3
+        l1       : 0. 
+        r1       : 12.566370614359172 # 2*pi / k_1
+        l2       : 0.
+        r2       : 1.
+        l3       : 0.
+        r3       : 1.
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
-        B0x  : 0.5 # magnetic field in x
+        B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
-        B0z  : 1.4 # magnetic field in z
+        B0z  : 0. # magnetic field in z
         beta : 0. # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
 electric_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         phi0  : 1. # constant electric potential
 
 em_fields :
     init :
         type : null # initial conditions (possible types seen below)
 
 kinetic :
     electrons :
+        phys_params :
+            A : 0.0005446170214876324  # electron mass number in units of proton mass
+            Z : -1 # signed charge number in units of elementary charge
         markers :
             type    : delta_f # full_f, control_variate, or delta_f
-            Np      : 5000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
-            eps     : 0.5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
+            Np      : 100000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
+            eps     : 0.25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
-                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                moments       : [0., 0., 0., 1.4, 1.4, 1.4] # moments of Gaussian s3, see background/moms_spec
+                spatial       : uniform # uniform or disc
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
                     n0 : 0.
                     perturbation :
-                        # l : [0.07957747154594767] # 0.5 / (2 * pi)
-                        l : [5]
+                        l : [1]
                         m : [0]
                         n : [0]
                         amps_sin : [0.]
                         amps_cos : [0.5]
                 u1 :
                     u01 : 0.
                 u2 :
                     u02 : 0.
                 u3 :
                     u03 : 0.
                 vth1 :
-                    vth01 : 2.
+                    vth01 : 1.4142135623730951 # sqrt(2)
                 vth2 :
-                    vth02 : 2.
+                    vth02 : 1.4142135623730951 # sqrt(2)
                 vth3 :
-                    vth03 : 2.
+                    vth03 : 1.4142135623730951 # sqrt(2)
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
                 u1 : 0.
                 u2 : 0.
                 u3 : 0.
-                vth1 : 2.
-                vth2 : 2.
-                vth3 : 2.
+                vth1 : 1.4142135623730951 # sqrt(2)
+                vth2 : 1.4142135623730951 # sqrt(2)
+                vth3 : 1.4142135623730951 # sqrt(2)
         save_data :
-            n_markers : 10 # number of markers to be saved during simulation
+            n_markers : 1 # number of markers to be saved during simulation
             f :
-                slices : [e3, v1_v2] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
-                n_bins : [[64], [64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
-                ranges : [[[0., 1.]], [[-5., 5.], [-5., 5.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
+                slices : [e1, v1] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
+                n_bins : [[64], [64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
+                ranges : [[[0., 1.]], [[-2., 2.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
 
 solvers :
+    solver_poisson :
+        type : PConjugateGradient
+        pc : MassMatrixPreconditioner
+        tol : 1.e-10
+        maxiter : 3000
+        info : False
+        verbose : False
     solver_ew :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or name of preconditioner class
+        pc : MassMatrixPreconditioner
         tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
     solver_eb :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or name of preconditioner class
+        pc : MassMatrixPreconditioner
         tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_linvlasovmaxwell_streaming_weibel.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# The Weibel instability with the following initial distribution function
+# The streaming Weibel instability with the following initial distribution function
 # 
-#     f(t=0,x,v) = 1 / [(2*pi)^(3/2) * sigma1 * sigma2 * sigma3] \
-#                   * exp(- v1^2/(2 * sigma1^2) - v2^2/(2 * sigma2^2) - v3^2/(2 * sigma3^2)) \
-#                   * [1 + alpha * cos(k*x)]
+#     f(t=0,x,v) = 1 / [(2*pi)^(3/2) * sigma^3] \
+#                   * exp(- v1^2/(2 * sigma^2)) \
+#                   * delta * exp(- (v2 - u1)^2/(2 * sigma^2) \
+#                   * (1 - delta) * exp(- (v2 - u2)^2/(2 * sigma^2)) \
+#                   * exp(- v3^2/(2 * sigma^2)) \
 # 
 # and magnetic field in z-direction
 # 
-#     B_3(t=0,x) = beta * cos(k*x)
+#     B_3(t=0,x) = beta * sin(k*x)
 # 
-# with sigma1 = 0.02/sqrt{2}, sigma2 = sqrt{12}*sigma1, sigma3 = sigma1, k = (1.25,0,0)^T,
-# alpha=0, beta = -10^{-4}
+# with sigma = 0.1/sqrt{2}, k = (0.2,0,0)^T, beta = -10^{-3}, delta = 1/6, u1 = 0.5, u2 = -0.1
 
 grid :
-    Nel       : [32, 2, 2] # number of grid cells, >p
+    Nel       : [128, 2, 2] # number of grid cells, >p
     p         : [3, 1, 1]  # spline degree
     spl_kind  : [True, True, True] # spline type: True=periodic, False=clamped
     bc        : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el     : [2, 2, 2] # quadrature points per grid cell
     nq_pr     : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck  : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
 units :
     x   : 0.0017045090240267625 # c * m_e / e
     B   : 1. # magnetic field unit in T
     n   : 0.09719853837468743 # eps_0 / m_e / 1e20 # bulk number density unit in 1 x 10^20 m^(-3)
 
 time :
-    dt         : 0.05 # time step
-    Tend       : 2. # simulation time interval is [0, Tend]
+    dt         : 0.01 # time step
+    Tend       : 50. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1       : 0. 
-        r1       : 5.026548245743669 # 2*pi / k_1
-        # r1       : 1.
+        r1       : 31.41592653589793 # 2*pi / k_1
         l2       : 0.
         r2       : 1.
         l3       : 0.
         r3       : 1.
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
@@ -54,75 +54,67 @@
 electric_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         phi0  : 1. # constant electric potential
 
 em_fields :
     init :
-        type : ModesCos # initial conditions (possible types seen below)
-        ModesCos :
+        type : ModesSin # initial conditions (possible types seen below)
+        ModesSin :
             coords : 'physical' # in which coordinates (logical or physical)
             comps :
                 e_field : [False, False, False]  # components to be initialized (for scalar fields: no list)
                 b_field : [False, False, True] # components to be initialized (for scalar fields: no list)
-            # variation_in : e1 # noise variation (logical space): e1, e2, e3 (1d), e1e2, e1e3, e2e3 (2d), e1e2e3 (3d)
             ls : [1.]
             ms : [0]
             ns : [0.]
-            amp : [-0.0001] # amplitudes of each mode
-            Lx : 5.026548245743669
+            amp : [-0.001] # amplitudes of each mode
+            Lx : 31.41592653589793
 
 kinetic :
     electrons :
         phys_params :
             A : 0.0005446170214876324  # electron mass number in units of proton mass
             Z : -1 # signed charge number in units of elementary charge
         markers :
             type    : delta_f # full_f, control_variate, or delta_f
-            Np      : 100000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
+            Np      : 2000000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
             eps     : 0.25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism
                 seed    : 4247 # seed for random number generator
-                moments : [0., 0., 0., 0.01, 0.03, 0.01] # moments of Gaussian s3, see background/moms_spec
+                moments : [0., 0., 0., 0.1, 0.1, 0.1] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
                     n0 : 0 # here 0 because we want to initialize f1
-                    perturbation :
-                        l : [1.]
-                        # l : [1.1989436788648692] # 1.25 / (2 * pi)
-                        m : [0.]
-                        n : [0.]
-                        amps_sin : [0.]
-                        amps_cos : [0.000] # alpha / [sqrt(2*pi)^3 * simga1 * simga2 * sigma3]
                 u1 :
                     u01 : 0.
                 u2 :
                     u02 : 0.
                 u3 :
                     u03 : 0.
                 vth1 :
-                    vth01 : 0.02 # 0.02 / sqrt(2) * sqrt(2)
+                    vth01 : 0.1
                 vth2 :
-                    vth02 : 0.06928203230275509 # 0.02 * sqrt(6) * sqrt(2)
+                    vth02 : 0.1
                 vth3 :
-                    vth03 : 0.02 # 0.02 / sqrt(2) * sqrt(2)
+                    vth03 : 0.1
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
                 u1 : 0.
                 u2 : 0.
                 u3 : 0.
-                vth1 : 0.02 # 0.02 / sqrt(2) * sqrt(2)
-                vth2 : 0.06928203230275509 # 0.02 * sqrt(6) * sqrt(2)
-                vth3 : 0.02 # 0.02 / sqrt(2) * sqrt(2)
+                vth1 : 0.1
+                vth2 : 0.1
+                vth3 : 0.1
         save_data :
             n_markers : 1 # number of markers to be saved during simulation
             f :
                 slices : [e1, v1_v2] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[64], [64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[0., 1.]], [[-0.1, 0.1], [-0.1, 0.1]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_maxwell.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_maxwell.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/examples/params_orbits_tokamak.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_orbits_tokamak.yml`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             Np      : 4 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : 2.0 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1608 # seed for random number generator
                 moments : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
                 initial : [[.501, 0.001, 0.001, 0.,  0.0450, -0.04], # co-passing particle
                            [.501, 0.001, 0.001, 0., -0.0450, -0.04], # counter passing particle
                            [.501, 0.001, 0.001, 0.,  0.0105, -0.04], # co-trapped particle
                            [.501, 0.001, 0.001, 0., -0.0155, -0.04]] # counter-trapped particle
         init : 
             type : Maxwellian6DUniform
         save_data :
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             Np      : 4 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : 1.0 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1608 # seed for random number generator
                 moments : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
                 initial : [[.52, 0.001, 0.001, 0., -0.0750, -0.06], # counter-passing particle
                            [.52, 0.001, 0.001, 0.,  0.0400, -0.06], # co-passing particle
                            [.52, 0.001, 0.001, 0., -0.0225, -0.06], # counter-trapped particle
                            [.52, 0.001, 0.001, 0.,  0.0125, -0.06]] # co-trapped particle
         init : 
             type : Maxwellian6DUniform
         background :
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             eps     : 0.25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
                 moments       : [0., 0., 0., 0.1, 0.1, 0.1] # moments of Gaussian s3, see background/moms_spec
+                spatial       : uniform # uniform or disc
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
                     n0 : 0.
                 u1 :
                     u01 : 0.
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_hybrid_fA.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_hybrid_fA.yml`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,16 @@
             ppc         : 20  # particles per 3d grid cell
             eps         : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type     : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism 
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
-                moments   : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial       : uniform # uniform or disc
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
                 u1 : 0.
                 u2 : 0.
                 u3 : 0.
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
         B0z  : 1. # magnetic field in z
-        beta : 0. # plasma beta = 2*p*mu_0/B^2
+        beta : .1 # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
 em_fields :
     init :
         type : null # type of initialization
 
 fluid :
@@ -80,14 +80,15 @@
             Np      : 6400 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
                 u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 mhd_equilibrium : 
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
         B0z  : 1. # magnetic field in z
-        beta : 0. # plasma beta = 2*p*mu_0/B^2
+        beta : 0.1 # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
 em_fields : 
     init :
         type : null # type of initialization
 
 fluid : 
@@ -80,14 +80,15 @@
             ppc     : 10 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init : 
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
                 u3 : 2.5
         background :
             type : Maxwellian6DUniform
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             Np      : 6400 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init : 
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
         push_algos :
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml` & `struphy-2.0.1/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [6, 6, 6] # quadrature points per grid cell
     nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
-units :
-    x  : 1. # length scale unit in m
-    B  : 1. # magnetic field unit in T
-    n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-
-time : 
-    dt         : 0.1  # time step
-    Tend       : .5 # simulation time interval is [0, Tend]
+units : # units not stated here can be viewed via "struphy units -h"
+    x : 1. # length scale unit in m
+    B : 1. # magnetic field unit in T
+    n : 0.0005185219355 # number density unit in 10^20 m^(-3)
+
+time :
+    dt         : 0.2  # time step
+    Tend       : 120. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
@@ -80,14 +80,15 @@
             ppc     : 800 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
             eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
                 type    : pseudo_random # particle loading mechanism
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                spatial : uniform # uniform or disc
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
                 u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_linearmhd.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd_gvec.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_linearmhd_gvec.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml`

 * *Files 3% similar despite different names*

```diff
@@ -64,44 +64,45 @@
             eps     : .5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
                 moments       : [0., 0., 0., 0.1, 0.1, 0.1] # moments of Gaussian s3, see background/moms_spec
+                spatial       : uniform # uniform or disc
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
                     n0 : 0.2
                     perturbation :
                         l : [1]
                         m : [0]
                         n : [0]
                         amps_sin : [0.]
                         amps_cos : [0.05]
                 u1 :
-                    u01 : 0.1
+                    u01 : 0.0
                 u2 :
-                    u02 : 0.1
+                    u02 : 0.0
                 u3 :
-                    u03 : 0.1
+                    u03 : 0.0
                 vth1 :
                     vth01 : 0.1
                 vth2 :
                     vth02 : 0.1
                 vth3 :
                     vth03 : 0.1
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.2
-                u1 : 0.1
-                u2 : 0.1
-                u3 : 0.1
+                u1 : 0.0
+                u2 : 0.0
+                u3 : 0.0
                 vth1 : 0.1
                 vth2 : 0.1
                 vth3 : 0.1
         save_data :
             n_markers : 3 # number of markers to be save during simulation
             f :
                 slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
```

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_1.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_maxwell_1.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_2.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/params_maxwell_2.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/strscl.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/strscl.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_1.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_1.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_2.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_2.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_3.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_3.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_4.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_4.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_5.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_5.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_6.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_6.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_7.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_7.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_8.yml` & `struphy-2.0.1/src/struphy/io/inp/tests/wkscl_8.yml`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/kinetic_background/analytical.py` & `struphy-2.0.1/src/struphy/kinetic_background/maxwellians.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,146 +1,44 @@
-from abc import ABCMeta, abstractmethod
 import numpy as np
 
+from struphy.kinetic_background.base import Maxwellian
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 
-class Maxwellian(metaclass=ABCMeta):
-    r"""
-    Base class for a Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^n, n \geq 1,` 
-    with logical position coordinates :math:`\boldsymbol{\eta} \in [0, 1]^3`:
-
-    .. math::
-
-        f(\boldsymbol{\eta}, v_1,\ldots,v_n) = n(\boldsymbol{\eta}) \prod_{i=1}^n \frac{1}{\sqrt{\pi}\,v_{\mathrm{th},i}(\boldsymbol{\eta})}
-        \exp\left[-\frac{(v_i-u_i(\boldsymbol{\eta}))^2}{v_{\mathrm{th},i}(\boldsymbol{\eta})^2}\right],
-
-    defined by its velocity moments: the density :math:`n(\boldsymbol{\eta})`, 
-    the mean-velocities :math:`u_i(\boldsymbol{\eta})`, 
-    and the thermal velocities :math:`v_{\mathrm{th},i}(\boldsymbol{\eta})`. 
-    """
-
-    @property
-    @abstractmethod
-    def vdim(self):
-        """Dimension of the velocity space (vdim = n).
-        """
-        pass
-
-    @abstractmethod
-    def n(self, *etas):
-        """ Number density (0-form). 
-
-        Parameters
-        ----------
-        etas : numpy.arrays
-            Evaluation points. All arrays must be of same shape (can be 1d for flat evaluation).
-
-        Returns
-        -------
-        A numpy.array with the density evaluated at evaluation points (same shape as etas).
-        """
-        pass
-
-    @abstractmethod
-    def u(self, *etas):
-        """ Mean velocities (Cartesian components evaluated at x = F(eta)).
-
-        Parameters
-        ----------
-        etas : numpy.arrays
-            Evaluation points. All arrays must be of same shape (can be 1d for flat evaluation).
-
-        Returns
-        -------
-        A numpy.array with the mean velocity evaluated at evaluation points (one dimension more than etas).
-        The additional dimension is in the first index.
-        """
-        pass
-
-    @abstractmethod
-    def vth(self, *etas):
-        """ Thermal velocities (0-forms).
-
-        Parameters
-        ----------
-        etas : numpy.arrays
-            Evaluation points. All arrays must be of same shape (can be 1d for flat evaluation).
-
-        Returns
-        -------
-        A numpy.array with the thermal velocity evaluated at evaluation points (one dimension more than etas).
-        The additional dimension is in the first index.
-        """
-        pass
-
-    def gaussian(self, v, u=0., vth=1.):
-        """1D Gaussian, to which array-valued mean- and thermal velocities can be passed.
-
-        Parameters
-        ----------
-        v : float | array-like
-            Velocity coordinate(s).
-
-        u : float | array-like
-            Mean velocity evaluated at position array.
-
-        vth : float | array-like
-            Thermal velocity evaluated at position array, same shape as u.
-
-        Returns
-        -------
-        An array of size(u).
-        """
-
-        if isinstance(v, np.ndarray) and isinstance(u, np.ndarray):
-            assert v.shape == u.shape
-
-        return 1./(np.sqrt(np.pi) * vth) * np.exp(-(v - u)**2/vth**2)
-
-    def __call__(self, *args):
-        """
-        Evaluates the Maxwellian distribution function M(etas, v1, ..., vn).
-
-        Parameters
-        ----------
-        *args : array_like
-            Position-velocity arguments in the order etas, v1, ..., vn.
-
-        Returns
-        -------
-        f : np.ndarray
-            The evaluated Maxwellian.
-        """
-
-        res = self.n(*args[:-self.vdim])
-        us = self.u(*args[:-self.vdim])
-        vths = self.vth(*args[:-self.vdim])
-
-        for i, v in enumerate(args[-self.vdim:]):
-            res *= self.gaussian(v, u=us[i], vth=vths[i])
-
-        return res
-
-
 class Maxwellian6DUniform(Maxwellian):
     r"""
-    6d Maxwellian distribution function defined on [0, 1]^3 x R^3, with logical position and Cartesian velocity coordinates, with uniform velocity moments.
+    6d Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^3`, 
+    with logical position and Cartesian velocity coordinates and uniform velocity moments.
 
     .. math::
 
-        f(\boldsymbol{\eta}, \mathbf v) = n \, \frac{1}{\pi^{3/2} \, v_{\mathrm{th},1} \, v_{\mathrm{th},2} \, v_{\mathrm{th},3}} \,
-            \exp\left[- \frac{(v_1 - u_1)^2}{v_{\mathrm{th},1}^2}
-                      - \frac{(v_2 - u_2)^2}{v_{\mathrm{th},2}^2}
-                      - \frac{(v_3 - u_3)^2}{v_{\mathrm{th},3}^2}\right].
+        f(\mathbf v) = \frac{n}{(2\pi)^{3/2} \, v_{\mathrm{th},1} \, v_{\mathrm{th},2} \, v_{\mathrm{th},3}} \,
+            \exp\left[- \frac{(v_1 - u_1)^2}{2v_{\mathrm{th},1}^2}
+                      - \frac{(v_2 - u_2)^2}{2v_{\mathrm{th},2}^2}
+                      - \frac{(v_3 - u_3)^2}{2v_{\mathrm{th},3}^2}\right].
 
     Parameters
     ----------
     **params
         Keyword arguments (n= , u1=, etc.) defining the moments of the 6d Maxwellian.
+        
+    Note
+    ----
+    In the parameter .yml, use the following in the section ``kinetic/<species>``::
+
+        init :
+            type : Maxwellian6DUniform
+            Maxwellian6DUniform :
+                n : 1.0
+                u1 : 0.0
+                u2 : 0.0
+                u3 : 0.0
+                vth1 : 1.0
+                vth2 : 1.0
+                vth3 : 1.0
     """
 
     def __init__(self, **params):
 
         # default parameters
         params_default = {'n': 1.,
                           'u1': 0.,
@@ -219,35 +117,68 @@
         res_list += [self.params['u3'] - 0*eta1]
 
         return np.array(res_list)
 
 
 class Maxwellian6DPerturbed(Maxwellian):
     r"""
-    6d Maxwellian distribution function defined on [0, 1]^3 x R^3, with logical position and Cartesian velocity coordinates, with sin/cos perturbed velocity moments.
+    6d Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^3`, 
+    with logical position and Cartesian velocity coordinates, with sin/cos perturbed velocity moments.
 
     .. math::
 
-        f(\boldsymbol{\eta}, \mathbf v) = n(\boldsymbol{\eta})&\frac{1}{\pi^{3/2}\,v_{\mathrm{th},x}(\boldsymbol{\eta})\,v_{\mathrm{th},y}(\boldsymbol{\eta})\,v_{\mathrm{th},z}(\boldsymbol{\eta})}\,\exp\left[-\frac{(v_x-u_x(\boldsymbol{\eta}))^2}{v_{\mathrm{th},x}(\boldsymbol{\eta})^2}-\frac{(v_y-u_y(\boldsymbol{\eta}))^2}{v_{\mathrm{th},y}(\boldsymbol{\eta})^2}-\frac{(v_z-u_z(\boldsymbol{\eta}))^2}{v_{\mathrm{th},z}(\boldsymbol{\eta})^2}\right]\,,
-
-        n(\boldsymbol{\eta})&= n_0 + \sum_i\left\lbrace A_i\sin\left[2\pi(l_i\,\eta_1+m_i\,\eta_2+n_i\,\eta_3)\right] + B_i\cos\left[2\pi(l_i\,\eta_1+m_i\,\eta_2+n_i\,\eta_3)\right] \right\rbrace\,,
+        f(\boldsymbol{\eta}, \mathbf v) = \frac{n(\boldsymbol{\eta})}{(2\pi)^{3/2}(v_{\mathrm{th},x}\,v_{\mathrm{th},y}\,v_{\mathrm{th},z})(\boldsymbol{\eta})}\,\exp\left[-\frac{(v_x-u_x(\boldsymbol{\eta}))^2}{2v_{\mathrm{th},x}(\boldsymbol{\eta})^2}-\frac{(v_y-u_y(\boldsymbol{\eta}))^2}{2v_{\mathrm{th},y}(\boldsymbol{\eta})^2}-\frac{(v_z-u_z(\boldsymbol{\eta}))^2}{2v_{\mathrm{th},z}(\boldsymbol{\eta})^2}\right]\,, 
+        
+    with perturbations of the form
+    
+    .. math::
+    
+        n(\boldsymbol{\eta})= n_0 + \sum_i\left\lbrace A_i\sin\left[2\pi(l_i\,\eta_1+m_i\,\eta_2+n_i\,\eta_3)\right] + B_i\cos\left[2\pi(l_i\,\eta_1+m_i\,\eta_2+n_i\,\eta_3)\right] \right\rbrace\,,
 
-    and similarly for the other moments :math:`u_x(\boldsymbol{\eta}),u_y(\boldsymbol{\eta})`, etc..
+    and similarly for the other moments :math:`u_x(\boldsymbol{\eta}),u_y(\boldsymbol{\eta})`, etc.
 
     Parameters
     ----------
     **params
         Keyword arguments defining the moments of the 6d Maxwellian. For each moment, a dictionary of the form {'n0' : float, 'perturbation' : {'l' : list, 'm' : list, 'n' : list, 'amps_sin' : list, 'amps_cos' : list}} must be passed.
+    
+    Note
+    ----
+    In the parameter .yml, use the following in the section ``kinetic/<species>``::
+
+        init :
+            type : Maxwellian6DPerturbed
+            Maxwellian6DPerturbed :
+                n :
+                    n0 : 1.
+                    perturbation :
+                        l : [0]
+                        m : [0]
+                        n : [0]
+                        amps_sin : [0.]
+                        amps_cos : [0.]
+                u1 :
+                    u10 : 0.
+                u2 :
+                    u20 : 0.
+                u3 :
+                    u30 : 0.
+                vth1 :
+                    vth10 : 1.
+                vth2 :
+                    vth20 : 1.
+                vth3 :
+                    vth30 : 1.
     """
 
     def __init__(self, **params):
 
         moment_keys = ['n', 'u1', 'u2', 'u3', 'vth1', 'vth2', 'vth3']
 
-        backgr_keys = ['n0', 'u01', 'u02', 'u0_3', 'vth01', 'vth02', 'vth03']
+        backgr_keys = ['n0', 'u01', 'u02', 'u03', 'vth01', 'vth02', 'vth03']
 
         # set default background, mode numbers and amplitudes if no perturbation of a moment in given
         for moment_key, backgr_key in zip(moment_keys, backgr_keys):
 
             # add moment key if not there
             if moment_key not in params.keys():
                 params[moment_key] = {}
@@ -415,15 +346,15 @@
         ls = self.params['u3']['perturbation']['l']
         ms = self.params['u3']['perturbation']['m']
         ns = self.params['u3']['perturbation']['n']
 
         amps_sin = self.params['u3']['perturbation']['amps_sin']
         amps_cos = self.params['u3']['perturbation']['amps_cos']
 
-        res = self.params['u3']['u0_3']
+        res = self.params['u3']['u03']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
         return np.array(res_list)
 
@@ -483,26 +414,45 @@
         res_list += [res]
 
         return np.array(res_list)
 
 
 class Maxwellian6DITPA(Maxwellian):
     r"""
-    6d Maxwellian distribution function defined on [0, 1]^3 x R^3, with logical position and Cartesian velocity coordinates, with isotropic, shifted distribution in velocity space and 1d density variation in first direction.
+    6d Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^3`, 
+    with logical position and Cartesian velocity coordinates, with isotropic, shifted distribution in velocity space and 1d density variation in first direction.
 
     .. math::
 
-        f(\boldsymbol{\eta}, \mathbf v) = n(\eta_1)&\,\frac{1}{\pi^{3/2}\,v_{\mathrm{th}}^3}\,\exp\left[-\frac{(v_x-u_x)^2+(v_y-u_y)^2+(v_z-u_z)^2}{v_{\mathrm{th}}^2}\right]\,,
+        f(\eta_1, \mathbf v) = \,\frac{n(\eta_1)}{(2\pi)^{3/2}\,v_{\mathrm{th}}^3}\,\exp\left[-\frac{(v_x-u_x)^2+(v_y-u_y)^2+(v_z-u_z)^2}{2v_{\mathrm{th}}^2}\right]\,,
+
+    with the density profile
+
+    .. math::
 
-        n(\eta_1)& = c_3\exp\left[-\frac{c_2}{c_1}\tanh\left(\frac{\eta_1 - c_0}{c_2}\right)\right]\,.
+        n(\eta_1) = c_3\exp\left[-\frac{c_2}{c_1}\tanh\left(\frac{\eta_1 - c_0}{c_2}\right)\right]\,.
 
     Parameters
     ----------
     **params
         Keyword arguments defining the moments of the 6d Maxwellian. For the density profile a dictionary of the form {'c0' : float, 'c1' : float, 'c2' : float, 'c3' : float} must be passed.
+    
+    Note
+    ----
+    In the parameter .yml, use the following in the section ``kinetic/<species>``::
+
+        init :
+            type : Maxwellian6DITPA
+            Maxwellian6DITPA :
+                n : 
+                    c0: 0.5
+                    c1: 0.5
+                    c2: 0.5
+                    c3: 0.5
+                vth : 1.0
     """
 
     def __init__(self, **params):
 
         # set default ITPA default parameters if not given
         if 'n' not in params.keys():
             params['n'] = {}
@@ -596,24 +546,38 @@
         res_list += [0*eta1]
 
         return np.array(res_list)
 
 
 class Maxwellian5DUniform(Maxwellian):
     r"""
-    5d Maxwellian distribution function defined on [0, 1]^3 x R^2, with logical position and Cartesian velocity coordinates, with uniform velocity moments.
+    5d Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^2`, 
+    with logical position and Cartesian velocity coordinates, with uniform velocity moments.
 
     .. math::
 
-        f(\boldsymbol{\eta}, v_\parallel, v_\perp) = n(\boldsymbol{\eta})\frac{1}{\pi\,v_{\mathrm{th},\parallel}(\boldsymbol{\eta})v_{\mathrm{th},\perp}(\boldsymbol{\eta})}\exp\left[-\frac{(v_\parallel-u_\parallel(\boldsymbol{\eta}))^2}{v_{\mathrm{th},\parallel}(\boldsymbol{\eta})^2}-\frac{(v_\perp-u_\perp(\boldsymbol{\eta}))^2}{v_{\mathrm{th},\perp}(\boldsymbol{\eta})^2}}\right]. 
+        f(v_\parallel, v_\perp) = \frac{n}{2\pi\,v_{\mathrm{th},\parallel}\,v_{\mathrm{th},\perp}}\exp\left[-\frac{(v_\parallel-u_\parallel)^2}{2v_{\mathrm{th},\parallel}^2} - \frac{(v_\perp-u_\perp)^2}{2v_{\mathrm{th},\perp}^2}\right]\,.
 
     Parameters
     ----------
     **params
         Keyword arguments (n= , u_parallel=, etc.) defining the moments of the 6d Maxwellian.
+        
+    Note
+    ----
+    In the parameter .yml, use the following in the section ``kinetic/<species>``::
+
+        init :
+            type : Maxwellian5DUniform
+            Maxwellian5DUniform :
+                n : 1.0
+                u_parallel : 0.0
+                u_perp : 0.0
+                vth_parallel : 1.0
+                vth_perp : 1.0
     """
 
     def __init__(self, **params):
 
         # default parameters
         params_default = {'n': 1.,
                           'u_parallel': 0.,
```

### Comparing `struphy-2.0.0/src/struphy/kinetic_background/background_eval.py` & `struphy-2.0.1/src/struphy/kinetic_background/background_eval.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/kinetic_background/f0_kernels.py` & `struphy-2.0.1/src/struphy/kinetic_background/f0_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/kinetic_background/moments_kernels.py` & `struphy-2.0.1/src/struphy/kinetic_background/moments_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/core.py` & `struphy-2.0.1/src/struphy/linear_algebra/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -218,7 +218,77 @@
     b[1, 0] = (a[1, 2]*a[2, 0] - a[2, 2]*a[1, 0]) / det_a
     b[1, 1] = (a[2, 2]*a[0, 0] - a[0, 2]*a[2, 0]) / det_a
     b[1, 2] = (a[0, 2]*a[1, 0] - a[1, 2]*a[0, 0]) / det_a
 
     b[2, 0] = (a[1, 0]*a[2, 1] - a[2, 0]*a[1, 1]) / det_a
     b[2, 1] = (a[2, 0]*a[0, 1] - a[0, 0]*a[2, 1]) / det_a
     b[2, 2] = (a[0, 0]*a[1, 1] - a[1, 0]*a[0, 1]) / det_a
+
+@pure
+def matrix_vector4(a: 'float[:,:]', b: 'float[:]', c: 'float[:]'):
+    """
+    Performs the matrix-vector product of a 4x4 matrix with a vector.
+
+    Parameters
+    ----------
+        a : array[float]
+            The input array (matrix) of shape (4,4).
+
+        b : array[float]
+            The input array (vector) of shape (4,).
+
+        c : array[float]
+            The output array (vector) of shape (4,) which is the result of the matrix-vector product a.dot(b).
+    """
+
+    c[:] = 0.
+
+    for i in range(4):
+        for j in range(4):
+            c[i] += a[i, j] * b[j]
+
+@pure
+def matrix_matrix4(a: 'float[:,:]', b: 'float[:,:]', c: 'float[:,:]'):
+    """
+    Performs the matrix-matrix product of a 4x4 matrix with another 4x4 matrix.
+
+    Parameters
+    ----------
+        a : array[float]
+            The first input array (matrix) of shape (4,4).
+
+        b : array[float]
+            The second input array (matrix) of shape (4,4).
+
+        c : array[float]
+            The output array (matrix) of shape (4,4) which is the result of the matrix-matrix product a.dot(b).
+    """
+
+    c[:, :] = 0.
+
+    for i in range(4):
+        for j in range(4):
+            for k in range(4):
+                c[i, j] += a[i, k] * b[k, j]
+
+@pure
+def det4(a: 'float[:,:]') -> float:
+    """
+    Computes the determinant of a 4x4 matrix.
+
+    Parameters
+    ----------
+        a : array[float]
+            The input array (matrix) of shape (4,4) of which the determinant shall be computed.
+
+    Returns
+    -------
+        det_a : float
+            The determinant of the 3x3 matrix a.
+    """
+
+    plus =  a[0,0]*det(a[1:,1:])      + a[2,0]*det(a[(0,1,3),1:])
+    minus = a[1,0]*det(a[(0,2,3),1:]) + a[3,0]*det(a[:3,1:])
+
+    det_a = plus - minus
+
+    return det_a
```

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/iterative_solvers.py` & `struphy-2.0.1/src/struphy/linear_algebra/iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/linalg_kron.py` & `struphy-2.0.1/src/struphy/linear_algebra/linalg_kron.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/schur_solver.py` & `struphy-2.0.1/src/struphy/linear_algebra/schur_solver.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/stencil_dot_kernels.py` & `struphy-2.0.1/src/struphy/linear_algebra/stencil_dot_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/linear_algebra/stencil_transpose_kernels.py` & `struphy-2.0.1/src/struphy/linear_algebra/stencil_transpose_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/models/base.py` & `struphy-2.0.1/src/struphy/models/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,32 +32,45 @@
     Note
     ----
     All Struphy models are subclasses of ``StruphyModel`` and should be added to ``struphy/models/models.py``.  
     """
 
     def __init__(self, params, comm, **species):
 
-        from struphy.models.utilities import setup_domain_mhd, setup_electric_background, setup_derham
+        from struphy.models.setup import setup_domain_mhd, setup_electric_background, setup_derham
         from struphy.psydac_api.mass import WeightedMassOperators
 
         self._params = params
         self._comm = comm
         self._species = species
 
         # initialize model variable dictionaries
         self._init_variable_dicts()
 
         # compute model units
-        self._units_basic, self._units_der, self._units_dimless = self.model_units(
+        self._units, self._eq_params = self.model_units(
             self.params, verbose=False)
 
         # create domain, MHD equilibrium, background electric field
-        self._domain, self._mhd_equil = setup_domain_mhd(params)
+        self._domain, self._mhd_equil = setup_domain_mhd(
+            params, units=self.units)
         self._electric_equil = setup_electric_background(params, self.domain)
 
+        if comm.Get_rank() == 0:
+            if 'mhd_equilibrium' in params:
+                print('\nMHD EQUILIBRIUM:')
+                print('type:'.ljust(25), self.mhd_equil.__class__.__name__)
+                for key, val in self.mhd_equil.params.items():
+                    print((key + ':').ljust(25), val)
+            if 'electric_equilibrium' in params:
+                print('\nELECTRIC EQUILIBRIUM:')
+                print('type:', self.electric_equil.__class__.__name__)
+                for key, val in self.electric_equil.params.items():
+                    print((key + ':').ljust(25), val)
+
         # create discrete derham sequence
         dims_mask = params['grid']['dims_mask']
         if dims_mask is None:
             dims_mask = [True]*3
 
         self._derham = setup_derham(
             params['grid'], comm=comm, domain=self.domain, mpi_dims_mask=dims_mask)
@@ -65,18 +78,25 @@
         # create weighted mass operators
         self._mass_ops = WeightedMassOperators(
             self.derham, self.domain, eq_mhd=self.mhd_equil)
 
         # allocate memory for variables
         self._allocate_variables()
 
+        # store plasma parameters
+        if comm.Get_rank() == 0:
+            self._pparams = self.print_plasma_params()
+            print('\nOPERATOR ASSEMBLY:')
+        else:
+            self._pparams = self.print_plasma_params(verbose=False)
+
     @classmethod
     @abstractmethod
     def bulk_species(cls):
-        '''Object identifying the bulk species of the plasma. Must be a value of self.fluid or self.kinetic, or None.'''
+        '''Name of the bulk species of the plasma. Must be a key of self.fluid or self.kinetic, or None.'''
         pass
 
     @classmethod
     @abstractmethod
     def timescale(cls):
         '''String that sets the time scale unit of the model. 
         Must be one of "alfvén", "cyclotron" or "light".'''
@@ -105,14 +125,19 @@
 
     @property
     def params(self):
         '''Model parameters from :code:`parameters.yml`.'''
         return self._params
 
     @property
+    def pparams(self):
+        '''Plasma parameters for each species.'''
+        return self._pparams
+
+    @property
     def comm(self):
         '''MPI communicator.'''
         return self._comm
 
     @property
     def species(self):
         '''Species dictionary.'''
@@ -150,30 +175,24 @@
 
     @property
     def derham(self):
         '''3d Derham sequence, see :ref:`derham`.'''
         return self._derham
 
     @property
-    def units_basic(self):
-        '''Basic units of the model.
+    def units(self):
+        '''All Struphy units.
         '''
-        return self._units_basic
+        return self._units
 
     @property
-    def units_der(self):
-        '''Derived units of the model.
+    def eq_params(self):
+        '''Parameters appearing in model equation due to Struphy normalization.
         '''
-        return self._units_der
-
-    @property
-    def units_dimless(self):
-        '''Dimensionless qunatities of the model.
-        '''
-        return self._units_dimless
+        return self._eq_params
 
     @property
     def mass_ops(self):
         '''WeighteMassOperators object, see :ref:`mass_ops`.'''
         return self._mass_ops
 
     def integrate(self, dt, split_algo='LieTrotter'):
@@ -250,15 +269,15 @@
 
     def print_scalar_quantities(self):
         '''
         Print quantities saved in scalar_quantities to screen.
         '''
         sq_str = ''
         for key, val in self._scalar_quantities.items():
-            sq_str += key + ': {:15.11f}'.format(val[0]) + '     '
+            sq_str += key + ': {:14.11f}'.format(val[0]) + '   '
         print(sq_str)
 
     def initialize_from_params(self):
         """
         Set initial conditions for FE coefficients (electromagnetic and fluid) and markers according to parameter file.
         """
 
@@ -280,14 +299,16 @@
                         subval['obj'].initialize_coeffs(
                             val['params']['init'], domain=self.domain)
 
         # initialize particles
         if len(self.kinetic) > 0:
 
             for val in self.kinetic.values():
+                val['obj'].draw_markers()
+
                 val['obj'].mpi_sort_markers(do_test=True)
 
                 typ = val['params']['markers']['type']
                 if typ == 'full_f':
                     val['obj'].initialize_weights(val['params']['init'])
                 elif typ == 'delta_f':
                     val['obj'].initialize_weights(val['params']['init'])
@@ -328,14 +349,15 @@
                         subval['obj'].initialize_coeffs_from_restart_file(
                             data.file, species)
 
         # initialize particles
         if len(self.kinetic) > 0:
 
             for key, val in self.kinetic.items():
+                val['obj'].draw_markers()
                 val['obj']._markers[:, :] = data.file['restart/' + key][-1, :, :]
 
                 # important: sets holes attribute of markers!
                 val['obj'].mpi_sort_markers(do_test=True)
 
     def initialize_data_output(self, data, size):
         """
@@ -473,55 +495,76 @@
         return save_keys_all, save_keys_end
 
     ###################
     # Class methods :
     ###################
 
     @classmethod
-    def model_units(cls, params, verbose=False):
+    def model_units(cls, params, verbose=False, comm=None):
         """
-        Compute model units and print them to screen.
+        Return model units and print them to screen.
 
         Parameters
         ----------
         params : dict
             model parameters.
 
         verbose : bool, optional
             print model units to screen.
+
+        comm : obj
+            MPI communicator.
+
+        Returns
+        -------
+        units_basic : dict
+            Basic units for time, length, mass and magnetic field.
+
+        units_der : dict
+            Derived units for velocity, pressure, mass density and particle density.
         """
 
-        from struphy.models.utilities import derive_units
+        from struphy.models.setup import derive_units
+
+        # physics constants
+        e = 1.602176634e-19  # elementary charge (C)
+        mH = 1.67262192369e-27  # proton mass (kg)
+        eps0 = 8.8541878128e-12  # vacuum permittivity (F/m)
 
         x_unit = params['units']['x']
         B_unit = params['units']['B']
 
-        if verbose:
-            print('\nNumerical values of variables are expressed in the following units:')
+        if comm is None:
+            rank = 0
+        else:
+            rank = comm.Get_rank()
+
+        if verbose and rank == 0:
+            print('\nUNITS:')
             print(f'Unit of length:'.ljust(25),
                   '{:4.3e}'.format(x_unit) + ' m')
 
         # special case for model Maxwell (no plasma species)
         if cls.bulk_species() is None:
-            if verbose:
+            if verbose and rank == 0:
                 print(f'Unit of time:'.ljust(25),
                       '{:4.3e}'.format(x_unit / 299792458) + ' s')
                 print(f'Unit of velocity:'.ljust(25),
                       '{:4.3e}'.format(299792458) + ' m/s')
                 print(f'Unit of magnetic field:'.ljust(
                     25), '{:4.3e}'.format(B_unit) + ' T')
                 print(f'Unit of electric field:'.ljust(25),
                       '{:4.3e}'.format(299792458*B_unit) + ' V/m')
 
-            units_basic = {}
-            units_basic['t'] = x_unit / 299792458
-            units_basic['x'] = x_unit
-            units_basic['B'] = B_unit
+            units = {}
+            units['t'] = x_unit / 299792458
+            units['x'] = x_unit
+            units['B'] = B_unit
 
-            return units_basic, {}, {}
+            eq_params = {}
         else:
 
             # look for bulk species in fluid OR kinetic parameter dictionaries
             if 'fluid' in params:
                 if cls.bulk_species() in params['fluid']:
                     Z_bulk = params['fluid'][cls.bulk_species()
                                              ]['phys_params']['Z']
@@ -530,41 +573,72 @@
             else:
                 Z_bulk = params['kinetic'][cls.bulk_species()
                                            ]['phys_params']['Z']
                 A_bulk = params['kinetic'][cls.bulk_species()
                                            ]['phys_params']['A']
 
             # compute units
-            units_basic, units_der, units_dimless = derive_units(
+            units = derive_units(
                 Z_bulk, A_bulk, params['units']['x'], params['units']['B'], params['units']['n'], cls.timescale())
 
-            if verbose:
+            if verbose and rank == 0:
                 print(f'Unit of time:'.ljust(25),
-                      '{:4.3e}'.format(units_basic['t']) + ' s')
+                      '{:4.3e}'.format(units['t']) + ' s')
                 print(f'Unit of velocity:'.ljust(25),
-                      '{:4.3e}'.format(units_der['v']) + ' m/s')
+                      '{:4.3e}'.format(units['v']) + ' m/s')
                 print(f'Unit of magnetic field:'.ljust(25),
-                      '{:4.3e}'.format(units_basic['B']) + ' T')
+                      '{:4.3e}'.format(units['B']) + ' T')
                 print(f'Unit of particle density:'.ljust(25),
-                      '{:4.3e}'.format(units_der['n']) + ' m⁻³')
-                print(f'Unit of mass:'.ljust(25),
-                      '{:4.3e}'.format(units_basic['m']) + ' kg')
+                      '{:4.3e}'.format(units['n']) + ' m⁻³')
                 print(f'Unit of mass density:'.ljust(25),
-                      '{:4.3e}'.format(units_der['rho']) + ' kg/m³')
+                      '{:4.3e}'.format(units['rho']) + ' kg/m³')
                 print(f'Unit of pressure:'.ljust(25),
-                      '{:4.3e}'.format(units_der['p'] * 1e-5) + ' bar')
+                      '{:4.3e}'.format(units['p'] * 1e-5) + ' bar')
+
+            # compute equation parameters arising from Struphy normalization
+            eq_params = {}
+            if 'fluid' in params:
+                for species in params['fluid']:
 
-                # dimensionless quantities
-                print('\nRelevant dimensionless quantities:')
-                print(f'alpha:'.ljust(25), '{:7.3f}'.format(
-                    units_dimless['alpha']))
-                print(f'kappa:'.ljust(25), '{:7.3f}'.format(
-                    units_dimless['kappa']))
+                    Z = params['fluid'][species]['phys_params']['Z']
+                    A = params['fluid'][species]['phys_params']['A']
 
-            return units_basic, units_der, units_dimless
+                    # compute equation parameters
+                    om_p = np.sqrt(units['n'] * (Z*e)**2 / (eps0 * A*mH))
+                    om_c = Z*e * units['B'] / (A*mH)
+                    eq_params[species] = {}
+                    eq_params[species]['alpha_unit'] = om_p / om_c
+                    eq_params[species]['epsilon_unit'] = 1. / \
+                        (om_c * units['t'])
+
+                    if verbose and rank == 0:
+                        print('- ' + species + ':')
+                        for key, val in eq_params[species].items():
+                            print((key + ':').ljust(25), '{:4.3e}'.format(val))
+
+            if 'kinetic' in params:
+                for species in params['kinetic']:
+
+                    Z = params['kinetic'][species]['phys_params']['Z']
+                    A = params['kinetic'][species]['phys_params']['A']
+
+                    # compute equation parameters
+                    om_p = np.sqrt(units['n'] * (Z*e)**2 / (eps0 * A*mH))
+                    om_c = Z*e * units['B'] / (A*mH)
+                    eq_params[species] = {}
+                    eq_params[species]['alpha_unit'] = om_p / om_c
+                    eq_params[species]['epsilon_unit'] = 1. / \
+                        (om_c * units['t'])
+
+                    if verbose and rank == 0:
+                        print('- ' + species + ':')
+                        for key, val in eq_params[species].items():
+                            print((key + ':').ljust(25), '{:4.3e}'.format(val))
+
+        return units, eq_params
 
     ###################
     # Private methods :
     ###################
 
     def _init_variable_dicts(self):
         """
@@ -650,26 +724,26 @@
         # marker arrays and plasma parameters of kinetic species
         if 'kinetic' in self.params:
 
             for species, val in self.kinetic.items():
 
                 if self.params['kinetic'][species]['markers']['type'] in ['control_variate', 'delta_f']:
                     assert 'background' in self.params['kinetic'][species], \
-                        f'If a control variate or delta-f method is used, a analytical background must be given!'
+                        f'If a control variate or delta-f method is used, a maxwellians background must be given!'
 
                 kinetic_class = getattr(particles, val['space'])
 
                 val['obj'] = kinetic_class(species,
                                            **val['params']['phys_params'],
                                            **val['params']['markers'],
                                            comm=self.derham.comm,
                                            domain_array=self.derham.domain_array,
                                            domain=self.domain,
                                            mhd_equil=self.mhd_equil,
-                                           units_basic=self.units_basic)
+                                           units_basic=self.units)
 
                 # for storing markers
                 n_markers = val['params']['save_data']['n_markers']
                 assert n_markers <= val['obj'].n_mks
                 if n_markers > 0:
                     val['kinetic_data'] = {}
                     val['kinetic_data']['markers'] = np.zeros(
@@ -694,205 +768,230 @@
                                     ranges[i][j][0], ranges[i][j][1], n_bins[i][j] + 1)]
                             val['kinetic_data']['f'][sli] = np.zeros(
                                 n_bins[i], dtype=float)
 
                 # other data (wave-particle power exchange, etc.)
                 # TODO
 
-    def print_plasma_params(self):
+    def print_plasma_params(self, verbose=True):
         """
         Compute and print volume averaged plasma parameters for each species of the model.
 
         Global parameters:
         - plasma volume
         - transit length
         - magnetic field
 
         Species dependent parameters:
         - mass
         - charge
         - density
         - pressure
-        - thermal energy
-        - thermal speed
-        - thermal frequency
-        - cyclotron frequency
-        - Larmor radius
+        - thermal energy kBT
+        - Alfvén speed v_A
+        - thermal speed v_th
+        - thermal frequency Omega_th
+        - cyclotron frequency Omega_c
+        - plasma frequency Omega_p
+        - Alfvèn frequency Omega_A
+        - thermal Larmor radius rho_th
+        - MHD length scale v_a/Omega_c
         - rho/L
-        - plasma frequency
+        - alpha = Omega_p/Omega_c
+        - epsilon = 1/(t*Omega_c)
 
-        in case of MHD species
-        - alfven speed
-        - alfven frequency
+        Returns
+        -------
+            pparams : dict
+                Plasma parameters for each species.
         """
 
-        characteristics = {}
+        from struphy.kinetic_background import maxwellians
+
+        pparams = {}
 
         # physics constants
         e = 1.602176634e-19  # elementary charge (C)
         m_p = 1.67262192369e-27  # proton mass (kg)
         mu0 = 1.25663706212e-6  # magnetic constant (N*A^-2)
         eps0 = 8.8541878128e-12  # vacuum permittivity (F*m^-1)
         kB = 1.380649e-23  # Boltzmann constant (J*K^-1)
 
         # exit when there is not any plasma species
         if len(self.fluid) == 0 and len(self.kinetic) == 0:
             return
 
         # compute model units
-        units_basic, units_der, unidts_dimless = self.model_units(
-            self.params, verbose=False)
+        units, eq_params = self.model_units(
+            self.params, verbose=True, comm=self.comm)
 
-        # SI units
-        units = {}
-        units['plasma volume'] = ' m³'
-        units['transit length'] = ' m'
-        units['magnetic field'] = ' T'
-        units['mass'] = ' kg'
-        units['charge'] = ' C'
-        units['density'] = ' m⁻³'
-        units['pressure'] = ' bar'
-        units['thermal energy'] = ' keV'
-        units['thermal speed'] = ' m/s'
-        units['thermal speed eta1'] = ' m/s'
-        units['thermal speed eta2'] = ' m/s'
-        units['thermal speed eta3'] = ' m/s'
-        units['thermal frequency'] = ' MHz'
-        units['cyclotron frequency'] = ' MHz'
-        units['Larmor radius'] = ' m'
-        units['rho/L'] = ''
-        units['plasma frequency'] = ' MHz'
-        units['alfvén speed'] = ' m/s'
-        units['alfvén frequency'] = ' MHz'
+        # units affices for printing
+        units_affix = {}
+        units_affix['plasma volume'] = ' m³'
+        units_affix['transit length'] = ' m'
+        units_affix['magnetic field'] = ' T'
+        units_affix['mass'] = ' kg'
+        units_affix['charge'] = ' C'
+        units_affix['density'] = ' m⁻³'
+        units_affix['pressure'] = ' bar'
+        units_affix['kBT'] = ' keV'
+        units_affix['v_A'] = ' m/s'
+        units_affix['v_th'] = ' m/s'
+        units_affix['vth1'] = ' m/s'
+        units_affix['vth2'] = ' m/s'
+        units_affix['vth3'] = ' m/s'
+        units_affix['Omega_th'] = ' Mrad/s'
+        units_affix['Omega_c'] = ' Mrad/s'
+        units_affix['Omega_p'] = ' Mrad/s'
+        units_affix['Omega_A'] = ' Mrad/s'
+        units_affix['rho_th'] = ' m'
+        units_affix['v_A/Omega_c'] = ' m'
+        units_affix['rho_th/L'] = ''
+        units_affix['alpha'] = ''
+        units_affix['epsilon'] = ''
 
         h = 1/20
         eta1 = np.linspace(h/2., 1.-h/2., 20)
         eta2 = np.linspace(h/2., 1.-h/2., 20)
         eta3 = np.linspace(h/2., 1.-h/2., 20)
 
         # global parameters
         # plasma volume (hat x^3)
-        vol1 = np.mean(np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) 
+        det_tmp = self.domain.jacobian_det(eta1, eta2, eta3)
+        vol1 = np.mean(np.abs(det_tmp))
         # plasma volume (m⁻³)
-        plasma_volume = vol1 * units_basic['x']**3
+        plasma_volume = vol1 * units['x']**3
         # transit length (m)
         transit_length = plasma_volume**(1/3)
         # magnetic field (T)
-        magnetic_field = np.mean(self.mhd_equil.absB0(eta1, eta2, eta3)
-                                 * np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) \
-            / vol1 * units_basic['B']
-
-        print('\nGlobal characteristics of the simulation:')
-        print(f'Plasma volume:'.ljust(25),
-              '{:4.3e}'.format(plasma_volume) + units['plasma volume'])
-        print(f'Transit length:'.ljust(25),
-              '{:4.3e}'.format(transit_length) + units['transit length'])
-        print(f'Volume-averaged magnetic field:'.ljust(25),
-              '{:4.3e}'.format(magnetic_field) + units['magnetic field'])
+        B_tmp = self.mhd_equil.absB0(eta1, eta2, eta3)
+        magnetic_field = np.mean(B_tmp * np.abs(det_tmp)) \
+            / vol1 * units['B']
+        B_max = np.max(B_tmp) * units['B']
+        B_min = np.min(B_tmp) * units['B']
+
+        if magnetic_field < 1e-14:
+            magnetic_field = np.nan
+            print('\n+++++++ WARNING +++++++ magnetic field is zero - set to nan !!')
+
+        if verbose:
+            print('\nPLASMA PARAMETERS:')
+            print(f'Plasma volume:'.ljust(25),
+                  '{:4.3e}'.format(plasma_volume) + units_affix['plasma volume'])
+            print(f'Transit length:'.ljust(25),
+                  '{:4.3e}'.format(transit_length) + units_affix['transit length'])
+            print(f'Avg. magnetic field:'.ljust(25),
+                  '{:4.3e}'.format(magnetic_field) + units_affix['magnetic field'])
+            print(f'Max magnetic field:'.ljust(25),
+                  '{:4.3e}'.format(B_max) + units_affix['magnetic field'])
+            print(f'Min magnetic field:'.ljust(25),
+                  '{:4.3e}'.format(B_min) + units_affix['magnetic field'])
 
         # species dependent parameters
+        pparams = {}
+
         if len(self.fluid) > 0:
 
             for species, val in self.fluid.items():
-                characteristics[species] = {}
+                pparams[species] = {}
+                # type
+                pparams[species]['type'] = 'fluid'
                 # mass (kg)
-                characteristics[species]['mass'] = val['params']['phys_params']['A']*m_p
+                pparams[species]['mass'] = val['params']['phys_params']['A'] * m_p
                 # charge (C)
-                characteristics[species]['charge'] = val['params']['phys_params']['Z']*e
+                pparams[species]['charge'] = val['params']['phys_params']['Z'] * e
                 # density (m⁻³)
-                characteristics[species]['density'] = np.mean(self.mhd_equil.n0(eta1, eta2, eta3)
-                                                              * np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) / plasma_volume*units_der['n']
+                pparams[species]['density'] = np.mean(self.mhd_equil.n0(
+                    eta1, eta2, eta3) * np.abs(det_tmp)) * units['x']**3 / plasma_volume * units['n']
                 # pressure (bar)
-                characteristics[species]['pressure'] = np.mean(self.mhd_equil.p0(eta1, eta2, eta3)
-                                                               * np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) / plasma_volume*units_der['p']
+                pparams[species]['pressure'] = np.mean(self.mhd_equil.p0(
+                    eta1, eta2, eta3) * np.abs(det_tmp)) * units['x']**3 / plasma_volume * units['p'] * 1e-5
                 # thermal energy (keV)
-                characteristics[species]['thermal energy'] = characteristics[species]['pressure'] * \
-                    1e5/characteristics[species]['density']/e*1e-3
-                # thermal speed (m/s)
-                characteristics[species]['thermal speed'] = np.sqrt(
-                    characteristics[species]['thermal energy'] * 1e3 * e / characteristics[species]['mass'])
-                # thermal frequency (MHz)
-                characteristics[species]['thermal frequency'] = characteristics[species]['thermal speed'] / \
-                    transit_length/(2*np.pi)*1e-6
-                # cyclotron frequency (MHz)
-                characteristics[species]['cyclotron frequency'] = characteristics[species]['charge'] * \
-                    magnetic_field / \
-                    characteristics[species]['mass'] / (2*np.pi) * 1e-6
-                # Larmor radius (m)
-                characteristics[species]['Larmor radius'] = characteristics[species]['mass'] * \
-                    characteristics[species]['thermal speed'] / \
-                    (characteristics[species]['charge'] * magnetic_field)
-                # rho/L (unitless)
-                characteristics[species]['rho/L'] = characteristics[species]['Larmor radius']/transit_length
-                # plasma frequency (MHz)
-                characteristics[species]['plasma frequency'] = np.sqrt(characteristics[species]['density']
-                                                                       * (characteristics[species]['charge'])**2 / eps0 / characteristics[species]['mass']) / (2*np.pi) * 1e-6
-                # alfvén speed (m/s)
-                characteristics[species]['alfvén speed'] = magnetic_field / np.sqrt(
-                    mu0 * characteristics[species]['mass'] * characteristics[species]['density'])
-                # alfvén frequency (MHz)
-                characteristics[species]['alfvén frequency'] = characteristics[species]['alfvén speed'] / \
-                    transit_length / (2*np.pi) * 1e-6
+                pparams[species]['kBT'] = pparams[species]['pressure'] * \
+                    1e5 / pparams[species]['density'] / e * 1e-3
 
         if len(self.kinetic) > 0:
 
-            for species, val in self.kinetic.items():
-                characteristics[species] = {}
+            eta1mg, eta2mg, eta3mg = np.meshgrid(
+                eta1, eta2, eta3, indexing='ij')
 
+            for species, val in self.kinetic.items():
+                pparams[species] = {}
+                # type
+                pparams[species]['type'] = 'kinetic'
                 # mass (kg)
-                characteristics[species]['mass'] = val['params']['phys_params']['A']*m_p
+                pparams[species]['mass'] = val['params']['phys_params']['A'] * m_p
                 # charge (C)
-                characteristics[species]['charge'] = val['params']['phys_params']['Z']*e
-                # density (m⁻³)
-                if 'background' in val['params']:
-                    type = val['params']['background']['type']
-                    characteristics[species]['density'] = val['params']['background'][type]['n']*units_der['n']
+                pparams[species]['charge'] = val['params']['phys_params']['Z'] * e
 
+                # create temp kinetic object for (default) parameter extraction
+                if 'background' in val['params']:
+                    tmp_str = 'background'
                 else:
-                    type = val['params']['init']['type']
-
-                    if type in val['params']['init'] and 'n' in val['params']['init'][type]:
-                        characteristics[species]['density'] = val['params']['init'][type]['n']*units_der['n']
+                    tmp_str = 'init'
+                tmp_type = val['params'][tmp_str]['type']
+                tmp_params = val['params'][tmp_str][tmp_type]
+                tmp = getattr(maxwellians, tmp_type)(**tmp_params)
 
-                    # When density is not specified, assume density = 1*density unit
-                    else:
-                        characteristics[species]['density'] = units_der['n']
-
-                # thermal speed (m/s)
+                # density (m⁻³)
+                pparams[species]['density'] = np.mean(tmp.n(
+                    eta1mg, eta2mg, eta3mg) * np.abs(det_tmp)) * units['x']**3 / plasma_volume * units['n']
+                # thermal speeds (m/s)
+                vth = tmp.vth(eta1mg, eta2mg, eta3mg) * \
+                    np.abs(det_tmp) * units['x']**3 / plasma_volume * units['v']
                 thermal_speed = 0.
                 for dir in range(val['obj'].vdim):
-                    thermal_kinds = 'thermal speed eta' + str(dir + 1)
-                    characteristics[species][thermal_kinds] = \
-                        val['params']['markers']['loading']['moments'][dir +
-                                                                       val['obj'].vdim] * units_der['v']
-                    thermal_speed += characteristics[species][thermal_kinds]
-
-                characteristics[species]['thermal speed'] = thermal_speed / \
+                    pparams[species]['vth' + str(dir + 1)] = np.mean(vth[dir])
+                    thermal_speed += pparams[species]['vth' + str(dir + 1)]
+                # TODO: here it is assumed that background density parameter is called "n",
+                # and that background thermal speeds are called "vthn"; make this a convention?
+                pparams[species]['v_th'] = thermal_speed / \
                     val['obj'].vdim
                 # thermal energy (keV)
-                characteristics[species]['thermal energy'] = characteristics[species]['mass'] * \
-                    characteristics[species]['thermal speed']**2 / e * 1e-3
+                pparams[species]['kBT'] = pparams[species]['mass'] * \
+                    pparams[species]['v_th']**2 / e * 1e-3
                 # pressure (bar)
-                characteristics[species]['pressure'] = characteristics[species]['thermal energy'] * \
-                    e*1e3*characteristics[species]['density'] * 1e-5
-                # thermal frequency (MHz)
-                characteristics[species]['thermal frequency'] = characteristics[species]['thermal speed'] / \
-                    transit_length / (2*np.pi) * 1e-6
-                # cyclotron frequency (MHz)
-                characteristics[species]['cyclotron frequency'] = characteristics[species]['charge'] * \
-                    magnetic_field / \
-                    characteristics[species]['mass'] / (2*np.pi) * 1e-6
-                # Larmor radius (m)
-                characteristics[species]['Larmor radius'] = characteristics[species]['mass'] * \
-                    characteristics[species]['thermal speed'] / \
-                    (characteristics[species]['charge'] * magnetic_field)
-                # rho/L (unitless)
-                characteristics[species]['rho/L'] = characteristics[species]['Larmor radius']/transit_length
-                # plasma frequency (MHz)
-                characteristics[species]['plasma frequency'] = np.sqrt(characteristics[species]['density'] *
-                                                                       (characteristics[species]['charge'])**2 / eps0 / characteristics[species]['mass']) / (2*np.pi) * 1e-6
-
-        print('\nSpecies dependent characteristics of the simulation:')
-        for species, ch in characteristics.items():
-            print(f'\nspecies: ' + species)
-            for kinds, vals in ch.items():
-                print(kinds.ljust(25), '{:4.3e}'.format(vals), units[kinds])
+                pparams[species]['pressure'] = pparams[species]['kBT'] * \
+                    e * 1e3 * pparams[species]['density'] * 1e-5
+
+        for species in pparams:
+            # alfvén speed (m/s)
+            pparams[species]['v_A'] = magnetic_field / np.sqrt(
+                mu0 * pparams[species]['mass'] * pparams[species]['density'])
+            # thermal speed (m/s)
+            pparams[species]['v_th'] = np.sqrt(
+                pparams[species]['kBT'] * 1e3 * e / pparams[species]['mass'])
+            # thermal frequency (Mrad/s)
+            pparams[species]['Omega_th'] = pparams[species]['v_th'] / \
+                transit_length * 1e-6
+            # cyclotron frequency (Mrad/s)
+            pparams[species]['Omega_c'] = pparams[species]['charge'] * \
+                magnetic_field / pparams[species]['mass'] * 1e-6
+            # plasma frequency (Mrad/s)
+            pparams[species]['Omega_p'] = np.sqrt(pparams[species]['density'] * (
+                pparams[species]['charge'])**2 / eps0 / pparams[species]['mass']) * 1e-6
+            # alfvén frequency (Mrad/s)
+            pparams[species]['Omega_A'] = pparams[species]['v_A'] / \
+                transit_length * 1e-6
+            # Larmor radius (m)
+            pparams[species]['rho_th'] = pparams[species]['v_th'] / \
+                (pparams[species]['Omega_c'] * 1e6)
+            # MHD length scale (m)
+            pparams[species]['v_A/Omega_c'] = pparams[species]['v_A'] / \
+                (np.abs(pparams[species]['Omega_c']) * 1e6)
+            # dim-less ratios
+            pparams[species]['rho_th/L'] = pparams[species]['rho_th'] / \
+                transit_length
+
+        if verbose:
+            print('\nSPECIES PARAMETERS:')
+            for species, ch in pparams.items():
+                print(f'name:'.ljust(25), species)
+                print(f'type:'.ljust(25), ch['type'])
+                ch.pop('type')
+                print(f'is bulk:'.ljust(25), species == self.bulk_species())
+                for kinds, vals in ch.items():
+                    print(kinds.ljust(25), '{:+4.3e}'.format(
+                        vals), units_affix[kinds])
+                print('------------------------------------')
+
+        return pparams
```

### Comparing `struphy-2.0.0/src/struphy/models/fluid.py` & `struphy-2.0.1/src/struphy/models/fluid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from struphy.models.base import StruphyModel
 
+
 class LinearMHD(StruphyModel):
     r'''Linear ideal MHD with zero-flow equilibrium (:math:`\mathbf U_0 = 0`).
 
     :ref:`normalization`:
 
     .. math::
 
@@ -246,46 +247,40 @@
         self._b = self.em_fields['b1']['obj'].vector
 
         # pointers to fluid variables
         self._n = self.fluid['mhd']['n3']['obj'].vector
         self._u = self.fluid['mhd']['u2']['obj'].vector
         self._p_i = self.fluid['mhd']['pi3']['obj'].vector
         self._p_e = self.fluid['mhd']['pe3']['obj'].vector
-
+        
         # extract necessary parameters
         alfven_solver = params['solvers']['solver_1']
         Hall_solver = params['solvers']['solver_2']
         SonicIon_solver = params['solvers']['solver_3']
         SonicElectron_solver = params['solvers']['solver_4']
 
         # project background magnetic field (1-form) and pressure (3-form)
         self._b_eq = self.derham.P['1']([self.mhd_equil.b1_1,
                                          self.mhd_equil.b1_2,
                                          self.mhd_equil.b1_3])
         self._p_i_eq = self.derham.P['3'](self.mhd_equil.p3)
         self._p_e_eq = self.derham.P['3'](self.mhd_equil.p3)
         self._ones = self._p_i.space.zeros()
-
+        #project background vector potential (1-form)
+        self._a_eq = self.derham.P['1']([self.mhd_equil.a1_1,
+                                         self.mhd_equil.a1_2,
+                                         self.mhd_equil.a1_3])
+        
         if isinstance(self._ones, PolarVector):
             self._ones.tp[:] = 1.
         else:
             self._ones[:] = 1.
 
-        # compute coupling parameter kappa
-        units_basic, units_der, units_dimless = self.model_units(
-            params, verbose=False)
-
-        ee = 1.602176634e-19  # elementary charge (C)
-        mH = 1.67262192369e-27  # proton mass (kg)
-
-        Ab = params['fluid']['mhd']['phys_params']['A']
-        Zb = params['fluid']['mhd']['phys_params']['Z']
-
-        omega_ch = (Zb*ee*units_basic['B'])/(Ab*mH)
-        kappa = omega_ch*units_basic['t']/(2.0 * np.pi)
+        # compute coupling parameters
+        kappa = 1. / self.eq_params['mhd']['epsilon_unit']
 
         if abs(kappa - 1) < 1e-6:
             kappa = 1.
 
         self._coupling_params = {}
         self._coupling_params['kappa'] = kappa
 
@@ -324,14 +319,15 @@
         self._scalar_quantities['en_p_e'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_B'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_p_i_eq'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_p_e_eq'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_B_eq'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_B_tot'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
+        self._scalar_quantities['helicity'] = np.empty(1, dtype=float)
 
         # temporary vectors for scalar quantities
         self._tmp_u1 = self.derham.Vh['2'].zeros()
 
         self._tmp_b1 = self.derham.Vh['1'].zeros()
         self._tmp_b2 = self.derham.Vh['1'].zeros()
 
@@ -348,22 +344,24 @@
         # perturbed fields
         self._mass_ops.M2n.dot(self._u, out=self._tmp_u1)
 
         self._mass_ops.M1.dot(self._b, out=self._tmp_b1)
 
         en_U = self._u.dot(self._tmp_u1)/2.0
         en_B = self._b.dot(self._tmp_b1)/2.0
+        helicity = self._a_eq.dot(self._tmp_b1)*2.0
         en_p_i = self._p_i.dot(self._ones)/(5.0/3.0 - 1.0)
         en_p_e = self._p_e.dot(self._ones)/(5.0/3.0 - 1.0)
 
         self._scalar_quantities['en_U'][0] = en_U
         self._scalar_quantities['en_B'][0] = en_B
         self._scalar_quantities['en_p_i'][0] = en_p_i
         self._scalar_quantities['en_p_e'][0] = en_p_e
-
+        self._scalar_quantities['helicity'][0] = helicity
+        
         self._scalar_quantities['en_tot'][0] = en_U
         self._scalar_quantities['en_tot'][0] += en_B
         self._scalar_quantities['en_tot'][0] += en_p_i
         self._scalar_quantities['en_tot'][0] += en_p_e
 
         # background fields
         self._mass_ops.M1.dot(self._b_eq, apply_bc=False, out=self._tmp_b1)
@@ -381,104 +379,115 @@
         self._tmp_b1 += self._b
 
         self._mass_ops.M1.dot(self._tmp_b1, apply_bc=False, out=self._tmp_b2)
 
         en_Btot = self._tmp_b1.dot(self._tmp_b2)/2.0
 
         self._scalar_quantities['en_B_tot'][0] = en_Btot
-        
-        
-# class ColdPlasma(StruphyModel):
-#     r'''Cold plasma model
 
-#     Normalization:
 
-#     .. math::
+class ColdPlasma(StruphyModel):
+    r'''Cold plasma model
 
-#         &c = \frac{\hat \omega}{\hat k} = \frac{\hat E}{\hat B}\,,
+    Normalization:
 
-#         &\hat \omega = \Omega_{ce}\,,
+    .. math::
 
-#         &\alpha = \frac{\Omega_{pe}}{\Omega_{ce}}\,,
+        c = \frac{\hat \omega}{\hat k} = \frac{\hat E}{\hat B}\,, \qquad \alpha = \frac{\Omega_{pe}}{\Omega_{ce}}\,, \qquad \varepsilon_c = \frac{\hat{\omega}}{\Omega_{ce}}\,, \qquad \hat j_c = \frac{c q_e}{\alpha} \hat n\,,
 
-#         &\hat j_c = \varepsilon_0 \Omega_{pe} \hat E\,,
+    where :math:`c` is the vacuum speed of light, :math:`\Omega_{ce}` the electron cyclotron frequency,
+    :math:`\Omega_{pe}` the plasma frequency and :math:`\varepsilon_0` the vacuum dielectric constant.
+    Implemented equations:
 
-#     where :math:`c` is the vacuum speed of light, :math:`\Omega_{ce}` the electron cyclotron frequency,
-#     :math:`\Omega_{pe}` the plasma frequency and :math:`\varepsilon_0` the vacuum dielectric constant.
-#     Implemented equations:
+    .. math::
 
-#     .. math::
+        &\frac{\partial \mathbf B}{\partial t} + \nabla\times\mathbf E = 0\,,
 
-#         &\frac{\partial \mathbf B}{\partial t} + \nabla\times\mathbf E = 0\,,
+        &-\frac{\partial \mathbf E}{\partial t} + \nabla\times\mathbf B =
+        \frac{\alpha}{\varepsilon_c} \mathbf j_c \,,
 
-#         &-\frac{\partial \mathbf E}{\partial t} + \nabla\times\mathbf B =
-#         \alpha \mathbf j_c \,,
+        &\frac{1}{n_0} \frac{\partial \mathbf j_c}{\partial t} = \frac{\alpha}{\varepsilon_c} \mathbf E + \frac{1}{\varepsilon_c n_0} \mathbf j_c \times \mathbf B_0\,.
 
-#         &\frac{\partial \mathbf j_c}{\partial t} = \alpha \mathbf E + \mathbf j_c \times \mathbf B\,.
 
+    Parameters
+    ----------
+    params : dict
+        Simulation parameters, see from :ref:`params_yml`.
 
-#     Parameters
-#     ----------
-#         params : dict
-#             Simulation parameters, see from :ref:`params_yml`.
-#     '''
+    comm : mpi4py.MPI.Intracomm
+        MPI communicator used for parallelization.
+    '''
 
-#     def __init__(self, params, comm):
+    @classmethod
+    def bulk_species(cls):
+        return 'electrons'
 
-#         from struphy.psydac_api.mass import WeightedMassOperators
-#         from struphy.propagators import propagators_fields
+    @classmethod
+    def timescale(cls):
+        return 'light'
 
-#         super().__init__(params, comm, e1='Hcurl', b2='Hdiv',
-#                          electron={'j1': 'Hcurl'}, hot_electrons='Particles6D')
+    def __init__(self, params, comm):
 
-#         # pointers to em-fields variables
-#         self._e = self.em_fields['e1']['obj'].vector
-#         self._b = self.em_fields['b2']['obj'].vector
+        super().__init__(params, comm, e1='Hcurl', b2='Hdiv',
+                         electrons={'j1': 'Hcurl'})
 
-#         # pointers to  fluid variables
-#         self._j = self.fluid['electrons']['j1']['obj'].vector
+        from struphy.propagators.base import Propagator
+        from struphy.propagators import propagators_fields
 
-#         # extract necessary parameters
-#         maxwell_solver = params['solvers']['solver_1']
-#         cold_solver = params['solvers']['solver_2']
+        # pointers to em-fields variables
+        self._e = self.em_fields['e1']['obj'].vector
+        self._b = self.em_fields['b2']['obj'].vector
 
-#         # Define callable for weighted mass matrices
-#         proton_mass = 1.6726219237e-27
-#         electron_mass = self.fluid['electrons']['plasma_params']['M'] * proton_mass
-#         vacuum_permittivity = 8.854187813e-12
-#         prefactor = (electron_mass / vacuum_permittivity)**0.5
+        # pointers to  fluid variables
+        self._j = self.fluid['electrons']['j1']['obj'].vector
 
-#         def call_alpha(e1, e2, e3):
-#             return prefactor * self.mhd_equil.n0(e1, e2, e3, sqeez_out=False)**0.5 / self.mhd_equil.absB0(e1, e2, e3, sqeez_out=False)
+        # extract necessary parameters
+        maxwell_solver = params['solvers']['solver_1']
+        cold_solver = params['solvers']['solver_2']
+        fluid_solver = params['solvers']['solver_3']
+
+        # additional model parameters for solvers
+        add_params = {}
+        add_params['alpha'] = self.eq_params['electrons']['alpha_unit']
+        add_params['epsilon'] = self.eq_params['electrons']['epsilon_unit']
 
-#         def call_M1alpha(e1, e2, e3, m, n):
-#             return self.domain.Ginv(e1, e2, e3)[:, :, :, m, n] * self.domain.sqrt_g(e1, e2, e3)*call_alpha(e1, e2, e3)
+        # set propagators base class attributes (available to all propagators)
+        Propagator.derham = self.derham
+        Propagator.domain = self.domain
+        Propagator.mass_ops = self.mass_ops
 
-#         # Assemble necessary mass matrices
-#         self._mass_ops = WeightedMassOperators(
-#             self.derham, self.domain, alpha=call_M1alpha)
+        # Initialize propagators/integrators used in splitting substeps
+        self._propagators = []
+        self._propagators += [propagators_fields.Maxwell(
+            self._e, self._b, **maxwell_solver)]
+        self._propagators += [propagators_fields.OhmCold(
+            self._j, self._e, **cold_solver, **add_params)]
+        self._propagators += [propagators_fields.JxBCold(
+            self._j, **fluid_solver, **add_params)]
 
-#         # Initialize propagators/integrators used in splitting substeps
-#         self._propagators = []
-#         self._propagators += [propagators_fields.Maxwell(
-#             self._e, self._b, self.derham, self._mass_ops, maxwell_solver)]
-#         self._propagators += [propagators_fields.OhmCold(
-#             self._j, self._e, self._mass_ops, cold_solver)]
+        # Scalar variables to be saved during simulation
+        self._scalar_quantities = {}
+        self._scalar_quantities['time'] = np.empty(1, dtype=float)
+        self._scalar_quantities['en_E'] = np.empty(1, dtype=float)
+        self._scalar_quantities['en_B'] = np.empty(1, dtype=float)
+        self._scalar_quantities['en_J'] = np.empty(1, dtype=float)
+        self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
+
+    @property
+    def propagators(self):
+        return self._propagators
 
-#         # Scalar variables to be saved during simulation
-#         self._scalar_quantities['time'] = np.empty(1, dtype=float)
-#         self._scalar_quantities['en_E'] = np.empty(1, dtype=float)
-#         self._scalar_quantities['en_B'] = np.empty(1, dtype=float)
-#         self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
+    @property
+    def scalar_quantities(self):
+        return self._scalar_quantities
 
-#     @property
-#     def propagators(self):
-#         return self._propagators
+    def update_scalar_quantities(self):
+
+        en_E = .5 * self._e.dot(self._mass_ops.M1.dot(self._e))
+        en_B = .5 * self._b.dot(self._mass_ops.M2.dot(self._b))
+        en_J = .5 * self._j.dot(self._mass_ops.M1ninv.dot(self._j))
+        en_tot = en_E + en_B + en_J
 
-#     def update_scalar_quantities(self, time):
-#         self._scalar_quantities['time'][0] = time
-#         self._scalar_quantities['en_E'][0] = .5 * \
-#             self._e.dot(self._mass_ops.M1.dot(self._e))
-#         self._scalar_quantities['en_B'][0] = .5 * \
-#             self._b.dot(self._mass_ops.M2.dot(self._b))
-#         self._scalar_quantities['en_tot'][0] = self._scalar_quantities['en_E'][0]
-#         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_B'][0]
+        self._scalar_quantities['en_E'][0] = en_E
+        self._scalar_quantities['en_B'][0] = en_B
+        self._scalar_quantities['en_J'][0] = en_J
+        self._scalar_quantities['en_tot'][0] = en_tot
```

### Comparing `struphy-2.0.0/src/struphy/models/hybrid.py` & `struphy-2.0.1/src/struphy/models/hybrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                          b2='Hdiv',
                          mhd={'n3': 'L2', u_name: self._u_space, 'p3': 'L2'},
                          energetic_ions='Particles6D')
 
         from struphy.polar.basic import PolarVector
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_fields, propagators_coupling, propagators_markers
-        from struphy.kinetic_background import analytical as kin_ana
+        from struphy.kinetic_background import maxwellians as kin_ana
         from struphy.psydac_api.basis_projection_ops import BasisProjectionOperators
         from mpi4py.MPI import SUM, IN_PLACE
 
         # pointers to em-field variables
         self._b = self.em_fields['b2']['obj'].vector
 
         # pointers to fluid variables
@@ -105,43 +105,27 @@
 
         # extract necessary parameters
         solver_params_1 = params['solvers']['solver_1']
         solver_params_2 = params['solvers']['solver_2']
         solver_params_3 = params['solvers']['solver_3']
         solver_params_4 = params['solvers']['solver_4']
 
-        # compute coupling parameter kappa
-        units_basic, units_der, units_dimless = self.model_units(
-            params, verbose=False)
-
-        ee = 1.602176634e-19  # elementary charge (C)
-        mH = 1.67262192369e-27  # proton mass (kg)
-
+        # compute coupling parameters
         Ab = params['fluid']['mhd']['phys_params']['A']
-        Zb = params['fluid']['mhd']['phys_params']['Z']
         Ah = params['kinetic']['energetic_ions']['phys_params']['A']
-        Zh = params['kinetic']['energetic_ions']['phys_params']['Z']
-
-        omega_ch = (Zh*ee*units_basic['B'])/(Ah*mH)
-        kappa = omega_ch*units_basic['t']
+        kappa = 1. / self.eq_params['energetic_ions']['epsilon_unit']
 
         if abs(kappa - 1) < 1e-6:
             kappa = 1.
 
         self._coupling_params = {}
         self._coupling_params['Ab'] = Ab
         self._coupling_params['Ah'] = Ah
         self._coupling_params['kappa'] = kappa
 
-        if comm.Get_rank() == 0:
-            print('Model parameters:')
-            print(f'Ah: {Ah}')
-            print(f'Ab: {Ab}')
-            print(f'kappa: {kappa}\n')
-
         # background distribution function used as control variate
         if params['kinetic']['energetic_ions']['markers']['type'] == 'control_variate':
             assert 'background' in params['kinetic']['energetic_ions'], 'no background distribution function for control variate specified'
             control = True
             f0_name = params['kinetic']['energetic_ions']['background']['type']
             f0 = getattr(kin_ana, f0_name)(
                 **params['kinetic']['energetic_ions']['background'][f0_name])
@@ -375,15 +359,15 @@
                          b2='Hdiv',
                          mhd={'n3': 'L2', u_name: self._u_space, 'p3': 'L2'},
                          energetic_ions='Particles6D')
 
         from struphy.polar.basic import PolarVector
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_fields, propagators_coupling, propagators_markers
-        from struphy.kinetic_background import analytical as kin_ana
+        from struphy.kinetic_background import maxwellians as kin_ana
         from struphy.psydac_api.basis_projection_ops import BasisProjectionOperators
         from mpi4py.MPI import SUM, IN_PLACE
 
         # pointers to em-field variables
         self._b = self.em_fields['b2']['obj'].vector
 
         # pointers to fluid variables
@@ -396,28 +380,18 @@
         ions_params = self.kinetic['energetic_ions']['params']
 
         # extract necessary parameters
         solver_params_1 = params['solvers']['solver_1']
         solver_params_2 = params['solvers']['solver_2']
         solver_params_3 = params['solvers']['solver_3']
 
-        # compute coupling parameter kappa
-        units_basic, units_der, units_dimless = self.model_units(
-            params, verbose=False)
-
-        ee = 1.602176634e-19  # elementary charge (C)
-        mH = 1.67262192369e-27  # proton mass (kg)
-
+        # compute coupling parameters
         Ab = params['fluid']['mhd']['phys_params']['A']
-        Zb = params['fluid']['mhd']['phys_params']['Z']
         Ah = params['kinetic']['energetic_ions']['phys_params']['A']
-        Zh = params['kinetic']['energetic_ions']['phys_params']['Z']
-
-        omega_ch = (Zh*ee*units_basic['B'])/(Ah*mH)
-        kappa = omega_ch*units_basic['t']
+        kappa = 1. / self.eq_params['energetic_ions']['epsilon_unit']
 
         if abs(kappa - 1) < 1e-6:
             kappa = 1.
 
         self._coupling_params = {}
         self._coupling_params['Ab'] = Ab
         self._coupling_params['Ah'] = Ah
@@ -657,15 +631,15 @@
                          b2='Hdiv',
                          mhd={'n3': 'L2', u_name: self._u_space, 'p3': 'L2'},
                          energetic_ions='Particles5D')
 
         from struphy.polar.basic import PolarVector
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_fields, propagators_coupling, propagators_markers
-        from struphy.kinetic_background import analytical as kin_ana
+        from struphy.kinetic_background import maxwellians as kin_ana
         from struphy.psydac_api.basis_projection_ops import BasisProjectionOperators
         from mpi4py.MPI import SUM
 
         # pointers to em-field variables
         self._b = self.em_fields['b2']['obj'].vector
 
         # pointers to fluid variables
@@ -680,28 +654,18 @@
         # extract necessary parameters
         solver_params_1 = params['solvers']['solver_1']
         solver_params_2 = params['solvers']['solver_2']
         solver_params_3 = params['solvers']['solver_3']
         solver_params_4 = params['solvers']['solver_4']
         solver_params_5 = params['solvers']['solver_5']
 
-        # compute coupling parameter kappa
-        units_basic, units_der, units_dimless = self.model_units(
-            params, verbose=False)
-
-        ee = 1.602176634e-19  # elementary charge (C)
-        mH = 1.67262192369e-27  # proton mass (kg)
-
+        # compute coupling parameters
         Ab = params['fluid']['mhd']['phys_params']['A']
-        Zb = params['fluid']['mhd']['phys_params']['Z']
         Ah = params['kinetic']['energetic_ions']['phys_params']['A']
-        Zh = params['kinetic']['energetic_ions']['phys_params']['Z']
-
-        omega_ch = (Zh*ee*units_basic['B'])/(Ah*mH)
-        kappa = omega_ch*units_basic['t']
+        kappa = 1. / self.eq_params['energetic_ions']['epsilon_unit']
 
         self._coupling_params = {}
         self._coupling_params['Ab'] = Ab
         self._coupling_params['Ah'] = Ah
         self._coupling_params['kappa'] = kappa
 
         # background distribution function used as control variate
@@ -757,25 +721,14 @@
         Propagator.domain = self.domain
         Propagator.mass_ops = self.mass_ops
         Propagator.basis_ops = BasisProjectionOperators(
             self.derham, self.domain, eq_mhd=self.mhd_equil)
 
         # Initialize propagators/integrators used in splitting substeps
         self._propagators = []
-        # updates u and b
-        self._propagators += [propagators_fields.ShearAlfvénCurrentCoupling5D(
-            self._u,
-            self._b,
-            particles=self._e_ions,
-            b_eq=self._b_eq,
-            f0=f0,
-            u_space=self._u_space,
-            **solver_params_1,
-            **self._coupling_params)]
-
         # # updates u and p
         # self._propagators += [propagators_fields.MagnetosonicCurrentCoupling5D(
         #     self._n,
         #     self._u,
         #     self._p,
         #     b=self._b,
         #     particles=self._e_ions,
@@ -791,44 +744,32 @@
             kappa=kappa,
             b=self._b,
             b_eq=self._b_eq,
             unit_b1=self._unit_b1,
             unit_b2=self._unit_b2,
             abs_b=self._abs_b,
             integrator=ions_params['push_algos']['integrator'],
-            method=ions_params['push_algos']['method'],
+            method='discrete_gradients',
             maxiter=ions_params['push_algos']['maxiter'],
             tol=ions_params['push_algos']['tol'])]
 
         # update H and v parallel
         self._propagators += [propagators_markers.StepPushDriftKinetic2(
             self._e_ions,
             kappa=kappa,
             b=self._b,
             b_eq=self._b_eq,
             unit_b1=self._unit_b1,
             unit_b2=self._unit_b2,
             abs_b=self._abs_b,
-            method=ions_params['push_algos']['method'],
+            method='discrete_gradients_Itoh_Newton',
             integrator=ions_params['push_algos']['integrator'],
             maxiter=ions_params['push_algos']['maxiter'],
             tol=ions_params['push_algos']['tol'])]
-
-        # update u and v parallel
-        self._propagators += [propagators_coupling.CurrentCoupling5DCurrent1(
-            self._e_ions,
-            self._u,
-            b=self._b,
-            b_eq=self._b_eq,
-            unit_b1=self._unit_b1,
-            f0=f0,
-            u_space=self._u_space,
-            **solver_params_3,
-            **self._coupling_params)]
-
+        
         # update u and H
         self._propagators += [propagators_coupling.CurrentCoupling5DCurrent2(
             self._e_ions,
             self._u,
             b=self._b,
             b_eq=self._b_eq,
             unit_b1=self._unit_b1,
@@ -837,37 +778,64 @@
             f0=f0,
             u_space=self._u_space,
             **solver_params_4,
             **self._coupling_params,
             integrator='explicit',
             method='rk4')]
 
+        # updates u and b
+        self._propagators += [propagators_fields.ShearAlfvénCurrentCoupling5D(
+            self._u,
+            self._b,
+            particles=self._e_ions,
+            b_eq=self._b_eq,
+            f0=f0,
+            u_space=self._u_space,
+            **solver_params_1,
+            **self._coupling_params)]
+        
+        # update u and v parallel
+        self._propagators += [propagators_coupling.CurrentCoupling5DCurrent1(
+            self._e_ions,
+            self._u,
+            b=self._b,
+            b_eq=self._b_eq,
+            unit_b1=self._unit_b1,
+            f0=f0,
+            u_space=self._u_space,
+            **solver_params_3,
+            **self._coupling_params)]
+
         # update u
-        self._propagators += [propagators_fields.CurrentCoupling6DDensity(
+        self._propagators += [propagators_fields.CurrentCoupling5DDensity(
             self._u,
             particles=self._e_ions,
             u_space=self._u_space,
             b_eq=self._b_eq,
             b_tilde=self._b,
             f0=f0,
             **solver_params_5,
             **self._coupling_params)]
 
         # Scalar variables to be saved during simulation
         self._scalar_quantities = {}
         self._scalar_quantities['en_U'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_p'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_B'] = np.empty(1, dtype=float)
-        self._scalar_quantities['en_p_eq'] = np.empty(1, dtype=float)
-        self._scalar_quantities['en_B_eq'] = np.empty(1, dtype=float)
-        self._scalar_quantities['en_B_tot'] = np.empty(1, dtype=float)
+        # self._scalar_quantities['en_p_eq'] = np.empty(1, dtype=float)
+        # self._scalar_quantities['en_B_eq'] = np.empty(1, dtype=float)
+        # self._scalar_quantities['en_B_tot'] = np.empty(1, dtype=float)
         self._en_fv_loc = np.empty(1, dtype=float)
         self._scalar_quantities['en_fv'] = np.empty(1, dtype=float)
         self._en_fB_loc = np.empty(1, dtype=float)
         self._scalar_quantities['en_fB'] = np.empty(1, dtype=float)
+        self._en_fv_loc_lost = np.empty(1, dtype=float)
+        self._scalar_quantities['en_fv_lost'] = np.empty(1, dtype=float)
+        self._en_fB_loc_lost = np.empty(1, dtype=float)
+        self._scalar_quantities['en_fB_lost'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
 
         # things needed in update_scalar_quantities
         self._mpi_sum = SUM
         self._prop = Propagator
 
     @property
@@ -892,50 +860,75 @@
             self._scalar_quantities['en_U'][0] = self._u.dot(
                 self._mass_ops.Mvn.dot(self._u))/2
 
         self._scalar_quantities['en_p'][0] = self._p.toarray().sum()/(5/3 - 1)
         self._scalar_quantities['en_B'][0] = self._b.dot(
             self._mass_ops.M2.dot(self._b))/2
 
-        self._scalar_quantities['en_p_eq'][0] = self._p_eq.dot(
-            self._ones)/(5/3 - 1)
-        self._scalar_quantities['en_B_eq'][0] = self._b_eq.dot(
-            self._mass_ops.M2.dot(self._b_eq, apply_bc=False))/2
+        # self._scalar_quantities['en_p_eq'][0] = self._p_eq.dot(
+        #     self._ones)/(5/3 - 1)
+        # self._scalar_quantities['en_B_eq'][0] = self._b_eq.dot(
+        #     self._mass_ops.M2.dot(self._b_eq, apply_bc=False))/2
 
         # calculate particle kinetic energy
         self._en_fv_loc = self._e_ions.markers[~self._e_ions.holes, 5].dot(
             self._e_ions.markers[~self._e_ions.holes, 3]**2) / (2*self._e_ions.n_mks)
         self.derham.comm.Reduce(
             self._en_fv_loc, self._scalar_quantities['en_fv'], op=self._mpi_sum, root=0)
 
+        self._en_fv_loc_lost = self._e_ions.lost_markers[:self._e_ions.n_lost_markers, 5].dot(
+            self._e_ions.lost_markers[:self._e_ions.n_lost_markers, 3]**2) / (2.*self._e_ions.n_mks)
+        self.derham.comm.Reduce(
+            self._en_fv_loc_lost, self._scalar_quantities['en_fv_lost'], op=self._mpi_sum, root=0)
+
+
         # sum up total magnetic field b_full1 = b_eq + b_tilde (in-place)
         self._b_eq.copy(out=self._b_full1)
         self._b_full1 += self._b
         self._b_full1.update_ghost_regions()
 
-        self._scalar_quantities['en_B_tot'][0] = (self._b_full1).dot(
-            self._mass_ops.M2.dot(self._b_full1, apply_bc=False))/2
+        # self._scalar_quantities['en_B_tot'][0] = (self._b_full1).dot(
+        #     self._mass_ops.M2.dot(self._b_full1, apply_bc=False))/2.
 
         # absolute value of parallel magnetic field
         self._prop.basis_ops.PB.dot(self._b_full1, out=self._PBb1)
         self._E0T.dot(self._PBb1, out=self._PBb2)
         self._PBb2.update_ghost_regions()
 
         self._e_ions.save_magnetic_energy(self._derham, self._PBb2)
         self._en_fB_loc = self._e_ions.markers[~self._e_ions.holes, 5].dot(
             self._e_ions.markers[~self._e_ions.holes, 8])/self._e_ions.n_mks
         self.derham.comm.Reduce(
             self._en_fB_loc, self._scalar_quantities['en_fB'], op=self._mpi_sum, root=0)
+        
+        self._en_fB_loc_lost = self._e_ions.lost_markers[:self._e_ions.n_lost_markers, 5].dot(
+            self._e_ions.lost_markers[:self._e_ions.n_lost_markers, 8]) / self._e_ions.n_mks
+        self.derham.comm.Reduce(
+            self._en_fB_loc_lost, self._scalar_quantities['en_fB_lost'], op=self._mpi_sum, root=0)
+
+
+        # # calculate particle magnetic energy
+        # self._e_ions.save_magnetic_energy(self._derham, self._E0T.dot(
+        #     self.derham.P['0'](self.mhd_equil.absB0)))
+
+        # self._en_fB_loc = self._e_ions.markers[~self._e_ions.holes, 5].dot(
+        #     self._e_ions.markers[~self._e_ions.holes, 8]) / self._e_ions.n_mks
+        # self.derham.comm.Reduce(
+        #     self._en_fB_loc, self._scalar_quantities['en_fB'], op=self._mpi_sum, root=0)
+
 
         self._scalar_quantities['en_tot'][0] = self._scalar_quantities['en_U'][0]
         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_p'][0]
         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_B'][0]
         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fv'][0]
         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fB'][0]
+        self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fv_lost'][0]
+        self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fB_lost'][0]
 
+        print('Number of lost markers:', self._e_ions.n_lost_markers)
 
 # class ColdPlasmaVlasov(StruphyModel):
 #     r'''Cold plasma model
 
 #     Normalization:
 
 #     .. math::
```

### Comparing `struphy-2.0.0/src/struphy/models/kinetic.py` & `struphy-2.0.1/src/struphy/models/kinetic.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,39 +66,47 @@
 
         super().__init__(params, comm,
                          e_field='Hcurl', b_field='Hdiv',
                          electrons='Particles6D')
 
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_fields, propagators_coupling, propagators_markers
-        from struphy.kinetic_background import analytical as kin_ana
+        from struphy.kinetic_background import maxwellians as kin_ana
         from mpi4py.MPI import SUM, IN_PLACE
 
         # pointers to em-field variables
         self._e = self.em_fields['e_field']['obj'].vector
         self._b = self.em_fields['b_field']['obj'].vector
 
+        self._en_e_tmp = self._e.space.zeros()
+        self._en_b_tmp = self._b.space.zeros()
+
         # Get rank and size
         self._rank = comm.Get_rank()
 
         # pointer to electrons
         self._electrons = self.kinetic['electrons']['obj']
         electron_params = params['kinetic']['electrons']
 
         # kinetic background
         assert electron_params['background']['type'] == 'Maxwellian6DUniform', \
-            "The background distribution function must be a uniform Maxwellian!"
+            AssertionError(
+                "The background distribution function must be a uniform Maxwellian!")
 
         self._maxwellian_params = electron_params['background']['Maxwellian6DUniform']
-        self._f0 = getattr(kin_ana, 'Maxwellian6DUniform')(
-            **self._maxwellian_params)
+        assert self._maxwellian_params['u1'] == 0., "No shifts in velocity space possible!"
+        assert self._maxwellian_params['u2'] == 0., "No shifts in velocity space possible!"
+        assert self._maxwellian_params['u3'] == 0., "No shifts in velocity space possible!"
+        self.kinetic['electrons']['obj']._f_backgr = getattr(
+            kin_ana, 'Maxwellian6DUniform')(**self._maxwellian_params)
+        self._f0 = self._electrons.f_backgr
 
         # Get coupling strength
-        self.alpha = self.units_dimless['alpha']
-        self.kappa = self.units_dimless['kappa']
+        self.alpha = self.eq_params['electrons']['alpha_unit']
+        self.kappa = 1. / self.eq_params['electrons']['epsilon_unit']
 
         # Get Poisson solver params
         self._poisson_params = params['solvers']['solver_poisson']
 
         # ====================================================================================
         # Initialize background magnetic field from MHD equilibrium
         self._b_background = self.derham.P['2']([self.mhd_equil.b2_1,
@@ -114,30 +122,30 @@
         Propagator.derham = self.derham
         Propagator.domain = self.domain
         Propagator.mass_ops = self.mass_ops
 
         # Initialize propagators/integrators used in splitting substeps
         self._propagators = []
 
-        # Only add StepStaticEfield if e-field is non-zero, otherwise it is more expensive
+        self._propagators += [propagators_markers.PushEta(
+            self._electrons,
+            algo=electron_params['push_algos']['eta'],
+            bc_type=electron_params['markers']['bc_type'],
+            f0=None)]  # no conventional weights update here, thus f0=None
+        if self._rank == 0:
+            print("Added Step PushEta\n")
+
+        # Only add StepVinEfield if e-field is non-zero, otherwise it is more expensive
         if np.all(self._e_background[0]._data < 1e-14) and np.all(self._e_background[1]._data < 1e-14) and np.all(self._e_background[2]._data < 1e-14):
-            self._propagators += [propagators_markers.PushEta(
-                self._electrons,
-                algo=electron_params['push_algos']['eta'],
-                bc_type=electron_params['markers']['bc_type'],
-                f0=None)]  # no conventional weights update here, thus f0=None
-            if self._rank == 0:
-                print("Added Step PushEta\n")
-        else:
-            self._propagators += [propagators_markers.StepStaticEfield(
+            self._propagators += [propagators_markers.StepVinEfield(
                 self._electrons,
-                e_eq=self._e_background,
+                e_field=self._e_background,
                 kappa=self.kappa)]
             if self._rank == 0:
-                print("Added Step StaticEfield\n")
+                print("Added Step VinEfield\n")
 
         # Only add VxB Step if b-field is non-zero, otherwise it is more expensive
         b_bckgr_params = params['mhd_equilibrium'][params['mhd_equilibrium']['type']]
         if (b_bckgr_params['B0x'] != 0.) or (b_bckgr_params['B0y'] != 0.) or (b_bckgr_params['B0z'] != 0.):
             self._propagators += [propagators_markers.PushVxB(
                 self._electrons,
                 algo=electron_params['push_algos']['vxb'],
@@ -188,21 +196,73 @@
     def scalar_quantities(self):
         return self._scalar_quantities
 
     def initialize_from_params(self):
         from struphy.propagators import solvers
         from struphy.pic.particles_to_grid import AccumulatorVector
 
+        # Get physical properties of the Maxwellian
+        init_type = self.kinetic['electrons']['params']['init']['type']
+        if init_type == 'Maxwellian6DUniform':
+            sigma1 = self.kinetic['electrons']['params']['init'][init_type]['vth1']
+            sigma2 = self.kinetic['electrons']['params']['init'][init_type]['vth2']
+            sigma3 = self.kinetic['electrons']['params']['init'][init_type]['vth3']
+        elif init_type == 'Maxwellian6DPerturbed':
+            sigma1 = self.kinetic['electrons']['params']['init'][init_type]['vth1']['vth01']
+            sigma2 = self.kinetic['electrons']['params']['init'][init_type]['vth2']['vth02']
+            sigma3 = self.kinetic['electrons']['params']['init'][init_type]['vth3']['vth03']
+        else:
+            raise NotImplementedError('Unknown initialization function!')
+
+        # Compute determinant of the diagonal matrix holding the thermal velocities
+        det_one_th = 1 / (sigma1 * sigma2 * sigma3)
+
+        # Compute scaled velocities
+        vth1 = sigma1**3 * det_one_th**(2/3)
+        vth2 = sigma2**3 * det_one_th**(2/3)
+        vth3 = sigma3**3 * det_one_th**(2/3)
+
+        # Set scaled velocities in params for initialization
+        if init_type == 'Maxwellian6DUniform':
+            self.kinetic['electrons']['params']['init'][init_type]['vth1'] = vth1
+            self.kinetic['electrons']['params']['init'][init_type]['vth2'] = vth2
+            self.kinetic['electrons']['params']['init'][init_type]['vth3'] = vth3
+        elif init_type == 'Maxwellian6DPerturbed':
+            self.kinetic['electrons']['params']['init'][init_type]['vth1']['vth01'] = vth1
+            self.kinetic['electrons']['params']['init'][init_type]['vth2']['vth02'] = vth2
+            self.kinetic['electrons']['params']['init'][init_type]['vth3']['vth03'] = vth3
+        
+        # Take smaller width of the two gaussians for markers drawing in order to avoid
+        # small values for f0 and hence division by zero
+        self.kinetic['electrons']['params']['markers']['loading']['moments'][3] = \
+            min(vth1, sigma1)
+        self.kinetic['electrons']['params']['markers']['loading']['moments'][4] = \
+            min(vth2, sigma2)
+        self.kinetic['electrons']['params']['markers']['loading']['moments'][5] = \
+            min(vth3, sigma3)
+
         # Initialize fields and particles
         super().initialize_from_params()
 
-        # Correct initialization of weights by dividing by N*sqrt(f_0)
+        # edges = self.kinetic['electrons']['bin_edges']['e1']
+        # # edges = [self.kinetic['electrons']['bin_edges']['v1_v2'][1]]
+        # components = [False] * 6
+        # components[0] = True
+
+        # self._electrons.show_distribution_function(components, edges, self.domain)
+
+        # Correct initialization of weights by dividing by sqrt(f_0)
         self._electrons.markers[~self._electrons.holes, 6] /= \
-            (self._electrons.n_mks *
-             np.sqrt(self._f0(*self._electrons.markers_wo_holes[:, :6].T)))
+            (np.sqrt(self._f0(*self._electrons.markers_wo_holes[:, :6].T)))
+
+        # # Set v3 = 0
+        # self._electrons.markers[~self._electrons.holes, 5] = 0.
+
+        # self._electrons.show_distribution_function(components, edges, self.domain)
+        # exit()
 
         # evaluate f0
         f0_values = self._f0(self._electrons.markers[:, 0],
                              self._electrons.markers[:, 1],
                              self._electrons.markers[:, 2],
                              self._electrons.markers[:, 3],
                              self._electrons.markers[:, 4],
@@ -227,41 +287,42 @@
         poisson_solver = solvers.PoissonSolver(
             rho=charge_accum.vectors[0],
             **self._poisson_params)
         poisson_solver(0.)
         self.derham.grad.dot(-poisson_solver._phi, out=self._e)
 
     def update_scalar_quantities(self):
-
-        # e^T * M_1 * e
+        # 0.5 * e^T * M_1 * e
+        self._mass_ops.M1.dot(self._e, out=self._en_e_tmp)
         self._scalar_quantities['en_e'][0] = self._e.dot(
-            self._mass_ops.M1.dot(self._e)) / 2.
+            self._en_e_tmp) / 2.
 
         # 0.5 * |e_1|^2
         self._scalar_quantities['en_e1'][0] = self._e._blocks[0].dot(
-            self._e._blocks[0]) / 2.
+            self._en_e_tmp._blocks[0]) / 2.
 
         # 0.5 * |e_2|^2
         self._scalar_quantities['en_e2'][0] = self._e._blocks[1].dot(
-            self._e._blocks[1]) / 2.
+            self._en_e_tmp._blocks[1]) / 2.
 
-        # b^T * M_2 * b
+        # 0.5 * b^T * M_2 * b
+        self._mass_ops.M2.dot(self._b, out=self._en_b_tmp)
         self._scalar_quantities['en_b'][0] = self._b.dot(
-            self._mass_ops.M2.dot(self._b)) / 2.
+            self._en_b_tmp) / 2.
 
         # 0.5 * |b_3|^2
         self._scalar_quantities['en_b3'][0] = self._b._blocks[2].dot(
-            self._b._blocks[2]) / 2.
+            self._en_b_tmp._blocks[2]) / 2.
 
-        # alpha^2 * v_th_1^2 * v_th_2^2 * v_th_3^2 * N/2 * sum_p s_0 * w_p^2
+        # alpha^2 / (2N) * (v_th_1 * v_th_2 * v_th_3)^(2/3) * sum_p s_0 * w_p^2
         self._scalar_quantities['en_w'][0] = \
-            self.alpha**2 * self._electrons.n_mks / 2. * \
-            self._maxwellian_params['vth1']**2 * \
-            self._maxwellian_params['vth2']**2 * \
-            self._maxwellian_params['vth3']**2 * \
+            self.alpha**2 / (2 * self._electrons.n_mks) * \
+            (self._maxwellian_params['vth1'] * \
+            self._maxwellian_params['vth2'] * \
+            self._maxwellian_params['vth3'])**(2/3) * \
             np.dot(self._electrons.markers_wo_holes[:, 6]**2,  # w_p^2
                    self._electrons.markers_wo_holes[:, 7])  # s_{0,p}
 
         self.derham.comm.Allreduce(
             self._mpi_in_place, self._scalar_quantities['en_w'], op=self._mpi_sum)
 
         # en_tot = en_w + en_e + en_b
@@ -329,15 +390,15 @@
 
         super().__init__(params, comm,
                          e_field='Hcurl', b_field='Hdiv',
                          electrons='Particles6D')
 
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_fields, propagators_coupling, propagators_markers
-        from struphy.kinetic_background import analytical as kin_ana
+        from struphy.kinetic_background import maxwellians as kin_ana
         from mpi4py.MPI import SUM, IN_PLACE
 
         # pointers to em-field variables
         self._e = self.em_fields['e_field']['obj'].vector
         self._b = self.em_fields['b_field']['obj'].vector
 
         # Get rank and size
@@ -348,20 +409,21 @@
         electron_params = params['kinetic']['electrons']
 
         # kinetic background
         assert electron_params['background']['type'] == 'Maxwellian6DUniform', \
             "The background distribution function must be a uniform Maxwellian!"
 
         self._maxwellian_params = electron_params['background']['Maxwellian6DUniform']
-        self._f0 = getattr(kin_ana, 'Maxwellian6DUniform')(
-            **self._maxwellian_params)
+        self.kinetic['electrons']['obj']._f_backgr = getattr(
+            kin_ana, 'Maxwellian6DUniform')(**self._maxwellian_params)
+        self._f0 = self._electrons.f_backgr
 
         # Get coupling strength
-        self.alpha = self.units_dimless['alpha']
-        self.kappa = self.units_dimless['kappa']
+        self.alpha = self.eq_params['electrons']['alpha_unit']
+        self.kappa = 1. / self.eq_params['electrons']['epsilon_unit']
 
         # Get Poisson solver params
         self._poisson_params = params['solvers']['solver_poisson']
 
         # ====================================================================================
         # Initialize background magnetic field from MHD equilibrium
         self._b_background = self.derham.P['2']([self.mhd_equil.b2_1,
@@ -377,20 +439,29 @@
         Propagator.derham = self.derham
         Propagator.domain = self.domain
         Propagator.mass_ops = self.mass_ops
 
         # Initialize propagators/integrators used in splitting substeps
         self._propagators = []
 
-        # self._propagators += [propagators_markers.StepStaticEfield(
-        #     self._electrons,
-        #     e_field=self._e_background + self._e,
-        #     kappa=self.kappa)]
-        # if self._rank == 0:
-        #     print("\nAdded Step StaticEfield\n")
+        self._propagators += [propagators_markers.PushEta(
+            self._electrons,
+            algo=electron_params['push_algos']['eta'],
+            bc_type=electron_params['markers']['bc_type'],
+            f0=None)]  # no conventional weights update here, thus f0=None
+        if self._rank == 0:
+            print("Added Step PushEta\n")
+
+        # Only add StepVinEfield if e-field is non-zero, otherwise it is more expensive
+        self._propagators += [propagators_markers.StepVinEfield(
+            self._electrons,
+            e_field=self._e_background + self._e,
+            kappa=self.kappa)]
+        if self._rank == 0:
+            print("Added Step VinEfield\n")
 
         self._propagators += [propagators_markers.PushVxB(
             self._electrons,
             algo=electron_params['push_algos']['vxb'],
             scale_fac=1.,
             b_eq=self._b_background + self._b,
             b_tilde=None,
```

### Comparing `struphy-2.0.0/src/struphy/models/main.py` & `struphy-2.0.1/src/struphy/models/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         Maximum run time of simulation in minutes. Will finish the time integration once this limit is reached (default=300).
 
     save_step : int, optional
         When to save data output: every time step (save_step=1), every second time step (save_step=2), etc (default=1).
     """
 
     from struphy.models import fluid, kinetic, hybrid, toy
-    from struphy.models.utilities import pre_processing
+    from struphy.models.setup import pre_processing
     from struphy.models.output_handling import DataContainer
 
     import numpy as np
     import time
 
     from mpi4py import MPI
 
@@ -49,21 +49,19 @@
                             rank,
                             size)
 
     # instantiate STRUPHY model (will only allocate model objects and associated memory)
     objs = [fluid, kinetic, hybrid, toy]
     for obj in objs:
         try:
-            model = getattr(obj, model_name)(params, comm)
+            model_class = getattr(obj, model_name)
         except AttributeError: 
             pass
 
-    # print plasma parameters to screen
-    if rank == 0:
-        model.print_plasma_params()
+    model = model_class(params, comm)
 
     # data object for saving (will either create new hdf5 files if restart==False or open existing files if restart==True)
     data = DataContainer(path_out, comm=comm)
 
     # time quantities (current time value and current time index)
     time_state = {}
     time_state['value'] = np.zeros(1, dtype=float)
@@ -104,23 +102,22 @@
     for method in model_updates:
         method()
 
     # prepare hdf5 file structure
     save_keys_all, save_keys_end = model.initialize_data_output(data, size)
 
     if rank == 0:
-        print('\nInitial time series saved.')
+        print('\nINITIAL SCALAR QUANTITIES:')
         model.print_scalar_quantities()
 
     # ======================== main time loop ======================
     if rank == 0:
         split_algo = time_params['split_algo']
         print(
-            f'\nStart time integration with {split_algo} splitting algorithm')
-        print()
+            f'\nSTART TIME STEPPING WITH "{split_algo}" SPLITTING:')
 
     # time loop
     while True:
 
         # synchronize MPI processes and check if simulation end is reached
         comm.Barrier()
         run_time_now = (time.time() - start_simulation)/60
```

### Comparing `struphy-2.0.0/src/struphy/models/output_handling.py` & `struphy-2.0.1/src/struphy/models/output_handling.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Creates/opens a hdf5 file for data ouput (each process locally).
 
     Parameters
     ----------
     path_out : str
         Path to hdf5 data files.
 
-    data_name : str, optional
+    file_name : str, optional
         Name of hdf5 file.
 
     comm : MPI communicator
     """
 
     def __init__(self, path_out, file_name=None, comm=None):
```

### Comparing `struphy-2.0.0/src/struphy/models/toy.py` & `struphy-2.0.1/src/struphy/models/toy.py`

 * *Files 22% similar despite different names*

```diff
@@ -127,21 +127,22 @@
 
     def __init__(self, params, comm):
 
         super().__init__(params, comm, ions='Particles6D')
 
         from struphy.propagators.base import Propagator
         from struphy.propagators import propagators_markers
+        from mpi4py.MPI import SUM, IN_PLACE
 
         # pointer to ions
-        ions = self.kinetic['ions']['obj']
+        self._ions = self.kinetic['ions']['obj']
         ions_params = self.kinetic['ions']['params']
 
         print(
-            f'Total number of markers : {ions.n_mks}, shape of markers array on rank {self.derham.comm.Get_rank()} : {ions.markers.shape}')
+            f'Total number of markers : {self._ions.n_mks}, shape of markers array on rank {self.derham.comm.Get_rank()} : {self._ions.markers.shape}')
 
         # project magnetic background
         self._b_eq = self.derham.P['2']([self.mhd_equil.b2_1,
                                          self.mhd_equil.b2_2,
                                          self.mhd_equil.b2_3])
 
         # set propagators base class attributes
@@ -149,46 +150,53 @@
         Propagator.domain = self.domain
         Propagator.mass_ops = self.mass_ops
 
         # Initialize propagators/integrators used in splitting substeps
         self._propagators = []
 
         self._propagators += [propagators_markers.PushVxB(
-            ions,
+            self._ions,
             algo=ions_params['push_algos']['vxb'],
             scale_fac=1.,
             b_eq=self._b_eq,
             b_tilde=None,
             f0=None)]
 
         self._propagators += [propagators_markers.PushEta(
-            ions,
+            self._ions,
             algo=ions_params['push_algos']['eta'],
             bc_type=ions_params['markers']['bc_type'],
             f0=None)]
 
         # Scalar variables to be saved during simulation
         self._scalar_quantities = {}
+        
+        self._scalar_quantities['en_f'] = np.empty(1, dtype=float)
 
-        self._en_fv_loc = np.empty(1, dtype=float)
-        self._scalar_quantities['en_fv'] = np.empty(1, dtype=float)
-        self._en_fB_loc = np.empty(1, dtype=float)
-        self._scalar_quantities['en_fB'] = np.empty(1, dtype=float)
-        self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
+        # MPI operations needed for scalar variables
+        self._mpi_sum = SUM
+        self._mpi_in_place = IN_PLACE
 
     @property
     def propagators(self):
         return self._propagators
 
     @property
     def scalar_quantities(self):
         return self._scalar_quantities
 
     def update_scalar_quantities(self):
-        pass
+        
+        self._scalar_quantities['en_f'][0] = self._ions.markers_wo_holes[:, 6].dot(
+            self._ions.markers_wo_holes[:, 3]**2 +
+            self._ions.markers_wo_holes[:, 4]**2 +
+            self._ions.markers_wo_holes[:, 5]**2)/(2*self._ions.n_mks)
+
+        self.derham.comm.Allreduce(
+            self._mpi_in_place, self._scalar_quantities['en_f'], op=self._mpi_sum)
 
 
 class DriftKinetic(StruphyModel):
     r'''Drift-kinetic equation in static background magnetic field (guiding-center motion). 
 
     :ref:`normalization`:
 
@@ -283,35 +291,39 @@
             self._ions,
             kappa=kappa,
             b_eq=self._b_eq,
             unit_b1=self._unit_b1,
             unit_b2=self._unit_b2,
             abs_b=self._abs_b,
             integrator=ions_params['push_algos']['integrator'],
-            method=ions_params['push_algos']['method'],
+            method='discrete_gradients',
             maxiter=ions_params['push_algos']['maxiter'],
             tol=ions_params['push_algos']['tol'])]
         self._propagators += [propagators_markers.StepPushGuidingCenter2(
             self._ions,
             kappa=kappa,
             b_eq=self._b_eq,
             unit_b1=self._unit_b1,
             unit_b2=self._unit_b2,
             abs_b=self._abs_b,
-            method=ions_params['push_algos']['method'],
+            method='discrete_gradients_Itoh_Newton',
             integrator=ions_params['push_algos']['integrator'],
             maxiter=ions_params['push_algos']['maxiter'],
             tol=ions_params['push_algos']['tol'])]
 
         # Scalar variables to be saved during simulation
         self._scalar_quantities = {}
         self._en_fv_loc = np.empty(1, dtype=float)
         self._scalar_quantities['en_fv'] = np.empty(1, dtype=float)
         self._en_fB_loc = np.empty(1, dtype=float)
         self._scalar_quantities['en_fB'] = np.empty(1, dtype=float)
+        self._en_fv_loc_lost = np.empty(1, dtype=float)
+        self._scalar_quantities['en_fv_lost'] = np.empty(1, dtype=float)
+        self._en_fB_loc_lost = np.empty(1, dtype=float)
+        self._scalar_quantities['en_fB_lost'] = np.empty(1, dtype=float)
         self._scalar_quantities['en_tot'] = np.empty(1, dtype=float)
 
         # MPI operations needed for scalar variables
         self._mpi_sum = SUM
 
     @property
     def propagators(self):
@@ -319,23 +331,40 @@
 
     @property
     def scalar_quantities(self):
         return self._scalar_quantities
 
     def update_scalar_quantities(self):
 
+        # particles' kinetic energy
         self._en_fv_loc = self._ions.markers[~self._ions.holes, 5].dot(
-            self._ions.markers[~self._ions.holes, 3]**2) / (2*self._ions.n_mks)
+            self._ions.markers[~self._ions.holes, 3]**2) / (2.*self._ions.n_mks)
         self.derham.comm.Reduce(
             self._en_fv_loc, self._scalar_quantities['en_fv'], op=self._mpi_sum, root=0)
+    
+        self._en_fv_loc_lost = self._ions.lost_markers[:self._ions.n_lost_markers, 5].dot(
+            self._ions.lost_markers[:self._ions.n_lost_markers, 3]**2) / (2.*self._ions.n_mks)
+        self.derham.comm.Reduce(
+            self._en_fv_loc_lost, self._scalar_quantities['en_fv_lost'], op=self._mpi_sum, root=0)
 
-        # calculate particle magnetic energy
-        self._ions.save_magnetic_energy(self._derham, self._E0T.dot(
-            self.derham.P['0'](self.mhd_equil.absB0)))
+        # particles' magnetic energy
+        self._ions.save_magnetic_energy(self._derham,
+            self._E0T.dot(self.derham.P['0'](self.mhd_equil.absB0)))
 
         self._en_fB_loc = self._ions.markers[~self._ions.holes, 5].dot(
             self._ions.markers[~self._ions.holes, 8]) / self._ions.n_mks
         self.derham.comm.Reduce(
             self._en_fB_loc, self._scalar_quantities['en_fB'], op=self._mpi_sum, root=0)
+        
+        self._en_fB_loc_lost = self._ions.lost_markers[:self._ions.n_lost_markers, 5].dot(
+            self._ions.lost_markers[:self._ions.n_lost_markers, 8]) / self._ions.n_mks
+        self.derham.comm.Reduce(
+            self._en_fB_loc_lost, self._scalar_quantities['en_fB_lost'], op=self._mpi_sum, root=0)
 
         self._scalar_quantities['en_tot'][0] = self._scalar_quantities['en_fv'][0]
         self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fB'][0]
+        self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fv_lost'][0]
+        self._scalar_quantities['en_tot'][0] += self._scalar_quantities['en_fB_lost'][0]
+
+        # print(self._ions.markers[~self._ions.holes,0:9])
+        print('Number of lost markers:', self._ions.n_lost_markers)
+        # print(self._ions.lost_markers[:self._ions.n_lost_markers,:])
```

### Comparing `struphy-2.0.0/src/struphy/models/utilities.py` & `struphy-2.0.1/src/struphy/models/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 import numpy as np
 
 
 def derive_units(Z_bulk=1, A_bulk=1., x=1., B=1., n=1., time_scale='alfvén'):
     """
-    Computes derived physics units of Struphy quantities.
+    Computes Struphy units used in Struphy model implementations.
+    
+    Input units from parameter file:
+    
+        * Length (m)
+        * Magnetic field (T)
+        * number density (10^20 1/m^3)
+        
+    Velocity unit must be defined in each model as one of "light", "alfvén" or "cyclotron":
+    
+        * Velocity (m/s)
+        
+    Derived units using mass and charge number of bulk species:
+    
+        * Time (s)
+        * Mass density (kg/m^3)
+        * Pressure (Pa)
 
     Parameters
     ---------
     Z_bulk : int
         Charge number of bulkd species.
 
     A_bulk : int
@@ -23,86 +39,66 @@
         Unit of particle number density (in 1e20 per cubic meter).
 
     time_scale : str
         Time scale to be used (determined by some characteristic velocity: "alfvén", "cyclotron" or "light").
 
     Returns
     -------
-    units_basic : dict
+    units : dict
         Basic units for time, length, mass and magnetic field.
 
-    units_der : dict
+    units : dict
         Derived units for velocity, pressure, mass density and particle density.
-
-    units_dimless :  dict
-        Some dimensionless quantities:
-            * alpha = omega_p / omega_c, ratio of bulk plasma to bulk cyclotron frequency.
     """
 
     # physics constants
     e = 1.602176634e-19  # elementary charge (C)
     mH = 1.67262192369e-27  # proton mass (kg)
     mu0 = 1.25663706212e-6  # magnetic constant (N/A^2)
     eps0 = 8.8541878128e-12  # vacuum permittivity (F/m)
     kB = 1.380649e-23  # Boltzmann constant (J/K)
     c = 299792458  # speed of light (m/s)
 
-    # prescribed units
-    x_unit = x * 1
-    B_unit = B * 1
-    n_unit = n * 1e20
-
-    # basic units in SI units (time, length, particle density and magnetic field)
-    units_basic = {}
+    units = {}
 
+    # length (m)
+    units['x'] = x
+    # magnetic field (T)
+    units['B'] = B
+    # number density (1/m^3)
+    units['n'] = n * 1e20
+    # velocity (m/s)
     if time_scale == 'light':
-        v_unit = 1*c
+        units['v'] = 1*c
     elif time_scale == 'alfvén':
-        v_unit = B_unit / np.sqrt(n_unit * A_bulk * mH * mu0)
+        units['v'] = units['B'] / np.sqrt(units['n'] * A_bulk * mH * mu0)
     elif time_scale == 'cyclotron':
-        v_unit = Z_bulk * e * B_unit / (A_bulk * mH) / (2*np.pi) * x_unit
-
-    units_basic['t'] = x_unit / v_unit
-    units_basic['x'] = x_unit
-    units_basic['m'] = A_bulk * mH * n_unit * x_unit**3
-    units_basic['B'] = B_unit
-
-    # derived units
-    units_der = {}
-
-    units_der['v'] = units_basic['x'] / units_basic['t']
-    units_der['p'] = units_basic['m'] / \
-        (units_basic['x'] * units_basic['t']**2)
-    units_der['rho'] = units_basic['m'] / units_basic['x']**3
-    units_der['n'] = units_basic['m'] / units_basic['x']**3 / (A_bulk * mH)
-
-    # relevant dimensionless quantities
-    units_dimless = {}
-
-    # unit of bulk plasma frequency
-    omega_p = np.sqrt(n_unit * (Z_bulk * e)**2 / (eps0 * A_bulk * mH))
-
-    # unit of bulk cyclotron frequency
-    omega_c = Z_bulk * e * B_unit / (A_bulk * mH)
+        units['v'] = Z_bulk * e * units['B'] / (A_bulk * mH) / (2*np.pi) * units['x']
+    # time (s)
+    units['t'] = units['x'] / units['v']
+    # pressure (Pa)
+    units['p'] = A_bulk * mH * units['n'] * units['x']**3 / \
+        (units['x'] * units['t']**2) # this is equal to B^2/(mu0*n) if time_scale='alfvén'
+    # mass density (kg/m^3)
+    units['rho'] = A_bulk * mH * units['n']
 
-    # relevant unit parameters
-    units_dimless['alpha'] = omega_p / omega_c
-    units_dimless['kappa'] = omega_c * units_basic['t']
+    return units
 
-    return units_basic, units_der, units_dimless
 
-
-def setup_domain_mhd(params):
+def setup_domain_mhd(params, units=None):
     """
     Creates the domain object and MHD equilibrium for a given parameter file.
 
     Parameters
     ----------
     params : dict
         The full simulation parameter dictionary.
+        
+    units : dict
+        All Struphy units.
 
     Returns
     -------
     domain : struphy.geometry.base.Domain
         The Struphy domain object for evaluating the mapping F : [0, 1]^3 --> R^3 and the corresponding metric coefficients.
 
     mhd : struphy.fields_background.base.MHDequilibrium
@@ -114,20 +110,23 @@
     from struphy.fields_background.mhd_equil.base import LogicalMHDequilibrium
 
     # MHD equilibrium given (load equilibrium first, then set domain)
     if 'mhd_equilibrium' in params:
 
         mhd_type = params['mhd_equilibrium']['type']
         mhd_class = getattr(equils, mhd_type)
-        mhd = mhd_class(**params['mhd_equilibrium'][mhd_type])
+
+        if mhd_type == 'EQDSKequilibrium':
+            mhd = mhd_class(units=units, **params['mhd_equilibrium'][mhd_type])
+        else:
+            mhd = mhd_class(**params['mhd_equilibrium'][mhd_type])
 
         # for logical MHD equilibria, the domain comes with the equilibrium
         if isinstance(mhd, LogicalMHDequilibrium):
             domain = mhd.domain
-
         # for cartesian MHD equilibria, the domain can be chosen idependently
         else:
             dom_type = params['geometry']['type']
             dom_class = getattr(domains, dom_type)
 
             if dom_type == 'Tokamak':
                 domain = dom_class(
@@ -235,17 +234,19 @@
                     comm=comm,
                     mpi_dims_mask=mpi_dims_mask,
                     with_projectors=True,
                     polar_ck=polar_ck,
                     domain=domain)
 
     if comm.Get_rank() == 0:
-        print('MPI processes per direction:',
+        print('\nDERHAM:')
+        print('MPI proc. per dir.:'.ljust(25),
               derham.domain_decomposition.nprocs)
-        print('')
+        print('use polar splines:'.ljust(25), derham.polar_ck == 1)
+        print('domain on process 0:'.ljust(25), derham.domain_array[0])
 
     return derham
 
 
 def pre_processing(model_name, parameters, path_out, restart, max_sim_time, mpi_rank, mpi_size):
     """
     Prepares simulation parameters, output folder and prints some information of the run to the screen. 
@@ -268,69 +269,77 @@
         Maximum run time of simulation in minutes. Will finish the time integration once this limit is reached.
 
     mpi_rank : int
         The rank of the calling process.
 
     mpi_size : int
         Total number of MPI processes of the run.
+        
+    Returns
+    -------
+    params : dict
+        The simulation parameters.
     """
 
     import os
     import shutil
     import datetime
     import sysconfig
     import glob
     import yaml
     from struphy.models import fluid, kinetic, hybrid, toy
 
     # prepare output folder
     if mpi_rank == 0:
-        print('')
+        print('\nPREPARATION AND CLEAN-UP:')
 
         # create output folder if it does not exit
         if not os.path.exists(path_out):
             os.mkdir(path_out)
-            print('\nCreated folder ' + path_out)
+            print('Created folder ' + path_out)
+            
+        # create data folder in output folder if it does not exist
+        if not os.path.exists(os.path.join(path_out, 'data/')):
             os.mkdir(os.path.join(path_out, 'data/'))
-            print('\nCreated folder ' + os.path.join(path_out, 'data/'))
+            print('Created folder ' + os.path.join(path_out, 'data/'))
 
         # clean output folder if it already exists
         else:
 
             # remove post_processing folder
             folder = os.path.join(path_out, 'post_processing')
             if os.path.exists(folder):
                 shutil.rmtree(folder)
-                print('Removed folder ' + folder)
+                print('Removed existing folder ' + folder)
 
             # remove meta file
             file = os.path.join(path_out, 'meta.txt')
             if os.path.exists(file):
                 os.remove(file)
-                print('Removed file ' + file)
+                print('Removed existing file ' + file)
 
             # remove profiling file
             file = os.path.join(path_out, 'profile_tmp')
             if os.path.exists(file):
                 os.remove(file)
-                print('Removed file ' + file)
+                print('Removed existing file ' + file)
 
             # remove .png files (if NOT a restart)
             if not restart:
                 files = glob.glob(os.path.join(path_out, '*.png'))
                 for n, file in enumerate(files):
                     os.remove(file)
                     if n < 10:  # print only ten statements in case of many processes
-                        print('Removed file ' + file)
+                        print('Removed existing file ' + file)
                         
                 files = glob.glob(os.path.join(path_out, 'data', '*.hdf5'))
                 for n, file in enumerate(files):
                     os.remove(file)
                     if n < 10:  # print only ten statements in case of many processes
-                        print('Removed file ' + file)
+                        print('Removed existing file ' + file)
 
     # save "parameters" dictionary as .yml file
     if isinstance(parameters, dict):
         parameters_path = os.path.join(path_out, 'parameters.yml')
 
         # write parameters to file and save it in output folder
         if mpi_rank == 0:
@@ -351,48 +360,45 @@
 
         # copy parameter file to output folder
         if parameters_path != os.path.join(path_out, 'parameters.yml'):
             shutil.copy2(parameters_path, os.path.join(
                 path_out, 'parameters.yml'))
 
         # print simulation info
-        print('')
-        print('model:'.ljust(30), model_name)
-        print('parameter file:'.ljust(30), parameters_path)
-        print('output folder:'.ljust(30), path_out)
-        print('restart:'.ljust(30), restart)
-        print('max wall-clock time [min]:'.ljust(30), max_sim_time)
-        print('number of MPI processes:'.ljust(30), mpi_size)
-
+        print('\nMETADATA:')
+        print('platform:'.ljust(25), sysconfig.get_platform())
+        print('python version:'.ljust(25), sysconfig.get_python_version())
+        print('model:'.ljust(25), model_name)
+        print('MPI processes:'.ljust(25), mpi_size)
+        print('parameter file:'.ljust(25), parameters_path)
+        print('output folder:'.ljust(25), path_out)
+        print('restart:'.ljust(25), restart)
+        print('max wall-clock [min]:'.ljust(25), max_sim_time)
+        
         # print domain info
-        print('\nDOMAIN parameters:')
-        print(f'domain type :', params['geometry']['type'])
-        print(f'domain parameters :')
+        print('\nDOMAIN:')
+        print(f'type:'.ljust(25), params['geometry']['type'])
         for key, val in params['geometry'][params['geometry']['type']].items():
             if key not in {'cx', 'cy', 'cz'}:
-                print(key, ':', val)
+                print((key + ':').ljust(25), val)
 
         # print grid info
-        print('\nGRID parameters:')
-        print(f'number of elements  :', params['grid']['Nel'])
-        print(f'spline degrees      :', params['grid']['p'])
-        print(f'periodic bcs        :', params['grid']['spl_kind'])
-        print(f'hom. Dirichlet bc   :', params['grid']['bc'])
-        print(f'GL quad pts (L2)    :', params['grid']['nq_el'])
-        print(f'GL quad pts (hist)  :', params['grid']['nq_pr'])
-
-        # print units info
-        objs = [fluid, kinetic, hybrid, toy]
-        for obj in objs:
-            try:
-                model = getattr(obj, model_name)
-            except:
-                pass
-        model.model_units(params, verbose=True)
-        print('')
+        print('\nGRID:')
+        print(f'number of elements:'.ljust(25), params['grid']['Nel'])
+        print(f'spline degrees:'.ljust(25), params['grid']['p'])
+        print(f'periodic bcs:'.ljust(25), params['grid']['spl_kind'])
+        print(f'hom. Dirichlet bc:'.ljust(25), params['grid']['bc'])
+        print(f'GL quad pts (L2):'.ljust(25), params['grid']['nq_el'])
+        print(f'GL quad pts (hist):'.ljust(25), params['grid']['nq_pr'])
+        
+        # print time info
+        print('\nTIME:')
+        print(f'time step:'.ljust(25), params['time']['dt'])
+        print(f'final time:'.ljust(25), params['time']['Tend'])
+        print(f'splitting algo:'.ljust(25), params['time']['split_algo'])
 
         # write meta data to output folder
         with open(path_out + '/meta.txt', 'w') as f:
             f.write('date of simulation: '.ljust(30) +
                     str(datetime.datetime.now()) + '\n')
             f.write('platform: '.ljust(30) + sysconfig.get_platform() + '\n')
             f.write('python version: '.ljust(30) +
```

### Comparing `struphy-2.0.0/src/struphy/pic/accum_kernels.py` & `struphy-2.0.1/src/struphy/pic/accum_kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,16 +356,16 @@
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         f0 = f0_values[ip]
 
-        # filling = alpha^2 * kappa * w_p * sqrt{f_0}
-        filling = alpha**2 * kappa * markers[ip, 6] * sqrt(f0) * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
+        # filling = alpha^2 * kappa * w_p * sqrt{f_0} / N
+        filling = alpha**2 * kappa * markers[ip, 6] * sqrt(f0) / n_markers_tot
 
         # spans (i.e. index for non-vanishing B-spline basis functions)
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
 
         # compute bn, bd, i.e. values for non-vanishing B-/splines at position eta
@@ -432,15 +432,15 @@
 
     # allocate for metric coeffs
     df = empty((3, 3), dtype=float)
     df_inv = empty((3, 3), dtype=float)
 
     # allocate for filling
     v = empty(3, dtype=float)
-    df_inv_times_v = empty(3, dtype=float)
+    df_inv_v = empty(3, dtype=float)
     filling_m = empty((3, 3), dtype=float)
     filling_v = empty(3, dtype=float)
 
     # get number of markers
     n_markers = shape(markers)[0]
 
     #$ omp parallel private (ip, eta1, eta2, eta3, f0, df, df_inv, v, df_inv_times_v, filling_m, filling_v)
@@ -452,39 +452,41 @@
             continue
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
+        # get velocity
+        v[0] = markers[ip, 3] / f0_params[4]**2
+        v[1] = markers[ip, 4] / f0_params[5]**2
+        v[2] = markers[ip, 5] / f0_params[6]**2
+
         f0 = f0_values[ip]
 
         # evaluate Jacobian, result in df
         map_eval.df(eta1, eta2, eta3,
                     kind_map, params_map,
                     t1_map, t2_map, t3_map, p_map,
                     ind1_map, ind2_map, ind3_map,
                     cx, cy, cz,
                     df)
 
-        # compute shifted and stretched velocity
-        v[0] = (markers[ip, 3] - f0_params[1]) / f0_params[4]**2
-        v[1] = (markers[ip, 4] - f0_params[2]) / f0_params[5]**2
-        v[2] = (markers[ip, 5] - f0_params[3]) / f0_params[6]**2
-
-        # filling functions
+        # invert Jacobian matrix
         linalg.matrix_inv(df, df_inv)
-        linalg.matrix_vector(df_inv, v, df_inv_times_v)
 
-        # filling_m = alpha^2 * kappa^2 * f0 / (N * s_0 * v_th_1^2 * v_th_2^2 * v_th_3^2) * (DF^{-1} \V_th (v_p - u))_mu * (DF^{-1} \V_th (v_p - u))_nu
-        linalg.outer(df_inv_times_v, df_inv_times_v, filling_m)
-        filling_m[:, :] *= alpha**2 * kappa**2 * f0 * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2 / (n_markers_tot * markers[ip, 7])
+        # compute DF^{-1} v
+        linalg.matrix_vector(df_inv, v, df_inv_v)
 
-        # filling_v = alpha^2 * kappa * w_p * sqrt{f_0} DL^{-1} * \V_th * (v_p - u)
-        filling_v[:] = alpha**2 * kappa * sqrt(f0) * markers[ip, 6] * df_inv_times_v[:] * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
+        # filling_m = alpha^2 * kappa^2 * f0 / (N * s_0) * (v_th_1 * v_th_2 * v_th_3)^2/3) * (DF^{-1} \V_th v_p)_mu * (DF^{-1} \V_th v_p)_nu
+        linalg.outer(df_inv_v, df_inv_v, filling_m)
+        filling_m[:, :] *= alpha**2 * kappa**2 * f0 * (f0_params[4] * f0_params[5] * f0_params[6])**(2/3) / (n_markers_tot * markers[ip, 7])
+
+        # filling_v = alpha^2 * kappa / N * (v_th_1 * v_th_2 * v_th_3)^2/3) * w_p * sqrt{f_0} DL^{-1} * \V_th * v_p
+        filling_v[:] = alpha**2 * kappa * sqrt(f0) * markers[ip, 6] * df_inv_v[:] / n_markers_tot * (f0_params[4] * f0_params[5] * f0_params[6])**(2/3)
 
         # call the appropriate matvec filler
         mvf.m_v_fill_b_v1_symm(pn,
                                tn1, tn2, tn3,
                                starts1,
                                eta1, eta2, eta3,
                                mat11, mat12, mat13, mat22, mat23, mat33,
@@ -1414,14 +1416,158 @@
     vec1_1 /= n_markers_tot
     vec2_1 /= n_markers_tot
     vec3_1 /= n_markers_tot
     vec1_2 /= n_markers_tot
     vec2_2 /= n_markers_tot
     vec3_2 /= n_markers_tot
 
+@stack_array('g_inv', 'tmp1', 'tmp2', 'b', 'b_prod', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+def cc_lin_mhd_5d_D(markers: 'float[:,:]', n_markers_tot: 'int',
+                    pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                    starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                    kind_map: 'int', params_map: 'float[:]',
+                    p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                    ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                    cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                    mat12: 'float[:,:,:,:,:,:]',
+                    mat13: 'float[:,:,:,:,:,:]',
+                    mat23: 'float[:,:,:,:,:,:]',
+                    b2_1: 'float[:,:,:]',   # model specific argument
+                    b2_2: 'float[:,:,:]',   # model specific argument
+                    b2_3: 'float[:,:,:]',   # model specific argument
+                    basis_u : 'int', scale_mat : 'float'):  # model specific argument
+    r"""
+    """
+
+    # allocate for magnetic field evaluation
+    b = empty(3, dtype=float)
+    b_prod = zeros((3, 3), dtype=float)
+
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # allocate for metric coefficients
+    df       = empty((3, 3), dtype=float)
+    df_inv   = empty((3, 3), dtype=float)
+    df_inv_t = empty((3, 3), dtype=float)
+    g_inv    = empty((3, 3), dtype=float)
+
+    # allocate some temporary buffers for filling
+    tmp1 = empty((3, 3), dtype=float)
+    tmp2 = empty((3, 3), dtype=float)
+
+    # get local number of markers
+    n_markers_loc = shape(markers)[0]
+
+    for ip in range(n_markers_loc):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        # marker positions
+        eta1 = markers[ip, 0]
+        eta2 = markers[ip, 1]
+        eta3 = markers[ip, 2]
+
+        # b-field evaluation
+        span1 = bsp.find_span(tn1, pn[0], eta1)
+        span2 = bsp.find_span(tn2, pn[1], eta2)
+        span3 = bsp.find_span(tn3, pn[2], eta3)
+
+        bsp.b_d_splines_slim(tn1, pn[0], eta1, span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], eta2, span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], eta3, span3, bn3, bd3)
+
+        b[0] = eval_3d.eval_spline_mpi_kernel(
+            pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, b2_1, starts2[0])
+        b[1] = eval_3d.eval_spline_mpi_kernel(
+            pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, b2_2, starts2[1])
+        b[2] = eval_3d.eval_spline_mpi_kernel(
+            pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, b2_3, starts2[2])
+
+        # operator bx() as matrix
+        b_prod[0, 1] = -b[2]
+        b_prod[0, 2] = +b[1]
+        b_prod[1, 0] = +b[2]
+        b_prod[1, 2] = -b[0]
+        b_prod[2, 0] = -b[1]
+        b_prod[2, 1] = +b[0]
+
+        # evaluate Jacobian matrix and Jacobian determinant
+        map_eval.df(eta1, eta2, eta3,
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+        
+        det_df = linalg.det(df)
+
+        # marker weight
+        weight = markers[ip, 5]
+
+        if basis_u == 0:
+
+            # filling functions
+            filling_m12 = - weight * b_prod[0, 1] * scale_mat
+            filling_m13 = - weight * b_prod[0, 2] * scale_mat
+            filling_m23 = - weight * b_prod[1, 2] * scale_mat
+
+            # call the appropriate matvec filler
+            mvf.mat_fill_v0vec_asym(pn, span1, span2, span3,
+                                 bn1, bn2, bn3,
+                                 starts0,
+                                 mat12, mat13, mat23,
+                                 filling_m12, filling_m13, filling_m23)
+            
+        elif basis_u == 1:
+
+            # filling functions
+            linalg.matrix_inv_with_det(df, det_df, df_inv)
+            linalg.transpose(df_inv, df_inv_t)
+            linalg.matrix_matrix(df_inv, df_inv_t, g_inv)
+            linalg.matrix_matrix(g_inv, b_prod, tmp1)
+            linalg.matrix_matrix(tmp1, g_inv, tmp2)
+
+            filling_m12 = - weight * tmp2[0, 1] * scale_mat
+            filling_m13 = - weight * tmp2[0, 2] * scale_mat
+            filling_m23 = - weight * tmp2[1, 2] * scale_mat
+
+            # call the appropriate matvec filler
+            mvf.mat_fill_v1_asym(pn, span1, span2, span3,
+                                 bn1, bn2, bn3,
+                                 bd1, bd2, bd3,
+                                 starts1,
+                                 mat12, mat13, mat23,
+                                 filling_m12, filling_m13, filling_m23)
+            
+        elif basis_u == 2:
+
+            # filling functions
+            filling_m12 = - weight * b_prod[0, 1] * scale_mat / det_df**2
+            filling_m13 = - weight * b_prod[0, 2] * scale_mat / det_df**2
+            filling_m23 = - weight * b_prod[1, 2] * scale_mat / det_df**2
+
+            # call the appropriate matvec filler
+            mvf.mat_fill_v2_asym(pn, span1, span2, span3,
+                                 bn1, bn2, bn3,
+                                 bd1, bd2, bd3,
+                                 starts1,
+                                 mat12, mat13, mat23,
+                                 filling_m12, filling_m13, filling_m23)
+            
+    mat12 /= n_markers_tot
+    mat13 /= n_markers_tot
+    mat23 /= n_markers_tot
 
 @stack_array('df', 'df_t', 'df_inv', 'g_inv', 'filling_m', 'filling_v', 'tmp', 'tmp1', 'tmp2', 'tmp_m', 'tmp_v', 'b', 'b_prod', 'b_star', 'norm_b1', 'curl_norm_b', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def cc_lin_mhd_5d_J1(markers: 'float[:,:]', n_markers_tot: 'int',
                      pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                      starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                      kind_map: 'int', params_map: 'float[:]',
                      p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
@@ -1602,19 +1748,19 @@
         elif basis_u == 1:
             
             # needed metric coefficients
             linalg.matrix_inv_with_det(df, det_df, df_inv)
             linalg.transpose(df_inv, df_inv_t)
             linalg.matrix_matrix(df_inv, df_inv_t, g_inv)
             linalg.matrix_matrix(g_inv, b_prod, tmp1)
+            linalg.matrix_vector(tmp1, curl_norm_b, tmp_v)
 
             linalg.matrix_matrix(tmp1, tmp, tmp2)
             linalg.matrix_matrix(tmp2, -b_prod, tmp1)
             linalg.matrix_matrix(tmp1, g_inv, tmp_m)
-            linalg.matrix_vector(tmp1, curl_norm_b, tmp_v)
 
             filling_m[:, :] = weight * tmp_m * v**2 / abs_b_star_para**2 / det_df**2 * scale_mat
             filling_v[:] = weight * tmp_v * v**2 / abs_b_star_para / det_df * scale_vec
 
             # call the appropriate matvec filler
             mvf.m_v_fill_v1_symm(pn, span1, span2, span3,
                                  bn1, bn2, bn3,
@@ -2073,15 +2219,15 @@
         if basis_u == 0:
             
             linalg.matrix_matrix(b_prod, g_inv, tmp1)
             linalg.matrix_matrix(tmp1, norm_b2_prod, tmp2)
             linalg.matrix_matrix(tmp2, g_inv, tmp1)
             linalg.matrix_vector(tmp1, grad_PB, tmp_v)
 
-            filling_v[:] =    weight * tmp_v * mu / abs_b_star_para    * scale_vec
+            filling_v[:] = weight * tmp_v * mu / abs_b_star_para * scale_vec
 
             # call the appropriate matvec filler
             mvf.vec_fill_v0(pn, span1, span2, span3,
                             bn1, bn2, bn3,
                             starts0,
                             vec1, vec2, vec3,
                             filling_v[0], filling_v[1], filling_v[2])
@@ -2730,15 +2876,15 @@
                             vec1, vec2, vec3,
                             filling_v[0], filling_v[1], filling_v[2])
 
     vec1 /= n_markers_tot
     vec2 /= n_markers_tot
     vec3 /= n_markers_tot
 
-@stack_array('df', 'df_t', 'df_inv', 'g_inv', 'filling_m', 'filling_v', 'tmp1', 'tmp2', 'tmp_t', 'tmp_m', 'tmp_v', 'b', 'b_prod', 'norm_b2_prod', 'b_star', 'curl_norm_b', 'norm_b1', 'norm_b2', 'grad_PB', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+@stack_array('df', 'df_t', 'df_inv', 'g_inv', 'filling_m', 'filling_v', 'tmp1', 'tmp2', 'tmp_t', 'tmp_m', 'tmp_v', 'b', 'b_prod', 'norm_b2_prod', 'b_star', 'curl_norm_b', 'norm_b1', 'norm_b2', 'grad_PB', 'grad_PB_mat', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def cc_lin_mhd_5d_J2(markers: 'float[:,:]', n_markers_tot: 'int',
                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                     kind_map: 'int', params_map: 'float[:]',
                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                     cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -2806,14 +2952,15 @@
     b_star = empty(3, dtype=float)
     b_prod = zeros((3, 3), dtype=float)
     norm_b2_prod = zeros((3, 3), dtype=float)
     curl_norm_b = empty(3, dtype=float)
     norm_b1 = empty(3, dtype=float)
     norm_b2 = empty(3, dtype=float)
     grad_PB = empty(3, dtype=float)
+    grad_PB_mat = zeros((3, 3), dtype=float)
 
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
     bn3 = empty(pn[2] + 1, dtype=float)
 
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -2899,14 +3046,18 @@
         curl_norm_b[1] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, curl_norm_b2, starts2[1])
         curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
+
+        grad_PB_mat[0,0] = grad_PB[0]
+        grad_PB_mat[1,1] = grad_PB[1]
+        grad_PB_mat[2,2] = grad_PB[2]
         
         # b_star; 2form transformed into H1vec
         b_star[:] = (b + curl_norm_b*v/kappa)/det_df
 
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
@@ -2928,19 +3079,21 @@
         if basis_u == 0:
             
             linalg.matrix_matrix(b_prod, g_inv, tmp1)
             linalg.matrix_matrix(tmp1, norm_b2_prod, tmp2)
             linalg.matrix_matrix(tmp2, g_inv, tmp1)
 
             linalg.transpose(tmp1, tmp_t)
-            
-            linalg.matrix_matrix(tmp1, tmp_t, tmp_m)
+
             linalg.matrix_vector(tmp1, grad_PB, tmp_v)
 
-            filling_m[:, :] = weight * tmp_m      / abs_b_star_para**2 * scale_mat
+            linalg.matrix_matrix(tmp1, grad_PB_mat, tmp2)
+            linalg.matrix_matrix(tmp2, tmp_t, tmp_m)
+
+            filling_m[:, :] = weight * tmp_m * mu / abs_b_star_para**2 * scale_mat
             filling_v[:] =    weight * tmp_v * mu / abs_b_star_para    * scale_vec
 
             # call the appropriate matvec filler
             mvf.m_v_fill_v0vec_symm(pn, span1, span2, span3,
                                     bn1, bn2, bn3,
                                     starts0,
                                     mat11, mat12, mat13, 
@@ -2956,19 +3109,21 @@
             
             linalg.matrix_matrix(g_inv, b_prod, tmp1)
             linalg.matrix_matrix(tmp1, g_inv, tmp2)
             linalg.matrix_matrix(tmp2, norm_b2_prod, tmp1)
             linalg.matrix_matrix(tmp1, g_inv, tmp2)
 
             linalg.transpose(tmp2, tmp_t)
-            
-            linalg.matrix_matrix(tmp2, tmp_t, tmp_m)
+
             linalg.matrix_vector(tmp2, grad_PB, tmp_v)
 
-            filling_m[:, :] = weight * tmp_m      / abs_b_star_para**2 * scale_mat
+            linalg.matrix_matrix(tmp2, grad_PB_mat, tmp1)
+            linalg.matrix_matrix(tmp1, tmp_t, tmp_m)
+
+            filling_m[:, :] = weight * tmp_m * mu / abs_b_star_para**2 * scale_mat
             filling_v[:] =    weight * tmp_v * mu / abs_b_star_para    * scale_vec
 
             # call the appropriate matvec filler
             mvf.m_v_fill_v1_symm(pn, span1, span2, span3,
                                  bn1, bn2, bn3,
                                  bd1, bd2, bd3,
                                  starts1,
@@ -2984,18 +3139,20 @@
         elif basis_u == 2:
             
             linalg.matrix_matrix(b_prod, g_inv, tmp1)
             linalg.matrix_matrix(tmp1, norm_b2_prod, tmp2)
             linalg.matrix_matrix(tmp2, g_inv, tmp1)
 
             linalg.transpose(tmp1, tmp_t)
-            
-            linalg.matrix_matrix(tmp1, tmp_t, tmp_m)
+ 
             linalg.matrix_vector(tmp1, grad_PB, tmp_v)
 
+            linalg.matrix_matrix(tmp1, grad_PB_mat, tmp2)
+            linalg.matrix_matrix(tmp2, tmp_t, tmp_m)
+
             filling_m[:, :] = weight * tmp_m * mu / abs_b_star_para**2 / det_df**2 * scale_mat
             filling_v[:] =    weight * tmp_v * mu / abs_b_star_para    / det_df    * scale_vec
 
             # call the appropriate matvec filler
             mvf.m_v_fill_v2_symm(pn, span1, span2, span3,
                                  bn1, bn2, bn3,
                                  bd1, bd2, bd3,
```

### Comparing `struphy-2.0.0/src/struphy/pic/filler_kernels.py` & `struphy-2.0.1/src/struphy/pic/filler_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/mat_vec_filler.py` & `struphy-2.0.1/src/struphy/pic/mat_vec_filler.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/particles.py` & `struphy-2.0.1/src/struphy/pic/particles.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import h5py
 import scipy.special as sp
 
 from struphy.pic import sampling, sobol_seq
 from struphy.pic.pusher_utilities import reflect
-from struphy.kinetic_background import analytical
+from struphy.kinetic_background import maxwellians
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 
 class Particles(metaclass=ABCMeta):
     """
     Base class for a particle based kinetic species.
 
@@ -51,28 +51,14 @@
         self._mpi_comm = params['comm']
         self._mpi_size = params['comm'].Get_size()
         self._mpi_rank = params['comm'].Get_rank()
 
         # create marker array
         self.create_marker_array()
 
-        # draw markers
-        self.draw_markers()
-
-        # number of holes and markers on process
-        self._holes = self._markers[:, 0] == -1.
-        self._n_holes_loc = np.count_nonzero(self._holes)
-        self._n_mks_loc = self._markers.shape[0] - self._n_holes_loc
-
-        # check if all particle positions are inside the unit cube [0, 1]^3
-        n_mks_load_loc = self._n_mks_load[self._mpi_rank]
-
-        assert np.all(~self._holes[:n_mks_load_loc]) and np.all(
-            self._holes[n_mks_load_loc:])
-
         # Assume full-f if type is not in parameters
         if 'type' in params.keys():
             if params['type'] == 'control_variate':
                 self._use_control_variate = True
             else:
                 self._use_control_variate = False
         else:
@@ -119,14 +105,26 @@
     @property
     def params(self):
         """ Parameters for markers.
         """
         return self._params
 
     @property
+    def f_init(self):
+        assert hasattr(self, '_f_init'), AttributeError(
+            'The method "initialize_weights" has not yet been called.')
+        return self._f_init
+
+    @property
+    def f_backgr(self):
+        assert hasattr(self, '_f_backgr'), AttributeError(
+            'No background distribution available, maybe this is a full-f model?')
+        return self._f_backgr
+
+    @property
     def domain_decomp(self):
         """ Array containing domain decomposition information.
         """
         return self._domain_decomp
 
     @property
     def comm(self):
@@ -196,16 +194,28 @@
 
     @property
     def bc(self):
         """ Kinetic boundary conditions in each direction.
         """
         return self._bc
 
+    @property
+    def lost_markers(self):
+        """ Array containing the last infos of removed markers
+        """
+        return self._lost_markers
+
+    @property
+    def n_lost_markers(self):
+        """ Number of removed particles.
+        """
+        return self._n_lost_markers
+
     def create_marker_array(self):
-        """Create marker array. (self.markers)
+        """ Create marker array. (self.markers)
         """
 
         # number of cells on current process
         n_cells_loc = np.prod(
             self._domain_decomp[self._mpi_rank, 2::3], dtype=int)
 
         # total number of cells
@@ -241,29 +251,66 @@
         n_mks_load_loc = self._n_mks_load[self._mpi_rank]
 
         # create markers array (3 x positions, vdim x velocities, weight, s0, w0, ..., ID) with eps send/receive buffer
         markers_size = round(n_mks_load_loc *
                              (1 + 1/np.sqrt(n_mks_load_loc) + self.params['eps']))
         self._markers = np.zeros((markers_size, self.n_cols), dtype=float)
 
+        # create array container (3 x positions, vdim x velocities, weight, s0, w0, ID) for removed markers
+        self._n_lost_markers = 0
+        self._lost_markers = np.zeros((int(markers_size*0.5), 10), dtype=float)
+
     def draw_markers(self):
-        """ Draw markers. 
+        r""" 
+        Drawing markers according to the volume density :math:`s^n_{\textnormal{in}}`.
+        In Struphy, the initial marker distribution :math:`s^n_{\textnormal{in}}` is always of the form
+
+        .. math::
+
+            s^n_{\textnormal{in}}(\eta,v) = n^3(\eta)\, \mathcal M(v)\,,
+
+        with :math:`\mathcal M(v)` a multi-variate Gaussian:
+
+        .. math:: 
+
+            \mathcal M(v) = \prod_{i=1}^{d_v} \frac{1}{\sqrt{2\pi}\,v_{\mathrm{th},i}}
+                \exp\left[-\frac{(v_i-u_i)^2}{2 v_{\mathrm{th},i}^2}\right]\,,
+
+        where :math:`d_v` stands for the dimension in velocity space, :math:`u_i` are velocity constant shifts
+        and :math:`v_{\mathrm{th},i}` are constant thermal velocities (standard deviations).
+        The function :math:`n^3:(0,1)^3 \to \mathbb R^+` is a normalized 3-form on the unit cube,
+
+        .. math::
+
+            \int_{(0,1)^3} n^3(\eta)\,\textnormal d \eta = 1\,.
+
+        The following choices are available in Struphy:
+
+        1. Uniform distribution on the unit cube: :math:`n^3(\eta) = 1`
+
+        2. Uniform distribution on the disc: :math:`n^3(\eta) = 2\eta_1` (radial coordinate = volume element of square-to-disc mapping) 
+
+        All needed parameters can be set in the parameter file, in the section ``kinetic/<species>/markers/loading``.
         """
 
         # number of markers on the local process at loading stage
         n_mks_load_loc = self.n_mks_load[self._mpi_rank]
 
         # cumulative sum of number of markers on each process at loading stage.
         n_mks_load_cum_sum = np.cumsum(self.n_mks_load)
+        
+        if self._mpi_rank == 0:
+            print('\nMARKERS:')
 
         # load markers from external .hdf5 file
         if self._params['loading']['type'] == 'external':
 
             if self._mpi_rank == 0:
                 file = h5py.File(self._params['loading']['dir_markers'], 'r')
+                print('Loading markers from file: '.ljust(25), file)
 
                 self._markers[:n_mks_load_cum_sum[0], :
                               ] = file['markers'][:n_mks_load_cum_sum[0], :]
 
                 for i in range(1, self._mpi_size):
                     self._mpi_comm.Send(
                         file['markers'][n_mks_load_cum_sum[i - 1]:n_mks_load_cum_sum[i], :], dest=i, tag=123)
@@ -273,53 +320,71 @@
                 recvbuf = np.zeros(
                     (n_mks_load_loc, self._markers.shape[1]), dtype=float)
                 self._mpi_comm.Recv(recvbuf, source=0, tag=123)
                 self._markers[:n_mks_load_loc, :] = recvbuf
 
         # load fresh markers
         else:
+            
+            if self._mpi_rank == 0:
+                for key, val in self._params['loading'].items():
+                    print((key + ' :').ljust(25), val)
 
             # 1. standard random number generator (pseudo-random)
             if self._params['loading']['type'] == 'pseudo_random':
 
-                np.random.seed(self._params['loading']['seed'])
+                _seed = self._params['loading']['seed']
+                if _seed is not None:
+                    np.random.seed(_seed)
 
                 for i in range(self._mpi_size):
-                    temp = np.random.rand(self.n_mks_load[i], 3+self.vdim)
+                    temp = np.random.rand(self.n_mks_load[i], 3 + self.vdim)
 
                     if i == self._mpi_rank:
-                        self._markers[:n_mks_load_loc, :3+self.vdim] = temp
+                        self._markers[:n_mks_load_loc, :3 + self.vdim] = temp
                         break
 
                 del temp
 
             # 2. plain sobol numbers with skip of first 1000 numbers
             elif self._params['loading']['type'] == 'sobol_standard':
 
-                self._markers[:n_mks_load_loc, :6] = sobol_seq.i4_sobol_generate(
-                    3+self.vdim, n_mks_load_loc, 1000 + (n_mks_load_cum_sum - self.n_mks_load)[self._mpi_rank])
+                self._markers[:n_mks_load_loc, :3 + self.vdim] = sobol_seq.i4_sobol_generate(
+                    3 + self.vdim, n_mks_load_loc, 1000 + (n_mks_load_cum_sum - self.n_mks_load)[self._mpi_rank])
 
             # 3. symmetric sobol numbers in all 6 dimensions with skip of first 1000 numbers
             elif self._params['loading']['type'] == 'sobol_antithetic':
 
+                assert self.vdim == 3, NotImplementedError(
+                    '"sobol_antithetic" requires vdim=3 at the moment.')
+
                 temp_markers = sobol_seq.i4_sobol_generate(
-                    3+self.vdim, n_mks_load_loc//64, 1000 + (n_mks_load_cum_sum - self.n_mks_load)[self._mpi_rank]//64)
+                    3 + self.vdim, n_mks_load_loc//64, 1000 + (n_mks_load_cum_sum - self.n_mks_load)[self._mpi_rank]//64)
 
                 sampling.set_particles_symmetric_3d_3v(
                     temp_markers, self._markers)
 
             # 4. Wrong specification
             else:
                 raise ValueError(
                     'Specified particle loading method does not exist!')
 
             # inversion of Gaussian in velocity space
             for i in range(self.vdim):
                 self._markers[:n_mks_load_loc, 3 + i] = sp.erfinv(
-                    2*self._markers[:n_mks_load_loc, 3 + i] - 1)*self._params['loading']['moments'][self.vdim + i] + self._params['loading']['moments'][i]
+                    2*self._markers[:n_mks_load_loc, 3 + i] - 1) \
+                    * self._params['loading']['moments'][self.vdim + i] + self._params['loading']['moments'][i]
+
+            # inversion method for drawing uniformly on the disc
+            _spatial = self._params['loading']['spatial']
+            if _spatial == 'disc':
+                self._markers[:n_mks_load_loc, 0] = np.sqrt(
+                    self._markers[:n_mks_load_loc, 0])
+            else:
+                assert _spatial == 'uniform', f'Spatial drawing must be "uniform" or "disc", is {_spatial}.'
 
         # fill holes in markers array with -1
         self._markers[n_mks_load_loc:] = -1.
 
         # set markers ID in last column
         self._markers[:n_mks_load_loc, -1] = (n_mks_load_cum_sum - self.n_mks_load)[
             self._mpi_rank] + np.arange(n_mks_load_loc, dtype=float)
@@ -334,14 +399,25 @@
 
                     for j in range(3+self.vdim):
                         if specific_markers[i][j] is not None:
                             self._markers[counter, j] = specific_markers[i][j]
 
                     counter += 1
 
+        # number of holes and markers on process
+        self._holes = self._markers[:, 0] == -1.
+        self._n_holes_loc = np.count_nonzero(self._holes)
+        self._n_mks_loc = self._markers.shape[0] - self._n_holes_loc
+
+        # check if all particle positions are inside the unit cube [0, 1]^3
+        n_mks_load_loc = self._n_mks_load[self._mpi_rank]
+
+        assert np.all(~self._holes[:n_mks_load_loc]) and np.all(
+            self._holes[n_mks_load_loc:])
+
     def mpi_sort_markers(self, do_test=False):
         """ 
         Sorts markers according to domain decomposition.
 
         Parameters
         ----------
         do_test : bool
@@ -381,93 +457,111 @@
                 self.markers[~self._holes, :3] < self.domain_decomp[self.mpi_rank, 1::3]))
 
             assert all_on_right_proc
 
         self.comm.Barrier()
 
     def initialize_weights(self, fun_params, bckgr_params=None):
-        """
-        Computes w0 = f0(t=0, eta(t=0), v(t=0)) / s0(t=0, eta(t=0), v(t=0)) from the initial
-        distribution function and sets the corresponding columns for w0, s0 and weights in markers array.
+        r"""
+        Computes the initial weights
+
+        .. math::
+
+            w_{k0} := \frac{f^0(t, q_k(t)) }{s^0(t, q_k(t)) } = \frac{f^0(0, q_k(0)) }{s^0(0, q_k(0)) } = \frac{f^0_{\textnormal{in}}(q_{k0}) }{s^0_{\textnormal{in}}(q_{k0}) }
+
+        from the initial distribution function :math:`f^0_{\textnormal{in}}` specified in the parmeter file
+        and from the initial volume density :math:`s^n_{\textnormal{in}}` specified in :meth:`struphy.pic.particles.Particles.draw_markers`.
+        Moreover, it sets the corresponding columns for "w0", "s0" and "weights" in the markers array.
         For the control variate method, the background is subtracted.
 
         Parameters
         ----------
         fun_params : dict
             Dictionary of the form {type : class_name, class_name : params_dict} defining the initial condition.
 
         bckgr_params : dict (optional)
             Dictionary of the form {type : class_name, class_name : params_dict} defining the background.
         """
+
+        assert self.domain is not None, 'A domain is needed to initialize weights.'
+
         if self._use_control_variate:
             assert bckgr_params is not None, 'When control variate is used, background parameters must be given!'
 
         # compute s0 and save at vdim + 4
         self._markers[~self._holes, self.vdim + 4] = \
             self.s0(*self.markers_wo_holes[:, :self.vdim + 3].T)
 
         # load distribution function (with given parameters or default parameters)
         fun_name = fun_params['type']
 
         if fun_name in fun_params:
-            f_init = getattr(analytical, fun_name)(**fun_params[fun_name])
+            self._f_init = getattr(maxwellians, fun_name)(
+                **fun_params[fun_name])
         else:
-            f_init = getattr(analytical, fun_name)()
+            self._f_init = getattr(maxwellians, fun_name)()
 
         # compute w0 and save at vdim + 5
-        self._markers[~self._holes, self.vdim + 5] = f_init(
+        self._markers[~self._holes, self.vdim + 5] = self._f_init(
             *self.markers_wo_holes[:, :self.vdim + 3].T) / self.markers_wo_holes[:, self.vdim + 4]
 
         # compute weights and save at vdim + 3
         if self._use_control_variate:
             fun_name = bckgr_params['type']
 
             if fun_name in bckgr_params:
-                f_bckgr = getattr(analytical, fun_name)(
+                self._f_backgr = getattr(maxwellians, fun_name)(
                     **bckgr_params[fun_name])
             else:
-                f_bckgr = getattr(analytical, fun_name)()
+                self._f_backgr = getattr(maxwellians, fun_name)()
 
             self._markers[~self._holes, self.vdim + 3] = self.markers_wo_holes[:, self.vdim + 5] - \
-                f_bckgr(*self.markers_wo_holes[:, :self.vdim + 3].T) / \
+                self.f_backgr(*self.markers_wo_holes[:, :self.vdim + 3].T) / \
                 self.markers_wo_holes[:, self.vdim + 4]
         else:
             self._markers[~self._holes, self.vdim + 3] = \
                 self.markers_wo_holes[:, self.vdim + 5]
 
     def update_weights(self, f0):
         """
-        Updates the marker weights according to w0 - control*f0(eta, v)/s0, where control=True or control=False.
+        Applies the control variate method;
+        updates the time-dependent marker weights according to the algorithm in the `Struphy documentation <https://struphy.pages.mpcdf.de/struphy/sections/discretization.html#control-variate-method>`_.
 
         Parameters
         ----------
         f0 : callable
-            The distribution function used as a control variate. Is called as f0(eta1, eta2, eta3, v1, v2, v3).
+            The distribution function used as a control variate. Is called as f0(eta1, eta2, eta3, *v).
         """
 
         if self._use_control_variate:
             self._markers[~self._holes, self.vdim + 3] = self.markers_wo_holes[:, self.vdim + 5] - \
                 f0(*self.markers_wo_holes[:, :self.vdim + 3].T) / \
                 self.markers_wo_holes[:, self.vdim + 4]
 
-    def binning(self, components, bin_edges, domain=None):
-        """
-        Computes the distribution function via marker binning in logical space using numpy's histogramdd.
+    def binning(self, components, bin_edges, domain=None, velocity_det=None):
+        r"""
+        Computes the distribution function via marker binning in logical space using numpy's histogramdd,
+        following the algorithm outlined in the `Struphy documentation <https://struphy.pages.mpcdf.de/struphy/sections/discretization.html#particle-binning>`_.
+        If both ``domain=None`` and ``velocity_det=None``, approximations of the volume density :math:`f^n(t)` are computed (of :math:`f^0(t)` otherwise). 
 
         Parameters
         ----------
         components : list[bool]
-            List of length 6 giving the directions in phase space in which to bin.
+            List of length n (dim. of phase space) giving the directions in phase space in which to bin.
 
         bin_edges : list[array]
             List of bin edges (resolution) having the length of True entries in components.
 
         domain : struphy.geometry.domains
             Mapping info for evaluating metric coefficients.
 
+        velocity_det : callable
+            The Jacobian deteminant of a velocity space transformation. 
+            Must perform "marker evaluation" if a 2D numpy array is passed, just as ``domain.jacobian_det()``.
+
         Returns
         -------
         f_sclice : array-like
             The reconstructed distribution function.
         """
 
         assert np.count_nonzero(components) == len(bin_edges)
@@ -475,70 +569,76 @@
         # volume of a bin
         bin_vol = 1.
 
         for bin_edges_i in bin_edges:
             bin_vol *= bin_edges_i[1] - bin_edges_i[0]
 
         # extend components list to number of columns of markers array
-        slicing = components + [False] * (self._markers.shape[1] - 6)
+        _n = len(components)
+        slicing = components + [False] * (self._markers.shape[1] - _n)
 
-        # binning with weight transformation
-        if domain is not None:
-            f_slice = np.histogramdd(self.markers_wo_holes[:, slicing],
-                                     bins=bin_edges,
-                                     weights=self.markers_wo_holes[:, 6]
-                                     / domain.jacobian_det(self.markers))[0]
+        # compute weights of histogram:
+        _weights = self.markers_wo_holes[:, _n]
 
-        # binning without weight transformation
-        else:
-            f_slice = np.histogramdd(self.markers_wo_holes[:, slicing],
-                                     bins=bin_edges,
-                                     weights=self.markers_wo_holes[:, 6])[0]
+        # in case of approximation of f^0
+        if domain is not None:
+            _weights /= domain.jacobian_det(self.markers)
+            
+        if velocity_det is not None:
+            _weights /= velocity_det(self.markers)
+
+        f_slice = np.histogramdd(self.markers_wo_holes[:, slicing],
+                                 bins=bin_edges,
+                                 weights=_weights)[0]
 
         return f_slice/(self._n_mks*bin_vol)
 
-    def show_distribution_function(self, components, bin_edges, domain=None):
+    def show_distribution_function(self, components, bin_edges, domain=None, velocity_det=None):
         """
         1D and 2D plots of slices of the distribution function via marker binning.
+        This routine is mainly for de-bugging.
 
         Parameters
         ----------
         components : list[bool]
             List of length 6 giving the directions in phase space in which to bin.
 
         bin_edges : list[array]
             List of bin edges (resolution) having the length of True entries in components.
 
         domain : struphy.geometry.domains
             Mapping info for evaluating metric coefficients.
+            
+        velocity_det : callable
+            The Jacobian deteminant of a velocity space transformation. 
+            Must perform "marker evaluation" if a 2D numpy array is passed, just as ``domain.jacobian_det()``.
         """
 
         import matplotlib.pyplot as plt
 
         n_dim = np.count_nonzero(components)
 
-        assert n_dim == 1 or n_dim == 2
+        assert n_dim == 1 or n_dim == 2, f'Distribution function can only be shown in 1D or 2D slices, not {n_dim}.'
 
-        f_slice = self.binning(components, bin_edges, domain)
+        f_slice = self.binning(components, bin_edges, domain=domain, velocity_det=velocity_det)
 
         bin_centers = [bi[:-1] + (bi[1] - bi[0])/2 for bi in bin_edges]
 
-        # labels = {0 : '$\eta_1$', 1 : '$\eta_2$', 2 : '$\eta_3$', 3 : '$v_x$', 4 : '$v_y$', 5 : '$v_z$'}
-
-        # indices = np.nonzero(components)[0]
+        labels = {0 : '$\eta_1$', 1 : '$\eta_2$', 2 : '$\eta_3$', 3 : '$v_1$', 4 : '$v_2$', 5 : '$v_3$'}
+        indices = np.nonzero(components)[0]
 
         if n_dim == 1:
             plt.plot(bin_centers[0], f_slice)
-            # plt.xlabel(labels[indices[0]])
+            plt.xlabel(labels[indices[0]])
         else:
             plt.contourf(bin_centers[0], bin_centers[1], f_slice, levels=20)
             plt.colorbar()
             plt.axis('square')
-            # plt.xlabel(labels[indices[0]])
-            # plt.ylabel(labels[indices[1]])
+            plt.xlabel(labels[indices[0]])
+            plt.ylabel(labels[indices[1]])
 
         plt.show()
 
     def apply_kinetic_bc(self):
         """
         Apply boundary conditions to markers that are outside of the logical unit cube.
 
@@ -558,16 +658,36 @@
             is_outside_cube[self.holes] = False
 
             # indices or particles that are outside of the logical unit cube
             outside_inds = np.nonzero(is_outside_cube)[0]
 
             # apply boundary conditions
             if bc == 'remove':
+
+                # save the positions and velocities just before the pushing step
+                if self.vdim == 3:
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), 0:3] = self.markers[outside_inds, 9:12]
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), 3:9] = self.markers[outside_inds, 3:9]
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), -1] = self.markers[outside_inds, -1]
+
+                elif self.vdim == 2:
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), 0:4] = self.markers[outside_inds, 9:13]
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), 4:9] = self.markers[outside_inds, 4:9]
+                    self.lost_markers[self.n_lost_markers:self.n_lost_markers +
+                                      len(outside_inds), -1] = self.markers[outside_inds, -1]
+
                 self.markers[outside_inds, :-1] = -1.
 
+                self._n_lost_markers += len(outside_inds)
+
             elif bc == 'periodic':
                 self.markers[outside_inds, axis] = \
                     self.markers[outside_inds, axis] % 1.
 
             elif bc == 'reflect':
                 reflect(self.markers, *self.domain.args_map, outside_inds, axis)
 
@@ -634,24 +754,24 @@
         Returns
         -------
         out : array-like
             The volume-form sampling density.
         -------
         """
         # load sampling density svol = s6 = s3 (normalized to 1 in logical space!)
-        Maxwellian6DUniform = getattr(analytical, 'Maxwellian6DUniform')
+        Maxwellian6DUniform = getattr(maxwellians, 'Maxwellian6DUniform')
 
         s3 = Maxwellian6DUniform(n=1.,
                                  u1=self._params['loading']['moments'][0],
                                  u2=self._params['loading']['moments'][1],
                                  u3=self._params['loading']['moments'][2],
                                  vth1=self._params['loading']['moments'][3],
                                  vth2=self._params['loading']['moments'][4],
                                  vth3=self._params['loading']['moments'][5])
-        
+
         return s3(eta1, eta2, eta3, *v)
 
     def s0(self, eta1, eta2, eta3, *v, remove_holes=True):
         """ 
         Sampling density function as 0 form.
 
         Parameters
@@ -733,15 +853,15 @@
         omega_ch = (Zh*ee*child_params['units_basic']['B'])/(Ah*mH)
         self._kappa = omega_ch*child_params['units_basic']['t']
 
     @property
     def n_cols(self):
         """Number of the columns at each markers.
         """
-        return 25
+        return 29
 
     @property
     def vdim(self):
         """Dimension of the velocity space.
         """
         return 2
 
@@ -760,15 +880,15 @@
         Returns
         -------
         out : array-like
             The volume-form sampling density.
         -------
         """
         # load sampling density svol = s5 (normalized to 1 in logical space!)
-        Maxwellian5DUniform = getattr(analytical, 'Maxwellian5DUniform')
+        Maxwellian5DUniform = getattr(maxwellians, 'Maxwellian5DUniform')
 
         s5 = Maxwellian5DUniform(n=1.,
                                  u_parallel=self.params['loading']['moments'][0],
                                  u_perp=self.params['loading']['moments'][1],
                                  vth_parallel=self.params['loading']['moments'][2],
                                  vth_perp=self.params['loading']['moments'][3])
 
@@ -796,15 +916,15 @@
         etas = (np.vstack((eta1, eta2, eta3)).T).copy()
         bv = self._mhd_equil.bv(etas)
         curlb = self._mhd_equil.jv(etas)/self._mhd_equil.absB0(etas)
         unit_b1 = self._mhd_equil.unit_b1(etas)
 
         # contra-variant components of B* = B + 1/kappa*v_parallel*curlb0
         bstar = bv + 1/self._kappa*v[0]*curlb
-        
+
         # B*_parallel = b0 . B*
         jacobian_det = np.einsum('ij,ij->j', unit_b1, bstar)/v[1]
 
         return self.svol(eta1, eta2, eta3, *v)/np.abs(jacobian_det)
 
     def s0(self, eta1, eta2, eta3, *v, remove_holes=True):
         """
```

### Comparing `struphy-2.0.0/src/struphy/pic/particles_to_grid.py` & `struphy-2.0.1/src/struphy/pic/particles_to_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
 class AccumulatorVector:
     r"""
     Struphy accumulation for only a vector of the form
 
     .. math::
 
-        V^\mu_{ijk} &= \sum_p \Lambda^\mu_{ijk}(\eta_p) * B^\mu_p
+        V^\mu_{ijk} = \sum_p \Lambda^\mu_{ijk}(\eta_p) * B^\mu_p
 
     where :math:`p` runs over the particles, :math:`\Lambda^\mu_{ijk}(\eta_p)` denotes the :math:`ijk`-th basis function
     of the :math:`\mu`-th component of a Derham space (V0, V1, V2, V3) evaluated at the particle position :math:`\eta_p`.
 
     :math:`B^\mu_p` is a particle-dependent "filling function", to be defined in the module **struphy.pic.accum_kernels**.
 
     Parameters
```

### Comparing `struphy-2.0.0/src/struphy/pic/pusher.py` & `struphy-2.0.1/src/struphy/pic/pusher.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 import struphy.pic.utilities_kernels as utilities
 
 import numpy as np
 
 
 class Pusher:
     """
-    Wrapper class for particle pushing.
-
+    Wrapper class for particle pushing. 
+    
+    It retrieves the correct pusher kernel and prepares the FEM arguments passed to the pusher kernel.
+    
     Parameters
     ----------
         derham : struphy.psydac_api.psydac_derham.Derham
             Discrete de Rham sequence on the logical unit cube.
 
         domain : struphy.geometry.domains
             All things mapping.
 
-        pusher_name : str
-            The name of the pusher in the file struphy.pic.pusher_kernels.
+        kernel_name : str
+            The name of the pusher kernel in the file struphy.pic.pusher_kernels.
 
         n_stages : int
             Number of stages of the pusher (e.g. 4 for RK4)
     """
 
-    def __init__(self, derham, domain, pusher_name, n_stages=1):
+    def __init__(self, derham, domain, kernel_name, n_stages=1):
 
         self._derham = derham
         self._domain = domain
         self._n_stages = n_stages
 
         # get FEM information
         self._args_fem = (np.array(derham.p),
                           derham.Vh_fem['0'].knots[0], derham.Vh_fem['0'].knots[1], derham.Vh_fem['0'].knots[2],
                           np.array(derham.Vh['0'].starts),
                           np.array(derham.Vh['1'].starts),
                           np.array(derham.Vh['2'].starts),
                           np.array(derham.Vh['3'].starts))
 
         # select pusher kernel
-        self._pusher_name = pusher_name
-        self._pusher = getattr(pushers, self._pusher_name)
+        self._kernel_name = kernel_name
+        self._kernel = getattr(pushers, self._kernel_name)
 
     def __call__(self, particles, dt, *args_opt, mpi_sort=None, verbose=False):
         """
         Applies the chosen pusher kernel by a time step dt, applies kinetic boundary conditions and performs MPI sorting.
 
         Parameters
         ----------
@@ -69,27 +71,27 @@
         particles.markers[~particles.holes,
                           9:12] = particles.markers[~particles.holes, 0:3]
 
         if particles.kinds == 'Particles5D':
             particles.markers[~particles.holes, 12] = particles.markers[~particles.holes, 3]
 
         for stage in range(self._n_stages):
-            self._pusher(particles.markers, dt, stage, *
+            self._kernel(particles.markers, dt, stage, *
                          self.args_fem, *self.domain.args_map, *args_opt)
 
             # applying kinetic boundary condition
             particles.apply_kinetic_bc()
             
             # sort markers according to domain decomposition
             if mpi_sort == 'each':
                 particles.mpi_sort_markers()
 
             # print stage info
             if self._derham.comm.Get_rank() == 0 and verbose:
-                print(self._pusher_name, 'done. (stage :', stage + 1, ')')
+                print(self._kernel_name, 'done. (stage :', stage + 1, ')')
 
         # sort markers according to domain decomposition
         if mpi_sort == 'last':
             particles.mpi_sort_markers(do_test=True)
 
         # clear buffer columns 9-14 for multi-stage pushers
         particles.markers[~particles.holes, 9:15] = 0.
@@ -118,23 +120,25 @@
     @property
     def args_fem(self):
         """ FEM and MPI related arguments taken by all pushers.
         """
         return self._args_fem
 
     @property
-    def pusher_name(self):
+    def kernel_name(self):
         """ The name of the pyccelized pusher kernel.
         """
-        return self._pusher_name
+        return self._kernel_name
 
 
 class ButcherTableau:
     """
-    Butcher tableau for explicit s-stage Runge-Kutta methods of the form
+    Butcher tableau for explicit s-stage Runge-Kutta methods. 
+    
+    A Butcher tableau has the form
 
       c_0   | 
       c_1   | a_10
       c_2   |   0  a_21
       c_3   |   0    0  a_32
        .    |   .    .    .
        .    |   .    .    .
@@ -191,34 +195,36 @@
     @property
     def n_stages(self):
         """ Number of stages of the s-stage Runge-Kutta method.
         """
         return self._n_stages
 
 
-class Pusher_iteration:
+class Pusher_iteration_Gonzalez:
     """
-    Wrapper class for particle pushing with iterative solver.
+    Wrapper class for particle pushing with discrete_gradient scheme (Gonzalez, mid-point).
+    
+    It retrieves the correct pusher kernel(s) and prepares the FEM arguments passed to the pusher kernel.
 
     Parameters
     ----------
         derham : struphy.psydac_api.psydac_derham.Derham
             Discrete de Rham sequence on the logical unit cube.
 
         domain : struphy.geometry.domains
             All things mapping.
 
-        pusher_name : str
-            The name of the pusher in the file struphy.pic.pusher_kernels.
+        kernel_name : str
+            The name of the pusher kernel in the file struphy.pic.pusher_kernels.
 
         n_stages : int
             Number of stages of the pusher (e.g. 4 for RK4)
     """
 
-    def __init__(self, derham, domain, pusher_name, maxiter=10, tol=1.e-12):
+    def __init__(self, derham, domain, kernel_name, maxiter=10, tol=1.e-12):
 
         self._derham = derham
         self._domain = domain
         self._maxiter = maxiter
         self._tol = tol
 
         self._args_fem = (derham.domain_array[derham.comm.Get_rank(), :],
@@ -226,18 +232,18 @@
                           derham.Vh_fem['0'].knots[0], derham.Vh_fem['0'].knots[1], derham.Vh_fem['0'].knots[2],
                           np.array(derham.Vh['0'].starts),
                           np.array(derham.Vh['1'].starts),
                           np.array(derham.Vh['2'].starts),
                           np.array(derham.Vh['3'].starts))
 
         # select kernels
-        self._pusher_name = pusher_name
-        self._pusher = getattr(pushers, self._pusher_name)
-        self._pusher_prepare = getattr(utilities, self._pusher_name + '_prepare')
-        self._pusher_eval_gradI = getattr(utilities, self._pusher_name + '_eval_gradI')
+        self._kernel_name = kernel_name
+        self._kernel = getattr(pushers, self._kernel_name)
+        self._kernel_prepare = getattr(utilities, self._kernel_name + '_prepare')
+        self._kernel_eval_gradI = getattr(utilities, self._kernel_name + '_eval_gradI')
 
 
     def __call__(self, particles, dt, *args_opt, mpi_sort=None, verbose=False):
         """
         Applies the chosen pusher kernel by a time step dt, applies kinetic boundary conditions and performs MPI sorting.
 
         Parameters
@@ -250,43 +256,164 @@
 
             args_opt : tuple
                 Optional arguments needed for the pushing (typically spline coefficients for field evaluation).
 
             verbose : bool
                 Whether to print some info or not.
         """
-        # TODO: only applicable to Particle5D case! if we have any iterative solver with Particle6D then we should generalize
-        # TODO: maybe we can modulize ... discrete gradient method, fixed-point iterative solver ...
-
-        # save initial etas in columns 9:12
+        # save initial etas and v_parallel in columns 9:13
         particles.markers[~particles.holes, 9:13] = particles.markers[~particles.holes, 0:4]
 
         # prepare the iteration:
-        self._pusher_prepare(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+        self._kernel_prepare(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
         particles.mpi_sort_markers()
 
         # eval gradI 
-        self._pusher_eval_gradI(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+        self._kernel_eval_gradI(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
         particles.mpi_sort_markers()
 
         # start iteration
         for stage in range(self._maxiter):
 
-            self._pusher(particles.markers, dt, stage, self._tol, *self.args_fem, *self.domain.args_map, *args_opt)
+            self._kernel(particles.markers, dt, stage, self._tol, *self.args_fem, *self.domain.args_map, *args_opt)
             particles.mpi_sort_markers()
 
-            self._pusher_eval_gradI(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+            self._kernel_eval_gradI(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
             particles.mpi_sort_markers()
 
-            # print stage info
-            if self._derham.comm.Get_rank() == 0 and verbose:
-                print(self._pusher_name, 'done. (stage :', stage + 1, ')')
+            if stage == self._maxiter-1 and verbose:
+                not_converged = np.logical_not(particles.markers[:,23]==-1.)
+                print('Number of not converged particles:', np.count_nonzero(not_converged))
+                # print('Non converged partices:')
+                # print(particles.markers[not_converged, 0:13])
+                # print('NUmber of iterations', np.average(particles.markers[~particles.holes,20])+1)
+
+        # clear buffer columns 9-23 for multi-stage pushers
+        particles.markers[~particles.holes, 9:28] = 0.
+
+    @property
+    def derham(self):
+        """ Discrete derham sequence.
+        """
+        return self._derham
+
+    @property
+    def domain(self):
+        """ Mapping from logical unit cube to physical domain.
+        """
+        return self._domain
+
+    @property
+    def n_stages(self):
+        """ Number of stages of the pusher.
+        """
+        return self._n_stages
+
+    @property
+    def args_fem(self):
+        """ FEM and MPI related arguments taken by all pushers.
+        """
+        return self._args_fem
+
+    @property
+    def kernel_name(self):
+        """ The name of the pyccelized pusher kernel.
+        """
+        return self._kernel_name
+    
+
+class Pusher_iteration_Itoh:
+    """
+    Wrapper class for particle pushing with discrete_gradient scheme (Itoh_Newton).
+    
+    It retrieves the correct pusher kernel(s) and prepares the FEM arguments passed to the pusher kernel.
+
+    Parameters
+    ----------
+        derham : struphy.psydac_api.psydac_derham.Derham
+            Discrete de Rham sequence on the logical unit cube.
+
+        domain : struphy.geometry.domains
+            All things mapping.
+
+        kernel_name : str
+            The name of the pusher kernel in the file struphy.pic.pusher_kernels.
+
+        n_stages : int
+            Number of stages of the pusher (e.g. 4 for RK4)
+    """
+
+    def __init__(self, derham, domain, kernel_name, maxiter=10, tol=1.e-12):
+
+        self._derham = derham
+        self._domain = domain
+        self._maxiter = maxiter
+        self._tol = tol
+
+        self._args_fem = (derham.domain_array[derham.comm.Get_rank(), :],
+                          np.array(derham.p),
+                          derham.Vh_fem['0'].knots[0], derham.Vh_fem['0'].knots[1], derham.Vh_fem['0'].knots[2],
+                          np.array(derham.Vh['0'].starts),
+                          np.array(derham.Vh['1'].starts),
+                          np.array(derham.Vh['2'].starts),
+                          np.array(derham.Vh['3'].starts))
+
+        # select kernels
+        self._kernel_name = kernel_name
+        self._kernel = getattr(pushers, self._kernel_name)
+        self._kernel_prepare = getattr(utilities, self._kernel_name + '_prepare')
+        self._kernel_prepare1 = getattr(utilities, self._kernel_name + '_prepare1')
+        self._kernel_prepare2 = getattr(utilities, self._kernel_name + '_prepare2')
+
+    def __call__(self, particles, dt, *args_opt, mpi_sort=None, verbose=False):
+        """
+        Applies the chosen pusher kernel by a time step dt, applies kinetic boundary conditions and performs MPI sorting.
+
+        Parameters
+        ----------
+            particles : struphy.pic.particles.Particles6D
+                The particles object holding the markers of shape (Np, 16) to push.
+
+            dt : float
+                The time step.
+
+            args_opt : tuple
+                Optional arguments needed for the pushing (typically spline coefficients for field evaluation).
+
+            verbose : bool
+                Whether to print some info or not.
+        """
+        # save initial etas and v_parallel in columns 9:13
+        particles.markers[~particles.holes, 9:13] = particles.markers[~particles.holes, 0:4]
+
+        # prepare the iteration:
+        self._kernel_prepare(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+        particles.mpi_sort_markers()
+
+        # start iteration
+        for stage in range(self._maxiter):
+
+            self._kernel_prepare1(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+            particles.mpi_sort_markers()
+
+            self._kernel_prepare2(particles.markers, dt, *self.args_fem, *self.domain.args_map, *args_opt)
+            particles.mpi_sort_markers()
+
+            self._kernel(particles.markers, dt, stage, self._maxiter, self._tol, *self.args_fem, *self.domain.args_map, *args_opt)
+            particles.mpi_sort_markers()
 
+            if stage == self._maxiter-1 and verbose:
+                not_converged = np.logical_not(particles.markers[:,13]==-1.)
+                print('Number of not converged particles:', np.count_nonzero(not_converged))
+                # print('Non converged partices:')
+                # print(particles.markers[not_converged, 0:13])
+                # print('Number of iterations', np.average(particles.markers[~particles.holes,14])+1)
+                
         # clear buffer columns 9-23 for multi-stage pushers
-        particles.markers[~particles.holes, 9:24] = 0.
+        particles.markers[~particles.holes, 9:25] = 0.
 
     @property
     def derham(self):
         """ Discrete derham sequence.
         """
         return self._derham
 
@@ -305,11 +432,11 @@
     @property
     def args_fem(self):
         """ FEM and MPI related arguments taken by all pushers.
         """
         return self._args_fem
 
     @property
-    def pusher_name(self):
+    def kernel_name(self):
         """ The name of the pyccelized pusher kernel.
         """
-        return self._pusher_name
+        return self._kernel_name
```

### Comparing `struphy-2.0.0/src/struphy/pic/pusher_kernels.py` & `struphy-2.0.1/src/struphy/pic/pusher_kernels.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 def push_v_with_efield(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
-                       e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]'):
+                       e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
+                       kappa: 'float'):
     r'''Updates
 
     .. math::
 
-        \frac{\mathbf v^{n+1}_p - \mathbf v^n_p}{\Delta t} = DF^{-\top} \hat{\mathbf E}^1(\eta^n_p)
+        \frac{\mathbf v^{n+1}_p - \mathbf v^n_p}{\Delta t} = \kappa DF^{-\top} \hat{\mathbf E}^1(\eta^n_p)
 
     for each marker :math:`p` in markers array, where :math:`\hat{\mathbf E}^1 in H(\textnormal{curl})`.
 
     Parameters
     ----------
         e1_1, e1_2, e1_3: array[float]
             3d array of FE coeffs of E-field as 1-form.
@@ -97,15 +98,15 @@
         e_form[2] = eval_3d.eval_spline_mpi_kernel(
             pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, e1_3, starts1[2])
 
         # electric field: Cartesian components
         linalg.matrix_vector(dfinvt, e_form, e_cart)
 
         # update velocities
-        markers[ip, 3:6] += dt * e_cart
+        markers[ip, 3:6] += dt * kappa * e_cart
 
     #$ omp end parallel
 
 
 @stack_array('df', 'b_form', 'b_cart', 'b_norm', 'e', 'v', 'vperp', 'vxb_norm', 'b_normxvperp', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def push_vxb_analytic(markers: 'float[:,:]', dt: float, stage: int,
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
@@ -197,35 +198,35 @@
         b_form[2] = eval_3d.eval_spline_mpi_kernel(
             pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, b2_3, starts2[2])
 
         # magnetic field: Cartesian components
         linalg.matrix_vector(df, b_form, b_cart)
         b_cart[:] = b_cart/det_df
 
-        # normalized magnetic field direction
+        # magnetic field: magnitude
         b_abs = sqrt(b_cart[0]**2 + b_cart[1]**2 + b_cart[2]**2)
 
+        # only push vxb if magnetic field is non-zero
         if b_abs != 0.:
+            # normalized magnetic field direction
             b_norm[:] = b_cart/b_abs
-        else:
-            b_norm[:] = b_cart
 
-        # parallel velocity v.b_norm
-        vpar = linalg.scalar_dot(v, b_norm)
+            # parallel velocity v.b_norm
+            vpar = linalg.scalar_dot(v, b_norm)
 
-        # first component of perpendicular velocity
-        linalg.cross(v, b_norm, vxb_norm)
-        linalg.cross(b_norm, vxb_norm, vperp)
-
-        # second component of perpendicular velocity
-        linalg.cross(b_norm, vperp, b_normxvperp)
-
-        # analytic rotation
-        markers[ip, 3:6] = vpar*b_norm + \
-            cos(b_abs*dt)*vperp - sin(b_abs*dt)*b_normxvperp
+            # first component of perpendicular velocity
+            linalg.cross(v, b_norm, vxb_norm)
+            linalg.cross(b_norm, vxb_norm, vperp)
+
+            # second component of perpendicular velocity
+            linalg.cross(b_norm, vperp, b_normxvperp)
+
+            # analytic rotation
+            markers[ip, 3:6] = vpar*b_norm + \
+                cos(b_abs*dt)*vperp - sin(b_abs*dt)*b_normxvperp
 
     #$ omp end parallel
 
 
 @stack_array('df', 'b_form', 'b_cart', 'b_prod', 'e', 'v', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'identity', 'rhs', 'lhs', 'lhs_inv', 'vec', 'res')
 def push_vxb_implicit(markers: 'float[:,:]', dt: float, stage: int,
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
@@ -2496,14 +2497,19 @@
             continue
 
         # position
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
+        # get velocity
+        v[0] = markers[ip, 3] / f0_params[4]**2
+        v[1] = markers[ip, 4] / f0_params[5]**2
+        v[2] = markers[ip, 5] / f0_params[6]**2
+
         # spans (i.e. index for non-vanishing basis functions)
         span1 = bsp.find_span(tn1, pn1, eta1)
         span2 = bsp.find_span(tn2, pn2, eta2)
         span3 = bsp.find_span(tn3, pn3, eta3)
 
         # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
         bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
@@ -2517,34 +2523,31 @@
                     kind_map, params_map,
                     t1_map, t2_map, t3_map,
                     p_map,
                     ind1_map, ind2_map, ind3_map,
                     cx, cy, cz,
                     df)
 
-        # compute shifted and stretched velocity
-        v[0] = (markers[ip, 3] - f0_params[1]) / f0_params[4]**2
-        v[1] = (markers[ip, 4] - f0_params[2]) / f0_params[5]**2
-        v[2] = (markers[ip, 5] - f0_params[3]) / f0_params[6]**2
-
         # invert Jacobian matrix
         linalg.matrix_inv(df, df_inv)
+
+        # compute DF^{-1} v
         linalg.matrix_vector(df_inv, v, df_inv_v)
 
         # E-field (1-form)
         e_vec_1 = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3,
                                                  span1, span2, span3, e1_1, starts1[0])
         e_vec_2 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3,
                                                  span1, span2, span3, e1_2, starts1[1])
         e_vec_3 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3,
                                                  span1, span2, span3, e1_3, starts1[2])
 
-        # w_{n+1} = w_n + dt * kappa / (2 * N * s_0) * sqrt(f_0) * ( DF^{-1} \V_th (v_p - u) ) \cdot ( e_{n+1} + e_n )
+        # w_{n+1} = w_n + dt * kappa / (2 * s_0) * sqrt(f_0) * ( DF^{-1} \V_th * v_p ) \cdot ( e_{n+1} + e_n )
         update = (df_inv_v[0] * e_vec_1 + df_inv_v[1] * e_vec_2 + df_inv_v[2] * e_vec_3) * \
-            sqrt(f0) * dt * kappa / (2 * n_markers_tot * markers[ip, 7])
+            sqrt(f0) * dt * kappa / (2 * markers[ip, 7])
         markers[ip, 6] += update
 
     #$ omp end parallel
 
 
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'df', 'df_inv', 'v', 'df_inv_v')
 def push_weights_with_efield_deltaf_vm(markers: 'float[:,:]', dt: float, stage: int,
@@ -3360,15 +3363,15 @@
 
         diff = sqrt((e[0] - markers[ip, 0])**2 +
                     (e[1] - markers[ip, 1])**2 + (e[2] - markers[ip, 2])**2)
 
         if diff < tol:
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
-
+            
             continue
 
         markers[ip, 0:4] = (markers[ip, 0:4] + markers[ip, 9:13])/2.
 
 
 def push_gc2_discrete_gradients(markers: 'float[:,:]', dt: float, stage: int, tol: float,
                                 domain_array: 'float[:]',
@@ -3688,14 +3691,351 @@
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
             continue
 
         markers[ip, 0:3] = (markers[ip, 0:3] + markers[ip, 9:12])/2.
 
 
+def push_gc1_discrete_gradients_Itoh_Newton(markers: 'float[:,:]', dt: float, stage: int, max_iter: int, tol: float,
+                                            domain_array: 'float[:]',
+                                            pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                            starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                            kind_map: int, params_map: 'float[:]',
+                                            p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                            ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                            cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                            kappa: float,
+                                            abs_b: 'float[:,:,:]',
+                                            b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                            norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                            norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                            curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                            grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r'''
+    '''
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # containers for fields
+    identity = zeros((3, 3), dtype=float)
+    temp = empty(3, dtype=float)
+    F = empty(3, dtype=float)
+    S = empty((3, 3), dtype=float)
+    grad_abs_b = empty(3, dtype=float)
+    grad_I = empty(3, dtype=float)
+    Jacobian_grad_I = empty((3, 3), dtype=float)
+    Jacobian = empty((3, 3), dtype=float)
+    Jacobian_inv = empty((3, 3), dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    e_old = empty(3, dtype=float)
+    e_diff = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+        e_old[:] = markers[ip, 9:12]
+        mu = markers[ip, 4]
+
+        e_diff[:] = e[:] - e_old[:]
+
+        for axis in range(3):
+            if e_diff[axis] > 0.5:
+                e_diff[axis] -= 1.
+            elif e_diff[axis] < -0.5:
+                e_diff[axis] += 1.
+
+        # assemble S
+        S[:, :] = ((              0.,  markers[ip, 13], markers[ip, 14]),
+                   (-markers[ip, 13],               0., markers[ip, 15]),
+                   (-markers[ip, 14], -markers[ip, 15],              0.))
+
+        # identity matrix
+        identity[0, 0] = 1.
+        identity[1, 1] = 1.
+        identity[2, 2] = 1.
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        abs_b0 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        grad_abs_b[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        grad_abs_b[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+        grad_abs_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_abs_b3, starts1[2])
+
+        # assemble gradI
+        grad_I[0] = mu*(markers[ip,20] - markers[ip,19])/(e_diff[0])
+        grad_I[1] = mu*(markers[ip,22] - markers[ip,20])/(e_diff[1])
+        grad_I[2] = mu*(abs_b0         - markers[ip,22])/(e_diff[2])
+
+        # calculate F = eta - eta_old + dt*S*grad_I
+        linalg.matrix_vector(S,grad_I,F)
+        F *= -dt
+        F += e_diff[:]
+
+        # assemble Jacobian_grad_I
+        Jacobian_grad_I[0,0] = mu*(markers[ip, 21]*(e_diff[0]) - markers[ip, 20] + markers[ip, 19])/(e_diff[0])**2
+        Jacobian_grad_I[1,0] = mu*(markers[ip, 23]                   - markers[ip, 21])/(e_diff[1])
+        Jacobian_grad_I[2,0] = mu*(grad_abs_b[0]                     - markers[ip, 23])/(e_diff[2])
+        Jacobian_grad_I[0,1] = 0.
+        Jacobian_grad_I[1,1] = mu*(markers[ip, 24]*(e_diff[1]) - markers[ip, 22] + markers[ip, 20])/(e_diff[1])**2
+        Jacobian_grad_I[2,1] = mu*(grad_abs_b[1]                     - markers[ip, 24])/(e_diff[2])
+        Jacobian_grad_I[0,2] = 0.
+        Jacobian_grad_I[1,2] = 0.
+        Jacobian_grad_I[2,2] = mu*(grad_abs_b[2]*(e_diff[2]) - abs_b0 + markers[ip, 22])/(e_diff[2])**2
+
+        # assemble Jacobian and its inverse
+        linalg.matrix_matrix(S,Jacobian_grad_I,Jacobian)
+        Jacobian *= dt
+        Jacobian += identity
+
+        linalg.matrix_inv(Jacobian, Jacobian_inv)
+
+        # calculate eta_new
+        linalg.matrix_vector(Jacobian_inv,F,temp)
+        markers[ip,16:19] = e[:] - temp
+
+        diff = sqrt((temp[0])**2 + (temp[1])**2 + (temp[2])**2)
+
+        if diff < tol:
+            markers[ip, 13] = -1.
+            markers[ip, 14] = stage
+            markers[ip, 0:3] = markers[ip, 16:19]
+
+            continue
+
+        if stage ==  max_iter-1:
+            markers[ip, 0:3] = markers[ip, 16:19]
+
+            continue
+
+        markers[ip, 0] = markers[ip,16]
+        markers[ip, 1] = e_old[1]
+        markers[ip, 2] = e_old[2]
+
+
+def push_gc2_discrete_gradients_Itoh_Newton(markers: 'float[:,:]', dt: float, stage: int, max_iter: int, tol: float,
+                                            domain_array: 'float[:]',
+                                            pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                            starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                            kind_map: int, params_map: 'float[:]',
+                                            p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                            ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                            cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                            kappa: float,
+                                            abs_b: 'float[:,:,:]',
+                                            b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                            norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                            norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                            curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                            grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r'''
+    '''
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # containers for fields
+    identity = zeros((4, 4), dtype=float)
+    temp = empty(4, dtype=float)
+    F = empty(4, dtype=float)
+    S = zeros((4, 4), dtype=float)
+    grad_abs_b = empty(3, dtype=float)
+    grad_I = empty(4, dtype=float)
+    Jacobian_grad_I = empty((4, 4), dtype=float)
+    Jacobian = empty((4, 4), dtype=float)
+    Jacobian_inv = empty((4, 4), dtype=float)
+    Jacobian_temp34 = empty((3,4), dtype=float)
+    Jacobian_temp33 = empty((3,3), dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    e_old = empty(3, dtype=float)
+    e_diff = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+        e_old[:] = markers[ip, 9:12]
+        v = markers[ip, 3]
+        v_old = markers[ip, 12]
+        v_mid = (v + v_old)/2.
+        mu = markers[ip, 4]
+
+        e_diff[:] = e[:] - e_old[:]
+
+        for axis in range(3):
+            if e_diff[axis] > 0.5:
+                e_diff[axis] -= 1.
+            elif e_diff[axis] < -0.5:
+                e_diff[axis] += 1.
+
+        # assemble S
+        S[0:3, 3] = markers[ip, 13:16]
+        S[3, 0:3] = -markers[ip, 13:16]
+
+        # identity matrix
+        identity[0, 0] = 1.
+        identity[1, 1] = 1.
+        identity[2, 2] = 1.
+        identity[3, 3] = 1.
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        abs_b0 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        grad_abs_b[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        grad_abs_b[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+        grad_abs_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_abs_b3, starts1[2])
+
+        # assemble gradI
+        grad_I[0] = mu*(markers[ip,20] - markers[ip,19])/(e_diff[0])
+        grad_I[1] = mu*(markers[ip,22] - markers[ip,20])/(e_diff[1])
+        grad_I[2] = mu*(abs_b0         - markers[ip,22])/(e_diff[2])
+        grad_I[3] = v_mid
+
+        # calculate F = eta - eta_old + dt*S*grad_I
+        linalg.matrix_vector4(S,grad_I,F)
+        F *= -dt
+        F[0:3] += e_diff[:]
+        F[3] += v - v_old
+
+        # assemble Jacobian_grad_I
+        Jacobian_grad_I[0,0] = mu*(markers[ip, 21]*(e_diff[0]) - markers[ip, 20] + markers[ip, 19])/(e_diff[0])**2
+        Jacobian_grad_I[1,0] = mu*(markers[ip, 20]                   - markers[ip, 21])/(e_diff[1])
+        Jacobian_grad_I[2,0] = mu*(grad_abs_b[0]                     - markers[ip, 20])/(e_diff[2])
+        Jacobian_grad_I[3,0] = 0.
+
+        Jacobian_grad_I[0,1] = 0.
+        Jacobian_grad_I[1,1] = mu*(markers[ip, 21]*(e_diff[1]) - markers[ip, 22] + markers[ip, 20])/(e_diff[1])**2
+        Jacobian_grad_I[2,1] = mu*(grad_abs_b[1]                     - markers[ip, 21])/(e_diff[2])
+        Jacobian_grad_I[3,1] = 0.
+
+        Jacobian_grad_I[0,2] = 0.
+        Jacobian_grad_I[1,2] = 0.
+        Jacobian_grad_I[2,2] = mu*(grad_abs_b[2]*(e_diff[2]) - abs_b0 + markers[ip, 22])/(e_diff[2])**2
+        Jacobian_grad_I[3,2] = 0.
+
+        Jacobian_grad_I[0,3] = 0.
+        Jacobian_grad_I[1,3] = 0.
+        Jacobian_grad_I[2,3] = 0.
+        Jacobian_grad_I[3,3] = 0.5
+
+        # assemble Jacobian and its inverse
+        linalg.matrix_matrix4(S,Jacobian_grad_I,Jacobian)
+        Jacobian *= -dt
+        Jacobian += identity
+
+        # Inverse of the Jacobian
+        det_J = linalg.det4(Jacobian)
+
+        Jacobian_inv[0, 0] =  linalg.det(Jacobian[1:     ,1:])/det_J
+        Jacobian_inv[0, 1] = -linalg.det(Jacobian[(0,2,3),1:])/det_J
+        Jacobian_inv[0, 2] =  linalg.det(Jacobian[(0,1,3),1:])/det_J
+        Jacobian_inv[0, 3] = -linalg.det(Jacobian[:3     ,1:])/det_J
+
+        Jacobian_inv[1, 0] = -linalg.det(Jacobian[1:,(0,2,3)])/det_J
+        Jacobian_temp34 = Jacobian[(0,2,3),:]
+        Jacobian_temp33 = Jacobian_temp34[:,(0,2,3)]
+        Jacobian_inv[1, 1] =  linalg.det(Jacobian_temp33)/det_J
+        Jacobian_temp34 = Jacobian[(0,1,3),:]
+        Jacobian_temp33 = Jacobian_temp34[:,(0,2,3)]
+        Jacobian_inv[1, 2] = -linalg.det(Jacobian_temp33)/det_J
+        Jacobian_inv[1, 3] =  linalg.det(Jacobian[:3,(0,2,3)])/det_J
+
+        Jacobian_inv[2, 0] =  linalg.det(Jacobian[1:,(0,1,3)])/det_J
+        Jacobian_temp34 = Jacobian[(0,2,3),:]
+        Jacobian_temp33 = Jacobian_temp34[:,(0,1,3)]
+        Jacobian_inv[2, 1] = -linalg.det(Jacobian_temp33)/det_J
+        Jacobian_temp34 = Jacobian[(0,1,3),:]
+        Jacobian_temp33 = Jacobian_temp34[:,(0,1,3)]
+        Jacobian_inv[2, 2] =  linalg.det(Jacobian_temp33)/det_J
+        Jacobian_inv[2, 3] = -linalg.det(Jacobian[:3,(0,1,3)])/det_J
+
+        Jacobian_inv[3, 0] = -linalg.det(Jacobian[1:     ,:3])/det_J
+        Jacobian_inv[3, 1] =  linalg.det(Jacobian[(0,2,3),:3])/det_J
+        Jacobian_inv[3, 2] = -linalg.det(Jacobian[(0,1,3),:3])/det_J
+        Jacobian_inv[3, 3] =  linalg.det(Jacobian[:3     ,:3])/det_J
+
+        # calculate eta_new
+        linalg.matrix_vector4(Jacobian_inv,F,temp)
+        markers[ip, 16:19] = e[:] - temp[0:3]
+        markers[ip, 3] = v - temp[3]
+
+        diff = sqrt((temp[0])**2 + (temp[1])**2 + (temp[2])**2)
+
+        if diff < tol:
+            markers[ip, 13] = -1.
+            markers[ip, 14] = stage
+            markers[ip, 0:3] = markers[ip, 16:19]
+
+            continue
+
+        if stage == max_iter-1:
+            markers[ip, 0:3] = markers[ip, 16:19]
+
+            continue
+
+        markers[ip, 0] = markers[ip,16]
+        markers[ip, 1] = e_old[1]
+        markers[ip, 2] = e_old[2]
+
+
 def push_gc_cc_J1_H1vec(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -4024,14 +4364,153 @@
 
         # curl_norm_b dot electric field
         temp = linalg.scalar_dot(e, curl_norm_b) / det_df
 
         markers[ip, 3] += temp/abs_b_star_para*v*dt
 
 
+def push_gc_cc_J2_dg_prepare_H1vec(markers: 'float[:,:]', dt: float, stage: int,
+                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                       starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                       kind_map: int, params_map: 'float[:]',
+                       p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                       ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                       cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                       kappa: float,
+                       b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                       norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                       norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                       curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                       u1: 'float[:,:,:]', u2: 'float[:,:,:]', u3: 'float[:,:,:]'):
+    r'''
+    TODO
+    '''
+
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+    df_inv   = empty((3, 3), dtype=float)
+    df_inv_t = empty((3, 3), dtype=float)
+    g_inv    = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # containers for fields
+    tmp1 = empty((3,3), dtype=float)
+    tmp2 = empty((3,3), dtype=float)
+    b_prod = zeros((3,3), dtype=float)
+    norm_b2_prod = zeros((3,3), dtype=float)
+    e = empty(3, dtype=float)
+    u = empty(3, dtype=float)
+    b = empty(3, dtype=float)
+    b_star = empty(3, dtype=float)
+    norm_b1 = empty(3, dtype=float)
+    norm_b2 = empty(3, dtype=float)
+    curl_norm_b = empty(3, dtype=float)
+
+    # marker position eta
+    eta = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        eta[:] = markers[ip, 0:3]
+        v = markers[ip, 3]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(eta[0], eta[1], eta[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # metric coeffs
+        det_df = linalg.det(df)
+        linalg.matrix_inv_with_det(df, det_df, df_inv)
+        linalg.transpose(df_inv, df_inv_t)
+        linalg.matrix_matrix(df_inv, df_inv_t, g_inv)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], eta[0])
+        span2 = bsp.find_span(tn2, pn[1], eta[1])
+        span3 = bsp.find_span(tn3, pn[2], eta[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], eta[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], eta[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], eta[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # b; 2form
+        b[0] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, b1, starts2[0])
+        b[1] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, b2, starts2[1])
+        b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, b3, starts2[2])
+
+        # u; 0form
+        u[0] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, u1, starts0)
+        u[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, u2, starts0)
+        u[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, u3, starts0)
+
+        # norm_b1; 1form
+        norm_b1[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, norm_b11, starts1[0])
+        norm_b1[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, norm_b12, starts1[1])
+        norm_b1[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, norm_b13, starts1[2])
+
+        # norm_b; 2form
+        norm_b2[0] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, norm_b21, starts2[0])
+        norm_b2[1] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, norm_b22, starts2[1])
+        norm_b2[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, norm_b23, starts2[2])
+
+        # curl_norm_b; 2form
+        curl_norm_b[0] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, curl_norm_b1, starts2[0])
+        curl_norm_b[1] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, curl_norm_b2, starts2[1])
+        curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
+
+        # operator bx() as matrix
+        b_prod[0, 1] = -b[2]
+        b_prod[0, 2] = +b[1]
+        b_prod[1, 0] = +b[2]
+        b_prod[1, 2] = -b[0]
+        b_prod[2, 0] = -b[1]
+        b_prod[2, 1] = +b[0]
+
+        norm_b2_prod[0, 1] = -norm_b2[2]
+        norm_b2_prod[0, 2] = +norm_b2[1]
+        norm_b2_prod[1, 0] = +norm_b2[2]
+        norm_b2_prod[1, 2] = -norm_b2[0]
+        norm_b2_prod[2, 0] = -norm_b2[1]
+        norm_b2_prod[2, 1] = +norm_b2[0]
+
+        # b_star; 2form in H1vec
+        b_star[:] = (b + curl_norm_b*v/kappa)/det_df
+
+        # calculate abs_b_star_para
+        abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
+
+        linalg.matrix_matrix(g_inv, norm_b2_prod, tmp1)
+        linalg.matrix_matrix(tmp1, g_inv, tmp2)
+        linalg.matrix_matrix(tmp2, b_prod, tmp1)
+
+        linalg.matrix_vector(tmp1, u, e)
+
+        markers[ip, 0:3] = markers[ip, 9:12]- e/abs_b_star_para*dt
+
+
 def push_gc_cc_J2_dg_H1vec(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
```

### Comparing `struphy-2.0.0/src/struphy/pic/pusher_utilities.py` & `struphy-2.0.1/src/struphy/pic/pusher_utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/sampling.py` & `struphy-2.0.1/src/struphy/pic/sampling.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/sobol_seq.py` & `struphy-2.0.1/src/struphy/pic/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/utilities.py` & `struphy-2.0.1/src/struphy/pic/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/pic/utilities_kernels.py` & `struphy-2.0.1/src/struphy/pic/utilities_kernels.py`

 * *Files 12% similar despite different names*

```diff
@@ -544,14 +544,18 @@
 
         bsp.b_splines_slim(tn1, pn[0], eta1, span1, bn1)
         bsp.b_splines_slim(tn2, pn[1], eta2, span2, bn2)
         bsp.b_splines_slim(tn3, pn[2], eta3, span3, bn3)
 
         B0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, PB, starts0)
 
+        if B0 < 0: 
+            print('eta', eta1, eta2, eta3)
+            print('minus', B0)
+
         markers[ip, 8] = abs(B0)*markers[ip, 4]
 
 
 @stack_array('df', 'dfinv', 'g', 'g_inv', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
 def push_gc1_discrete_gradients_prepare(markers: 'float[:,:]', dt: float,
                                         domain_array: 'float[:]',
                                         pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
@@ -1475,14 +1479,584 @@
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
         # save at the markers
         markers[ip, 13:16] = b_star[:]/abs_b_star_para
         markers[ip, 20:23] = mu*grad_abs_b[:]
 
+@stack_array('df', 'dfinv', 'g', 'g_inv', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc1_discrete_gradients_Itoh_Newton_prepare(markers: 'float[:,:]', dt: float,
+                                                    domain_array: 'float[:]',
+                                                    pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                    starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                    kind_map: int, params_map: 'float[:]',
+                                                    p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                    ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                    cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                    kappa: float, 
+                                                    abs_b: 'float[:,:,:]',
+                                                    b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                    norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                    norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                    curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                    grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""
+    """
+
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+    df_t = empty((3, 3), dtype=float)
+    g = empty((3, 3), dtype=float)
+    g_inv = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # containers 
+    b = empty(3, dtype=float)
+    curl_norm_b = empty(3, dtype=float)
+    S = zeros((3, 3), dtype=float)
+    temp = empty(3, dtype=float)
+    bcross = empty((3, 3), dtype=float)
+    temp1 = empty((3, 3), dtype=float)
+    norm_b2 = empty(3, dtype=float)
+    temp2 = empty((3, 3), dtype=float)
+    b_star = empty(3, dtype=float)
+    norm_b1 = empty(3, dtype=float)
+    grad_abs_b = empty(3, dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+        v = markers[ip, 3]
+        mu = markers[ip, 4]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # evaluate inverse of G
+        linalg.transpose(df, df_t)
+        linalg.matrix_matrix(df_t, df, g)
+        linalg.matrix_inv(g, g_inv)
+
+        # metric coeffs
+        det_df = linalg.det(df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        abs_b0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # norm_b1; 1form
+        norm_b1[0] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, norm_b11, starts1[0])
+        norm_b1[1] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, norm_b12, starts1[1])
+        norm_b1[2] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, norm_b13, starts1[2])
+
+        # norm_b2; 2form
+        norm_b2[0] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, norm_b21, starts2[0])
+        norm_b2[1] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, norm_b22, starts2[1])
+        norm_b2[2] = eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, norm_b23, starts2[2])
+
+        # b; 2form
+        b[0] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, b1, starts2[0])
+        b[1] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, b2, starts2[1])
+        b[2] = eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, b3, starts2[2])
+
+        # curl_norm_b; 2form
+        curl_norm_b[0] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, curl_norm_b1, starts2[0])
+        curl_norm_b[1] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, curl_norm_b2, starts2[1])
+        curl_norm_b[2] = eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
+
+        # grad_abs_b; 1form
+        grad_abs_b[0] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        grad_abs_b[1] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+        grad_abs_b[2] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_abs_b3, starts1[2])
+
+        # transform to H1vec
+        b_star[:] = b + 1/kappa*v*curl_norm_b
+        b_star[:] = b_star/det_df
+
+        # calculate abs_b_star_para
+        abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
+
+        # assemble b cross (.) as 3x3 matrix
+        bcross[:,:] = ( (     0.     ,  -norm_b2[2],   norm_b2[1]), 
+                        (  norm_b2[2],      0.     ,  -norm_b2[0]), 
+                        ( -norm_b2[1],   norm_b2[0],      0.     ) )
+
+        # calculate G^-1 b cross G^-1 
+        linalg.matrix_matrix(bcross, g_inv, temp1)
+        linalg.matrix_matrix(g_inv, temp1, temp2)
+
+        # calculate S
+        S[:,:] = (1/kappa*temp2)/abs_b_star_para
+
+        # save at the markers
+        markers[ip, 13:15] = S[0,1:3]
+        markers[ip, 15] = S[1,2]
+        markers[ip, 19]    = abs_b0
+
+        # calculate S1 * grad I1
+        linalg.matrix_vector(S, grad_abs_b, temp)
+
+        # save at the markers
+        markers[ip, 16:19] = markers[ip, 0:3] + dt*temp[:]*mu
+        
+        # send particles to the (eta^0_n+1,eta_n, eta_n)
+        markers[ip, 0] = markers[ip, 16]
+
+@stack_array('df', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc1_discrete_gradients_Itoh_Newton_prepare1(markers: 'float[:,:]', dt: float,
+                                                     domain_array: 'float[:]',
+                                                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                     kind_map: int, params_map: 'float[:]',
+                                                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                     cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                     kappa: float, 
+                                                     abs_b: 'float[:,:,:]',
+                                                     b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                     norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                     norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                     curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                     grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""TODO
+
+    """
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        markers[ip, 20] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        markers[ip, 21] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+
+        # send particles to the (eta^0_n+1,eta^0_n+1, eta_n)
+        markers[ip, 1] = markers[ip, 17]
+        
+@stack_array('df', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc1_discrete_gradients_Itoh_Newton_prepare2(markers: 'float[:,:]', dt: float,
+                                                     domain_array: 'float[:]',
+                                                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                     kind_map: int, params_map: 'float[:]',
+                                                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                     cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                     kappa: float, 
+                                                     abs_b: 'float[:,:,:]',
+                                                     b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                     norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                     norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                     curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                     grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""TODO
+
+    """
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        markers[ip, 22] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        markers[ip, 23] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        markers[ip, 24] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+
+        # send particles to the (eta^0_n+1,eta^0_n+1, eta^0_n+1)
+        markers[ip, 2] = markers[ip, 18]
+
+@stack_array('df', 'dfinv', 'g', 'g_inv', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc2_discrete_gradients_Itoh_Newton_prepare(markers: 'float[:,:]', dt: float,
+                                                    domain_array: 'float[:]',
+                                                    pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                    starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                    kind_map: int, params_map: 'float[:]',
+                                                    p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                    ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                    cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                    kappa: float, 
+                                                    abs_b: 'float[:,:,:]',
+                                                    b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                    norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                    norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                    curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                    grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""
+    """
+
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # containers 
+    b = empty(3, dtype=float)
+    curl_norm_b = empty(3, dtype=float)
+    b_star = empty(3, dtype=float)
+    norm_b1 = empty(3, dtype=float)
+    grad_abs_b = empty(3, dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+        v = markers[ip, 3]
+        mu = markers[ip, 4]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # metric coeffs
+        det_df = linalg.det(df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        abs_b0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # norm_b1; 1form
+        norm_b1[0] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, norm_b11, starts1[0])
+        norm_b1[1] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, norm_b12, starts1[1])
+        norm_b1[2] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, norm_b13, starts1[2])
+
+        # b; 2form
+        b[0] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, b1, starts2[0])
+        b[1] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, b2, starts2[1])
+        b[2] = eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, b3, starts2[2])
+
+        # curl_norm_b; 2form
+        curl_norm_b[0] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2] - 1, bn1, bd2, bd3, span1, span2, span3, curl_norm_b1, starts2[0])
+        curl_norm_b[1] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, curl_norm_b2, starts2[1])
+        curl_norm_b[2] = eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
+
+        # grad_abs_b; 1form
+        grad_abs_b[0] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        grad_abs_b[1] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+        grad_abs_b[2] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_abs_b3, starts1[2])
+
+        # transform to H1vec
+        b_star[:] = b + 1/kappa*v*curl_norm_b
+        b_star[:] = b_star/det_df
+
+        # calculate abs_b_star_para
+        abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
+
+        # save at the markers
+        markers[ip, 13:16] = b_star[:]/abs_b_star_para
+        markers[ip, 19]    = abs_b0
+
+        # calculate b_star . grad_abs_b
+        b_star_dot_grad_abs_b = linalg.scalar_dot(b_star, grad_abs_b)*mu
+
+        # save at the markers
+        markers[ip, 16:19] = markers[ip, 0:3] + dt*b_star[:]/abs_b_star_para*v
+        markers[ip, 3] = markers[ip, 12] - dt*b_star_dot_grad_abs_b/abs_b_star_para
+        
+        # send particles to the (eta^0_n+1,eta_n, eta_n)
+        markers[ip, 0] = markers[ip, 16]
+
+@stack_array('df', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc2_discrete_gradients_Itoh_Newton_prepare1(markers: 'float[:,:]', dt: float,
+                                                     domain_array: 'float[:]',
+                                                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                     kind_map: int, params_map: 'float[:]',
+                                                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                     cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                     kappa: float, 
+                                                     abs_b: 'float[:,:,:]',
+                                                     b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                     norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                     norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                     curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                     grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""TODO
+
+    """
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        markers[ip, 20] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        markers[ip, 21] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+
+        # send particles to the (eta^0_n+1,eta^0_n+1, eta_n)
+        markers[ip, 1] = markers[ip, 17]
+
+@stack_array('df', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
+def push_gc2_discrete_gradients_Itoh_Newton_prepare2(markers: 'float[:,:]', dt: float,
+                                                     domain_array: 'float[:]',
+                                                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                                     kind_map: int, params_map: 'float[:]',
+                                                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                                     cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                                     kappa: float, 
+                                                     abs_b: 'float[:,:,:]',
+                                                     b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                                                     norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                                                     norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                                                     curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                                                     grad_abs_b1: 'float[:,:,:]', grad_abs_b2: 'float[:,:,:]', grad_abs_b3: 'float[:,:,:]'):
+    r"""TODO
+
+    """
+    # allocate metric coeffs
+    df = empty((3, 3), dtype=float)
+
+    # allocate spline values
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # marker position e
+    e = empty(3, dtype=float)
+    
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    for ip in range(n_markers):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        if markers[ip, 13] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(e[0], e[1], e[2],
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # spline evaluation
+        span1 = bsp.find_span(tn1, pn[0], e[0])
+        span2 = bsp.find_span(tn2, pn[1], e[1])
+        span3 = bsp.find_span(tn3, pn[2], e[2])
+
+        bsp.b_d_splines_slim(tn1, pn[0], e[0], span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn[1], e[1], span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn[2], e[2], span3, bn3, bd3)
+
+        # eval all the needed field
+        # abs_b; 0form
+        markers[ip, 22] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, abs_b, starts0)
+
+        # grad_abs_b; 1form
+        markers[ip, 23] = eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_abs_b1, starts1[0])
+        markers[ip, 24] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_abs_b2, starts1[1])
+
+        # send particles to the (eta^0_n+1,eta^0_n+1, eta^0_n+1)
+        markers[ip, 2] = markers[ip, 18]
 
 @stack_array('grad_PB', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def accum_gradI_const(markers: 'float[:,:]', n_markers_tot: 'int',
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                       starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                       grad_PB1: 'float[:,:,:]', grad_PB2: 'float[:,:,:]', grad_PB3: 'float[:,:,:]',
                       scale: 'float'):
@@ -1535,14 +2109,63 @@
         grad_PB[1] = eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
 
         res += linalg.scalar_dot(markers[ip, 15:18] , grad_PB) * weight * mu * scale
         
     return res/n_markers_tot
 
+@stack_array('PB', 'bn1', 'bn2', 'bn3')
+def accum_en_fB(markers: 'float[:,:]', n_markers_tot: 'int',
+                pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                PB: 'float[:,:,:]'):
+    
+    r"""TODO
+    """
+    # allocate for magnetic field evaluation
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # allocate for filling
+    res = zeros(1, dtype=float)
+
+    # get number of markers
+    n_markers_loc = shape(markers)[0]
+    
+    for ip in range(n_markers_loc):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        # marker positions
+        eta1 = markers[ip, 0]
+        eta2 = markers[ip, 1]
+        eta3 = markers[ip, 2]
+
+        # marker weight and velocity
+        mu = markers[ip, 4]
+        weight = markers[ip, 5]
+
+        # b-field evaluation
+        span1 = bsp.find_span(tn1, pn[0], eta1)
+        span2 = bsp.find_span(tn2, pn[1], eta2)
+        span3 = bsp.find_span(tn3, pn[2], eta3)
+
+        bsp.b_splines_slim(tn1, pn[0], eta1, span1, bn1)
+        bsp.b_splines_slim(tn2, pn[1], eta2, span2, bn2)
+        bsp.b_splines_slim(tn3, pn[2], eta3, span3, bn3)
+
+        B0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, PB, starts0)
+
+        res += abs(B0)*mu*weight
+        
+    return res/n_markers_tot
+
 @stack_array('e', 'e_diff')
 def check_eta_diff(markers: 'float[:,:]'):
     r'''TODO
     '''
     # marker position e
     e = empty(3, dtype=float)
     e_diff = empty(3, dtype=float)
@@ -1563,14 +2186,42 @@
             if e_diff[axis] > 0.5:
                 e_diff[axis] -= 1.
             elif e_diff[axis] < -0.5:
                 e_diff[axis] += 1.
 
         markers[ip,15:18] = e_diff[:]
 
+@stack_array('e', 'e_diff')
+def check_eta_diff2(markers: 'float[:,:]'):
+    r'''TODO
+    '''
+    # marker position e
+    e = empty(3, dtype=float)
+    e_diff = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers_loc = shape(markers)[0]
+
+    for ip in range(n_markers_loc):
+        
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        e[:] = markers[ip, 0:3]
+        e_diff[:] = e[:] - markers[ip, 12:15]
+
+        for axis in range(3):
+            if e_diff[axis] > 0.5:
+                e_diff[axis] -= 1.
+            elif e_diff[axis] < -0.5:
+                e_diff[axis] += 1.
+
+        markers[ip,15:18] = e_diff[:]
+
 @stack_array('e', 'e_diff', 'e_mid')
 def check_eta_mid(markers: 'float[:,:]'):
     r'''TODO
     '''
     # marker position e
     e = empty(3, dtype=float)
     e_diff = empty(3, dtype=float)
@@ -1582,27 +2233,26 @@
     for ip in range(n_markers_loc):
         
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
         e[:] = markers[ip, 0:3]
+        markers[ip, 12:15] = e[:]
+
         e_diff[:] = e[:] - markers[ip, 9:12]
         e_mid[:] = (e[:] + markers[ip, 9:12])/2.
 
         for axis in range(3):
             if e_diff[axis] > 0.5:
                 e_mid[axis] += 0.5
             elif e_diff[axis] < -0.5:
                 e_mid[axis] += 0.5
 
-        markers[ip,12:15] = e_mid[:]
-
-
-
+        markers[ip,0:3] = e_mid[:]
 
 @stack_array('df', 'dfinv', 'dfinv_t', 'e', 'v', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'a_form', 'dfta_form')
 def canonical_kinetic_particles(res: 'float[:]', markers: 'float[:,:]',
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                       starts1: 'int[:,:]',
                       kind_map: int, params_map: 'float[:]',
                       p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
```

### Comparing `struphy-2.0.0/src/struphy/polar/basic.py` & `struphy-2.0.1/src/struphy/polar/basic.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/polar/extraction_operators.py` & `struphy-2.0.1/src/struphy/polar/extraction_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/polar/linear_operators.py` & `struphy-2.0.1/src/struphy/polar/linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/post_processing/cprofile_analyser.py` & `struphy-2.0.1/src/struphy/post_processing/cprofile_analyser.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/post_processing/pproc_struphy.py` & `struphy-2.0.1/src/struphy/post_processing/pproc_struphy.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/post_processing/profile_struphy.py` & `struphy-2.0.1/src/struphy/post_processing/profile_struphy.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/propagators/base.py` & `struphy-2.0.1/src/struphy/propagators/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 
 
 class Propagator(metaclass=ABCMeta):
     '''Base class for Struphy propagators used in Struphy models.
 
     Note
     ---- 
-        All Struphy propagators are subclasses of ``Propagator``. This parent class is also used
-        for solvers.'''
+        All Struphy propagators are subclasses of ``Propagator``.
+        
+        The ``__init__`` of child classes must take as first arguments the variables to be updated.
+        All additional arguments MUST be passed as **keyword arguments**.
+    '''
 
     @property
     @abstractmethod
     def variables(self):
-        '''List of variabels to be updated by the propagator. Can contain
-
-            * FE coefficients from the ``Field.vector`` property of :ref:`fields`.
-            * Marker arrays from the ``Particles6D.markers`` (or ``Particles5D.markers``) property of :ref:`particles`.    
+        '''List of FEEC variables (not particles) to be updated by the propagator. 
+        Contains FE coefficients from the ``Field.vector`` property of :ref:`fields`.
         '''
         pass
 
     @abstractmethod
     def __call__(self, dt):
-        '''Push entries in ``Propagator.variables`` from t -> t + dt.
-        Use ``Propagators.in_place_update`` to write to ``Propagator.variables``.
+        '''Update from t -> t + dt.
+        Use ``Propagators.in_place_update`` to write to FE variables to ``Propagator.variables``.
 
         Parameters
         ----------
             dt : float
                 Time step size.
         '''
         pass
@@ -77,15 +78,15 @@
         return self._basis_ops
 
     @basis_ops.setter
     def basis_ops(self, basis_ops):
         self._basis_ops = basis_ops
 
     def in_place_update(self, *variables_new):
-        '''Writes new entries into ``Propagator.variables``.
+        '''Writes new entries into the FEEC variables in ``Propagator.variables``.
 
         Parameters
         ----------
             variables_new : list
                 Same sequence as in ``Propagator.variables`` but with the updated variables, 
                 i.e. for variables = [e, b] we must have variables_new = [e_updated, b_updated].
```

### Comparing `struphy-2.0.0/src/struphy/propagators/propagators_coupling.py` & `struphy-2.0.1/src/struphy/propagators/propagators_coupling.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from struphy.propagators.base import Propagator
 from struphy.linear_algebra.schur_solver import SchurSolver
 from struphy.pic.particles import Particles6D
 from struphy.pic.particles_to_grid import Accumulator, AccumulatorVector
 from struphy.pic.pusher import Pusher
 import struphy.pic.utilities_kernels as utilities
 from struphy.polar.basic import PolarVector
-from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform, Maxwellian5DUniform
+from struphy.kinetic_background.base import Maxwellian
+from struphy.kinetic_background.maxwellians import Maxwellian6DUniform, Maxwellian5DUniform
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 from struphy.psydac_api.linear_operators import CompositeLinearOperator as Compose
 from struphy.psydac_api.linear_operators import ScalarTimesLinearOperator as Multiply
 from struphy.psydac_api.linear_operators import InverseLinearOperator as Inverse
 from struphy.psydac_api import preconditioner
 from struphy.psydac_api.linear_operators import LinOpWithTransp
@@ -65,25 +66,25 @@
 
     **params : dict
         Solver- and/or other parameters for this splitting step.
     '''
 
     def __init__(self, e, particles, **params):
 
-        from struphy.kinetic_background.analytical import Maxwellian6DUniform
+        from struphy.kinetic_background.maxwellians import Maxwellian6DUniform
 
         # pointers to variables
         assert isinstance(e, (BlockVector, PolarVector))
         self._e = e
 
         assert isinstance(particles, Particles6D)
         self._particles = particles
 
         # parameters
-        params_default = {'alpha': 1e2,
+        params_default = {'alpha': 1.,
                           'kappa': 1.,
                           'f0': Maxwellian6DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
@@ -158,23 +159,24 @@
                                self._f0_params, self._alpha, self._kappa)
 
         # Update Schur solver
         self._schur_solver.BC = - self._accum.operators[0].matrix / 4
 
         # allocate temporary BlockVector during solution
         self._e_temp, info = self._schur_solver(
-            self._e, self._accum.vectors[0] / 2., dt)
+            self._e, self._accum.vectors[0] / 2., dt,
+            out=self._e_temp)
 
         # Store old weights
         self._old_weights[~self._particles.holes] = self._particles.markers[~self._particles.holes, 6]
 
         # reset _e_sum
         self._e_sum *= 0.
 
-        # self._e_sum = self._e_temp + self._e
+        # Compute e^{n+1} + e^n
         self._e_sum += self._e_temp
         self._e_sum += self._e
 
         # Update weights
         self._pusher(self._particles, dt,
                      self._e_sum.blocks[0]._data,
                      self._e_sum.blocks[1]._data,
@@ -220,15 +222,15 @@
 
     **params : dict
         Solver- and/or other parameters for this splitting step.
     '''
 
     def __init__(self, e, particles, **params):
 
-        from struphy.kinetic_background.analytical import Maxwellian6DUniform
+        from struphy.kinetic_background.maxwellians import Maxwellian6DUniform
 
         # pointers to variables
         assert isinstance(e, (BlockVector, PolarVector))
         self._e = e
 
         assert isinstance(particles, Particles6D)
         self._particles = particles
@@ -991,15 +993,15 @@
 
         # write new coeffs into Propagator.variables
         max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
             print('Status     for CurrentCoupling5DCurrent1:', info['success'])
             print('Iterations for CurrentCoupling5DCurrent1:', info['niter'])
-            print('Maxdiff u1 for CurrentCoupling5DCurrent1:', max_du)
+            print('Maxdiff up for CurrentCoupling5DCurrent1:', max_du)
             print()
 
 
 class CurrentCoupling5DCurrent2(Propagator):
     r'''
     TODO
     '''
@@ -1196,23 +1198,24 @@
         self._pusher(self._particles, dt,
                      self._kappa,
                      self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
                      self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                      self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                      self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                      self._u_avg2[0]._data, self._u_avg2[1]._data, self._u_avg2[2]._data,
-                     self._butcher.a, self._butcher.b, self._butcher.c)
+                     self._butcher.a, self._butcher.b, self._butcher.c,
+                     mpi_sort='each')
 
         # write new coeffs into Propagator.variables
         max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
             print('Status     for CurrentCoupling5DCurrent2:', info['success'])
             print('Iterations for CurrentCoupling5DCurrent2:', info['niter'])
-            print('Maxdiff u1 for CurrentCoupling5DCurrent2:', max_du)
+            print('Maxdiff up for CurrentCoupling5DCurrent2:', max_du)
             print()
 
 
 class CurrentCoupling5DCurrent2dg(Propagator):
     r'''
     TODO
     '''
@@ -1298,24 +1301,22 @@
         if params['pc'] is None:
             self._pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             self._pc = pc_class(self._A)
 
         # Call the accumulation and Pusher class
-        # self._ACC_prepare = Accumulator(self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg_prepare', add_vector=True, symmetry='symm')
-        # self._ACC = Accumulator(self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg', add_vector=True, symmetry='symm')
-        # self._pusher = Pusher(self.derham, self.domain, 'push_gc_cc_J2_dg_' + params['u_space'])
-
-        self._ACC_prepare = Accumulator(
-            self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg_prepare_faster', add_vector=True, symmetry='symm')
-        self._ACC = Accumulator(
-            self.derham, self.domain,  params['u_space'], 'cc_lin_mhd_5d_J2_dg_faster', add_vector=True, symmetry='symm')
-        self._pusher = Pusher(self.derham, self.domain,
-                              'push_gc_cc_J2_dg_faster_' + params['u_space'])
+        self._ACC_prepare = Accumulator(self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg_prepare', add_vector=True, symmetry='symm')
+        self._ACC = Accumulator(self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg', add_vector=True, symmetry='symm')
+        self._pusher_prepare = Pusher(self.derham, self.domain, 'push_gc_cc_J2_dg_prepare_' + params['u_space'])
+        self._pusher = Pusher(self.derham, self.domain, 'push_gc_cc_J2_dg_' + params['u_space'])
+
+        # self._ACC_prepare = Accumulator(self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_J2_dg_prepare_faster', add_vector=True, symmetry='symm')
+        # self._ACC = Accumulator(self.derham, self.domain,  params['u_space'], 'cc_lin_mhd_5d_J2_dg_faster', add_vector=True, symmetry='symm')
+        # self._pusher = Pusher(self.derham, self.domain,'push_gc_cc_J2_dg_faster_' + params['u_space'])
 
         # linear solver
         self._solver = getattr(it_solvers, params['type'])(self._A.domain)
 
         # allocate dummy vectors to avoid temporary array allocations
         self._rhs1 = u.space.zeros()
         self._rhs2 = u.space.zeros()
@@ -1342,28 +1343,29 @@
     def __call__(self, dt):
 
         # save old u
         self.variables[0].copy(out=self._u_old)
 
         self._u_old.update_ghost_regions()
 
+        # sum up total magnetic field b_full1 = b_eq + b_tilde (in-place)
+        self._b_eq.copy(out=self._b_full)
+
         # sum up total magnetic field
         if self._b is not None:
             self._b_full += self._b
 
         self._b_full.update_ghost_regions()
 
         self._PBb = self._PB.dot(self._b_full)
+        self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
-        # reorganize particles
-        self._particles.mpi_sort_markers()
-
         #####################################
         # discrete gradient solver(mid point)#
         #####################################
         # eval initial particle energy
         self._particles.save_magnetic_energy(self.derham, self._PBb)
         self._en_fB_old = self._particles.markers[~self._particles.holes, 5].dot(
             self._particles.markers[~self._particles.holes, 8])/self._particles.n_mks
@@ -1395,58 +1397,59 @@
 
         # ------------ initial guess of H ------------#
         # save old etas in columns 9-11
         self._particles.markers[~self._particles.holes,
                                 9:12] = self._particles.markers[~self._particles.holes, 0:3]
 
         # initial guess of eta is stored in columns 0:3
-        self._pusher._pusher(self._particles.markers, dt, 0, *self._pusher._args_fem, *self.domain.args_map,
-                             self._kappa,
-                             self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                             self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                             self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                             self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                             self._u_old[0]._data, self._u_old[1]._data, self._u_old[2]._data)
+        self._pusher_prepare._pusher(self._particles.markers, dt, 0, *self._pusher._args_fem, *self.domain.args_map,
+                                     self._kappa,
+                                     self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                                     self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                                     self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                                     self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                                     self._u_old[0]._data, self._u_old[1]._data, self._u_old[2]._data)
 
         self._particles.mpi_sort_markers()
 
         # print('H initial guess', np.max(self._particles.markers[~self._particles.holes,0:3]))
 
         # ------------ fixed point iteration ------------#
-        for stage in range(20):
+        for stage in range(30):
 
-            print(self._particles.markers[~self._particles.holes, 0:8])
+            # print(self._particles.markers[~self._particles.holes,0:8])
 
             self._u_new.copy(out=self._u_temp)
 
             # save eta diff at markers[ip, 15:18]
             utilities.check_eta_diff(self._particles.markers)
             # self._particles.markers[~self._particles.holes, 15:18] = self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 9:12]
 
             self._sum_H_diff_loc = np.sum(
                 self._particles.markers[~self._particles.holes, 15:18]**2)
             self._u_norm_loc = np.sum(
                 (self._u_new.toarray_local() - self._u_old.toarray_local())**2)
             self._denominator = self._sum_H_diff_loc + self._u_norm_loc
 
             # eval particle magnetic energy
-            self._particles.save_magnetic_energy(self.derham, self._PBb)
-            self._en_fB_loc = self._particles.markers[~self._particles.holes, 5].dot(
-                self._particles.markers[~self._particles.holes, 8])/self._particles.n_mks
+            self._en_fB_loc = utilities.accum_en_fB(self._particles.markers, self._particles.n_mks, *self._pusher._args_fem,
+                                                    self._PBb._data)[0]
+            # self._particles.save_magnetic_energy(self.derham, self._PBb)
+            # self._en_fB_loc = self._particles.markers[~self._particles.holes, 5].dot(
+            #     self._particles.markers[~self._particles.holes, 8])/self._particles.n_mks
 
             # move particle to the mid point position and then the real position is saved at markers[ip, 12:15]
             utilities.check_eta_mid(self._particles.markers)
-            self._particles.markers[~self._particles.holes, 0:3], self._particles.markers[~self._particles.holes,
-                                                                                          12:15] = self._particles.markers[~self._particles.holes, 12:15].copy(), self._particles.markers[~self._particles.holes, 0:3].copy()
+            # self._particles.markers[~self._particles.holes, 0:3], self._particles.markers[~self._particles.holes,
+            #                                                                               12:15] = self._particles.markers[~self._particles.holes, 12:15].copy(), self._particles.markers[~self._particles.holes, 0:3].copy()
             self._particles.mpi_sort_markers()
 
             # Accumulate
             self._accum_gradI_const_loc = utilities.accum_gradI_const(self._particles.markers, self._particles.n_mks, *self._pusher._args_fem,
-                                                                      self._grad_PBb[0]._data, self._grad_PBb[
-                                                                          1]._data, self._grad_PBb[2]._data,
+                                                                      self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
                                                                       self._coupling_vec)[0]
 
             # gradI_const = (en_u - en_u_old - u_diff.dot(self._A.dot(u_mid)) + np.sum(en_fB) - np.sum(en_fB_old) - np.sum(accum_gradI_const))/denominator
             self._gradI_const = (
                 self._en_fB_loc - self._en_fB_old - self._accum_gradI_const_loc)/self._denominator
 
             # Accumulate
@@ -1467,67 +1470,78 @@
             info = self._solver.solve(self._A, self._rhs1, self._pc,
                                       x0=self._u_temp, tol=self._tol,
                                       maxiter=self._maxiter, verbose=self._verbose,
                                       out=self._u_new)[1]
 
             self._u_new.update_ghost_regions()
 
-            # send particle back to the real position
-            self._particles.markers[~self._particles.holes, 0:3], self._particles.markers[~self._particles.holes,
-                                                                                          12:15] = self._particles.markers[~self._particles.holes, 12:15].copy(), self._particles.markers[~self._particles.holes, 0:3].copy()
-            self._particles.mpi_sort_markers()
-
-            self._particles.markers[~self._particles.holes,
-                                    12:15] = self._particles.markers[~self._particles.holes, 0:3]
+            # send particle back to the mid position
+            # self._particles.markers[~self._particles.holes, 0:3] = self._particles.markers[~self._particles.holes, 9:12].copy()
+            # self._particles.mpi_sort_markers()
 
             # update H (1 step ealiler u is needed, u_temp)
             # calculate average u
             self._u_old.copy(out=self._u_pusher)
             self._u_pusher += self._u_temp
             self._u_pusher /= 2
 
             self._u_temp.copy(out=self._u_diff)
             self._u_diff -= self._u_old
             self._u_diff *= self._gradI_const
 
             self._u_diff.update_ghost_regions()
 
             self._u_pusher += Inverse(self._A, pc=self._pc,
-                                      tol=1e-18).dot(self._u_diff)
+                                      tol=1e-15).dot(self._u_diff)
 
             self._u_pusher.update_ghost_regions()
 
             self._pusher._pusher(self._particles.markers, dt, 0, *self._pusher._args_fem, *self.domain.args_map,
                                  self._kappa,
                                  self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
                                  self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                                  self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                                  self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                  self._u_pusher[0]._data, self._u_pusher[1]._data, self._u_pusher[2]._data)
-
+            
+            n_lost_markers_before = self._particles.n_lost_markers
+            print('Number of lost markers before iteration push', n_lost_markers_before)
             self._particles.mpi_sort_markers()
+            n_lost_markers_after = self._particles.n_lost_markers
+            print('Number of lost markers after iteration push', n_lost_markers_after)
+            print()
 
+            if n_lost_markers_after != n_lost_markers_before:
+                # go back to former step
+                self._particles.markers[~self._particles.holes, 0:3] = self._particles.markers[~self._particles.holes, 12:15].copy()
+                self._u_temp.copy(out=self._u_new)
+                continue
             print('stage', stage+1)
 
             self._u_norm_loc = np.sum(
                 (self._u_new.toarray_local() - self._u_temp.toarray_local())**2)
             print('u differences',  np.sqrt(self._u_norm_loc))
 
+            # self._sum_H_diff_loc = np.sum(
+            #     (self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 12:15])**2)
+            utilities.check_eta_diff2(self._particles.markers)
+            # self._particles.markers[~self._particles.holes, 15:18] = self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 9:12]
+
             self._sum_H_diff_loc = np.sum(
-                (self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 12:15])**2)
+                self._particles.markers[~self._particles.holes, 15:18]**2)
             print('H differences', np.sqrt(self._sum_H_diff_loc))
 
             diff = np.sqrt(self._u_norm_loc + self._sum_H_diff_loc)
             print('diff', diff)
 
-            if diff < 1e-15:
+            if diff < 1e-11:
                 print('converged!')
                 break
 
         # write new coeffs into Propagator.variables
         max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
-            print('Status     for StepPressurecoupling:', info['success'])
-            print('Iterations for StepPressurecoupling:', info['niter'])
-            print('Maxdiff u1 for StepPressurecoupling:', max_du)
+            print('Status     for CurrentCoupling5DCurrent2dg:', info['success'])
+            print('Iterations for CurrentCoupling5DCurrent2dg:', info['niter'])
+            print('Maxdiff up for CurrentCoupling5DCurrent2dg:', max_du)
             print()
```

### Comparing `struphy-2.0.0/src/struphy/propagators/propagators_fields.py` & `struphy-2.0.1/src/struphy/propagators/propagators_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import numpy as np
 from numpy import zeros
 
 from struphy.propagators.base import Propagator
 from struphy.linear_algebra.schur_solver import SchurSolver
 from struphy.pic.particles_to_grid import Accumulator
 from struphy.polar.basic import PolarVector
-from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform, Maxwellian5DUniform
+from struphy.kinetic_background.base import Maxwellian
+from struphy.kinetic_background.maxwellians import Maxwellian6DUniform, Maxwellian5DUniform
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 from struphy.psydac_api.linear_operators import CompositeLinearOperator as Compose
 from struphy.psydac_api.linear_operators import SumLinearOperator as Sum
 from struphy.psydac_api.linear_operators import ScalarTimesLinearOperator as Multiply
 from struphy.psydac_api.linear_operators import InverseLinearOperator as Inverse
+from struphy.psydac_api.linear_operators import IdentityOperator
 from struphy.psydac_api import preconditioner
 from struphy.psydac_api.mass import WeightedMassOperator
 import struphy.linear_algebra.iterative_solvers as it_solvers
 from psydac.linalg.iterative_solvers import pcg
 
 from psydac.linalg.stencil import StencilVector
 from psydac.linalg.block import BlockVector
@@ -128,94 +130,75 @@
 
 class OhmCold(Propagator):
     r'''Crank-Nicolson step
 
     .. math::
 
         \begin{bmatrix}
-            \mathbf e^{n+1} - \mathbf e^n \\
-            \mathbf j^{n+1} - \mathbf j^n
+            \mathbf j^{n+1} - \mathbf j^n \\
+            \mathbf e^{n+1} - \mathbf e^n
         \end{bmatrix}
         = \frac{\Delta t}{2} \begin{bmatrix}
-            0 & - \mathbb M_1^{-1} M_{1, \alpha} \\
-            \mathbb M_1^{-1} M_{1, \alpha} & 0
+            0 & \frac{\alpha}{\varepsilon_c} \mathbb M_{1,1/n}^{-1} \\
+            - \frac{\alpha}{\varepsilon_c} \mathbb M_{1,1/n}^{-1} & 0
         \end{bmatrix}
         \begin{bmatrix}
-            \mathbf e^n \\
-            \mathbf j^n
+            \mathbb M_{1,1/n} (\mathbf j^n + \mathbf j^{n+1}) \\
+            \mathbb M_1 (\mathbf e^n + \mathbf e^{n+1})
         \end{bmatrix} ,
 
-    based on the :ref:`Schur complement <schur_solver>`, of the rotation problem
-
-    .. math::
-
-        \frac{\partial}{\partial t}
-        \begin{bmatrix}
-            \mathbf e \\
-            \mathbf j
-        \end{bmatrix}
-        = \begin{bmatrix}
-            0 & - \mathbb M_1^{-1} \mathbb M_{1, \alpha} \\
-            \mathbb M_1^{-1} \mathbb M_{1, \alpha} & 0
-        \end{bmatrix}
-        \begin{bmatrix}
-            \mathbf e \\
-            \mathbf j
-        \end{bmatrix}\,, \qquad \begin{bmatrix}
-            \mathbf e \\
-            \mathbf j
-        \end{bmatrix}(0) = 
-        \begin{bmatrix}
-            \mathbf e^n \\
-            \mathbf j^n
-        \end{bmatrix}\,,
-
-
-    where :math:`\mathbb M_{1, \alpha}` denotes the mass matrix weighted by :math:`\alpha`,
-    which represents the plasma frequency in units of the electron cyclotron frequency.
+    based on the :ref:`Schur complement <schur_solver>`.
 
     Parameters
     ----------
         j : psydac.linalg.block.BlockVector
             FE coefficients of a 1-form.
 
         e : psydac.linalg.block.BlockVector
             FE coefficients of a 1-form.
 
-        derham : struphy.psydac_api.psydac_derham.Derham
-            Discrete Derham complex.
-
         params : dict
             Solver parameters for this splitting step.
     '''
 
-    def __init__(self, e, j, mass_ops, params):
+    def __init__(self, e, j, **params):
 
         assert isinstance(e, (BlockVector, PolarVector))
         assert isinstance(j, (BlockVector, PolarVector))
-
         self._e = e
         self._j = j
+
+        # parameters
+        params_default = {'type': 'PConjugateGradient',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False,
+                          'alpha': 1.0,
+                          'epsilon': 1.0}
+
+        params = set_defaults(params, params_default)
+
         self._info = params['info']
+        self._prefactor = params['alpha'] / params['epsilon']
 
         # Define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
-        _A = 1
+        _A = self.mass_ops.M1ninv
 
-        self._B = Multiply(-1./2., Compose(mass_ops.M1.invert(),
-                           mass_ops.M1alpha))  # no dt
-        self._C = Multiply(
-            1./2., Compose(mass_ops.M1.invert(), mass_ops.M1alpha))  # no dt
+        self._B = Multiply(-1/2 * self._prefactor, self.mass_ops.M1)  # no dt
+        self._C = Multiply(1/2 * self._prefactor,
+                           IdentityOperator(self.derham._Vh["1"]))  # no dt
 
         # Preconditioner
         if params['pc'] is None:
             pc = None
         else:
-            # TODO ???
             pc_class = getattr(preconditioner, params['pc'])
-            pc = pc_class(mass_ops.M1)
+            pc = pc_class(self.mass_ops.M1ninv)
 
         # Instantiate Schur solver (constant in this case)
         _BC = Compose(self._B, self._C)
 
         self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
                                          tol=params['tol'], maxiter=params['maxiter'],
                                          verbose=params['verbose'])
@@ -227,28 +210,116 @@
     def __call__(self, dt):
 
         # current variables
         en = self.variables[0]
         jn = self.variables[1]
 
         # allocate temporary FemFields _e, _j during solution
-        _e, info = self._schur_solver(en, self._B.dot(jn), dt)
-        _j = jn - dt*self._C.dot(_e + en)
+        _j, info = self._schur_solver(jn, self._B.dot(en), dt)
+        _e = en - dt/2 * self._prefactor * (_j + jn)
 
         # write new coeffs into Propagator.variables
         max_de, max_dj = self.in_place_update(_e, _j)
 
         if self._info:
             print('Status     for OhmCold:', info['success'])
             print('Iterations for OhmCold:', info['niter'])
             print('Maxdiff e1 for OhmCold:', max_de)
             print('Maxdiff j1 for OhmCold:', max_dj)
             print()
 
 
+class JxBCold(Propagator):
+    r'''Crank-Nicolson step
+
+    .. math::
+
+        \mathbb M_{1,1/n} \left( \mathbf j^{n+1} - \mathbf j^n \right) = \frac{\Delta t}{2} \frac{1}{\varepsilon_c} \mathbb M_{1,B_0} \left( \mathbf j^{n+1} - \mathbf j^n \right).
+
+    Parameters
+    ----------
+        j : psydac.linalg.block.BlockVector
+            FE coefficients of a 1-form.
+
+        params : dict
+            Solver parameters for this splitting step.
+    '''
+
+    def __init__(self, j, **params):
+
+        assert isinstance(j, (BlockVector, PolarVector))
+        self._j = j
+
+        # parameters
+        params_default = {'type': 'PConjugateGradient',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False,
+                          'alpha': 1.0,
+                          'epsilon': 1.0}
+
+        params = set_defaults(params, params_default)
+
+        self._info = params['info']
+        self._tol = params['tol']
+        self._maxiter = params['maxiter']
+        self._verbose = params['verbose']
+        self._epsc = params['epsilon']
+
+        # mass matrix in system (M - dt/2 * A)*j^(n + 1) = (M + dt/2 * A)*j^n
+        self._M = self.mass_ops.M1ninv
+        self._A = Multiply(-1/self._epsc, self.mass_ops.M1Bninv)  # no dt
+
+        # Preconditioner
+        if params['pc'] is None:
+            self._pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            self._pc = pc_class(self.mass_ops.M1ninv)
+
+        # Instantiate linear solver
+        self._solver = getattr(it_solvers, params['type'])(self._M.domain)
+
+        # allocate dummy vectors to avoid temporary array allocations
+        self._rhs_j = self._M.codomain.zeros()
+        self._j_new = j.space.zeros()
+
+    @property
+    def variables(self):
+        return [self._j]
+
+    def __call__(self, dt):
+
+        # current variables
+        jn = self.variables[0]
+
+        # define system (M - dt/2 * A)*b^(n + 1) = (M + dt/2 * A)*b^n
+        lhs = Sum(self._M, Multiply(-dt/2.0, self._A))
+        rhs = Sum(self._M, Multiply(dt/2.0, self._A))
+
+        # solve linear system for updated u coefficients (in-place)
+        rhs.dot(jn, out=self._rhs_j)
+
+        info = self._solver.solve(lhs, self._rhs_j, self._pc,
+                                  x0=jn, tol=self._tol,
+                                  maxiter=self._maxiter, verbose=self._verbose,
+                                  out=self._j_new)[1]
+
+        # write new coeffs into Propagator.variables
+        max_dj = self.in_place_update(self._j_new)[0]
+
+        if self._info:
+            print('Status     for FluidCold:', info['success'])
+            print('Iterations for FluidCold:', info['niter'])
+            print('Maxdiff j1 for FluidCold:', max_dj)
+            print()
+
+
 class ShearAlfvén(Propagator):
     r'''Crank-Nicolson step for shear Alfvén part in MHD equations,
 
     .. math::
 
         \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf b^{n+1} - \mathbf b^n \end{bmatrix} 
         = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_\alpha)^{-1} \mathcal {T^\alpha}^\top \mathbb C^\top \\ - \mathbb C \mathcal {T^\alpha} (\mathbb M^\rho_\alpha)^{-1} & 0 \end{bmatrix} 
@@ -404,16 +475,17 @@
         self._rank = self.derham.comm.Get_rank()
 
         # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
         _A = self.mass_ops.M2n
         self._M1inv = Inverse(self.mass_ops.M1, tol=1e-8)
         self._B = Multiply(1/2, Compose(self.mass_ops.M2B,
                            self.derham.curl))
-        #I still have to invert M1
-        self._C = Multiply(1/2, Compose(self._M1inv,self.derham.curl.T, self.mass_ops.M2B))
+        # I still have to invert M1
+        self._C = Multiply(
+            1/2, Compose(self._M1inv, self.derham.curl.T, self.mass_ops.M2B))
 
         # Preconditioner
         if params['pc'] is None:
             pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             pc = pc_class(getattr(self.mass_ops, 'M2n'))
@@ -511,23 +583,24 @@
         self._kappa = params['kappa']
 
         # mass matrix in system (M - dt/2 * A)*b^(n + 1) = (M + dt/2 * A)*b^n
         id_M = 'M1'
         id_M2Bn = 'M2Bn'
         self._M = getattr(self.mass_ops, id_M)
         self._M2Bn = getattr(self.mass_ops, id_M2Bn)
-        self._A = Multiply(self._kappa, Compose(self.derham.curl.T,self._M2Bn,self.derham.curl))
+        self._A = Multiply(self._kappa, Compose(
+            self.derham.curl.T, self._M2Bn, self.derham.curl))
 
         # Preconditioner
         if params['pc'] is None:
             self._pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             self._pc = pc_class(getattr(self.mass_ops, id_M))
-            
+
         # Instantiate linear solver
         self._solver = getattr(it_solvers, params['type'])(self._M.domain)
 
         # allocate dummy vectors to avoid temporary array allocations
         self._rhs_b = self._M.codomain.zeros()
         self._b_new = b.space.zeros()
 
@@ -732,15 +805,15 @@
 
         \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf p^{n+1}_i - \mathbf p^n_i \end{bmatrix} 
         = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_2)^{-1} \mathbb D^\top \mathbb M_3 \\ - \gamma \mathcal K^3 \mathbb D & 0 \end{bmatrix} 
         \begin{bmatrix} (\mathbf u^{n+1} + \mathbf u^n) \\ (\mathbf p^{n+1}_i + \mathbf p^n_i) \end{bmatrix} ,
 
     where :math:`\mathbb M^\rho_2`  is a weighted mass matrix in 2-space, 
     the weight being the MHD equilibirum density :math:`\rho_0`. Furthermore, :math:`\mathcal K^3` is the basis projection operator given by :
-    
+
     .. math::
 
         \mathcal{K}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{p}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
     The solution of the above system is based on the :ref:`Schur complement <schur_solver>`.
 
     Decoupled density update:
 
@@ -784,24 +857,24 @@
         params = set_defaults(params, params_default)
 
         self._info = params['info']
         self._bc = self.derham.bc
         self._rank = self.derham.comm.Get_rank()
 
         # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
-        id_Mn = 'M2n' 
+        id_Mn = 'M2n'
         id_K, id_Q = 'K3', 'Q3'
-        
+
         _A = getattr(self.mass_ops, id_Mn)
         _K = getattr(self.basis_ops, id_K)
 
         self._B = Multiply(-1/2., Compose(self.derham.div.T, self.mass_ops.M3))
         self._C = Multiply(5/6., Compose(_K, self.derham.div))
 
-        self._QD = Compose(getattr(self.basis_ops, id_Q) ,self.derham.div)
+        self._QD = Compose(getattr(self.basis_ops, id_Q), self.derham.div)
 
         # preconditioner
         if params['pc'] is None:
             pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             pc = pc_class(getattr(self.mass_ops, id_Mn))
@@ -869,15 +942,15 @@
 
         \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf p^{n+1}_i - \mathbf p^n_i \end{bmatrix} 
         = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_2)^{-1} \mathbb D^\top \mathbb M_3 \\ - \gamma \mathcal K^3 \mathbb D & 0 \end{bmatrix} 
         \begin{bmatrix} (\mathbf u^{n+1} + \mathbf u^n) \\ (\mathbf p^{n+1}_i + \mathbf p^n_i) \end{bmatrix} ,
 
     where :math:`\mathbb M^\rho_2`  is a weighted mass matrix in 2-space, 
     the weight being the MHD equilibirum density :math:`\rho_0`. Furthermore, :math:`\mathcal K^3` is the basis projection operator given by :
-    
+
     .. math::
 
         \mathcal{K}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{p}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
     The solution of the above system is based on the :ref:`Schur complement <schur_solver>`.
 
     Decoupled density update:
 
@@ -921,26 +994,26 @@
         params = set_defaults(params, params_default)
 
         self._info = params['info']
         self._bc = self.derham.bc
         self._rank = self.derham.comm.Get_rank()
 
         # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
-        id_Mn = 'M2n' 
+        id_Mn = 'M2n'
         # ONCE THE CODE SUPPORTS HAVING A DIFFERENT EQUILIBRIUM ELECTRON PRESSURE TO THE EQUILIBRIUM ION PRESSURE; WE MUST ADD A NEW PROJECTION MATRIX Ke3 THAT TAKES THE EQUILIBRIUM ELECTRON PRESSURE
-        #INSTEAD OF THE EQUILIBRIUM ION PRESSURE: AND USE HERE Ke3, NOT K3.
+        # INSTEAD OF THE EQUILIBRIUM ION PRESSURE: AND USE HERE Ke3, NOT K3.
         id_K, id_Q = 'K3', 'Q3'
-        
+
         _A = getattr(self.mass_ops, id_Mn)
         _K = getattr(self.basis_ops, id_K)
 
         self._B = Multiply(-1/2., Compose(self.derham.div.T, self.mass_ops.M3))
         self._C = Multiply(5/6., Compose(_K, self.derham.div))
 
-        self._QD = Compose(getattr(self.basis_ops, id_Q) ,self.derham.div)
+        self._QD = Compose(getattr(self.basis_ops, id_Q), self.derham.div)
 
         # preconditioner
         if params['pc'] is None:
             pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             pc = pc_class(getattr(self.mass_ops, id_Mn))
@@ -1166,15 +1239,15 @@
 
     **params : dict
             Solver- and/or other parameters for this splitting step.
     """
 
     def __init__(self, u, **params):
 
-        from struphy.pic.particles import Particles6D, Particles5D
+        from struphy.pic.particles import Particles6D
 
         # pointers to variables
         assert isinstance(u, (BlockVector, PolarVector))
         self._u = u
 
         # parameters
         params_default = {'particles': None,
@@ -1191,15 +1264,15 @@
                           'Ab': 1,
                           'Ah': 1,
                           'kappa': 1.}
 
         params = set_defaults(params, params_default)
 
         # assert parameters and expose some quantities to self
-        assert isinstance(params['particles'], (Particles6D, Particles5D))
+        assert isinstance(params['particles'], (Particles6D))
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
         if params['u_space'] == 'H1vec':
             self._space_key_int = 0
         else:
             self._space_key_int = int(
                 self.derham.spaces_dict[params['u_space']])
@@ -1660,7 +1733,143 @@
         if self._info and self._rank == 0:
             print('Status     for Magnetosonic:', info['success'])
             print('Iterations for Magnetosonic:', info['niter'])
             print('Maxdiff n3 for Magnetosonic:', max_dn)
             print('Maxdiff up for Magnetosonic:', max_du)
             print('Maxdiff p3 for Magnetosonic:', max_dp)
             print()
+
+
+class CurrentCoupling5DDensity(Propagator):
+    """
+    """
+
+    def __init__(self, u, **params):
+
+        from struphy.pic.particles import Particles5D
+
+        # pointers to variables
+        assert isinstance(u, (BlockVector, PolarVector))
+        self._u = u
+
+        # parameters
+        params_default = {'particles': None,
+                          'u_space': 'Hdiv',
+                          'b_eq': None,
+                          'b_tilde': None,
+                          'f0': Maxwellian5DUniform(),
+                          'type': 'PBiConjugateGradientStab',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False,
+                          'Ab': 1,
+                          'Ah': 1,
+                          'kappa': 1.}
+
+        params = set_defaults(params, params_default)
+
+        # assert parameters and expose some quantities to self
+        assert isinstance(params['particles'], (Particles5D))
+
+        assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
+        if params['u_space'] == 'H1vec':
+            self._space_key_int = 0
+        else:
+            self._space_key_int = int(
+                self.derham.spaces_dict[params['u_space']])
+
+        assert isinstance(params['b_eq'], (BlockVector, PolarVector))
+
+        if params['b_tilde'] is not None:
+            assert isinstance(params['b_tilde'], (BlockVector, PolarVector))
+
+        self._particles = params['particles']
+        self._b_eq = params['b_eq']
+        self._b_tilde = params['b_tilde']
+        self._f0 = params['f0']
+
+        self._type = params['type']
+        self._tol = params['tol']
+        self._maxiter = params['maxiter']
+        self._info = params['info']
+        self._verbose = params['verbose']
+        self._rank = self.derham.comm.Get_rank()
+
+        self._coupling_const = params['Ah'] * params['kappa'] / params['Ab']
+        # load accumulator
+        self._accumulator = Accumulator(
+            self.derham, self.domain, params['u_space'], 'cc_lin_mhd_5d_D', add_vector=False, symmetry='asym')
+
+        # transposed extraction operator PolarVector --> BlockVector (identity map in case of no polar splines)
+        self._E2T = self.derham.E['2'].transpose()
+
+        # mass matrix in system (M - dt/2 * A)*u^(n + 1) = (M + dt/2 * A)*u^n
+        u_id = self.derham.spaces_dict[params['u_space']]
+        self._M = getattr(self.mass_ops, 'M' + u_id + 'n')
+
+        # preconditioner
+        if params['pc'] is None:
+            self._pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            self._pc = pc_class(self._M)
+
+        # linear solver
+        self._solver = getattr(it_solvers, params['type'])(self._M.domain)
+
+        # temporary vectors to avoid memory allocation
+        self._b_full1 = self._b_eq.space.zeros()
+        self._b_full2 = self._E2T.codomain.zeros()
+
+        self._rhs_v = self._u.space.zeros()
+        self._u_new = self._u.space.zeros()
+
+    @property
+    def variables(self):
+        return [self._u]
+
+    def __call__(self, dt):
+        """
+        TODO
+        """
+
+        # pointer to old coefficients
+        un = self.variables[0]
+
+        # sum up total magnetic field b_full1 = b_eq + b_tilde (in-place)
+        self._b_eq.copy(out=self._b_full1)
+
+        if self._b_tilde is not None:
+            self._b_full1 += self._b_tilde
+
+        # extract coefficients to tensor product space (in-place)
+        self._E2T.dot(self._b_full1, out=self._b_full2)
+
+        # update ghost regions because of non-local access in accumulation kernel!
+        self._b_full2.update_ghost_regions()
+
+        self._accumulator.accumulate(self._particles,
+                                     self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
+                                     self._space_key_int, self._coupling_const)
+
+        # define system (M - dt/2 * A)*u^(n + 1) = (M + dt/2 * A)*u^n
+        lhs = Sum(self._M, Multiply(-dt/2, self._accumulator.operators[0]))
+        rhs = Sum(self._M, Multiply(dt/2, self._accumulator.operators[0]))
+
+        # solve linear system for updated u coefficients (in-place)
+        rhs.dot(un, out=self._rhs_v)
+
+        info = self._solver.solve(lhs, self._rhs_v, self._pc,
+                                  x0=un, tol=self._tol,
+                                  maxiter=self._maxiter, verbose=self._verbose,
+                                  out=self._u_new)[1]
+
+        # write new coeffs into Propagator.variables
+        max_du = self.in_place_update(self._u_new)
+
+        if self._info and self._rank == 0:
+            print('Status     for CurrentCoupling5DDensity:', info['success'])
+            print('Iterations for CurrentCoupling5DDensity:', info['niter'])
+            print('Maxdiff up for CurrentCoupling5DDensity:', max_du)
+            print()
```

### Comparing `struphy-2.0.0/src/struphy/propagators/propagators_markers.py` & `struphy-2.0.1/src/struphy/propagators/propagators_markers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from numpy import array, polynomial
 
 from psydac.linalg.block import BlockVector
 
 from struphy.polar.basic import PolarVector
 from struphy.propagators.base import Propagator
 from struphy.pic.particles import Particles6D, Particles5D
-from struphy.pic.pusher import Pusher, Pusher_iteration
+from struphy.pic.pusher import Pusher, Pusher_iteration_Gonzalez, Pusher_iteration_Itoh
 from struphy.pic.pusher import ButcherTableau
 from struphy.fields_background.mhd_equil.equils import set_defaults
-from struphy.kinetic_background.analytical import Maxwellian6DUniform
+from struphy.kinetic_background.maxwellians import Maxwellian6DUniform
 
 
 class PushEta(Propagator):
     r"""Solves
 
     .. math::
 
@@ -484,15 +484,15 @@
     def __init__(self, particles, **params):
 
         # pointer to variable
         assert isinstance(particles, Particles5D)
         self._particles = particles
 
         # parameters
-        params_default = {'kappa': 100.,
+        params_default = {'kappa': 1.,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
                           'integrator': 'implicit',
                           'method': 'discrete_gradient_faster',
                           'maxiter': 10,
@@ -561,20 +561,24 @@
                                    self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                    self._grad_abs_b[0]._data, self._grad_abs_b[1]._data, self._grad_abs_b[2]._data,
                                    self._butcher.a, self._butcher.b, self._butcher.c)
 
         elif params['integrator'] == 'implicit':
 
             if params['method'] == 'discrete_gradients':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc1_discrete_gradients', params['maxiter'], params['tol'])
 
             elif params['method'] == 'discrete_gradients_faster':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc1_discrete_gradients_faster', params['maxiter'], params['tol'])
+                
+            elif params['method'] == 'discrete_gradients_Itoh_Newton':
+                self._pusher = Pusher_iteration_Itoh(
+                    self.derham, self.domain, 'push_gc1_discrete_gradients_Itoh_Newton', params['maxiter'], params['tol'])
 
             else:
                 raise NotImplementedError(
                     'Chosen implicit method is not implemented.')
 
             self._pusher_inputs = (self._kappa, self._abs_b._data,
                                    self._b_eq[0]._data, self._b_eq[1]._data, self._b_eq[2]._data,
@@ -591,15 +595,15 @@
         return self._particles
 
     def __call__(self, dt):
         """
         TODO
         """
         self._pusher(self._particles, dt,
-                     *self._pusher_inputs, mpi_sort='each', verbose=False)
+                     *self._pusher_inputs, mpi_sort='each', verbose=True)
 
         # save magnetic field at each particles' position
         self._particles.save_magnetic_energy(self.derham, self._abs_b)
 
 
 class StepPushGuidingCenter2(Propagator):
     r"""Solves
@@ -630,15 +634,15 @@
     def __init__(self, particles, **params):
 
         # pointer to variable
         assert isinstance(particles, Particles5D)
         self._particles = particles
 
         # parameters
-        params_default = {'kappa': 100.,
+        params_default = {'kappa': 1.,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
                           'integrator': 'implicit',
                           'method': 'discrete_gradient_faster',
                           'maxiter': 10,
@@ -707,20 +711,24 @@
                                    self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                    self._grad_abs_b[0]._data, self._grad_abs_b[1]._data, self._grad_abs_b[2]._data,
                                    self._butcher.a, self._butcher.b, self._butcher.c)
 
         elif params['integrator'] == 'implicit':
 
             if params['method'] == 'discrete_gradients':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc2_discrete_gradients', params['maxiter'], params['tol'])
 
             elif params['method'] == 'discrete_gradients_faster':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc2_discrete_gradients_faster', params['maxiter'], params['tol'])
+                
+            elif params['method'] == 'discrete_gradients_Itoh_Newton':
+                self._pusher = Pusher_iteration_Itoh(
+                     self.derham, self.domain, 'push_gc2_discrete_gradients_Itoh_Newton', params['maxiter'], params['tol'])
 
             else:
                 raise NotImplementedError(
                     'Chosen implicit method is not implemented.')
 
             self._pusher_inputs = (self._kappa, self._abs_b._data,
                                    self._b_eq[0]._data, self._b_eq[1]._data, self._b_eq[2]._data,
@@ -737,20 +745,83 @@
         return self._particles
 
     def __call__(self, dt):
         """
         TODO
         """
         self._pusher(self._particles, dt,
-                     *self._pusher_inputs, mpi_sort='each', verbose=False)
+                     *self._pusher_inputs, mpi_sort='each', verbose=True)
 
         # save magnetic field at each particles' position
         self._particles.save_magnetic_energy(self.derham, self._abs_b)
 
 
+class StepVinEfield(Propagator):
+    r'''Push the velocities according to
+
+    .. math::
+
+        \frac{\text{d} \mathbf{v}_p}{\text{d} t} & = \kappa \, DL^{-T} \mathbf{E}
+
+    which is solved analytically.
+
+    Parameters
+    ----------
+    particles : struphy.pic.particles.Particles6D
+        Holdes the markers to push.
+
+    **params : dict
+        Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, particles, **params):
+
+        from numpy import polynomial, floor
+
+        # pointer to variable
+        assert isinstance(particles, Particles6D)
+        self._particles = particles
+
+        # parameters
+        params_default = {
+            'e_field': BlockVector(self.derham.Vh_fem['1'].vector_space),
+            'method': 'analytical',
+            'kappa': 1e2
+        }
+
+        params = set_defaults(params, params_default)
+        self.kappa = params['kappa']
+        method = params['method']
+
+        assert isinstance(params['e_field'], (BlockVector, PolarVector))
+        self._e_field = params['e_field']
+
+        if method == 'analytical':
+            self._pusher = Pusher(self.derham, self.domain,
+                                'push_v_with_efield')
+        elif method == 'discrete_gradient':
+            raise NotImplementedError('Not yet implemented.')
+            # self._pusher = Pusher(self.derham, self.domain,
+            #                     'push_v_in_static_efield_dg')
+        else:
+            raise ValueError(f'Method {method} not known.')
+
+    @property
+    def variables(self):
+        return [self._particles]
+
+    def __call__(self, dt):
+        """
+        TODO
+        """
+        self._pusher(self._particles, dt,
+                     self._e_field.blocks[0]._data, self._e_field.blocks[1]._data, self._e_field.blocks[2]._data,
+                     self.kappa)
+
+
 class StepStaticEfield(Propagator):
     r'''Solve the following system
 
     .. math::
 
         \frac{\text{d} \mathbf{\eta}_p}{\text{d} t} & = DL^{-1} \mathbf{v}_p \,,
 
@@ -781,17 +852,18 @@
         from numpy import polynomial, floor
 
         # pointer to variable
         assert isinstance(particles, Particles6D)
         self._particles = particles
 
         # parameters
-        params_default = {'e_field': BlockVector(
-            self.derham.Vh_fem['1'].vector_space),
-            'kappa': 1e2}
+        params_default = {
+            'e_field': BlockVector(self.derham.Vh_fem['1'].vector_space),
+            'kappa': 1e2
+        }
 
         params = set_defaults(params, params_default)
         self.kappa = params['kappa']
 
         assert isinstance(params['e_field'], (BlockVector, PolarVector))
         self._e_field = params['e_field']
 
@@ -908,14 +980,16 @@
         self._PB = getattr(self.basis_ops, 'PB')
         self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
+        self._integrator = params['integrator']
+        
         if params['integrator'] == 'explicit':
 
             if params['method'] == 'forward_euler':
                 a = []
                 b = [1.]
                 c = [0.]
             elif params['method'] == 'heun2':
@@ -938,42 +1012,32 @@
                 raise NotImplementedError(
                     'Chosen algorithm is not implemented.')
 
             self._butcher = ButcherTableau(a, b, c)
             self._pusher = Pusher(
                 self.derham, self.domain, 'push_gc1_explicit_stage', self._butcher.n_stages)
 
-            self._pusher_inputs = (self._kappa, self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
-                                   self._butcher.a, self._butcher.b, self._butcher.c)
-
         elif params['integrator'] == 'implicit':
 
             if params['method'] == 'discrete_gradients':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc1_discrete_gradients', params['maxiter'], params['tol'])
 
             elif params['method'] == 'discrete_gradients_faster':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc1_discrete_gradients_faster', params['maxiter'], params['tol'])
+                
+            elif params['method'] == 'discrete_gradients_Itoh_Newton':
+                self._pusher = Pusher_iteration_Itoh(
+                    self.derham, self.domain, 'push_gc1_discrete_gradients_Itoh_Newton', params['maxiter'], params['tol'])
 
             else:
                 raise NotImplementedError(
                     'Chosen implicit method is not implemented.')
 
-            self._pusher_inputs = (self._kappa, self._PBb._data,
-                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
-
         else:
             raise NotImplementedError('Chosen integrator is not implemented.')
 
     @property
     def variables(self):
         return self._particles
 
@@ -992,23 +1056,32 @@
         # define gradient of absolute value of parallel magnetic field
         self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
-        self._pusher_inputs = (self._kappa, self._PBb._data,
-                               self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                               self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                               self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                               self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                               self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
+        if self._integrator == 'explicit':
+            self._pusher_inputs = (self._kappa, 
+                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
+                                   self._butcher.a, self._butcher.b, self._butcher.c)
+        else:
+            self._pusher_inputs = (self._kappa, self._PBb._data,
+                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
 
         self._pusher(self._particles, dt,
-                     *self._pusher_inputs, mpi_sort='each', verbose=False)
+                     *self._pusher_inputs, mpi_sort='each', verbose=True)
 
 
 class StepPushDriftKinetic2(Propagator):
     r"""Solves
 
     .. math::
 
@@ -1078,14 +1151,16 @@
         self._PB = getattr(self.basis_ops, 'PB')
         self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
+        self._integrator = params['integrator']
+
         if params['integrator'] == 'explicit':
 
             if params['method'] == 'forward_euler':
                 a = []
                 b = [1.]
                 c = [0.]
             elif params['method'] == 'heun2':
@@ -1108,42 +1183,32 @@
                 raise NotImplementedError(
                     'Chosen algorithm is not implemented.')
 
             self._butcher = ButcherTableau(a, b, c)
             self._pusher = Pusher(
                 self.derham, self.domain, 'push_gc2_explicit_stage', self._butcher.n_stages)
 
-            self._pusher_inputs = (self._kappa, self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
-                                   self._butcher.a, self._butcher.b, self._butcher.c)
-
         elif params['integrator'] == 'implicit':
 
             if params['method'] == 'discrete_gradients':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc2_discrete_gradients', params['maxiter'], params['tol'])
 
             elif params['method'] == 'discrete_gradients_faster':
-                self._pusher = Pusher_iteration(
+                self._pusher = Pusher_iteration_Gonzalez(
                     self.derham, self.domain, 'push_gc2_discrete_gradients_faster', params['maxiter'], params['tol'])
+                
+            elif params['method'] == 'discrete_gradients_Itoh_Newton':
+                self._pusher = Pusher_iteration_Itoh(
+                     self.derham, self.domain, 'push_gc2_discrete_gradients_Itoh_Newton', params['maxiter'], params['tol'])
 
             else:
                 raise NotImplementedError(
                     'Chosen implicit method is not implemented.')
 
-            self._pusher_inputs = (self._kappa, self._PBb._data,
-                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
-
         else:
             raise NotImplementedError('Chosen integrator is not implemented.')
 
     @property
     def variables(self):
         return self._particles
 
@@ -1161,16 +1226,25 @@
         # define gradient of absolute value of parallel magnetic field
         self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
-        self._pusher_inputs = (self._kappa, self._PBb._data,
-                               self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
-                               self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
-                               self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
-                               self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                               self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
+        if self._integrator == 'explicit':
+            self._pusher_inputs = (self._kappa, 
+                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
+                                   self._butcher.a, self._butcher.b, self._butcher.c)
+        else:
+            self._pusher_inputs = (self._kappa, self._PBb._data,
+                                   self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                                   self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                                   self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                                   self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                                   self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
 
         self._pusher(self._particles, dt,
-                     *self._pusher_inputs, mpi_sort='each', verbose=False)
+                     *self._pusher_inputs, mpi_sort='each', verbose=True)
```

### Comparing `struphy-2.0.0/src/struphy/propagators/solvers.py` & `struphy-2.0.1/src/struphy/propagators/solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, rho=None, x0=None, **solver_params):
 
         self._rho = StencilVector(self.derham.Vh['0'])
         if rho is not None:
             # check solvability condition
             solvability = np.zeros(1)
             self.derham.comm.Allreduce(np.sum(rho.toarray()), solvability, op=MPI.SUM)
-            assert solvability[0] <= 1e-15, f'Solvability condition not met: {solvability[0]}'
+            assert solvability[0] <= 1e-14, f'Solvability condition not met: {solvability[0]}'
 
             assert isinstance(rho, (StencilVector, PolarVector))
             # assert rho.space.space_id == "H1" TODO: doesn't work, but we should check that rho is in H1
             self._rho[:] = rho[:]
 
         self._phi = StencilVector(self.derham.Vh['0'])
```

### Comparing `struphy-2.0.0/src/struphy/psydac-0.1-py3-none-any.whl` & `struphy-2.0.1/src/struphy/psydac-0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/banded_to_stencil_kernels.py` & `struphy-2.0.1/src/struphy/psydac_api/banded_to_stencil_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/basis_projection_kernels.py` & `struphy-2.0.1/src/struphy/psydac_api/basis_projection_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/basis_projection_ops.py` & `struphy-2.0.1/src/struphy/psydac_api/basis_projection_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,30 +121,30 @@
 
         .. math::
 
             \mathcal{K}^{0}_{ijk,mno} := \hat{\Pi}^0_{ijk} \left[  \hat{p}^0_{\text{eq}} \mathbf{\Lambda}^0_{mno} \right] \,.
         '''
         if not hasattr(self, '_K0'):
             fun = [[lambda e1, e2, e3: self.weights['eq_mhd'].p0(e1, e2, e3)]]
-            self._K0 = self.assemble_basis_projection_operator(fun, 'H1', 'H1')
+            self._K0 = self.assemble_basis_projection_operator(fun, 'H1', 'H1', name='K0')
 
         return self._K0
 
     @property
     def K3(self):
         r'''Basis projection operator
 
         .. math::
 
             \mathcal{K}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{p}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
         '''
         if not hasattr(self, '_K3'):
             fun = [[lambda e1, e2, e3: self.weights['eq_mhd'].p3(
                 e1, e2, e3) / self.sqrt_g(e1, e2, e3)]]
-            self._K3 = self.assemble_basis_projection_operator(fun, 'L2', 'L2')
+            self._K3 = self.assemble_basis_projection_operator(fun, 'L2', 'L2', name='K3')
 
         return self._K3
 
     @property
     def Qv(self):
         r'''Basis projection operator 
 
@@ -157,15 +157,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.weights['eq_mhd'].n3(e1, e2, e3) if m == n else 0*e1]
             self._Qv = self.assemble_basis_projection_operator(
-                fun, 'H1vec', 'Hdiv')
+                fun, 'H1vec', 'Hdiv', name='Qv')
 
         return self._Qv
 
     @property
     def Q1(self):
         r'''Basis projection operator 
 
@@ -179,15 +179,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.weights['eq_mhd'].n3(e1, e2, e3) * self.Ginv(e1, e2, e3)[:, :, :, m, n]]
 
             self._Q1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hdiv')
+                fun, 'Hcurl', 'Hdiv', name='Q1')
 
         return self._Q1
 
     @property
     def Q2(self):
         r'''Basis projection operator 
 
@@ -201,30 +201,30 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.weights['eq_mhd'].n3(
                         e1, e2, e3) / self.sqrt_g(e1, e2, e3) if m == n else 0*e1]
 
             self._Q2 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hdiv')
+                fun, 'Hdiv', 'Hdiv', name='Q2')
 
         return self._Q2
 
     @property
     def Q3(self):
         r'''Basis projection operator
 
         .. math::
 
             \mathcal{Q}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{\rho}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
         '''
         if not hasattr(self, '_Q3'):
             fun = [[lambda e1, e2, e3: self.weights['eq_mhd'].n3(
                 e1, e2, e3) / self.sqrt_g(e1, e2, e3)]]
-            self._Q3 = self.assemble_basis_projection_operator(fun, 'L2', 'L2')
+            self._Q3 = self.assemble_basis_projection_operator(fun, 'L2', 'L2', name='Q3')
 
         return self._Q3
 
     @property
     def Tv(self):
         r'''Basis projection operator 
 
@@ -249,15 +249,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_B(e1, e2, e3)[:, :, :, m, n]]
 
             self._Tv = self.assemble_basis_projection_operator(
-                fun, 'H1vec', 'Hcurl')
+                fun, 'H1vec', 'Hcurl', name='Tv')
 
         return self._Tv
 
     @property
     def T1(self):
         r'''Basis projection operator 
 
@@ -283,15 +283,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: (rot_B(e1, e2, e3) @ self.Ginv(e1, e2, e3))[:, :, :, m, n]]
 
             self._T1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hcurl')
+                fun, 'Hcurl', 'Hcurl', name='T1')
 
         return self._T1
 
     @property
     def T2(self):
         r'''Basis projection operator 
 
@@ -316,15 +316,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
             self._T2 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hcurl')
+                fun, 'Hdiv', 'Hcurl', name='T2')
 
         return self._T2
 
     @property
     def Sv(self):
         r'''Basis projection operator 
 
@@ -338,15 +338,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.weights['eq_mhd'].p3(e1, e2, e3) if m == n else 0*e1]
 
             self._Sv = self.assemble_basis_projection_operator(
-                fun, 'H1vec', 'Hdiv')
+                fun, 'H1vec', 'Hdiv', name='Sv')
 
         return self._Sv
 
     @property
     def S1(self):
         r'''Basis projection operator
 
@@ -360,15 +360,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.weights['eq_mhd'].p3(e1, e2, e3) * self.Ginv(e1, e2, e3)[:, :, :, m, n]]
 
             self._S1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hdiv')
+                fun, 'Hcurl', 'Hdiv', name='S1')
 
         return self._S1
 
     @property
     def S2(self):
         r'''Basis projection operator 
 
@@ -383,15 +383,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.weights['eq_mhd'].p3(
                         e1, e2, e3) / self.sqrt_g(e1, e2, e3) if m == n else 0*e1]
 
             self._S2 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hdiv')
+                fun, 'Hdiv', 'Hdiv', name='S2')
 
         return self._S2
 
     @property
     def S11(self):
         r'''Basis projection operator
 
@@ -405,15 +405,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.weights['eq_mhd'].p0(e1, e2, e3) if m == n else 0*e1]
 
             self._S11 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hcurl')
+                fun, 'Hcurl', 'Hcurl', name='S11')
 
         return self._S11
 
     @property
     def S21(self):
         r'''Basis projection operator 
 
@@ -427,15 +427,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.weights['eq_mhd'].p0(
                         e1, e2, e3) * self.G(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
             self._S21 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hcurl')
+                fun, 'Hdiv', 'Hcurl', name='S21')
 
         return self._S21
 
     @property
     def Uv(self):
         r'''Basis projection operator
 
@@ -449,15 +449,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.sqrt_g(e1, e2, e3) if m == n else 0*e1]
 
             self._Uv = self.assemble_basis_projection_operator(
-                fun, 'H1vec', 'Hdiv')
+                fun, 'H1vec', 'Hdiv', name='Uv')
 
         return self._Uv
 
     @property
     def U1(self):
         r'''Basis projection operator 
 
@@ -471,15 +471,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.sqrt_g(e1, e2, e3) * self.Ginv(e1, e2, e3)[:, :, :, m, n]]
 
             self._U1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hdiv')
+                fun, 'Hcurl', 'Hdiv', name='U1')
 
         return self._U1
 
     @property
     def Xv(self):
         r'''Basis projection operator 
 
@@ -493,15 +493,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.DF(e1, e2, e3)[:, :, :, m, n]]
 
             self._Xv = self.assemble_basis_projection_operator(
-                fun, 'H1vec', 'H1vec')
+                fun, 'H1vec', 'H1vec', name='Xv')
 
         return self._Xv
 
     @property
     def X1(self):
         r'''Basis projection operator 
 
@@ -515,15 +515,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.DFinvT(e1, e2, e3)[:, :, :, m, n]]
 
             self._X1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'H1vec')
+                fun, 'Hcurl', 'H1vec', name='X1')
 
         return self._X1
 
     @property
     def X2(self):
         r'''Basis projection operator 
 
@@ -537,15 +537,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.DF(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
             self._X2 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'H1vec')
+                fun, 'Hdiv', 'H1vec', name='X2')
 
         return self._X2
 
     @property
     def W1(self):
         r'''Basis projection operator 
 
@@ -559,15 +559,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.weights['eq_mhd'].n3(
                         e1, e2, e3) / self.sqrt_g(e1, e2, e3) if m == n else 0*e1]
 
             self._W1 = self.assemble_basis_projection_operator(
-                fun, 'Hcurl', 'Hcurl')
+                fun, 'Hcurl', 'Hcurl', name='W1')
 
         return self._W1
 
     @property
     def R1(self):
         r'''Basis projection operator 
 
@@ -593,15 +593,15 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_J(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
             self._R1 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hcurl')
+                fun, 'Hdiv', 'Hcurl', name='R1')
 
         return self._R1
 
     @property
     def R2(self):
         r'''Basis projection operator 
 
@@ -626,43 +626,43 @@
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: (self.Ginv(e1, e2, e3) @ rot_J(e1, e2, e3))[:, :, :, m, n]]
 
             self._R2 = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'Hdiv')
+                fun, 'Hdiv', 'Hdiv', name='R2')
 
         return self._R2
 
     @property
     def PB(self):
         r'''
         Basis projection operator
 
         .. math::
 
-            \mathcal P^B_{ijk, (\mu, mno)} := \hat \Pi^0_{ijk} \left[ \frac{\hat B^1_{\mu}}{\sqrt g} \Lambda^2_{\mu, mno}\right]\,.
+            \mathcal P^B_{ijk, (\mu, mno)} := \hat \Pi^0_{ijk} \left[ \frac{\hat b^1_{0,\mu}}{\sqrt g} \Lambda^2_{\mu, mno}\right]\,.
         '''
         if not hasattr(self, '_PB'):
 
             fun = [[]]
             for m in range(3):
                 fun[-1] += [lambda e1, e2, e3,
                             m=m: self.weights['eq_mhd'].unit_b1(e1, e2, e3)[m] / self.sqrt_g(e1, e2, e3)]
 
             self._PB = self.assemble_basis_projection_operator(
-                fun, 'Hdiv', 'H1')
+                fun, 'Hdiv', 'H1', name='PB')
 
         return self._PB
 
     ##########################################
     # Wrapper around BasisProjectionOperator #
     ##########################################
-    def assemble_basis_projection_operator(self, fun: list, V_id: str, W_id: str, verbose=True):
+    def assemble_basis_projection_operator(self, fun: list, V_id: str, W_id: str, verbose=True, name=None):
         r"""Basis projection operator :math:`V^\alpha_h \to V^\beta_h` with given (rank 0, 1 or 2) weight function :math:`A(\boldsymbol \eta)`:
 
         .. math::
 
             \mathcal P_{(\mu, ijk),(\nu, mno)} = \hat \Pi^\beta_{\mu, ijk} \left( A_{\mu,\nu}\,\Lambda^\alpha_{\nu, mno} \right)\,.
 
         Here, :math:`\alpha \in \{0, 1, 2, 3, v\}` indicates the domain and :math:`\beta \in \{0, 1, 2, 3, v\}` indicates the co-domain 
@@ -696,15 +696,15 @@
             assert isinstance(row, list)
             if V_id in {'H1', 'L2'}:
                 assert len(row) == 1
             else:
                 assert len(row) == 3
 
         if self.derham.comm.Get_rank() == 0 and verbose:
-            print(f'Assembling BasisProjectionOperator with V={V_id}, W={W_id}.')
+            print(f'Assembling BasisProjectionOperator "{name}" with V={V_id}, W={W_id}.')
 
         V_id = self.derham.spaces_dict[V_id]
         W_id = self.derham.spaces_dict[W_id]
 
         out = BasisProjectionOperator(self.derham.P[W_id], self.derham.Vh_fem[V_id], fun,
                                       self.derham.E[V_id], self.derham.B[V_id],
                                       transposed=False, polar_shift=self.domain.pole)
```

### Comparing `struphy-2.0.0/src/struphy/psydac_api/fields.py` & `struphy-2.0.1/src/struphy/psydac_api/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Parameters
     ----------
         name : str
             Field's key to be used for saving in the hdf5 file.
 
         space_id : str
-            Space identifier for the field (H1, Hcurl, Hdiv, L2 or H1vec).
+            Space identifier for the field ("H1", "Hcurl", "Hdiv", "L2" or "H1vec").
 
         derham : struphy.psydac_api.psydac_derham.Derham
             Discrete Derham complex.
     """
 
     def __init__(self, name, space_id, derham):
 
@@ -347,17 +347,17 @@
             self.vector._data[:] = file[key][-1]
         else:
             for n in range(3):
                 self.vector[n]._data[:] = file[key + '/' + str(n + 1)][-1]
 
         self._vector.update_ghost_regions()
 
-    def __call__(self, eta1, eta2, eta3, squeeze_output=False):
+    def __call__(self, eta1, eta2, eta3, squeeze_output=False, local=False):
         """
-        Evaluates the spline function on the local domain.
+        Evaluates the spline function on the global domain, unless local is given to True (in which case the spline function is evaluated only on the local domain).
 
         Parameters
         ----------
             eta1, eta2, eta3 : array-like
                 Logical coordinates at which to evaluate.
 
             flat_eval : bool
@@ -430,15 +430,16 @@
                                                         np.array(self.derham.p), T1, T2, T3, np.array(self.starts), tmp)
             else:
                 # eval_mpi needs flagged arrays E1, E2, E3 as input
                 eval_3d.eval_spline_mpi_matrix(E1, E2, E3, self._vector_stencil._data, kind,
                                                np.array(self.derham.p), T1, T2, T3, np.array(self.starts), tmp)
 
             if self.derham.comm is not None:
-                self.derham.comm.Allreduce(MPI.IN_PLACE, tmp, op=MPI.SUM)
+                if local == False :
+                    self.derham.comm.Allreduce(MPI.IN_PLACE, tmp, op=MPI.SUM)
 
             # all processes have all values
             values = tmp
 
             if squeeze_output:
                 values = np.squeeze(values)
 
@@ -454,15 +455,16 @@
                     eval_3d.eval_spline_mpi_sparse_meshgrid(E1, E2, E3, self._vector_stencil[n]._data, kind,
                                                             np.array(self.derham.p), T1, T2, T3, np.array(self.starts[n]), tmp)
                 else:
                     eval_3d.eval_spline_mpi_matrix(E1, E2, E3, self._vector_stencil[n]._data, kind,
                                                    np.array(self.derham.p), T1, T2, T3, np.array(self.starts[n]), tmp)
 
                 if self.derham.comm is not None:
-                    self.derham.comm.Allreduce(MPI.IN_PLACE, tmp, op=MPI.SUM)
+                    if local == False:
+                        self.derham.comm.Allreduce(MPI.IN_PLACE, tmp, op=MPI.SUM)
 
                 # all processes have all values
                 values += [tmp.copy()]
                 tmp[:] = 0.
 
                 if squeeze_output:
                     values[-1] = np.squeeze(values[-1])
```

### Comparing `struphy-2.0.0/src/struphy/psydac_api/linear_operators.py` & `struphy-2.0.1/src/struphy/psydac_api/linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/mass.py` & `struphy-2.0.1/src/struphy/psydac_api/mass.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from struphy.psydac_api import mass_kernels
 from struphy.psydac_api.utilities import RotationMatrix
 from struphy.psydac_api.linear_operators import LinOpWithTransp, BoundaryOperator, IdentityOperator
 from struphy.psydac_api.linear_operators import CompositeLinearOperator as Compose
 
 from struphy.polar.linear_operators import PolarExtractionOperator
 
+from struphy.psydac_api.fields import Field
 
 class WeightedMassOperators:
     r"""
     Class for assembling weighted mass matrices in 3d.
 
     Weighted mass matrices :math:`\mathbb M^{\beta\alpha}: \mathbb R^{N_\alpha} \to \mathbb R^{N_\beta}` are of the general form
 
@@ -98,15 +99,15 @@
         .. math::
 
             \mathbb M^0_{ijk, mno} = \int \Lambda^0_{ijk}\,  \Lambda^0_{mno} \sqrt g\,  \textnormal d \boldsymbol\eta.
         """
 
         if not hasattr(self, '_M0'):
             fun = [[lambda e1, e2, e3: self.sqrt_g(e1, e2, e3)]]
-            self._M0 = self.assemble_weighted_mass(fun, 'H1', 'H1')
+            self._M0 = self.assemble_weighted_mass(fun, 'H1', 'H1', name='M0')
 
         return self._M0
 
     @property
     def M1(self):
         r"""
         Mass matrix 
@@ -120,15 +121,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.Ginv(e1, e2, e3)[:, :, :, m, n] * self.sqrt_g(e1, e2, e3)]
 
-            self._M1 = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl')
+            self._M1 = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl', name='M1')
 
         return self._M1
 
     @property
     def M2(self):
         r"""
         Mass matrix 
@@ -142,15 +143,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.G(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
-            self._M2 = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+            self._M2 = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv', name='M2')
 
         return self._M2
 
     @property
     def M3(self):
         r"""
         Mass matrix 
@@ -158,15 +159,15 @@
         .. math::
 
             \mathbb M^3_{ijk, mno} = \int \Lambda^3_{ijk}\,  \Lambda^3_{mno} \frac{1}{\sqrt g}\,  \textnormal d \boldsymbol\eta.
         """
 
         if not hasattr(self, '_M3'):
             fun = [[lambda e1, e2, e3: 1. / self.sqrt_g(e1, e2, e3)]]
-            self._M3 = self.assemble_weighted_mass(fun, 'L2', 'L2')
+            self._M3 = self.assemble_weighted_mass(fun, 'L2', 'L2', name='M3')
 
         return self._M3
 
     @property
     def Mv(self):
         r"""
         Mass matrix 
@@ -180,15 +181,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: self.G(e1, e2, e3)[:, :, :, m, n] * self.sqrt_g(e1, e2, e3)]
 
-            self._Mv = self.assemble_weighted_mass(fun, 'H1vec', 'H1vec')
+            self._Mv = self.assemble_weighted_mass(fun, 'H1vec', 'H1vec', name='Mv')
 
         return self._Mv
 
     ######################################
     # Predefined weighted mass operators #
     ######################################
     @property
@@ -208,15 +209,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.Ginv(e1, e2, e3)[:, :, :, m, n] * self.sqrt_g(
                         e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False)]
 
-            self._M1n = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl')
+            self._M1n = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl', name='M1n')
 
         return self._M1n
 
     @property
     def M2n(self):
         r"""
         Mass matrix 
@@ -233,15 +234,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.G(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(
                         e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False)]
 
-            self._M2n = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+            self._M2n = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv', name='M2n')
 
         return self._M2n
 
     @property
     def Mvn(self):
         r"""
         Mass matrix 
@@ -258,17 +259,42 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.G(e1, e2, e3)[:, :, :, m, n] * self.sqrt_g(
                         e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False)]
 
-            self._Mvn = self.assemble_weighted_mass(fun, 'H1vec', 'H1vec')
+            self._Mvn = self.assemble_weighted_mass(fun, 'H1vec', 'H1vec', name='Mvn')
 
         return self._Mvn
+    
+    @property
+    def M1ninv(self):
+        r"""
+        Mass matrix 
+
+        .. math::
+
+            \mathbb M^{1,\frac{1}{n}}_{(\mu,ijk), (\nu,mno)} = \int \frac{1}{n^0_{\textnormal{eq}}(\boldsymbol \eta)} \Lambda^1_{\mu,ijk}\, G^{-1}_{\mu,\nu}\, \Lambda^1_{\nu, mno} \sqrt g\,  \textnormal d \boldsymbol\eta. 
+
+        where :math:`n^0_{\textnormal{eq}}(\boldsymbol \eta)` is an MHD equilibrium density (0-form).
+        """
+
+        if not hasattr(self, '_M1ninv'):
+            assert 'eq_mhd' in self.weights
+            fun = []
+            for m in range(3):
+                fun += [[]]
+                for n in range(3):
+                    fun[-1] += [lambda e1, e2, e3, m=m, n=n: self.Ginv(e1, e2, e3)[:, :, :, m, n] * self.sqrt_g(
+                        e1, e2, e3) / self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False)]
+
+            self._M1ninv = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl')
+
+        return self._M1ninv
 
     @property
     def M1J(self):
         r"""
         Mass matrix 
 
         .. math::
@@ -292,15 +318,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: (self.Ginv(e1, e2, e3) @ rot_J(e1, e2, e3))[:, :, :, m, n]]
 
-            self._M1J = self.assemble_weighted_mass(fun, 'Hdiv', 'Hcurl')
+            self._M1J = self.assemble_weighted_mass(fun, 'Hdiv', 'Hcurl', name='M1J')
 
         return self._M1J
 
     @property
     def M2J(self):
         r"""
         Mass matrix 
@@ -326,15 +352,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_J(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
-            self._M2J = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+            self._M2J = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv', name='M2J')
 
         return self._M2J
 
     @property
     def MvJ(self):
         r"""
         Mass matrix 
@@ -360,15 +386,15 @@
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_J(e1, e2, e3)[:, :, :, m, n]]
 
-            self._MvJ = self.assemble_weighted_mass(fun, 'Hdiv', 'H1vec')
+            self._MvJ = self.assemble_weighted_mass(fun, 'Hdiv', 'H1vec', name='MvJ')
 
         return self._MvJ
     
     @property
     def M2B(self):
         r"""
         Mass matrix 
@@ -383,26 +409,38 @@
 
             \mathcal R^J_{\alpha, \nu} := \epsilon_{\alpha \beta \nu}\, B^2_{\textnormal{eq}, \beta}\,,\qquad s.t. \qquad \mathcal R^J \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,
 
         where :math:`\epsilon_{\alpha \beta \nu}` stands for the Levi-Civita tensor and :math:`B^2_{\textnormal{eq}, \beta}` is the :math:`\beta`-component of the MHD equilibrium magnetic field (2-form).
         """
 
         if not hasattr(self, '_M2B'):
-
+            
+            a_eq = self.derham.P['1']([self.weights['eq_mhd'].a1_1,
+                                         self.weights['eq_mhd'].a1_2,
+                                         self.weights['eq_mhd'].a1_3])
+            
+            tmp_a2 = self.derham.curl.dot(a_eq)
+            b02fun = Field('b02', 'Hdiv', self.derham)
+            b02fun.vector = tmp_a2
+            b02funx = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[0]
+            b02funy = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[1]
+            b02funz = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[2]
+            #rot_B = RotationMatrix(
+                #self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
             rot_B = RotationMatrix(
-                self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
+                b02funx, b02funy, b02funz)
 
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
 
-            self._M2B = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+            self._M2B = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv', name='M2B')
 
         return self._M2B
     
     @property
     def M2Bn(self):
         r"""
         Mass matrix 
@@ -417,33 +455,79 @@
 
             \mathcal R^J_{\alpha, \nu} := \epsilon_{\alpha \beta \nu}\, B^2_{\textnormal{eq}, \beta}\,,\qquad s.t. \qquad \mathcal R^J \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,
 
         where :math:`\epsilon_{\alpha \beta \nu}` stands for the Levi-Civita tensor and :math:`B^2_{\textnormal{eq}, \beta}` is the :math:`\beta`-component of the MHD equilibrium magnetic field (2-form).
         """
 
         if not hasattr(self, '_M2BN'):
+            
+            a_eq = self.derham.P['1']([self.weights['eq_mhd'].a1_1,
+                                         self.weights['eq_mhd'].a1_2,
+                                         self.weights['eq_mhd'].a1_3])
+            
+            tmp_a2 = self.derham.Vh['2'].zeros()
+            self.derham.curl.dot(a_eq, out=tmp_a2)
+            b02fun = Field('b02', 'Hdiv', self.derham)
+            b02fun.vector = tmp_a2
+            b02funx = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[0]
+            b02funy = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[1]
+            b02funz = lambda x, y, z : b02fun(x,y,z, squeeze_output=True, local=True)[2]
+            #rot_B = RotationMatrix(
+                #self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
+            rot_B = RotationMatrix(
+                b02funx, b02funy, b02funz)
+            fun = []
+            for m in range(3):
+                fun += [[]]
+                for n in range(3):
+                    fun[-1] += [lambda e1, e2, e3, m=m,
+                                n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / (self.sqrt_g(e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False))]
+
+            self._M2BN = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv', name='M2Bn')
+
+        return self._M2BN
+    
+    @property
+    def M1Bninv(self):
+        r"""
+        Mass matrix 
+
+        .. math::
+
+            \mathbb M^{1,B\frac{1}{n}}_{(\mu,ijk), (\nu,mno)} = \int \frac{1}{n^0_{\textnormal{eq}}(\boldsymbol \eta)}\, \Lambda^1_{\mu,ijk}\, G^{-1}_{\mu,\alpha}\, \mathcal R^J_{\alpha, \gamma}\, G^{-1}_{\gamma,\nu}\, \Lambda^1_{\nu, mno} \, \sqrt g\,  \textnormal d \boldsymbol\eta. 
+
+        with the rotation matrix
+
+        .. math::
+
+            \mathcal R^J_{\alpha, \nu} := \epsilon_{\alpha \beta \nu}\, B^2_{\textnormal{eq}, \beta}\,,\qquad s.t. \qquad \mathcal R^J \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,
+
+        where :math:`\epsilon_{\alpha \beta \nu}` stands for the Levi-Civita tensor and :math:`B^2_{\textnormal{eq}, \beta}` is the :math:`\beta`-component of the MHD equilibrium magnetic field (2-form).
+        """
+
+        if not hasattr(self, '_M1Bninv'):
 
             rot_B = RotationMatrix(
                 self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
 
             fun = []
             for m in range(3):
                 fun += [[]]
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
-                                n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / (self.sqrt_g(e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False))]
+                                n=n: (self.Ginv(e1, e2, e3) @ rot_B(e1, e2, e3) @ self.Ginv(e1, e2, e3))[:, :, :, m, n] * (self.sqrt_g(e1, e2, e3) / self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False))]
 
-            self._M2BN = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+            self._M1Bninv = self.assemble_weighted_mass(fun, 'Hcurl', 'Hcurl')
 
-        return self._M2BN
+        return self._M1Bninv
 
     #######################################
     # Wrapper around WeightedMassOperator #
     #######################################
-    def assemble_weighted_mass(self, fun: list, V_id: str, W_id: str):
+    def assemble_weighted_mass(self, fun: list, V_id: str, W_id: str, name=None):
         r""" Weighted mass matrix :math:`V^\alpha_h \to V^\beta_h` with given (matrix-valued) weight function :math:`W(\boldsymbol \eta)`:
 
         .. math::
 
             \mathbb M_{(\mu, ijk), (\nu, mno)}(W) = \int \Lambda^\beta_{\mu, ijk}\, W_{\mu,\nu}(\boldsymbol \eta)\,  \Lambda^\alpha_{\nu, mno} \,  \textnormal d \boldsymbol\eta. 
 
         Here, :math:`\alpha \in \{0, 1, 2, 3, v\}` indicates the domain and :math:`\beta \in \{0, 1, 2, 3, v\}` indicates the co-domain 
@@ -456,14 +540,17 @@
             3d arrays must have shape corresponding to the 1d quad_grids of V1-ProductFemSpace.
 
         V_id : str
             Specifier for the domain of the operator ('H1', 'Hcurl', 'Hdiv', 'L2' or 'H1vec').
 
         W_id : str
             Specifier for the co-domain of the operator ('H1', 'Hcurl', 'Hdiv', 'L2' or 'H1vec').
+        
+        name: str
+            Name of the operator.
 
         Returns
         -------
         out : A WeightedMassOperator object.
         """
 
         assert isinstance(fun, list)
@@ -484,15 +571,15 @@
         W_id = self.derham.spaces_dict[W_id]
 
         out = WeightedMassOperator(self.derham.Vh_fem[V_id], self.derham.Vh_fem[W_id],
                                    V_extraction_op=self.derham.E[V_id], W_extraction_op=self.derham.E[W_id],
                                    V_boundary_op=self.derham.B[V_id], W_boundary_op=self.derham.B[W_id],
                                    weights_info=fun, transposed=False)
 
-        out.assemble()
+        out.assemble(name=name)
 
         return out
 
 
 class WeightedMassOperator(LinOpWithTransp):
     """
     Weighted mass matrix of the form B * E * M * E^T * B^T, with E and B being basis extraction and boundary operators, respectively.
@@ -896,15 +983,15 @@
                                      self._V_boundary_op, self._W_boundary_op,
                                      self._symmetry, not self._transposed)
 
             M.assemble(weights=weights, verbose=False)
 
         return M
 
-    def assemble(self, weights=None, clear=True, verbose=True):
+    def assemble(self, weights=None, clear=True, verbose=True, name=None):
         """
         Assembles a weighted mass matrix (StencilMatrix/BlockLinearOperator) corresponding to given domain/codomain spline spaces.
 
         General form (in 3d) is mat_(ijk,mno) = integral[ Lambda_ijk * weight * Lambda_lmn ],
         where Lambda_ijk are the basis functions of the spline space and weight is some weight function.
 
         The integration is performed with Gauss-Legendre quadrature over the whole logical domain.
@@ -915,14 +1002,17 @@
             Weight function(s) (callables or np.ndarrays) in a 2d list of shape corresponding to number of components of domain/codomain. If weights=None, the weight is taken from the given weights in the instanziation of the object, else it will ne overriden.
 
         clear : bool
             Whether to first set all data to zero before assembly. If False, the new contributions are added to existing ones.
 
         verbose : bool
             Whether to do some printing.
+            
+        name : str
+            Name of the operator.
         """
 
         # clear data
         if clear:
             if isinstance(self._mat, StencilMatrix):
                 self._mat._data[:] = 0.
             else:
@@ -941,15 +1031,15 @@
             if self._V.vector_space[0].cart.comm is not None:
                 rank = self._V.vector_space[0].cart.comm.Get_rank()
             else:
                 rank = 0
 
         if rank == 0 and verbose:
             print(
-                f'Assembling matrix of WeightedMassOperator with V={self._domain_symbolic_name}, W={self._codomain_symbolic_name}.')
+                f'Assembling matrix of WeightedMassOperator "{name}" with V={self._domain_symbolic_name}, W={self._codomain_symbolic_name}.')
 
         # collect domain/codomain TensorFemSpaces for each component in tuple
         if self._transposed:
             if isinstance(self._W, TensorFemSpace):
                 domain_spaces = (self._W,)
             else:
                 domain_spaces = self._W.spaces
```

### Comparing `struphy-2.0.0/src/struphy/psydac_api/mass_kernels.py` & `struphy-2.0.1/src/struphy/psydac_api/mass_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/preconditioner.py` & `struphy-2.0.1/src/struphy/psydac_api/preconditioner.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/projectors.py` & `struphy-2.0.1/src/struphy/psydac_api/projectors.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/psydac_derham.py` & `struphy-2.0.1/src/struphy/psydac_api/psydac_derham.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/quadrature_evaluation_kernels.py` & `struphy-2.0.1/src/struphy/psydac_api/quadrature_evaluation_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/utilities.py` & `struphy-2.0.1/src/struphy/psydac_api/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/psydac_api/utilities_kernels.py` & `struphy-2.0.1/src/struphy/psydac_api/utilities_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_accumulation.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_accumulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     # load distributed markers first and use Send/Receive to make global marker copies for the legacy routines
     params_markers = {'Np': Np, 'eps': .25,
                       'loading': {'type': 'pseudo_random', 'seed': 1607, 'moments': [0., 0., 0., 1., 2., 3.]}
                       }
 
     particles = Particles6D(
         'test_particles', **params_markers, domain_array=derham.domain_array, comm=mpi_comm)
+    particles.draw_markers()
 
     # set random weights on each process
     particles.markers[~particles.holes,
                       6] = np.random.rand(particles.n_mks_loc)
 
     # copy of markers for legacy kernel
     particles_leg = particles.markers.copy()
@@ -163,30 +164,34 @@
 
     # =========================
     # ======== Compare ========
     # =========================
 
     # compare blocks
     atol = 1e-10
-    
-    compare_arrays(acc.operators[0].matrix[0, 1], acc_leg.blocks_glo[0][1], mpi_rank, atol=atol, verbose=verbose)
+
+    compare_arrays(acc.operators[0].matrix[0, 1], acc_leg.blocks_glo[0]
+                   [1], mpi_rank, atol=atol, verbose=verbose)
     if verbose and mpi_rank == 0:
         print('mat12 passed test')
-    compare_arrays(acc.operators[0].matrix[0, 2], acc_leg.blocks_glo[0][2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[0, 2], acc_leg.blocks_glo[0]
+                   [2], mpi_rank, atol=atol, verbose=verbose)
     if verbose and mpi_rank == 0:
         print('mat13 passed test')
-    compare_arrays(acc.operators[0].matrix[1, 2], acc_leg.blocks_glo[1][2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[1, 2], acc_leg.blocks_glo[1]
+                   [2], mpi_rank, atol=atol, verbose=verbose)
     if verbose and mpi_rank == 0:
         print('mat23 passed test')
 
     # compare matrix-vector product
-    x, x_psy = create_equal_random_arrays(derham.Vh_fem[space_key], seed=5624, flattened=True)
-    
+    x, x_psy = create_equal_random_arrays(
+        derham.Vh_fem[space_key], seed=5624, flattened=True)
+
     r_psy = acc.operators[0].dot(x_psy)
-    
+
     r = acc_leg.to_sparse_step1().dot(x)
 
     compare_arrays(r_psy, r, mpi_rank, atol=atol, verbose=verbose)
     if verbose and mpi_rank == 0:
         print('matrix-vector product passed test')
 
 
@@ -230,14 +235,15 @@
     # load distributed markers first and use Send/Receive to make global marker copies for the legacy routines
     params_markers = {'Np': Np, 'eps': .25,
                       'loading': {'type': 'pseudo_random', 'seed': 1607, 'moments': [0., 0., 0., 1., 2., 3.]}
                       }
 
     particles = Particles6D(
         'test_particles', **params_markers, domain_array=derham.domain_array, comm=mpi_comm)
+    particles.draw_markers()
 
     # set random weights on each process
     particles.markers[~particles.holes,
                       6] = np.random.rand(particles.n_mks_loc)
 
     # copy of markers for legacy kernel
     particles_leg = particles.markers.copy()
@@ -318,52 +324,63 @@
     # =========================
     # ======== Compare ========
     # =========================
 
     # compare blocks
     atol = 1e-10
 
-    compare_arrays(acc.operators[0].matrix[0, 0], acc_leg.blocks_glo[0][0], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[0, 0], acc_leg.blocks_glo[0]
+                   [0], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11 passed test')
-    compare_arrays(acc.operators[0].matrix[0, 1], acc_leg.blocks_glo[0][1], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[0, 1], acc_leg.blocks_glo[0]
+                   [1], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12 passed test')
-    compare_arrays(acc.operators[0].matrix[0, 2], acc_leg.blocks_glo[0][2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[0, 2], acc_leg.blocks_glo[0]
+                   [2], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13 passed test')
-    compare_arrays(acc.operators[0].matrix[1, 1], acc_leg.blocks_glo[1][1], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[1, 1], acc_leg.blocks_glo[1]
+                   [1], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22 passed test')
-    compare_arrays(acc.operators[0].matrix[1, 2], acc_leg.blocks_glo[1][2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[1, 2], acc_leg.blocks_glo[1]
+                   [2], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23 passed test')
-    compare_arrays(acc.operators[0].matrix[2, 2], acc_leg.blocks_glo[2][2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.operators[0].matrix[2, 2], acc_leg.blocks_glo[2]
+                   [2], mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33 passed test')
-    
-    compare_arrays(acc.vectors[0][0], acc_leg.vecs_glo[0], mpi_rank, atol=atol, verbose=verbose)
+
+    compare_arrays(acc.vectors[0][0], acc_leg.vecs_glo[0],
+                   mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec1 passed test')
-    compare_arrays(acc.vectors[0][1], acc_leg.vecs_glo[1], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.vectors[0][1], acc_leg.vecs_glo[1],
+                   mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec2 passed test')
-    compare_arrays(acc.vectors[0][2], acc_leg.vecs_glo[2], mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.vectors[0][2], acc_leg.vecs_glo[2],
+                   mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec3 passed test')
 
-    compare_arrays(acc.vectors[0], acc_leg.vecs_glo, mpi_rank, atol=atol, verbose=verbose)
+    compare_arrays(acc.vectors[0], acc_leg.vecs_glo,
+                   mpi_rank, atol=atol, verbose=verbose)
     if verbose:
         print('full block vector passed test')
 
     # compare matrix-vector product
-    x, x_psy = create_equal_random_arrays(derham.Vh_fem[space_key], seed=5624, flattened=True)
-    
+    x, x_psy = create_equal_random_arrays(
+        derham.Vh_fem[space_key], seed=5624, flattened=True)
+
     r_psy = acc.operators[0].dot(x_psy)
-    
+
     r = acc_leg.to_sparse_step3().dot(x)
 
     compare_arrays(r_psy, r, mpi_rank, atol=atol, verbose=verbose)
     if verbose and mpi_rank == 0:
         print('matrix-vector product passed test')
 
 
@@ -397,19 +414,20 @@
     derham = Derham(Nel, p, spl_kind, comm=mpi_comm)
 
     if rank == 0:
         print(derham.domain_array)
 
     # load distributed markers first and use Send/Receive to make global marker copies for the legacy routines
     params_markers = {'Np': Np, 'eps': .25,
-                      'loading': {'type': 'pseudo_random', 'seed': 1607, 'moments': [0., 0., 0., 1., 2., 3.]}
+                      'loading': {'type': 'pseudo_random', 'seed': 1607, 'moments': [0., 0., 0., 1., 2., 3.], 'spatial': 'uniform'}
                       }
 
     particles = Particles6D(
         'test_particles', **params_markers, domain_array=derham.domain_array, comm=mpi_comm)
+    particles.draw_markers()
 
     # set random weights on each process
     particles.markers[~particles.holes,
                       6] = np.random.rand(particles.n_mks_loc)
 
     # gather all particles for legacy kernel
     marker_shapes = np.zeros(mpi_size, dtype=int)
@@ -533,139 +551,178 @@
     #              [ mat[0][2][:,:,:,:,:,:,1,1].transpose(), mat[1][2][:,:,:,:,:,:,1,1].transpose(), mat[2][2][:,:,:,:,:,:,1,1]]]
     # mat_temp23 = [[mat[0][0][:,:,:,:,:,:,1,2], mat[0][1][:,:,:,:,:,:,1,2], mat[0][2][:,:,:,:,:,:,1,2]],
     #              [ mat[0][1][:,:,:,:,:,:,1,2].transpose(), mat[1][1][:,:,:,:,:,:,1,2], mat[1][2][:,:,:,:,:,:,1,2]],
     #              [ mat[0][2][:,:,:,:,:,:,1,2].transpose(), mat[1][2][:,:,:,:,:,:,1,2].transpose(), mat[2][2][:,:,:,:,:,:,1,2]]]
     # mat_temp33 = [[mat[0][0][:,:,:,:,:,:,2,2], mat[0][1][:,:,:,:,:,:,2,2], mat[0][2][:,:,:,:,:,:,2,2]],
     #              [ mat[0][1][:,:,:,:,:,:,2,2].transpose(), mat[1][1][:,:,:,:,:,:,2,2], mat[1][2][:,:,:,:,:,:,2,2]],
     #              [ mat[0][2][:,:,:,:,:,:,2,2].transpose(), mat[1][2][:,:,:,:,:,:,2,2].transpose(), mat[2][2][:,:,:,:,:,:,2,2]]]
-    vec_temp1 = [vec[0][:,:,:,0], vec[1][:,:,:,0], vec[2][:,:,:,0]]
-    vec_temp2 = [vec[0][:,:,:,1], vec[1][:,:,:,1], vec[2][:,:,:,1]]
-    vec_temp3 = [vec[0][:,:,:,2], vec[1][:,:,:,2], vec[2][:,:,:,2]]
+    vec_temp1 = [vec[0][:, :, :, 0], vec[1][:, :, :, 0], vec[2][:, :, :, 0]]
+    vec_temp2 = [vec[0][:, :, :, 1], vec[1][:, :, :, 1], vec[2][:, :, :, 1]]
+    vec_temp3 = [vec[0][:, :, :, 2], vec[1][:, :, :, 2], vec[2][:, :, :, 2]]
 
-    compare_arrays(ACC.operators[0].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_11 passed test')
-    compare_arrays(ACC.operators[0].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_11 passed test')
-    compare_arrays(ACC.operators[0].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_11 passed test')
-    compare_arrays(ACC.operators[0].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_11 passed test')
-    compare_arrays(ACC.operators[0].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_11 passed test')
-    compare_arrays(ACC.operators[0].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,0,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[0].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 0, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_11 passed test')
 
-    compare_arrays(ACC.operators[1].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_12 passed test')
-    compare_arrays(ACC.operators[1].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_12 passed test')
-    compare_arrays(ACC.operators[1].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_12 passed test')
-    compare_arrays(ACC.operators[1].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_12 passed test')
-    compare_arrays(ACC.operators[1].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_12 passed test')
-    compare_arrays(ACC.operators[1].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,0,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[1].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 0, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_12 passed test')
 
-    compare_arrays(ACC.operators[2].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_13 passed test')
-    compare_arrays(ACC.operators[2].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_13 passed test')
-    compare_arrays(ACC.operators[2].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_13 passed test')
-    compare_arrays(ACC.operators[2].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_13 passed test')
-    compare_arrays(ACC.operators[2].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_13 passed test')
-    compare_arrays(ACC.operators[2].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,0,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[2].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 0, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_13 passed test')
 
-    compare_arrays(ACC.operators[3].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_22 passed test')
-    compare_arrays(ACC.operators[3].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_22 passed test')
-    compare_arrays(ACC.operators[3].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_22 passed test')
-    compare_arrays(ACC.operators[3].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_22 passed test')
-    compare_arrays(ACC.operators[3].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_22 passed test')
-    compare_arrays(ACC.operators[3].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,1,1], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[3].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 1, 1], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_22 passed test')
 
-    compare_arrays(ACC.operators[4].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_23 passed test')
-    compare_arrays(ACC.operators[4].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_23 passed test')
-    compare_arrays(ACC.operators[4].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_23 passed test')
-    compare_arrays(ACC.operators[4].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_23 passed test')
-    compare_arrays(ACC.operators[4].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_23 passed test')
-    compare_arrays(ACC.operators[4].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,1,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[4].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 1, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_23 passed test')
 
-    compare_arrays(ACC.operators[5].matrix.blocks[0][0], mat[0][0][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[0][0], mat[0][0]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat11_33 passed test')
-    compare_arrays(ACC.operators[5].matrix.blocks[0][1], mat[0][1][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[0][1], mat[0][1]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat12_33 passed test')
-    compare_arrays(ACC.operators[5].matrix.blocks[0][2], mat[0][2][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[0][2], mat[0][2]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat13_33 passed test')
-    compare_arrays(ACC.operators[5].matrix.blocks[1][1], mat[1][1][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[1][1], mat[1][1]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat22_33 passed test')
-    compare_arrays(ACC.operators[5].matrix.blocks[1][2], mat[1][2][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[1][2], mat[1][2]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat23_33 passed test')
-    compare_arrays(ACC.operators[5].matrix.blocks[2][2], mat[2][2][:,:,:,:,:,:,2,2], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.operators[5].matrix.blocks[2][2], mat[2][2]
+                   [:, :, :, :, :, :, 2, 2], rank, atol=atol, verbose=verbose)
     if verbose:
         print('mat33_33 passed test')
-        
-    compare_arrays(ACC.vectors[0].blocks[0], vec[0][:,:,:,0], rank, atol=atol, verbose=verbose)
+
+    compare_arrays(ACC.vectors[0].blocks[0], vec[0]
+                   [:, :, :, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec1_1 passed test')
-    compare_arrays(ACC.vectors[0].blocks[1], vec[1][:,:,:,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.vectors[0].blocks[1], vec[1]
+                   [:, :, :, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec2_1 passed test')
-    compare_arrays(ACC.vectors[0].blocks[2], vec[2][:,:,:,0], rank, atol=atol, verbose=verbose)
+    compare_arrays(ACC.vectors[0].blocks[2], vec[2]
+                   [:, :, :, 0], rank, atol=atol, verbose=verbose)
     if verbose:
         print('vec3_1 passed test')
     # compare_arrays(ACC.operators[0].matrix, mat_temp11, rank, atol=atol, verbose=verbose)
     # if verbose:
     #     print('full block matrix_11 passed test')
     # compare_arrays(ACC.operators[1].matrix, mat_temp12, rank, atol=atol, verbose=verbose)
     # if verbose:
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_basis_operators.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_basis_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,26 +44,26 @@
 
     if show_plots:
         domain.show()
 
     # MHD equilibrium
     if mapping[0] == 'Cuboid':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['r1'] - mapping[1]['l1'], 'R0': (mapping[1]['r3'] - mapping[1]['l3'])/(
-            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': 10.0})
+            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': .1})
 
     elif mapping[0] == 'Colella':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['Lx'], 'R0': mapping[1]['Lz']/(
-            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': 10.0})
+            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     elif mapping[0] == 'HollowCylinder':
         eq_mhd = ScrewPinch(**{'a': mapping[1]['a2'], 'R0': 3., 'B0': 1.0,
-                            'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': 10.0})
+                            'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     # set equilibrium object domain
     eq_mhd.domain = domain
 
@@ -473,15 +473,15 @@
                          'R0': 3.,
                          'B0': 1.0,
                          'q0': 1.05,
                          'q1': 1.80,
                          'n1': 3.0,
                          'n2': 4.0,
                          'na': 0.0,
-                         'beta': 10.0})
+                         'beta': .1})
 
     if show_plots:
         eq_mhd.plot_profiles()
 
     eq_mhd.domain = domain
 
     # make sure that boundary conditions are compatible with spline space
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_draw_parallel.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_draw_parallel.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,33 +24,49 @@
     from struphy.pic.particles import Particles6D
 
     comm = MPI.COMM_WORLD
     assert comm.size >= 2
     rank = comm.Get_rank()
 
     seed = int(np.random.rand()*1000)
-    loading_params = {'type': 'pseudo_random', 'seed': seed,
-                      'moments': [0., 0., 0., 1., 1., 1.]}
-
-    marker_params = {'ppc': ppc, 'eps': .25, 'loading': loading_params, 'bc_type' : ['periodic', 'periodic', 'periodic']}
 
     # Domain object
     domain_class = getattr(domains, mapping[0])
     domain = domain_class(**mapping[1])
 
     # Psydac discrete Derham sequence
     derham = Derham(Nel, p, spl_kind, comm=comm)
 
     if rank == 0:
         print()
         print('Domain decomposition according to : ')
         print(derham.domain_array)
 
     # create particles
-    particles = Particles6D('energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    loading_params = {'type': 'pseudo_random',
+                      'seed': seed,
+                      'moments': [0., 0., 0., 1., 1., 1.],
+                      'spatial': 'uniform'}
+    marker_params = {'ppc': ppc,
+                     'eps': .25,
+                     'loading': loading_params,
+                     'bc_type': ['periodic', 'periodic', 'periodic'],
+                     'domain': domain}
+    init_params = {'type': 'Maxwellian6DUniform', 'Maxwellian6DUniform': {}}
+
+    particles = Particles6D('energetic_ions', **marker_params,
+                            domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
+
+    # test weights
+    particles.initialize_weights(init_params)
+    _vdim = particles.vdim
+    _w0 = particles.markers_wo_holes[:, 3 + _vdim]
+    print('Test weights:')
+    print(f'rank {rank}:', _w0.shape, np.min(_w0), np.max(_w0))
 
     comm.Barrier()
     print('Number of particles w/wo holes on each process before sorting : ')
     print('Rank', rank, ':', particles.n_mks_loc,
           particles.markers.shape[0])
 
     # sort particles according to domain decomposition
@@ -73,9 +89,11 @@
     print(
         f'rank {rank} | markers not on correct process: {np.nonzero(np.logical_and(~stay, ~holes))} \n corresponding positions:\n {error_mks[:, :3]}')
 
     assert error_mks.size == 0
 
 
 if __name__ == '__main__':
+    # test_draw([8, 9, 10], [2, 3, 4], [False, False, True], ['Cuboid', {
+    #     'l1': 1., 'r1': 2., 'l2': 10., 'r2': 20., 'l3': 100., 'r3': 200.}])
     test_draw([8, 9, 10], [2, 3, 4], [False, False, True], ['Cuboid', {
-        'l1': 1., 'r1': 2., 'l2': 10., 'r2': 20., 'l3': 100., 'r3': 200.}])
+        'l1': 0., 'r1': 1., 'l2': 0., 'r2': 1., 'l3': 0., 'r3': 1.}])
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_iterative_solvers.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_iterative_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,19 @@
     if show_plots:
         import matplotlib.pyplot as plt
         domain.show()
 
     # MHD equilibrium
     if mapping[0] == 'Cuboid':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['r1'] - mapping[1]['l1'], 'R0': (mapping[1]['r3'] - mapping[1]['l3'])/(
-            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': 10.0})
+            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': .1})
 
     elif mapping[0] == 'Colella':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['Lx'], 'R0': mapping[1]['Lz']/(
-            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': 10.0})
+            2*np.pi), 'B0': 1.0, 'q0': 1.05, 'q1': 1.8, 'n1': 3.0, 'n2': 4.0, 'na': 0.0, 'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     # set equilibrium object domain
     eq_mhd.domain = domain
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_mass_matrices.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_mass_matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,40 +49,40 @@
     # load MHD equilibrium
     if mapping[0] == 'Cuboid':
         eq_mhd = ShearedSlab(**{'a': (mapping[1]['r1'] - mapping[1]['l1']),
                               'R0': (mapping[1]['r3'] - mapping[1]['l3'])/(2*np.pi),
                               'B0': 1.0, 'q0': 1.05,
                               'q1': 1.8, 'n1': 3.0,
                               'n2': 4.0, 'na': 0.0,
-                              'beta': 10.0})
+                              'beta': .1})
 
     elif mapping[0] == 'Colella':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['Lx'],
                               'R0': mapping[1]['Lz']/(2*np.pi),
                               'B0': 1.0,
                               'q0': 1.05,
                               'q1': 1.8,
                               'n1': 3.0,
                               'n2': 4.0,
                               'na': 0.0,
-                              'beta': 10.0})
+                              'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     elif mapping[0] == 'HollowCylinder':
         eq_mhd = ScrewPinch(**{'a': mapping[1]['a2'],
                              'R0': 3.,
                              'B0': 1.0,
                              'q0': 1.05,
                              'q1': 1.8,
                              'n1': 3.0,
                              'n2': 4.0,
                              'na': 0.0,
-                             'beta': 10.0})
+                             'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     eq_mhd.domain = domain
 
     # make sure that boundary conditions are compatible with spline space (periodic only allows for None)
@@ -257,15 +257,15 @@
                          'R0': mapping[1]['Lz'],
                          'B0': 1.0,
                          'q0': 1.05,
                          'q1': 1.8,
                          'n1': 3.0,
                          'n2': 4.0,
                          'na': 0.0,
-                         'beta': 10.0})
+                         'beta': .1})
 
     if show_plots:
         eq_mhd.plot_profiles()
 
     eq_mhd.domain = domain
 
     # make sure that boundary conditions are compatible with spline space (periodic only allows for None)
@@ -451,40 +451,40 @@
     # load MHD equilibrium
     if mapping[0] == 'Cuboid':
         eq_mhd = ShearedSlab(**{'a': (mapping[1]['r1'] - mapping[1]['l1']),
                               'R0': (mapping[1]['r3'] - mapping[1]['l3'])/(2*np.pi),
                               'B0': 1.0, 'q0': 1.05,
                               'q1': 1.8, 'n1': 3.0,
                               'n2': 4.0, 'na': 0.0,
-                              'beta': 10.0})
+                              'beta': .1})
 
     elif mapping[0] == 'Colella':
         eq_mhd = ShearedSlab(**{'a': mapping[1]['Lx'],
                               'R0': mapping[1]['Lz']/(2*np.pi),
                               'B0': 1.0,
                               'q0': 1.05,
                               'q1': 1.8,
                               'n1': 3.0,
                               'n2': 4.0,
                               'na': 0.0,
-                              'beta': 10.0})
+                              'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     elif mapping[0] == 'HollowCylinder':
         eq_mhd = ScrewPinch(**{'a': mapping[1]['a2'],
                              'R0': 3.,
                              'B0': 1.0,
                              'q0': 1.05,
                              'q1': 1.8,
                              'n1': 3.0,
                              'n2': 4.0,
                              'na': 0.0,
-                             'beta': 10.0})
+                             'beta': .1})
 
         if show_plots:
             eq_mhd.plot_profiles()
 
     eq_mhd.domain = domain
 
     # make sure that boundary conditions are compatible with spline space (periodic only allows for None)
@@ -762,15 +762,15 @@
                          'R0': mapping[1]['Lz'],
                          'B0': 1.0,
                          'q0': 1.05,
                          'q1': 1.8,
                          'n1': 3.0,
                          'n2': 4.0,
                          'na': 0.0,
-                         'beta': 10.0})
+                         'beta': .1})
 
     if show_plots:
         eq_mhd.plot_profiles()
 
     eq_mhd.domain = domain
 
     # make sure that boundary conditions are compatible with spline space
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_mat_vec_filler.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_mat_vec_filler.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_polar.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_polar.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_basics.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_psydac_basics.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_derham.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_psydac_derham.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pushers.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_pushers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 
 # ==================================================================================
+
+
 @pytest.mark.mpi(min_size=2)
 @pytest.mark.parametrize('Nel', [[8, 9, 5], [7, 8, 9]])
 @pytest.mark.parametrize('p',   [[2, 3, 1], [1, 2, 3]])
 @pytest.mark.parametrize('spl_kind', [[False, True, True], [True, False, True], [False, False, True], [True, True, True]])
 @pytest.mark.parametrize('mapping', [
     ['Colella', {
         'Lx': 2., 'Ly': 3., 'alpha': .1, 'Lz': 4.}]])
@@ -45,20 +47,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
@@ -139,20 +142,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
@@ -240,20 +244,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
@@ -341,20 +346,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
@@ -442,20 +448,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
@@ -546,20 +553,21 @@
               for Nel, p, spl_kind in zip(Nel, p, spl_kind)]
 
     space = Tensor_spline_space(spaces)
 
     # particle loading and sorting
     seed = int(np.random.rand()*1000)
     loader_params = {'type': 'pseudo_random',
-                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.]}
+                     'seed': seed, 'moments': [0., 0., 0., 1., 1., 1.], 'spatial': 'uniform'}
     marker_params = {'ppc': 2, 'eps': .25, 'loading': loader_params,
                      'bc_type': ['periodic', 'periodic', 'periodic']}
 
     particles = Particles6D(
         'energetic_ions', **marker_params, domain_array=derham.domain_array, comm=comm)
+    particles.draw_markers()
 
     if show_plots:
         particles.show_physical()
     comm.Barrier()
     particles.mpi_sort_markers()
     comm.Barrier()
     if show_plots:
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_bsplines_kernels.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_domain.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_domain.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_gvec_equil.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_gvec_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     tensor_space_FEM.assemble_Mk(domain, 'V2')
     tensor_space_FEM.assemble_Mk(domain, 'V3')
     print('Assembly of mass matrices done.')
     print()
 
     # mhd projectors dot operator
     eq_MHD = HomogenSlab(
-        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 200., 'n0': 1.})
+        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 2., 'n0': 1.})
     eq_MHD.domain = domain
 
     dot_ops = mhd_op_V2.projectors_dot_x(tensor_space_FEM, eq_MHD)
 
     # random x which is going to product with projectors
     x_0 = np.random.rand(tensor_space_FEM.Ntot_0form)
     x_1 = np.random.rand(tensor_space_FEM.Ntot_1form_cum[-1])
@@ -379,15 +379,15 @@
     tensor_space_FEM.assemble_Mk(domain, 'V2')
     tensor_space_FEM.assemble_Mk(domain, 'V3')
     print('Assembly of mass matrices done.')
     print()
 
     # mhd projectors dot operator
     eq_MHD = HomogenSlab(
-        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 200., 'n0': 1.})
+        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 2., 'n0': 1.})
     eq_MHD.domain = domain
 
     dot_ops = mhd_op_V2.projectors_dot_x(tensor_space_FEM, eq_MHD)
 
     # random x which is going to product with projectors
     x_0 = np.random.rand(tensor_space_FEM.Ntot_0form)
     x_1 = np.random.rand(tensor_space_FEM.Ntot_1form_cum[-1])
@@ -680,15 +680,15 @@
     tensor_space_FEM.assemble_Mk(domain, 'V2')
     tensor_space_FEM.assemble_Mk(domain, 'V3')
     print('Assembly of mass matrices done.')
     print()
 
     # mhd projectors dot operator
     eq_MHD = HomogenSlab(
-        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 200., 'n0': 1.})
+        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 2., 'n0': 1.})
     eq_MHD.domain = domain
 
     dot_ops = mhd_op_V2.projectors_dot_x(tensor_space_FEM, eq_MHD)
 
     # test conditions
     print()
     print('MHD_equilibrium :')
@@ -853,15 +853,15 @@
     tensor_space_FEM.assemble_Mk(domain, 'V2')
     tensor_space_FEM.assemble_Mk(domain, 'V3')
     print('Assembly of mass matrices done.')
     print()
 
     # mhd projectors dot operator
     eq_MHD = HomogenSlab(
-        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 200., 'n0': 1.})
+        **{'B0x': 0., 'B0y': 0., 'B0z': 1., 'beta': 2., 'n0': 1.})
     eq_MHD.domain = domain
 
     dot_ops = mhd_op_V2.projectors_dot_x(tensor_space_FEM, eq_MHD)
 
     # test conditions
     print()
     print('MHD_equilibrium :')
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_polar_splines.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_legacy_polar_splines.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_mhd_equils.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_mhd_equils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,35 +4,40 @@
 
 import numpy as np
 
 @pytest.mark.parametrize('equil_domain_pair', [
     ('HomogenSlab', {}, 'Cuboid', {}),
     ('HomogenSlab', {}, 'Colella', {'alpha': 0.06}),
     ('ShearedSlab', {'a': 0.75, 'R0': 3.5}, 'Cuboid', {'r1': 0.75, 'r2': 2*np.pi*0.75, 'r3': 2*np.pi*3.5}),
+    ('ShearedSlab', {'a': 0.75, 'R0': 3.5, 'q0': 'inf', 'q1': 'inf'}, 'Cuboid', {'r1': 0.75, 'r2': 2*np.pi*0.75, 'r3': 2*np.pi*3.5}),
     ('ShearedSlab', {'a': 0.55, 'R0': 4.5}, 'Orthogonal', {'Lx': 0.55, 'Ly': 2*np.pi*0.55, 'Lz': 2*np.pi*4.5}),
     ('ScrewPinch', {'a': 0.45, 'R0': 2.5}, 'HollowCylinder', {'a1': 0.05, 'a2': 0.45, 'Lz': 2*np.pi*2.5}),
     ('ScrewPinch', {'a': 1.45, 'R0': 6.5}, 'IGAPolarCylinder', {'a': 1.45, 'Lz': 2*np.pi*6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'HollowTorusStraightFieldLine', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'HollowTorusStraightFieldLine', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'HollowTorusStraightFieldLine', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
-    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'HollowTorusStraightFieldLine', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5}),
+    ('ScrewPinch', {'a': 0.45, 'R0': 2.5, 'q0': 1.5, 'q1': 1.5}, 'HollowCylinder', {'a1': 0.05, 'a2': 0.45, 'Lz': 2*np.pi*2.5}),
+    ('ScrewPinch', {'a': 1.45, 'R0': 6.5, 'q0': 1.5, 'q1': 1.5}, 'IGAPolarCylinder', {'a': 1.45, 'Lz': 2*np.pi*6.5}),
+    ('ScrewPinch', {'a': 0.45, 'R0': 2.5, 'q0': 'inf', 'q1': 'inf'}, 'HollowCylinder', {'a1': 0.05, 'a2': 0.45, 'Lz': 2*np.pi*2.5}),
+    ('ScrewPinch', {'a': 1.45, 'R0': 6.5, 'q0': 'inf', 'q1': 'inf'}, 'IGAPolarCylinder', {'a': 1.45, 'Lz': 2*np.pi*6.5}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': False}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': False}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': False}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': False}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': True}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': True}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': True}),
+    ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'HollowTorus', {'a1': 0.05, 'a2': 1.45, 'R0': 6.5, 'sfl': True}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'IGAPolarTorus', {'a': 1.45, 'R0': 6.5, 'sfl': True}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'IGAPolarTorus', {'a': 1.45, 'R0': 6.5, 'sfl': True}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'IGAPolarTorus', {'a': 1.45, 'R0': 6.5, 'sfl': True}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'IGAPolarTorus', {'a': 1.45, 'R0': 6.5, 'sfl': True}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 0}, 'Tokamak', {}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 0, 'p_kind': 1}, 'Tokamak', {}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 0}, 'Tokamak', {}),
     ('AdhocTorus', {'a': 1.45, 'R0': 6.5, 'q_kind': 1, 'p_kind': 1}, 'Tokamak', {}),
-    ('AdhocTorusQPsi', {'a': 0.8, 'R0': 3.6}, 'HollowTorus', {'a1': 0.05, 'a2': 0.8, 'R0': 3.6}),
-    ('AdhocTorusQPsi', {'a': 0.8, 'R0': 3.6}, 'HollowTorusStraightFieldLine', {'a1': 0.05, 'a2': 0.8, 'R0': 3.6}),
+    ('AdhocTorusQPsi', {'a': 0.8, 'R0': 3.6}, 'HollowTorus', {'a1': 0.05, 'a2': 0.8, 'R0': 3.6, 'sfl': False}),
+    ('AdhocTorusQPsi', {'a': 0.8, 'R0': 3.6}, 'HollowTorus', {'a1': 0.05, 'a2': 0.8, 'R0': 3.6, 'sfl': True}),
     ('AdhocTorusQPsi', {'a': 0.8, 'R0': 3.6}, 'IGAPolarTorus', {'a': 0.8, 'R0': 3.6, 'sfl': True}),
     ('AdhocTorusQPsi', {'a': 1.0, 'R0': 3.6}, 'Tokamak', {}),
     ('EQDSKequilibrium', {}, 'Tokamak', {}),
     
 ])
 def test_equils(equil_domain_pair):
     """
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_projectors_global.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_prop_solvers.py` & `struphy-2.0.1/src/struphy/tests/tests_mpi/test_prop_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from struphy.psydac_api.mass import WeightedMassOperator
 from struphy.propagators.base import Propagator
 from struphy.propagators.solvers import PoissonSolver
 from struphy.psydac_api.utilities import compare_arrays
 from psydac.linalg.stencil import StencilVector
 
 
+@pytest.mark.mpi(min_size=2)
 @pytest.mark.parametrize('Nel', [[10, 2, 2], [40, 2, 2]])
 @pytest.mark.parametrize('p', [[1, 1, 1], [3, 1, 1]])
 @pytest.mark.parametrize('spl_kind', [[True, True, True]])
 @pytest.mark.parametrize('mapping', [
     ['Cuboid', {
         'l1': 0., 'r1': 1., 'l2': 0., 'r2': 1., 'l3': 0., 'r3': 1.}],
 ])
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_basis_operators.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_basis_operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         print(f'Rank {mpi_rank} | Nel: {Nel}')
         print(f'Rank {mpi_rank} | p: {p}')
         print(f'Rank {mpi_rank} | spl_kind: {spl_kind}')
         print(f'Rank {mpi_rank} | ')
 
     # Mhd equilibirum (slab)
     mhd_equil_params = {'B0x': 0., 'B0y': 0.,
-                        'B0z': 1., 'beta': 200., 'n0': 1.}
+                        'B0z': 1., 'beta': 2., 'n0': 1.}
 
     EQ_MHD = HomogenSlab(**mhd_equil_params)
     EQ_MHD.domain = domain
 
     # Psydac spline spaces
     V0 = DERHAM_PSY.Vh_fem['0']
     V1 = DERHAM_PSY.Vh_fem['1']
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_linear_operators.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_mapping.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_psydac_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,14 @@
         'l1': 1., 'r1': 2., 'l2': 10., 'r2': 20., 'l3': 100., 'r3': 200.}],
     ['Orthogonal', {
         'Lx': 1., 'Ly': 2., 'alpha': .5, 'Lz': 3.}],
     ['Colella', {
         'Lx': 1., 'Ly': 2., 'alpha': .5, 'Lz': 3.}],
     ['HollowCylinder', {
         'a1': 1., 'a2': 2., 'Lz': 5.}],
-    ['HollowTorus', {
-        'a1': 1., 'a2': 2., 'R0': 3., 'tor_period': 1}],
     ['ShafranovShiftCylinder', {
         'rx': 4., 'ry': 5., 'Lz': 6., 'delta': 7.}],
     ['ShafranovSqrtCylinder', {
         'rx': 4., 'ry': 5., 'Lz': 6., 'delta': 7.}],
     ['ShafranovDshapedCylinder', {
         'R0': 4., 'Lz': 5., 'delta_x': 0.06, 'delta_y': 0.07, 'delta_gs': 0.08, 'epsilon_gs': 9., 'kappa_gs': 10.}],
 ])
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/test_spline_space_1d.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/test_spline_space_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     # Psydac discrete De Rham
     DOMAIN_PSY  = discretize(DOMAIN_symb, ncells=Nel, comm=MPI_COMM) # The parallelism is initiated here.
     DERHAM_PSY  = discretize(DERHAM_symb, DOMAIN_PSY, degree=p, periodic=spl_kind)
 
     # Mhd equilibirum
     mhd_equil_general = {'type': 'slab', 'mass_number' : 1 }
-    mhd_equil_params = {'B0x': 0., 'B0y': 0., 'B0z': 1., 'rho0': 1., 'beta': 200.}
+    mhd_equil_params = {'B0x': 0., 'B0y': 0., 'B0z': 1., 'rho0': 1., 'beta': 2.}
 
     EQ_MHD_P = Equilibrium_mhd_physical(mhd_equil_general['type'], mhd_equil_params)
     EQ_MHD_L = Equilibrium_mhd_logical(DOMAIN, EQ_MHD_P)
 
     # Psydac spline spaces
     V0 = DERHAM_PSY.V0
     V1 = DERHAM_PSY.V1
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_GVEC.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_GVEC.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_codes.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_codes.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_cprofiler.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_cprofiler.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_divB.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_divB.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_filler_kernel.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_filler_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mappings.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mappings.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mhd_equil.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_mhd_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_paraview.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_paraview.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_preconditioner.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_preconditioner.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     # Psydac discrete De Rham
     DOMAIN_PSY  = discretize(DOMAIN_PSYDAC_LOGICAL, ncells=Nel, comm=MPI_COMM) # The parallelism is initiated here.
     DERHAM_PSY  = discretize(DERHAM_symb, DOMAIN_PSY, degree=p, periodic=spl_kind)
 
     # Mhd equilibirum
     mhd_equil_general = {'type': 'slab', 'mass_number' : 1 }
-    mhd_equil_params = {'B0x': 0., 'B0y': 0., 'B0z': 1., 'rho0': 1., 'beta': 200.}
+    mhd_equil_params = {'B0x': 0., 'B0y': 0., 'B0z': 1., 'rho0': 1., 'beta': 2.}
 
     EQ_MHD_P = Equilibrium_mhd_physical(mhd_equil_general['type'], mhd_equil_params)
     EQ_MHD_L = Equilibrium_mhd_logical(DOMAIN, EQ_MHD_P)
 
     # Psydac spline spaces
     V0 = DERHAM_PSY.V0
     V1 = DERHAM_PSY.V1
```

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_template_gvec.py` & `struphy-2.0.1/src/struphy/tests/tests_serial/xx_test_template_gvec.py`

 * *Files identical despite different names*

### Comparing `struphy-2.0.0/src/struphy.egg-info/PKG-INFO` & `struphy-2.0.1/src/struphy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struphy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Multi-model plasma physics package
 Author: Max Planck Institute for Plasma Physics
 Author-email: stefan.possanner@ipp.mpg.de, florian.holderied@ipp.mpg.de
 License: Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and 
         associated documentation files (the "Software"), to deal in the Software without restriction, 
@@ -42,19 +42,19 @@
 # STRUPHY - STRUcture-Preserving HYbrid codes
 
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
-## What you can do with struphy
+## What you can do with Struphy
 
 * Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
 * Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html#module-struphy.fields_background.mhd_equil.equils) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
 * Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
 * Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
 * Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
 * [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
     * model equations
     * domains (geometry)
     * MHD equilibria
@@ -70,24 +70,23 @@
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [Struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
 
 ## Tutorials
 
-* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+* [Tutorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
 
-* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
-of field/fluid and kinetic variables.
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Data generated by Struphy simulations, post processing and simple plotting of variables.
 
-* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
@@ -106,10 +105,10 @@
 In addition, we ask you to cite the following reference in scientific publications which contain results obtained with
 this software and developments:
 
 F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", J. Comp. Phys. 433 (2021) 110143
 
 ## Contact
 
-* Florian Holderied [floho@ipp.mpg.de](floho@ipp.mpg.de)
 * Stefan Possanner [spossann@ipp.mpg.de](spossann@ipp.mpg.de)
+* Eric Sonnendrücker [spossann@ipp.mpg.de](eric.sonnendruecker@ipp.mpg.de)
 * Xin Wang [xin.wang@ipp.mpg.de](xin.wang@ipp.mpg.de)
```

### Comparing `struphy-2.0.0/src/struphy.egg-info/SOURCES.txt` & `struphy-2.0.1/src/struphy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/struphy/console/main.py
 src/struphy/console/pproc.py
 src/struphy/console/profile.py
 src/struphy/console/run.py
 src/struphy/console/test.py
 src/struphy/console/units.py
 src/struphy/diagnostics/__init__.py
+src/struphy/diagnostics/console_diagn.py
 src/struphy/diagnostics/continuous_spectra.py
 src/struphy/diagnostics/diagn_tools.py
 src/struphy/diagnostics/paraview/__init__.py
 src/struphy/diagnostics/paraview/mesh_creator.py
 src/struphy/diagnostics/paraview/vtk_writer.py
 src/struphy/dispersion_relations/__init__.py
 src/struphy/dispersion_relations/analytic.py
@@ -157,19 +158,21 @@
 src/struphy/io/inp/examples/params_TAE_tokamak.yml
 src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
 src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
 src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
 src/struphy/io/inp/examples/params_linearextendedmhd.yml
 src/struphy/io/inp/examples/params_linearmhd.yml
 src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
+src/struphy/io/inp/examples/params_linvlasovmaxwell_streaming_weibel.yml
 src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
 src/struphy/io/inp/examples/params_maxwell.yml
 src/struphy/io/inp/examples/params_orbits_tokamak.yml
 src/struphy/io/inp/tests/__init__.py
 src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
+src/struphy/io/inp/tests/params_coldplasma.yml
 src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml
 src/struphy/io/inp/tests/params_hybrid_fA.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
 src/struphy/io/inp/tests/params_linearmhd.yml
@@ -184,17 +187,18 @@
 src/struphy/io/inp/tests/wkscl_4.yml
 src/struphy/io/inp/tests/wkscl_5.yml
 src/struphy/io/inp/tests/wkscl_6.yml
 src/struphy/io/inp/tests/wkscl_7.yml
 src/struphy/io/inp/tests/wkscl_8.yml
 src/struphy/io/out/__init__.py
 src/struphy/kinetic_background/__init__.py
-src/struphy/kinetic_background/analytical.py
 src/struphy/kinetic_background/background_eval.py
+src/struphy/kinetic_background/base.py
 src/struphy/kinetic_background/f0_kernels.py
+src/struphy/kinetic_background/maxwellians.py
 src/struphy/kinetic_background/moments_kernels.py
 src/struphy/linear_algebra/__init__.py
 src/struphy/linear_algebra/core.py
 src/struphy/linear_algebra/iterative_solvers.py
 src/struphy/linear_algebra/linalg_kron.py
 src/struphy/linear_algebra/schur_solver.py
 src/struphy/linear_algebra/stencil_dot_kernels.py
@@ -202,16 +206,16 @@
 src/struphy/models/__init__.py
 src/struphy/models/base.py
 src/struphy/models/fluid.py
 src/struphy/models/hybrid.py
 src/struphy/models/kinetic.py
 src/struphy/models/main.py
 src/struphy/models/output_handling.py
+src/struphy/models/setup.py
 src/struphy/models/toy.py
-src/struphy/models/utilities.py
 src/struphy/pic/__init__.py
 src/struphy/pic/accum_kernels.py
 src/struphy/pic/filler_kernels.py
 src/struphy/pic/mat_vec_filler.py
 src/struphy/pic/particles.py
 src/struphy/pic/particles_to_grid.py
 src/struphy/pic/pusher.py
@@ -256,20 +260,20 @@
 src/struphy/tests/tests_mpi/test_basis_operators.py
 src/struphy/tests/tests_mpi/test_draw_parallel.py
 src/struphy/tests/tests_mpi/test_eval_spline_mpi.py
 src/struphy/tests/tests_mpi/test_iterative_solvers.py
 src/struphy/tests/tests_mpi/test_mass_matrices.py
 src/struphy/tests/tests_mpi/test_mat_vec_filler.py
 src/struphy/tests/tests_mpi/test_polar.py
+src/struphy/tests/tests_mpi/test_prop_solvers.py
 src/struphy/tests/tests_mpi/test_psydac_basics.py
 src/struphy/tests/tests_mpi/test_psydac_derham.py
 src/struphy/tests/tests_mpi/test_pushers.py
 src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py
 src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py
-src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/__init__.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py
 src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py
@@ -282,15 +286,14 @@
 src/struphy/tests/tests_serial/test_domain.py
 src/struphy/tests/tests_serial/test_gvec_equil.py
 src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
 src/struphy/tests/tests_serial/test_legacy_polar_splines.py
 src/struphy/tests/tests_serial/test_mhd_equils.py
 src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
 src/struphy/tests/tests_serial/test_projectors_global.py
-src/struphy/tests/tests_serial/test_prop_solvers.py
 src/struphy/tests/tests_serial/test_psydac_basis_operators.py
 src/struphy/tests/tests_serial/test_psydac_linear_operators.py
 src/struphy/tests/tests_serial/test_psydac_mapping.py
 src/struphy/tests/tests_serial/test_spline_space_1d.py
 src/struphy/tests/tests_serial/xx_psydac_lin_ops.py
 src/struphy/tests/tests_serial/xx_test_GVEC.py
 src/struphy/tests/tests_serial/xx_test_codes.py
```

