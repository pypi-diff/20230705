# Comparing `tmp/tangelo-gc-0.4.0.tar.gz` & `tmp/tangelo-gc-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangelo-gc-0.4.0.tar", last modified: Wed Jul  5 21:16:38 2023, max compression
+gzip compressed data, was "tangelo-gc-0.4.0rc0.tar", last modified: Thu Jun 29 23:16:01 2023, max compression
```

## Comparing `tangelo-gc-0.4.0.tar` & `tangelo-gc-0.4.0rc0.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.284652 tangelo-gc-0.4.0/
--rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/LICENSE
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      437 2023-07-05 21:16:38.284515 tangelo-gc-0.4.0/PKG-INFO
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11203 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/README.rst
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)       38 2023-07-05 21:16:38.284690 tangelo-gc-0.4.0/setup.cfg
--rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      916 2023-07-05 09:00:00.000000 tangelo-gc-0.4.0/setup.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.235551 tangelo-gc-0.4.0/tangelo/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      723 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      735 2023-07-05 21:15:32.000000 tangelo-gc-0.4.0/tangelo/_version.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.236128 tangelo-gc-0.4.0/tangelo/algorithms/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      783 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.237413 tangelo-gc-0.4.0/tangelo/algorithms/classical/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      738 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13884 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/ccsd_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14155 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/fci_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14715 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/mp2_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3088 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/semi_empirical_solver.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.238100 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3613 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_ccsd_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3012 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_fci_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4247 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_mp2_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1617 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2120 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/electronic_structure_solver.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.238375 tangelo-gc-0.4.0/tangelo/algorithms/projective/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      633 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/projective/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15369 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/projective/quantum_imaginary_time.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.238663 tangelo-gc-0.4.0/tangelo/algorithms/projective/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/projective/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6064 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/projective/tests/test_qite.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.240108 tangelo-gc-0.4.0/tangelo/algorithms/variational/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      898 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17441 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/adapt_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15567 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/iqcc_ilc_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14915 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/iqcc_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15440 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/sa_oo_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12679 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/sa_vqe_solver.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.241491 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7445 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3574 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4033 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_iqcc_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2765 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11665 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2251 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    29311 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2934 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36829 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/algorithms/variational/vqe_solver.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.241939 tangelo-gc-0.4.0/tangelo/helpers/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      642 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/helpers/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2873 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/helpers/math.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3762 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/helpers/utils.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.242778 tangelo-gc-0.4.0/tangelo/linq/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      937 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19075 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8982 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/gate.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.243047 tangelo-gc-0.4.0/tangelo/linq/helpers/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      635 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.243584 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      656 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3914 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/clifford_circuits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/measurement_basis.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/statevector.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.244002 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1871 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3208 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/test_statevector.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.244277 tangelo-gc-0.4.0/tangelo/linq/helpers/operators/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      611 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/operators/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1724 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/helpers/operators/operators.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.244558 tangelo-gc-0.4.0/tangelo/linq/noisy_simulation/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      614 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/noisy_simulation/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5051 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/noisy_simulation/noise_models.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2268 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qdk_template.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.245397 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6112 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/braket_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7428 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/ibm_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9539 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/ionq_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6696 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/qemist_cloud_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      909 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/qpu_connection/qpu_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2578 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/simulator.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.246810 tangelo-gc-0.4.0/tangelo/linq/target/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1239 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    37084 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/backend.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12794 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_cirq.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4596 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_qdk.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12428 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_qiskit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11780 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_qulacs.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7657 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_stim.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5024 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/target/target_sympy.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.248828 tangelo-gc-0.4.0/tangelo/linq/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2799 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_braket_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14256 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_circuits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7437 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_gates.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3962 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_ibm_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3194 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_ionq_connection.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    32240 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_simulator.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13817 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_simulator_noisy.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3246 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_symbolic_simulator.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    25603 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4278 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_perf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8362 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_qubitop.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.251391 tangelo-gc-0.4.0/tangelo/linq/translator/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2015 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2281 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/qdk_template.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5896 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_braket.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3575 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8285 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_cirq.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4770 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_json_ionq.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5552 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_openqasm.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5753 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_pennylane.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6133 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_projectq.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5692 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_qdk.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8706 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_qiskit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3668 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_qubitop.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9287 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_qulacs.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5677 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_stim.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7610 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/linq/translator/translate_sympy.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5310 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/molecule_library.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.251701 tangelo-gc-0.4.0/tangelo/problem_decomposition/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.252645 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      639 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.253646 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1381 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6636 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2656 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3761 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9799 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4936 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4378 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36407 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10607 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/fragment.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.254246 tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      743 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10061 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/iao_localization.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1200 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1255 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/nao_localization.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.254570 tangelo-gc-0.4.0/tangelo/problem_decomposition/incremental/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/incremental/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17513 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/incremental/mifno_helper.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.254926 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.255400 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2410 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12174 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5725 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      863 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/problem_decomposition.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.255569 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.257155 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11803 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2814 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5347 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2876 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3466 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2602 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.257868 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4272 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_capping.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6868 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_oniom.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6129 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.258066 tangelo-gc-0.4.0/tangelo/toolboxes/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.263436 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      943 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21631 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2198 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9590 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14250 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9849 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16155 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3645 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4442 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7277 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1709 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ansatz.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21208 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6132 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7772 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/hea.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14088 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ilc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6397 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/penalty_terms.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8521 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/puccd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14565 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/qcc.py
--rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)    12343 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/qmf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8542 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/rucc.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.266327 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2131 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16763 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11680 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5816 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4746 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8408 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13153 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2596 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7868 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5980 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3394 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3747 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6253 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5452 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2439 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5312 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9103 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/uccgd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14028 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/uccsd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10165 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/upccgsd.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3378 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/variational_circuit.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12665 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/vsqs.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.268080 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7032 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/diagonal_coulomb.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3673 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/discrete_clock.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3854 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/grid_circuits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17697 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/lcu.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5839 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/multiproduct.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12208 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/qsp.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.269412 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2212 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5828 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3412 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_grid.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8725 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_lcu.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5207 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_mp.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5038 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_qsp.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.270156 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1045 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/__init__.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.271328 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      598 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8043 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6221 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10453 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9000 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/randomized.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/estimate_measurements.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5618 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/qubit_terms_grouping.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.272740 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4398 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3730 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4794 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_measurements.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6905 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4894 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.274535 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      876 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2082 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/coefficients.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7488 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4598 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10238 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver_psi4.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12003 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    26948 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/molecule.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19213 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/rdms.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.276224 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1465 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5531 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8616 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4069 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4432 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_psi4.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9120 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_rdms.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.277595 tangelo-gc-0.4.0/tangelo/toolboxes/operators/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      844 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16328 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/multiformoperator.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14593 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/operators.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4539 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/taper_qubits.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.278874 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4595 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_multiformoperator.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7869 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_operators.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6052 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_taper_qubits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4744 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4174 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_z2_tapering.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6442 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/trim_trivial_qubits.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7085 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/operators/z2_tapering.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.279180 tangelo-gc-0.4.0/tangelo/toolboxes/optimizers/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      619 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/optimizers/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3333 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/optimizers/rotosolve.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.280479 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      860 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2191 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/bootstrapping.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6517 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/extrapolation.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8963 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/histogram.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3071 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5535 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/post_selection.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.281239 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3048 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7088 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_histogram.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2298 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_post_selection.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.282703 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      813 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2383 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8432 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/combinatorial.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2986 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/hcb.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8073 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/jkmn.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2025 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7502 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/mapping_transform.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7350 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10494 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.283783 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/__init__.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2779 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4635 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2175 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7972 2023-07-05 08:57:34.000000 tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py
-drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-07-05 21:16:38.284357 tangelo-gc-0.4.0/tangelo_gc.egg-info/
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)      437 2023-07-05 21:16:38.000000 tangelo-gc-0.4.0/tangelo_gc.egg-info/PKG-INFO
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13175 2023-07-05 21:16:38.000000 tangelo-gc-0.4.0/tangelo_gc.egg-info/SOURCES.txt
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)        1 2023-07-05 21:16:38.000000 tangelo-gc-0.4.0/tangelo_gc.egg-info/dependency_links.txt
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)       26 2023-07-05 21:16:38.000000 tangelo-gc-0.4.0/tangelo_gc.egg-info/requires.txt
--rw-r--r--   0 valentinsenicourt   (502) staff       (20)        8 2023-07-05 21:16:38.000000 tangelo-gc-0.4.0/tangelo_gc.egg-info/top_level.txt
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.500423 tangelo-gc-0.4.0rc0/
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/LICENSE
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      440 2023-06-29 23:16:01.500288 tangelo-gc-0.4.0rc0/PKG-INFO
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11203 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/README.rst
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)       38 2023-06-29 23:16:01.500464 tangelo-gc-0.4.0rc0/setup.cfg
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)      913 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/setup.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.453415 tangelo-gc-0.4.0rc0/tangelo/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      723 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      738 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/_version.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.454028 tangelo-gc-0.4.0rc0/tangelo/algorithms/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      783 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.454998 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      738 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13884 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/ccsd_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14155 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/fci_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14715 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/mp2_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3088 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/semi_empirical_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.455737 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3613 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_ccsd_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3012 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_fci_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4247 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_mp2_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1617 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2120 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/electronic_structure_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.456014 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      633 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15369 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/quantum_imaginary_time.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.456297 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6064 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/test_qite.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.457956 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      898 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17441 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15567 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_ilc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14915 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    15440 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_oo_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12679 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_vqe_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.459513 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7445 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3574 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4033 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2765 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11665 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2251 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    29311 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2934 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36829 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/vqe_solver.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.459996 tangelo-gc-0.4.0rc0/tangelo/helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      642 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2873 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/math.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3762 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/helpers/utils.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.460804 tangelo-gc-0.4.0rc0/tangelo/linq/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      937 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19075 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8982 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/gate.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.461041 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      635 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.461613 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      656 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3914 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/clifford_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/measurement_basis.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/statevector.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462114 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1871 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3208 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_statevector.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462396 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      611 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1724 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/operators.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.462670 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      614 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5051 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/noise_models.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2268 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qdk_template.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.463601 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6112 2023-06-29 23:14:37.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/braket_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7428 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ibm_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9539 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ionq_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6696 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qemist_cloud_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      909 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qpu_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2578 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/simulator.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.465070 tangelo-gc-0.4.0rc0/tangelo/linq/target/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1239 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    37084 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/backend.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12794 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_cirq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4596 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qdk.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12428 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qiskit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11780 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qulacs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7657 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_stim.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5024 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/target/target_sympy.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.467267 tangelo-gc-0.4.0rc0/tangelo/linq/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2799 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_braket_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14256 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7437 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_gates.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3962 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ibm_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3194 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ionq_connection.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    32240 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13817 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator_noisy.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3246 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_symbolic_simulator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    25603 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4278 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_perf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8362 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_qubitop.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.470031 tangelo-gc-0.4.0rc0/tangelo/linq/translator/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2015 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2281 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/qdk_template.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5896 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_braket.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3575 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8285 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_cirq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4770 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_json_ionq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5552 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_openqasm.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5753 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_pennylane.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6133 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_projectq.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5692 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qdk.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8706 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qiskit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3668 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qubitop.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9287 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qulacs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5677 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_stim.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7610 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_sympy.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5310 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/molecule_library.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.470375 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      779 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.471223 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      639 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.472249 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1381 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6636 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2656 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3761 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9799 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4936 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4378 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    36407 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10607 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/fragment.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.472850 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      743 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10061 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/iao_localization.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1200 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1255 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/nao_localization.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.473160 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17513 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/mifno_helper.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.473525 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.474084 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2410 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12174 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5725 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      863 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/problem_decomposition.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.474267 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.475694 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11803 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2814 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5347 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2876 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3466 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2602 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.476490 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4272 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_capping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6868 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6129 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.476682 tangelo-gc-0.4.0rc0/tangelo/toolboxes/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.481540 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      943 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21631 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2198 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9590 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14250 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9849 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16155 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3645 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4442 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7277 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1709 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    21208 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6132 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7772 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/hea.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14088 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6397 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/penalty_terms.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8521 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/puccd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14565 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qcc.py
+-rwxr-xr-x   0 valentinsenicourt   (502) staff       (20)    12343 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qmf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8542 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/rucc.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.484571 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2131 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16763 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    11680 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5816 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4746 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8408 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13153 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2596 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7868 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5980 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3394 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3747 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6253 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5452 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2439 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5312 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9103 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccgd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14028 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10165 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/upccgsd.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3378 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/variational_circuit.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12665 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/vsqs.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.485757 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      638 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7032 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/diagonal_coulomb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3673 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/discrete_clock.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3854 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/grid_circuits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    17697 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/lcu.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5839 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/multiproduct.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12208 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/qsp.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.488126 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2212 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5828 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3412 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_grid.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8725 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_lcu.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5207 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_mp.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5038 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_qsp.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.488686 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1045 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/__init__.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.489535 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      598 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8043 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6221 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10453 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9000 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/randomized.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/estimate_measurements.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5618 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/qubit_terms_grouping.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.490492 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4398 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3730 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4794 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_measurements.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6905 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4894 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.491846 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      876 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2082 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/coefficients.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7488 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4598 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10238 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_psi4.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    12003 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    26948 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/molecule.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    19213 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/rdms.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.493229 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     1465 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5531 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8616 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4069 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4432 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_psi4.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     9120 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_rdms.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.494166 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      844 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    16328 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/multiformoperator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    14593 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4539 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/taper_qubits.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.495062 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4595 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_multiformoperator.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7869 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_operators.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6052 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_taper_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4744 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4174 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_z2_tapering.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6442 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/trim_trivial_qubits.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7085 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/z2_tapering.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.495363 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      619 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3333 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/rotosolve.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.496297 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      860 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2191 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/bootstrapping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     6517 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/extrapolation.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8963 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/histogram.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3071 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     5535 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/post_selection.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.497070 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     3048 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7088 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_histogram.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2387 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2298 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_post_selection.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.498544 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      813 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2383 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8432 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/combinatorial.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2986 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/hcb.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     8073 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jkmn.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2025 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7502 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/mapping_transform.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7350 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10494 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.499472 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      585 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/__init__.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2779 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     4635 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    10280 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     2175 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)     7972 2023-06-29 23:14:38.000000 tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py
+drwxr-xr-x   0 valentinsenicourt   (502) staff       (20)        0 2023-06-29 23:16:01.500109 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)      440 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/PKG-INFO
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)    13175 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/SOURCES.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)        1 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/dependency_links.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)       26 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/requires.txt
+-rw-r--r--   0 valentinsenicourt   (502) staff       (20)        8 2023-06-29 23:16:01.000000 tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/top_level.txt
```

### Comparing `tangelo-gc-0.4.0/LICENSE` & `tangelo-gc-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/README.rst` & `tangelo-gc-0.4.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/setup.py` & `tangelo-gc-0.4.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 import sys
 import subprocess
 import os
 
 
-#def install(package):
-#    subprocess.check_call([sys.executable, "-m", "pip", "install", package])
+def install(package):
+    subprocess.check_call([sys.executable, "-m", "pip", "install", package])
 
 
 with open("tangelo/_version.py") as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
-#install('wheel')
+install('wheel')
 
 description = "Maintained by Good Chemistry Company, focusing on the development of end-to-end materials simulation workflows on quantum computers."
 
 setuptools.setup(
     name="tangelo-gc",
     author="The Tangelo developers",
     version=version,
```

### Comparing `tangelo-gc-0.4.0/tangelo/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/_version.py` & `tangelo-gc-0.4.0rc0/tangelo/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Define version number here. It is read in setup.py, and bumped automatically
 when using the new release Github action. """
-__version__ = "0.4.0"
+__version__ = "0.4.0.RC"
```

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/ccsd_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/ccsd_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/fci_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/fci_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/mp2_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/mp2_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/semi_empirical_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/semi_empirical_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_ccsd_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_ccsd_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_fci_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_fci_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_mp2_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_mp2_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/classical/tests/test_semi_empirical_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/electronic_structure_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/electronic_structure_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/projective/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/projective/quantum_imaginary_time.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/quantum_imaginary_time.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/projective/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/projective/tests/test_qite.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/projective/tests/test_qite.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/iqcc_ilc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_ilc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/iqcc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/iqcc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/sa_oo_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_oo_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/sa_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/sa_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_ilc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_iqcc_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_iqcc_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_oo_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_sa_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_tetris_adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tests/test_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tests/test_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/tetris_adapt_vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/algorithms/variational/vqe_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/algorithms/variational/vqe_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/helpers/math.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/math.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/helpers/utils.py` & `tangelo-gc-0.4.0rc0/tangelo/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/gate.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/gate.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/clifford_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/clifford_circuits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/measurement_basis.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/measurement_basis.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/statevector.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/statevector.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_clifford_circuits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/circuits/tests/test_statevector.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/circuits/tests/test_statevector.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/operators/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/helpers/operators/operators.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/helpers/operators/operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/noisy_simulation/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/noisy_simulation/noise_models.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/noisy_simulation/noise_models.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qdk_template.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qdk_template.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/braket_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/braket_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/ibm_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ibm_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/ionq_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/ionq_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/qemist_cloud_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qemist_cloud_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/qpu_connection/qpu_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/qpu_connection/qpu_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/simulator.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/simulator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/backend.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/backend.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_cirq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_cirq.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_qdk.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qdk.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_qiskit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qiskit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_qulacs.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_qulacs.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_stim.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_stim.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/target/target_sympy.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/target/target_sympy.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_braket_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_braket_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_circuits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_gates.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_ibm_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ibm_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_ionq_connection.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_ionq_connection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_simulator.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_simulator_noisy.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_simulator_noisy.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_symbolic_simulator.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_symbolic_simulator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_perf.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_perf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/tests/test_translator_qubitop.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/tests/test_translator_qubitop.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/qdk_template.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/qdk_template.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_braket.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_braket.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_cirq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_cirq.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_json_ionq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_json_ionq.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_openqasm.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_openqasm.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_pennylane.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_pennylane.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_projectq.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_projectq.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_qdk.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qdk.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_qiskit.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qiskit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_qubitop.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qubitop.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_qulacs.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_qulacs.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_stim.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_stim.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/linq/translator/translate_sympy.py` & `tangelo-gc-0.4.0rc0/tangelo/linq/translator/translate_sympy.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/molecule_library.py` & `tangelo-gc-0.4.0rc0/tangelo/molecule_library.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_bath.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_fragment.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_onerdm.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/_helpers/dmet_scf_guess.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/dmet_problem_decomposition.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/dmet/fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/dmet/fragment.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/iao_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/iao_localization.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/meta_lowdin_localization.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/electron_localization/nao_localization.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/electron_localization/nao_localization.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/incremental/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/incremental/mifno_helper.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/incremental/mifno_helper.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/capping_groups.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/_helpers/helper_classes.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/oniom/oniom_problem_decomposition.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/problem_decomposition.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/problem_decomposition.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_fragment.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_oneshot_loop.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_dmet_vqe.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/dmet/test_osdmet.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_capping.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_capping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_oniom.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py` & `tangelo-gc-0.4.0rc0/tangelo/problem_decomposition/tests/oniom/test_oniom_quantum.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_general_unitary_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_hea_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_qubit_mf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_openshell.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_cc_paired.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/_unitary_majorana_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/adapt_ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ansatz_utils.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/fermionic_operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/hea.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/hea.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/penalty_terms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/penalty_terms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/puccd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/puccd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/qcc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qcc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/qmf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/qmf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/rucc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/rucc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_adapt_ansatz.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ansatz_util.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_fermionic_operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_general_unitary_cc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_hea.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_ilc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_penalty_terms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_puccd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qcc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_qmf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_rucc.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccgd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_uccsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_upccgsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_variational_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/tests/test_vsqs.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/uccgd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccgd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/uccsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/uccsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/upccgsd.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/upccgsd.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/variational_circuit.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/variational_circuit.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/ansatz_generator/vsqs.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/ansatz_generator/vsqs.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/diagonal_coulomb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/diagonal_coulomb.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/discrete_clock.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/discrete_clock.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/grid_circuits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/grid_circuits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/lcu.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/lcu.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/multiproduct.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/multiproduct.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/qsp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/qsp.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_diagonal_coulomb.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_discrete_clock.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_grid.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_lcu.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_lcu.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_mp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/circuits/tests/test_qsp.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/circuits/tests/test_qsp.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/adaptive.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/derandomized.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/classical_shadows/randomized.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/classical_shadows/randomized.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/estimate_measurements.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/estimate_measurements.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/qubit_terms_grouping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/qubit_terms_grouping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_adaptive_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_derandomized_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_measurements.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_qubit_terms_grouping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/measurements/tests/test_randomized_classical_shadows.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/coefficients.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/coefficients.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/frozen_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver_psi4.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_psi4.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/integral_solver_pyscf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/molecule.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/molecule.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/rdms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/rdms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_coefficients.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_frozen_orbitals.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_nopyscf.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_psi4.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_psi4.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/molecular_computation/tests/test_rdms.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/molecular_computation/tests/test_rdms.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/multiformoperator.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/multiformoperator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/taper_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/taper_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_multiformoperator.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_multiformoperator.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_operators.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_taper_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_taper_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_trim_trivial_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/tests/test_z2_tapering.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/tests/test_z2_tapering.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/trim_trivial_qubits.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/trim_trivial_qubits.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/operators/z2_tapering.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/operators/z2_tapering.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/optimizers/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/optimizers/rotosolve.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/optimizers/rotosolve.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/bootstrapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/extrapolation.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/extrapolation.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/histogram.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/histogram.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/mc_weeny_rdm_purification.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/post_selection.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/post_selection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_extrapolation.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_histogram.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_mcweeny_purification.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/post_processing/tests/test_post_selection.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/post_processing/tests/test_post_selection.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/combinatorial.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/combinatorial.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/hcb.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/hcb.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/jkmn.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jkmn.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/jordan_wigner.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/mapping_transform.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/mapping_transform.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/statevector_mapping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/symmetry_conserving_bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/__init__.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_bravyi_kitaev.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_combinatorial.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_mapping_transform.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_qubitizer.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py` & `tangelo-gc-0.4.0rc0/tangelo/toolboxes/qubit_mappings/tests/test_statevector_mapping.py`

 * *Files identical despite different names*

### Comparing `tangelo-gc-0.4.0/tangelo_gc.egg-info/SOURCES.txt` & `tangelo-gc-0.4.0rc0/tangelo_gc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

