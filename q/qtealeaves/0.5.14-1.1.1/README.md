# Comparing `tmp/qtealeaves-0.5.14.tar.gz` & `tmp/qtealeaves-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtealeaves-0.5.14.tar", last modified: Wed Apr 17 12:37:20 2024, max compression
+gzip compressed data, was "qtealeaves-1.1.1.tar", last modified: Fri Apr 19 13:18:46 2024, max compression
```

## Comparing `qtealeaves-0.5.14.tar` & `qtealeaves-1.1.1.tar`

### file list

```diff
@@ -1,88 +1,112 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-0.5.14/README.md
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/pyproject.toml
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/
--rw-r--r--   0 quantum    (128) quantum    (128)     1222 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/convergence_parameters/
--rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    14801 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params_finite_temp.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.019526 qtealeaves-0.5.14/qtealeaves/emulator/
--rw-r--r--   0 quantum    (128) quantum    (128)     1098 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/emulator/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    75181 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/abstract_tn.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7902 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/ed_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    35555 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/lptn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19885 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/emulator/mpi_mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    83620 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    16308 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/state_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)   149524 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/ttn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    45441 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/emulator/tto_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/fortran_interfaces.py
--rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5854 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/lattice_layout.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/modeling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1381 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6102 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/baseterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7597 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/blockterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13591 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/localterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7351 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/plaquetteterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    27889 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/quantummodel.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9928 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2566 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/modeling/sparsematrixproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/stringterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8769 2024-02-26 14:55:43.000000 qtealeaves-0.5.14/qtealeaves/modeling/tensorproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12414 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13003 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10416 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm3d.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/models/
--rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/bosehubbard.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/models/quantumising.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/models/xxzmodel.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/observables/
--rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5892 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/bond_entropy.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13865 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/custom_correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4688 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/distance2pure.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5853 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/local.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7296 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/probabilities.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5172 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/projective.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5098 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/state2file.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5821 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tensor_product.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5595 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/timecorrelator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6348 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tnobase.py
--rw-r--r--   0 quantum    (128) quantum    (128)    18241 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/observables/tnobservables.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7681 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/observables/weighted_sum.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves/operators/
--rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/operators/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2904 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/bosonicoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2622 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/qtealeaves/operators/combinedoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/quditoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1358 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/spinoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8367 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/operators/tnoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2856 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/qtealeaves/parameterized.py
--rw-r--r--   0 quantum    (128) quantum    (128)    60390 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/qtealeaves/simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)      532 2024-04-17 12:35:13.000000 qtealeaves-0.5.14/qtealeaves/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/qtealeaves.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3286 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2608 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-04-17 12:37:20.000000 qtealeaves-0.5.14/qtealeaves.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-04-17 12:37:20.027526 qtealeaves-0.5.14/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     2660 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-17 12:37:20.023526 qtealeaves-0.5.14/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_fortran_interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2739 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)    24306 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-0.5.14/tests/tests_model_terms.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-0.5.14/tests/tests_operators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2785 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_quantum_trajectories.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-0.5.14/tests/tests_rydberg_model.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4429 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5531 2024-01-12 22:24:30.000000 qtealeaves-0.5.14/tests/tests_ttn_simulation.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3285 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-1.1.1/README.md
+-rw-r--r--   0 quantum    (128) quantum    (128)      101 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/pyproject.toml
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.523728 qtealeaves-1.1.1/qtealeaves/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1088 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.523728 qtealeaves-1.1.1/qtealeaves/convergence_parameters/
+-rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20340 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params_finite_temp.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/emulator/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1485 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    89626 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/abstract_tn.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13132 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/attn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9504 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/ed_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    42376 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/lptn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    22059 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/mpi_mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   110894 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19742 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/state_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    39080 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tn_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2535 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tnnode.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   168825 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/ttn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    46305 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tto_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2125 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/unitariesprojmeas.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/modeling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1289 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6956 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/baseterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7625 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/blockterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16787 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/localterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7379 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/plaquetteterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    32850 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/quantummodel.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-1.1.1/qtealeaves/modeling/stringterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13223 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13088 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10657 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm3d.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/models/
+-rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/bosehubbard.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/models/quantumising.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/xxzmodel.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/mpos/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1239 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4018 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/abstracteffop.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15982 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/densempos.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15908 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/disentangler.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    76751 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/indexedtpo.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    23290 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20242 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixproductoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    21798 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/tensorproductoperator.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/observables/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-1.1.1/qtealeaves/observables/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6009 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/bond_entropy.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19724 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/custom_correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4703 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/distance2pure.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5908 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/local.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7874 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/probabilities.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5653 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/projective.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5110 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/state2file.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5834 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tensor_product.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5609 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/timecorrelator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6351 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tnobase.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    18721 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tnobservables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10161 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/weighted_sum.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/operators/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/operators/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2894 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/bosonicoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2622 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/operators/combinedoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/operators/quditoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1368 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/spinoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9216 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/tnoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    68904 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/simulation_setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/solvers/
+-rw-r--r--   0 quantum    (128) quantum    (128)      698 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4067 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/eigen_solver.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7352 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/krylovexp_solver.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/tensors/
+-rw-r--r--   0 quantum    (128) quantum    (128)      801 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17043 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/abstracttensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    75601 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/tensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1663 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/tensor_backend.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/tooling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1179 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/fortran_interfaces.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5883 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4080 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/parameterized.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1768 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/permutations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1785 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/restrictedclasses.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      531 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3285 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     2979 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_fortran_interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2732 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    27539 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_model_terms.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9812 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-1.1.1/tests/tests_operators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2962 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_quantum_trajectories.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/tests/tests_rydberg_model.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4401 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_simulation_setup.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    11537 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_tn_simulation.py
```

### Comparing `qtealeaves-0.5.14/LICENSE` & `qtealeaves-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/PKG-INFO` & `qtealeaves-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 0.5.14
+Version: 1.1.1
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-0.5.14/README.md` & `qtealeaves-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/__init__.py` & `qtealeaves-1.1.1/qtealeaves/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 # that they have been altered from the originals.
 
 """
 init for qtealeaves module.
 """
 from qtealeaves.version import __version__
 
-# parameterized has __all__ definition
-from qtealeaves.parameterized import *
+# tooling
+from qtealeaves.tooling import *
 
-# fortran_interfaces have __all__ definition
-from qtealeaves.fortran_interfaces import *
+# solvers
+from qtealeaves.solvers import *
 
-# hilbert_curvature has __all__ attribute
-from qtealeaves.hilbert_curvature import *
+# Convergence parameters submodule
+from . import convergence_parameters
 
 # Hamiltonian and Lindblad model terms / default models
 from . import modeling
 from . import models
 
+# Operators submodule
+from . import operators
+
+# tensors
+from . import tensors
+
 # Simulators written in python
 from . import emulator
 
 # Observables submodule
 from . import observables
 
 # qtealeaves model and setup have all three __all__ definitions
 from qtealeaves.simulation_setup import *
-
-# Operators submodule
-from . import operators
-
-# Convergence parameters submodule
-from . import convergence_parameters
```

### Comparing `qtealeaves-0.5.14/qtealeaves/convergence_parameters/__init__.py` & `qtealeaves-1.1.1/qtealeaves/convergence_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params.py` & `qtealeaves-1.1.1/qtealeaves/modeling/localterm.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,422 +5,520 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Module defining the convergence parameters for tensor network simulations.
+Local terms in a Hamiltonian or Lindblad equation.
 """
+from copy import deepcopy
+import numpy as np
 
-import os
-from collections import OrderedDict
-from qtealeaves import write_nml, StrBuffer
-from qtealeaves.parameterized import _ParameterizedClass
+from qtealeaves import map_selector
+from .baseterm import _ModelTerm
 
 
-__all__ = ["TNConvergenceParameters"]
+__all__ = ["LocalTerm", "LindbladTerm", "RandomizedLocalTerm"]
 
 
-class TNConvergenceParameters(_ParameterizedClass):
+class LocalTerm(_ModelTerm):
     """
-    Handling of the convergence parameters for the tensor network
-    simulations.
+    Local Hamiltonian terms are versatile and probably part of any model
+    which will be implemented. For example, the external field in the
+    quantum Ising model can be represented as a local term.
 
     **Arguments**
 
-    max_iter : integer, optional
-        Number of sweeps in the ground state search.
-        default to 20
-
-    abs_deviation : float, optional
-        exit criterion for ground state search if the energy of the
-        current sweep has an absolute deviation from the previous
-        data points below this threshold.
-        default to 4e-12
-
-    rel_deviation : float, optional
-        exit criterion for ground state search if the energy of the
-        current sweep has a relative deviation from the previous data
-        points below this threshold.
-        default to 1e-12
-
-    n_points_conv_check : int, optional
-        number of points to check convergence, e.g., for the ground
-        state search. If the value is smaller than the number of sweeps,
-        the exit criteria for the sweeps will never be checked.
-        default to 4
-
-    max_bond_dimension : int, optional
-        The maximal bond dimension used during the simulations.
-        The default value is purely a starting point for testing
-        simulations.
-        default to 5
-
-    data_type : str, optional
-        The data precision used during the simulations. (Not queried for now).
-        Values are automatic ("A"), single ("S"), double ("D"),
-        singe complex ("C"), and double complex ("Z").
-        The default value is "A".
-
-    trunc_method: str, optional
-        Method use to truncate the singular values. Default to "R".
-        Available:
-        - "R": use cut_ratio
-        - "N": use maximum norm
-
-    cut_ratio: float, optional
-        If trunc_method="r":
-            Cut ratio :math:`\\epsilon` after which the singular values are
-            neglected, i.e. if :math:`\\lamda_1` is the bigger singular values
-            then after an SVD we neglect all the singular values such that
-            :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`.
-        If trunc_method="n":
-            Maximum value of the norm neglected for the singular values during
-            the trunctation.
-        Default to 1e-9
-
-    increase_precision
-        TBA
-
-    measure_obs_every_n_iter : int
-        Modulo for measuring statics every n iterations. Not
-        propagated through yet on the fortran side.
-
-    svd_ctrl : character, optional
-        Control for the SVD algorithm, either 'V', 'D', or 'E'
-        Default to 'V'.
-
-    random_sweep : bool
-        Use random sweep scheme instead of default scheme.
-
-    skip_exact_rgtensors : logical, optional
-        Allows to skip space expansion if the tensors has already
-        reached the maximal bond dimension of the underlying
-        local Hilbert spaces, i.e., full Hilbert space is captured
-        without truncation of entanglement. Only applies to
-        sweep with space expansion.
-        Default to False.
-
-    svd_threshold : float
-        TBA (only first accessed if array on fortran side)
-
-    min_expansion : int, optional
-        Bond dimension expansion used in the fortran code for a single
-        site optimization. The bond dimension is increased of this integer.
-        It is also used in the python simulation to increase the
-        bond dimension when doing an expanding QR. In that case,
-        the integer represent the percentage.
-        Default to 10.
-
-    expansion_cycles
-        TBA
-
-    arnoldi_initial_tolerance
-        TBA
-
-    arnoldi_min_tolerance
-        TBA
-
-    arnoldi_max_tolerance
-        TBA
-
-    aggression_tolerance
-        TBA
-
-    aggression_expansion
-        TBA
-
-    statics_method : integer, optional
-        Method to run ground state search for this/all iteration.
-        0 : default (1)
-        1 : sweep
-        2 : sweep with space expansion (can still be reduced to sweep
-            during the simulation based on a energy condition)
-        3 : imaginary time evolution with TDVP single-site
-
-    imag_evo_dt : float, optional
-        Time-step size for the imaginary time evolution.
-        Default to 0.1.
-
-    filename_conv : str, optional
-        The convergence parameters are saved under this filename
-        inside the input folder.
-        default to ``ConvergenceInput.dat``
-
-    trunc_tracking_mode : str, optional
-        Modus for storing truncation, 'M' for maximum, 'C' for
-        cumulated of the singvals squared (Norm truncated) (default).
-
+    operator : str
+        String identifier for the operator. Before launching the simulation,
+        the python API will check that the operator is defined.
+
+    strength : str, callable, numeric (optional)
+        Defines the coupling strength of the local terms. It can
+        be parameterized via a value in the dictionary for the
+        simulation or a function.
+        Default to 1.
+
+    prefactor : numeric, scalar (optional)
+        Scalar prefactor, e.g., in order to take into account signs etc.
+        Default to 1.
+
+    mask : callable or ``None``, optional
+        The true-false-mask allows to apply the local Hamiltonians
+        only to specific sites, i.e., with true values. The function
+        takes the dictionary with the simulation parameters as an
+        argument.
+        Default to ``None`` (all sites have a local term)
+
+    **Attributes**
+
+    map_type : str, optional
+        Selecting the mapping from a n-dimensional system to the
+        1d system required for the TTN simulations.
     """
 
-    def __init__(
-        self,
-        max_iter=20,
-        abs_deviation=4e-12,
-        rel_deviation=1e-12,
-        n_points_conv_check=4,
-        max_bond_dimension=5,
-        trunc_method="R",
-        cut_ratio=1e-9,
-        increase_precision=False,
-        measure_obs_every_n_iter=1,
-        svd_ctrl="V",
-        random_sweep=False,
-        skip_exact_rgtensors=False,
-        svd_threshold=1e-15,
-        min_expansion=20,
-        expansion_cycles=1,
-        arnoldi_initial_tolerance=1e-2,
-        arnoldi_min_tolerance=0.0,
-        arnoldi_max_tolerance=1e-2,
-        aggression_tolerance=1.0,
-        aggression_expansion=1.0,
-        statics_method=2,
-        imag_evo_dt=0.1,
-        filename_conv="ConvergenceInput.dat",
-        trunc_tracking_mode="C",
-        data_type="A",
-    ):
-        self.filename_conv = filename_conv
+    def __init__(self, operator, strength=1, prefactor=1, mask=None):
+        super().__init__()
+
+        self.operator = operator
+        self.strength = strength
+        self.prefactor = prefactor
+        self.mask = mask
 
-        # Convergence parameters for statics / decision on convergence
-        self.max_iter = max_iter
-        self.abs_deviation = abs_deviation
-        self.rel_deviation = rel_deviation
-        self.n_points_conv_check = n_points_conv_check
-        self.measure_obs_every_n_iter = measure_obs_every_n_iter
-        self.svd_ctrl = svd_ctrl
-
-        # Consumed in python
-        self.trunc_method = trunc_method.upper()
-        self.cut_ratio = cut_ratio
-        self.trunc_tracking_mode = trunc_tracking_mode.upper()
-
-        # Settings for one or all iterations
-        self.sim_params = {}
-        self.sim_params["max_bond_dimension"] = max_bond_dimension
-        self.sim_params["increase_precision"] = increase_precision
-        self.sim_params["random_sweep"] = random_sweep
-        self.sim_params["skip_exact_rgtensors"] = skip_exact_rgtensors
-        self.sim_params["svd_threshold"] = svd_threshold
-        self.sim_params["min_expansion"] = min_expansion
-        self.sim_params["expansion_cycles"] = expansion_cycles
-        self.sim_params["arnoldi_initial_tolerance"] = arnoldi_initial_tolerance
-        self.sim_params["arnoldi_min_tolerance"] = arnoldi_min_tolerance
-        self.sim_params["arnoldi_max_tolerance"] = arnoldi_max_tolerance
-        self.sim_params["aggression_tolerance"] = aggression_tolerance
-        self.sim_params["aggression_expansion"] = aggression_expansion
-        self.sim_params["statics_method"] = statics_method
-        self.sim_params["imag_evo_dt"] = imag_evo_dt
-        self.sim_params["data_type"] = data_type
-
-    def prepare_parameters_for_iteration(self, params):
-        """
-        Preparation to write parameters for each iteration. It checks
-        if a list of convergence settings has to be written and builds
-        a dictionary with the resolved entries for each parameters,
-        which is either a the value or a list of values.
+        # Will be set when adding Hamiltonian terms
+        self.map_type = None
+
+    def count(self, params):
+        """
+        Defines length as number of terms in fortran input file,
+        which by now depends the presence of a mask.
 
         **Arguments**
 
-        params : dict
-            Dictionary with the simulation parameters.
+        params : dictionary
+            Contains the simulation parameters.
+        """
+        if self.mask is None:
+            return 1
 
-        **Results**
+        return np.sum(self.mask(params))
 
-        has_vector_of_settings : bool
-            True if settings change over the iterations and
-            the parameters have to be written for each iteration.
-
-        sim_param_all : dict
-            Contains the resolved convergence parameters, i.e.,
-            strings and functions are resolved with the actual values.
-        """
-        max_iter = self.eval_numeric_param(self.max_iter, params)
-
-        sim_params_all = {}
-        has_vector_of_settings = False
-
-        str_params = ["data_type"]
-
-        for key, value in self.sim_params.items():
-            if isinstance(value, str):
-                # Have to catch strings first as they have a length
-                # attribute
-                if key in str_params:
-                    # String parameters
-                    entry = self.eval_str_param(value, params)
-                else:
-                    # Numeric parameters
-                    entry = self.eval_numeric_param(value, params)
-            elif hasattr(value, "__len__"):
-                # List of any kind
-                if key in str_params:
-                    # String parameters
-                    entry = [
-                        self.eval_str_param(value[ii], params)
-                        for ii in range(len(value))
-                    ]
-                else:
-                    # Numeric parameters
-                    entry = [
-                        self.eval_numeric_param(value[ii], params)
-                        for ii in range(len(value))
-                    ]
-            else:
-                # Scalar values (cannot be a str parameter, which
-                # would go into the first if)
-                entry = self.eval_numeric_param(value, params)
-
-            if isinstance(entry, str):
-                # String never activates list
-                pass
-            elif hasattr(entry, "__len__"):
-                has_vector_of_settings = True
-                if len(entry) != max_iter:
-                    raise Exception(
-                        "Length of convergence parameter list for "
-                        + "%s must match " % (key)
-                        + "max_iter=%d." % (max_iter)
-                    )
+    def get_entries(self, params):
+        """
+        Return the operator and the strength of this term.
 
-            sim_params_all[key] = entry
+        **Arguments**
 
-        return has_vector_of_settings, sim_params_all
+        params : dictionary
+            Contains the simulation parameters.
+        """
+        strength = self.eval_strength(params)
 
-    @property
-    def max_bond_dimension(self):
+        return self.operator, strength
+
+    def collect_operators(self):
+        """
+        The required operators must be provided through this
+        method; thus, we return the operator in the local term.
         """
-        Provide the getter method for this property important to
-        the MPS emulator. It allows to get values without a
-        dictionary, but prevents doing it if the values is not
-        an integer.
+        yield self.operator, None
+
+    def get_fortran_str(self, ll, params, operator_map, param_map, dim):
         """
-        value = self.sim_params["max_bond_dimension"]
-        if hasattr(value, "__len__"):
-            value = value[0]
+        Get the string representation needed to write the
+        local terms as an plocal_type for Fortran.
 
-        if isinstance(value, int):
-            return value
+        **Arguments**
 
-        raise Exception("Try to use getter on non-int bond dimension.")
+        ll : int
+            Number of sites along the dimensions, i.e., not the
+            total number of sites. Assuming list of sites
+            along all dimension.
+
+        params : dictionary
+            Contains the simulation parameters.
+
+        operator_map : OrderedDict
+            For operator string as dictionary keys, it returns the
+            corresponding integer IDs.
+
+        param_map : dict
+            This dictionary contains the mapping from the parameters
+            to integer identifiers.
+
+        dim : int
+            Dimensionality of the problem, e.g., a 2d system.
+        """
+        str_repr = ""
+        op_id_str = str(operator_map[(self.operator, None)])
+
+        has_spatial_dependency = False
+        param_repr = self.get_param_repr(param_map)
+
+        if self.mask is not None:
+            for _, idx in self.get_interactions(ll, params, dim=dim):
+                # Convert from python index to fortran index by
+                # adding offset 1
+                str_repr += "%d\n" % (idx[0] + 1)
+                str_repr += op_id_str + "\n"
+                str_repr += param_repr
+                str_repr += "%30.15E\n" % (self.prefactor)
+
+        elif has_spatial_dependency:
+            # Write for each site
+            raise NotImplementedError("To-do ...")
+        else:
+            str_repr += "-1\n"
+            str_repr += op_id_str + "\n"
+            str_repr += param_repr
+            str_repr += "%30.15E\n" % (self.prefactor)
+
+        return str_repr
+
+    def get_interactions(self, ll, params, **kwargs):
+        """
+        Iterator returning the local terms one-by-one, e.g., to build
+        a Hamiltonian matrix. (In that sense, the "interaction" is
+        obviously misleading here.)
 
-    @property
-    def data_type(self):
+        **Arguments**
+
+        ll : int
+            Number of sites along the dimension, i.e., not the
+            total number of sites. Assuming list of sites
+            along all dimension.
+
+        params : dictionary
+            Contains the simulation parameters.
+
+        dim : int (as keyword argument!)
+            Dimensionality of the problem, e.g., a 2d system.
         """
-        Provide the getter method for this property important to
-        the MPS emulator. It allows to get values without a
-        dictionary, but prevents doing it if the values is not
-        an integer. (Not queried from the MPS for now).
-        """
-        value = self.sim_params["data_type"]
-        if isinstance(value, str):
-            # Value is string itself, return first
-            return value
+        if "dim" not in kwargs:
+            raise Exception("Local terms needs dim information")
+        dim = kwargs["dim"]
 
-        if hasattr(value, "__len__"):
-            value = value[0]
+        elem = {"coordinates": None, "operators": [self.operator]}
 
-        raise Exception("Try to use getter on non-str data type.")
+        if self.mask is None:
 
-    @property
-    def min_expansion_qr(self):
+            def check_mask(*args):
+                return True
+
+        else:
+            local_mask = self.mask(params)
+            if len(local_mask.shape) != dim:
+                raise Exception("Mask dimension does not match system dimension.")
+
+            def check_mask(*args, local_mask=local_mask):
+                if len(args) == 1:
+                    return local_mask[args[0]]
+                if len(args) == 2:
+                    return local_mask[args[0], args[1]]
+                if len(args) == 3:
+                    return local_mask[args[0], args[1], args[2]]
+
+                raise Exception("Unknown length of *args.")
+
+        if dim > 1:
+            map_to_1d = map_selector(dim, ll, self.map_type)
+
+        if dim == 1:
+            for ii in range(ll[0]):
+                if not check_mask(ii):
+                    continue
+
+                elem_ii = deepcopy(elem)
+                elem_ii["coordinates_nd"] = (ii,)
+
+                yield elem_ii, [ii]
+        elif dim == 2:
+            idx = 0
+            for ii in range(ll[0]):
+                for jj in range(ll[1]):
+                    idx += 1
+
+                    if not check_mask(ii, jj):
+                        continue
+
+                    elem_ii = deepcopy(elem)
+                    elem_ii["coordinates_nd"] = (ii, jj)
+
+                    yield elem_ii, [map_to_1d[(ii, jj)]]
+        elif dim == 3:
+            idx = 0
+            for ii in range(ll[0]):
+                for jj in range(ll[1]):
+                    for kk in range(ll[2]):
+                        idx += 1
+
+                        if not check_mask(ii, jj, kk):
+                            continue
+
+                        elem_ii = deepcopy(elem)
+                        elem_ii["coordinates_nd"] = (ii, jj, kk)
+
+                        yield elem_ii, [map_to_1d[(ii, jj, kk)]]
+        else:
+            raise Exception("Dimension unknown.")
+
+        return
+
+    def get_sparse_matrix_operators(
+        self, ll, params, operator_map, param_map, sp_ops_cls, **kwargs
+    ):
         """
-        Provide the getter method for this property important to
-        the python emulator. It is the percentage of the bond dimension
-        increase in the qr
+        Construct the sparse matrix operator for this term.
+
+        **Arguments**
+
+        ll : int
+            System size.
+
+        params : dictionary
+            Contains the simulation parameters.
+
+        operator_map : OrderedDict
+            For operator string as dictionary keys, it returns the
+            corresponding integer IDs.
+
+        param_map : dict
+            This dictionary contains the mapping from the parameters
+            to integer identifiers.
+
+        sp_ops_cls : callable (e.g., constructor)
+            Constructor for the sparse MPO operator to be built
+            Has input bool (is_first_site), bool (is_last_site),
+            bool (do_vectors).
+
+        kwargs : keyword arguments
+            Keyword arguments are passed to `get_interactions`
         """
-        value = self.sim_params["min_expansion"]
-        if hasattr(value, "__len__"):
-            value = value[0]
+        op_id = operator_map[(self.operator, None)]
+        param_id = self.get_param_repr(param_map)
+
+        sp_mat_ops = []
+        for ii in range(np.prod(ll)):
+            sp_mat_ops.append(sp_ops_cls(ii == 0, ii + 1 == np.prod(ll), True))
+
+        for _, inds in self.get_interactions(ll, params, **kwargs):
+            sp_mat_ops[inds[0]].add_local(op_id, param_id, self.prefactor, self.is_oqs)
+
+        return sp_mat_ops
+
 
-        if isinstance(value, int):
-            return value / 100
+class LindbladTerm(LocalTerm):
+    """
+    Local Lindblad operators acting at one site are defined via this
+    term. For the arguments see See :class:`LocalTerm.check_dim`.
+
+    **Details**
+
+    The Lindblad equation is implemented as
 
-        raise Exception("Try to use getter on non-valid min_expansion")
+    .. math::
+
+        \\frac{d}{dt} \\rho = -i [H, \\rho]
+           + \\sum \\gamma (L \\rho L^{\\dagger}
+           - \\frac{1}{2} \\{ L^{\\dagger} L, \\rho \\})
+
+    """
 
-    def get_chi(self, params):
+    @property
+    def is_oqs(self):
+        """Status flag if term belongs to Hamiltonian or is Lindblad."""
+        return True
+
+    def quantum_jump_weight(self, state, operators, quench, time, params):
         """
-        Shortcut to evaluate the bond dimension as numeric parameter.
+        Evaluate the unnormalized weight for a jump with this Lindblad term.
 
         **Arguments**
 
-        params : dict
-            The parameter dictionary for the simulation.
+        state : :class:`_AbstractTN`
+            Current quantum state where jump should be applied.
+
+        operators : :class:`TNOperators`
+            Operator dictionary of the simulation.
+
+        quench : :class:`DynamicsQuench`
+            Current quench to evaluate time-dependent couplings.
+
+        time : float
+            Time of the time evolution (accumulated dt)
+
+        params :  dict
+            Dictionary with parameters, e.g., to extract parameters which
+            are not in quench or to build mask.
         """
-        return self.eval_numeric_param(self.sim_params["max_bond_dimension"], params)
+        if self.mask is None:
+            mask = np.ones(state.num_sites, dtype=bool)
+        else:
+            mask = self.mask(params)
+
+        mask = mask.astype(int).astype(np.float64)
+
+        if self.strength in quench:
+            strength = quench[self.strength](time)
+        else:
+            strength = self.eval_numeric_param(self.strength, params)
+
+        total_scaling = strength * self.prefactor
+        lindblad = operators[self.operator]
+        operator = lindblad.conj().tensordot(lindblad, ([0, 1, 3], [0, 1, 3]))
+        meas_vec = state.meas_local(operator)
 
-    def write_input(self, folder_name, params):
+        return np.sum(meas_vec * mask) * total_scaling
+
+    def quantum_jump_apply(self, state, operators, params, rand_generator):
         """
-        Write convergence parameters for input version 2 and 3.
+        Apply jump with this Lindblad. Contains inplace update of state.
 
         **Arguments**
 
-        folder_name : str
-            Name of the input folder, where the file with the convergence
-            parameters is written to.
+        state : :class:`_AbstractTN`
+            Current quantum state where jump should be applied.
+
+        operators : :class:`TNOperators`
+            Operator dictionary of the simulation.
 
-        params : dict
-            Dictionary with the simulation parameters.
+        params :  dict
+            Dictionary with parameters, e.g., to extract parameters which
+            are not in quench or to build mask.
+
+        rand_generator : random number generator
+            Needs method `random()`, used to decide on jump within
+            the sites.
         """
-        # First build a dictionary which allows listed entries
-        has_vector_of_settings, sim_params_all = self.prepare_parameters_for_iteration(
-            params
-        )
+        if self.mask is None:
+            mask = np.ones(state.num_sites, dtype=bool)
+        else:
+            mask = self.mask(params)
 
-        filename_conv = self.eval_str_param(self.filename_conv, params)
+        mask = mask.astype(int).astype(np.float64)
 
-        full_nml = os.path.join(folder_name, filename_conv)
-        if not full_nml.endswith(".nml"):
-            full_nml += ".nml"
+        lindblad = operators[self.operator]
+        operator = lindblad.conj().tensordot(lindblad, ([0, 1, 3], [0, 1, 3]))
+        meas_vec = state.meas_local(operator)
 
-        conv_params = OrderedDict()
-        conv_params["num_cpoints"] = self.eval_numeric_param(
-            self.n_points_conv_check, params
-        )
+        meas_vec = meas_vec * mask
+        meas_vec = np.cumsum(meas_vec)
+        meas_vec /= meas_vec[-1]
 
-        conv_params["max_iterations"] = self.eval_numeric_param(self.max_iter, params)
+        rand = rand_generator.random()
 
-        conv_params["abs_dev"] = self.eval_numeric_param(self.abs_deviation, params)
+        idx = meas_vec.shape[0] - 1
+        for ii in range(idx):
+            if rand < meas_vec[ii]:
+                idx = ii
+                break
 
-        conv_params["rel_dev"] = self.eval_numeric_param(self.rel_deviation, params)
+        if lindblad.ndim == 4:
+            if lindblad.shape[0] == 1 and lindblad.shape[3] == 1:
+                lindblad = lindblad.remove_dummy_link(3).remove_dummy_link(0)
+            else:
+                raise Exception("Cannot remove-non dummy links.")
+        elif lindblad.ndim != 2:
+            raise Exception("Operator neither rank-2 nor rank-4.")
 
-        conv_params["has_vector_of_settings"] = has_vector_of_settings
+        state.site_canonize(idx)
+        state.apply_one_site_operator(lindblad, idx)
+        state.normalize()
 
-        conv_params["measure_obs_every_n_iter"] = self.eval_numeric_param(
-            self.measure_obs_every_n_iter, params
-        )
 
-        if self.svd_ctrl in ["S", "V", "D"]:
-            # Single characters are vulnerable to having some Hamiltonian
-            # parameter named V etc
-            conv_params["svd_ctrl"] = self.svd_ctrl
-        else:
-            conv_params["svd_ctrl"] = self.eval_str_param(self.svd_ctrl, params)
+class RandomizedLocalTerm(LocalTerm):
+    """
+    Randomized local Hamiltonian terms are useful to model spinglass systems
+    where the coupling of the local term is different for each site.
 
-        file_content = StrBuffer()
-        write_nml("CONV_VARS", conv_params, file_content)
+    **Arguments**
 
-        # Require maximum(1, ...) for skipping statics
-        for ii in range(max(1, conv_params["max_iterations"])):
-            sim_params_ii = OrderedDict()
+    operator : string
+        String identifier for the operators. Before launching the simulation,
+        the python API will check that the operator is defined.
+
+    coupling_entries : numpy ndarray of rank-1,2,3
+        The coupling for the different sites.
+        These values can only be set once and cannot
+        be time-dependent in a time-evolution. The rank depends
+        on the usage in 1d, 2d, or 3d systems.
+
+    strength : str, callable, numeric (optional)
+        Defines the coupling strength of the local terms. It can
+        be parameterized via a value in the dictionary for the
+        simulation or a function.
+        Default to 1.
+
+    prefactor : numeric, scalar (optional)
+        Scalar prefactor, e.g., in order to take into account signs etc.
+        Default to 1.
+    """
 
-            for key in self.sim_params:
-                entry = sim_params_all[key]
+    mask = None
 
-                if isinstance(entry, str):
-                    sim_params_ii[key] = entry
-                elif hasattr(entry, "__len__"):
-                    sim_params_ii[key] = entry[ii]
-                else:
-                    sim_params_ii[key] = entry
+    def __init__(self, operator, coupling_entries, strength=1, prefactor=1):
+        super().__init__(operator=operator, strength=strength, prefactor=prefactor)
+        self.coupling_entries = coupling_entries
 
-            write_nml("SIM_PARAMS", sim_params_ii, file_content)
+    def count(self, params):
+        """
+        Defines length as number of terms in fortran input file,
+        which by now depends the presence of the coupling entries.
 
-            if not has_vector_of_settings:
-                break
+        **Arguments**
+
+        params : dictionary
+            Contains the simulation parameters.
+        """
+        ctens = self.eval_numeric_param(self.coupling_entries, params)
+        return np.sum(np.abs(ctens) != 0)
+
+    def get_interactions(self, ll, params, **kwargs):
+        """
+        See :class:`LocalTerm`
+        """
+        ctens = self.eval_numeric_param(self.coupling_entries, params)
+
+        for elem, coords_1d in super().get_interactions(ll, params, **kwargs):
+            elem["weight"] = ctens[elem["coordinates_nd"]]
+
+            if elem["weight"] == 0.0:
+                continue
+
+            yield elem, coords_1d
+
+    def get_fortran_str(self, ll, params, operator_map, param_map, dim):
+        """
+        Get the string representation needed to write the
+        local terms as an plocal_type for Fortran.
+
+        **Arguments**
+
+        ll : int
+            Number of sites along one dimension, i.e., not the
+            total number of sites. Assuming equal number of sites
+            along all dimension.
+
+        params : dictionary
+            Contains the simulation parameters.
+
+        operator_map : OrderedDict
+            For operator string as dictionary keys, it returns the
+            corresponding integer IDs.
+
+        param_map : dict
+            This dictionary contains the mapping from the parameters
+            to integer identifiers.
+
+        dim : int
+            Dimensionality of the problem, e.g., a 2d system.
+        """
+        str_repr = ""
+        op_id_str = str(operator_map[(self.operator, None)])
+
+        param_repr = self.get_param_repr(param_map)
+
+        ctens = self.eval_numeric_param(self.coupling_entries, params)
+        if isinstance(ctens, np.ndarray):
+            if len(ctens.shape) != dim:
+                raise Exception(
+                    "Coupling %d and " % (len(ctens.shape))
+                    + "dimensionality %d do not match." % (dim)
+                )
+        else:
+            raise Exception("Unknown type for coupling.")
 
-        with open(full_nml, "w+") as fh:
-            fh.write(file_content())
+        for meta_info, idx in self.get_interactions(ll, params, dim=dim):
+            if abs(ctens[meta_info["coordinates_nd"]]) == 0.0:
+                # Skip entries with 0 coupling from randomization
+                continue
+
+            # Convert from python index to fortran index by
+            # adding offset 1
+            str_repr += "%d\n" % (idx[0] + 1)
+            str_repr += op_id_str + "\n"
+            str_repr += param_repr
+            prefactor = self.prefactor * ctens[meta_info["coordinates_nd"]]
+            str_repr += "%30.15E\n" % (prefactor)
 
-        return full_nml
+        return str_repr
```

### Comparing `qtealeaves-0.5.14/qtealeaves/convergence_parameters/conv_params_finite_temp.py` & `qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params_finite_temp.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/abstract_tn.py` & `qtealeaves-1.1.1/qtealeaves/emulator/abstract_tn.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,50 +8,37 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 The module contains an abstract tensor network, from which other tensor
 networks can be derived.
 """
-import warnings
+
+import abc
+import json
+import pickle
+import os
+from time import time as tictoc
+from warnings import warn
 from copy import deepcopy
 import numpy as np
-import scipy as sp
-import scipy.sparse.linalg as ssla
 import mpmath as mp
 
-# Try to import cupy
-try:
-    import cupy as cp
-    import cupyx.scipy.sparse.linalg as csla
-    from cupy_backends.cuda.api.runtime import CUDARuntimeError
-
-    try:
-        _ = cp.cuda.Device()
-        GPU_AVAILABLE = True
-    except CUDARuntimeError:
-        GPU_AVAILABLE = False
-except ImportError:
-    cp = None
-    GPU_AVAILABLE = False
-
 # try to import mpi4py
 try:
     from mpi4py import MPI
 except ImportError:
     MPI = None
 
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from qtealeaves.modeling import IndexedOperator
+from qtealeaves.tensors import TensorBackend
 
 __all__ = [
     "_AbstractTN",
     "postprocess_statedict",
-    "UnitarySetupProjMeas",
-    "TNnode",
     "MPI",
     "TN_MPI_TYPES",
 ]
 
 
 # pickle in deepcopy fails if stored within the TN type
 if MPI is not None:
@@ -62,306 +49,367 @@
         "<f8": MPI.DOUBLE_PRECISION,
         "<i8": MPI.INT,
     }
 else:
     TN_MPI_TYPES = {}
 
 
-class TNnode:
-    """
-    Class to encode a node in a tensor network, to work
-    with arbitrary tensor network.
-
-    Parameters
-    ----------
-    layer: int
-        Layer of the network where the node lives
-    index: int
-        Index of the tensor inside the layer
-    children: list of TNnode
-        Children nodes
-    link_idx: int
-        Number for the new index for the links
-    """
-
-    def __init__(self, layer, index, children, link_idx):
-        self.layer = layer
-        self.index = index
-
-        if children is not None:
-            self.link_idxs = []
-            for child in children:
-                child.add_parent(self)
-                self.link_idxs.append(child.link_idxs[-1])
-            self.link_idxs.append(link_idx)
-        else:
-            self.link_idxs = [link_idx + ii for ii in range(3)]
-        self.children = children
-        # By default, the parent is None and should be added with
-        # the appropriate method
-        self.parent = None
-
-    def __repr__(self) -> str:
-        return f"({self.layer}, {self.index})"
-
-    def is_child(self, parent_node):
-        """
-        Check if the class is the child of `parent_node`
-
-        Parameters
-        ----------
-        parent_node : TNnode
-            Potential parent node
-
-        Returns
-        -------
-        bool
-            True if `parent_node` is the parent
-        """
-        return parent_node == self.parent
-
-    def is_parent(self, child_node):
-        """
-        Check if the class is the parent of `child_node`
-
-        Parameters
-        ----------
-        child_node : TNnode
-            Potential child node
-
-        Returns
-        -------
-        bool
-            True if `child_node` is the child
-        """
-        return child_node in self.children
-
-    def add_parent(self, parent):
-        """
-        Add the node `parent` as parent node of the class
-
-        Parameters
-        ----------
-        parent : TNnode
-            New parent node
-        """
-        self.parent = parent
-
-
-class UnitarySetupProjMeas:
-    """
-    Setup for applying unitaries prior to a projective measurement
-    via `meas_projective`.
-
-    Parameters
-    ----------
-
-    unitaries : list of xp.ndarrays of rank-2
-        List of unitaries, which will be applied to the local
-        Hilbert space according to the mode.
-    mode : char
-        Mode `R`, we draw randomly unitaries from the list
-        and apply them before the projective measurement.
-        Mode `S` select the unitary at the corresponding site,
-        i.e., the i-th site applies always the i-th unitary.
-    """
-
-    def __init__(self, unitaries, mode="R"):
-        self.unitaries = unitaries
-        self.mode = mode
-
-        if mode not in ["R", "S"]:
-            raise ValueError("Unknown mode for UnitarySetupProjMeas.")
-
-    def get_unitary(self, site_idx):
-        """
-        Retrieve the unitary for a site.
-
-        Parameters
-        ----------
-        site_idx : int
-            Get unitary for this site. Although it has to be passed always,
-            it is only evaluated in `mode=S`.
-
-        Returns
-        -------
-        unitary : np.ndarray of rank-2
-            Tensor to be applied as local unitary to the site.
-        """
-        if self.mode == "R":
-            idx = np.random.randint(len(self.unitaries))
-            return self.unitaries[idx]
-        else:
-            if site_idx >= len(self.unitaries):
-                raise Exception("List of provided unitaries not long enough.")
-
-            return self.unitaries[site_idx]
-
-
-class _AbstractTN:
+class _AbstractTN(abc.ABC):
     """
     Abstract tensor network class with methods applicable to any
     tensor network.
 
     Parameters
     ----------
 
     num_sites: int
         Number of sites
 
-    local_dim: int, optional
-        Local dimension of the degrees of freedom. Default to 2.
-
     convergence_parameters: :py:class:`TNConvergenceParameters`
         Class for handling convergence parameters. In particular,
         in the python TN simulator, we are interested in:
         - the *maximum bond dimension* :math:`\\chi`;
         - the *cut ratio* :math:`\\epsilon` after which the singular
             values are neglected, i.e. if :math:`\\lamda_1` is the
             bigger singular values then after an SVD we neglect all the
             singular values such that
             :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`
-    device: string, optional
-        Device where to create the MPS. Default to 'cpu'.
-        Implemented devices:
-        - 'cpu'
-        - 'gpu'
-    dtype: np.dtype, optional
-        Type of the tensors in the TN. By default `np.complex128`
+
+    local_dim: int, optional
+        Local dimension of the degrees of freedom. Default to 2.
+
+    requires_singvals : boolean, optional
+        Allows to enforce SVD to have singular values on each link available
+        which might be useful for measurements, e.g., bond entropy (the
+        alternative is traversing the whole TN again to get the bond entropy
+        on each link with an SVD).
+
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
     """
 
-    implemented_devices = ("cpu", "gpu")
+    extension = "tn"
+    has_de = False
 
     def __init__(
         self,
         num_sites,
         convergence_parameters,
         local_dim=2,
-        device="cpu",
-        dtype=np.complex128,
+        requires_singvals=False,
+        tensor_backend=None,
     ):
-        if isinstance(convergence_parameters, TNConvergenceParameters):
-            max_bond_dim = convergence_parameters.max_bond_dimension
-            cut_ratio = convergence_parameters.cut_ratio
-        else:
+        # Class attributes by arguments
+        self._num_sites = num_sites
+        self._local_dim = (
+            [local_dim] * num_sites if np.isscalar(local_dim) else local_dim
+        )
+        self._convergence_parameters = convergence_parameters
+        self._tensor_backend = (
+            TensorBackend() if tensor_backend is None else tensor_backend
+        )
+
+        # Other class attributes
+        self._iso_center = None
+        self.eff_op = None
+
+        # internal storage for last energy measurement for algorithms whic
+        # need an estimate where it is sufficient to rely that this number
+        # is not too outdated
+        self._prev_energy = None
+
+        # Selection of QR vs SVD
+        self._requires_singvals = requires_singvals
+        # store solver to be used
+        self._solver = None
+
+        # log file for a simulation
+        self._log_file = None
+        self._log_verbosity = 0
+
+        # Attributes for MPI
+        self.comm = None
+
+        # Run checks on input
+        # -------------------
+
+        if not isinstance(convergence_parameters, TNConvergenceParameters):
             raise TypeError(
                 "convergence parameters must be " + "TNConvergenceParameters class"
             )
 
-        if max_bond_dim < 1:
+        if not isinstance(self._tensor_backend, TensorBackend):
+            raise TypeError(
+                f"Passed wrong type {type(self._tensor_backend)} to backend."
+            )
+
+        if self._convergence_parameters.max_bond_dimension < 1:
             raise ValueError("The minimum bond dimension for a product state is 1")
 
-        if cut_ratio <= 0:
+        if self._convergence_parameters.cut_ratio <= 0:
             raise ValueError("The cut_ratio value must be positive")
 
-        self._num_sites = num_sites
-        self._local_dim = local_dim
-        self.dtype = dtype
+        if len(self.local_dim) != num_sites:
+            raise ValueError(
+                f"Length of local_dim {len(local_dim)} differs "
+                + f"from num_sites {num_sites}."
+            )
 
-        self._convergence_parameters = convergence_parameters
-        self._max_bond_dim = max_bond_dim
-        self._cut_ratio = cut_ratio
-        self._device = device
-        self._iso_center = None
-        self.eff_op = None
-        self.comm = None
+        if np.min(self.local_dim) < 2:
+            raise ValueError("Local dimension cannot be smaller than 2.")
+
+        # internal variable for flex-TDVP
+        self._timestep_mode_5_counter = 0
 
+        # MPI initialization
         self._initialize_mpi()
 
-    def __repr__(self):
+    # --------------------------------------------------------------------------
+    #                               Properties
+    # --------------------------------------------------------------------------
+
+    @property
+    def convergence_parameters(self):
+        """Get the convergence settings from the TN."""
+        return self._convergence_parameters
+
+    @convergence_parameters.setter
+    def convergence_parameters(self, value):
         """
-        Return the class name as representation.
+        Set the convergence settings from the TN. (no immediate effect, only
+        in next steps).
         """
-        return self.__class__.__name__
+        self._convergence_parameters = value
 
-    def __len__(self):
+    @property
+    @abc.abstractmethod
+    def default_iso_pos(self):
         """
-        Provide number of sites in the TN.
+        Returns default isometry center position, e.g., for initialziation
+        of effective operators.
         """
-        return self.num_sites
 
     @property
-    def cut_ratio(self):
-        """Cut ratio for truncation of singular values"""
-        return self._convergence_parameters.cut_ratio
+    def device(self):
+        """Device where the tensor is stored."""
+        for tensor in self._iter_tensors():
+            return tensor.device
+
+        return None
+
+    @property
+    def dtype(self):
+        """Data type of the underlying arrays."""
+        for tensor in self._iter_tensors():
+            return tensor.dtype
+
+        return None
+
+    @property
+    def dtype_eps(self):
+        """Data type's machine precision of the underlying arrays."""
+        for tensor in self._iter_tensors():
+            return tensor.dtype_eps
+
+        return None
+
+    @property
+    def iso_center(self):
+        """Isometry center of the tensor network"""
+        return self._iso_center
+
+    @iso_center.setter
+    def iso_center(self, value):
+        """Change the value of the iso center"""
+        self._iso_center = value
+
+    @property
+    def has_symmetry(self):
+        """Check if TN is built out of symmetric tensors."""
+        for tensor in self._iter_tensors():
+            return tensor.has_symmetry
+
+        return None
+
+    @property
+    def log_file(self):
+        """Return the open filehandle for the log file or `None` if not open."""
+        return self._log_file
 
     @property
     def num_sites(self):
         """Number of sites property"""
         return self._num_sites
 
     @property
     def local_dim(self):
         """Local dimension property"""
-        return self._local_dim
+        if isinstance(self._local_dim, int):
+            return self._local_dim
+        elif isinstance(self._local_dim, np.ndarray):
+            return self._local_dim
+        elif isinstance(self._local_dim[0], int):
+            return self._local_dim
+        else:
+            # Case for symmetries
+            return [elem.shape for elem in self._local_dim]
 
     @property
-    def device(self):
-        """Device where the Tensor network is stored"""
-        return self._device
+    def local_links(self):
+        """Return information on local link (for symmetries more than integer)."""
+        return self._local_dim
 
     @property
-    def max_bond_dim(self):
-        """Maximum bond dimension property"""
-        return self._convergence_parameters.max_bond_dimension
+    def solver(self):
+        """Return current solver for the TN."""
+        return self._solver
+
+    @solver.setter
+    def solver(self, value):
+        """Set the solver, e.g., currently used for exp(-i H dt) |psi>."""
+        self._solver = value
+
+    # --------------------------------------------------------------------------
+    #                          Overwritten operators
+    # --------------------------------------------------------------------------
 
-    def get_tensor_of_site(self, idx):
+    def __repr__(self):
         """
-        Generic function to retrieve the tensor for a specific site. Compatible
-        across different tensor network geometries.
+        Return the class name as representation.
+        """
+        return self.__class__.__name__
 
-        Parameters
-        ----------
-        idx : int
-            Return tensor containin the link of the local
-            Hilbert space of the idx-th site.
+    def __len__(self):
         """
-        raise NotImplementedError("This function has to be overwritten.")
+        Provide number of sites in the TN.
+        """
+        return self.num_sites
 
-    def norm(self):
+    # --------------------------------------------------------------------------
+    #                       classmethod, classmethod like
+    # --------------------------------------------------------------------------
+
+    @classmethod
+    @abc.abstractmethod
+    def from_statevector(
+        cls, statevector, local_dim=2, conv_params=None, tensor_backend=None
+    ):
+        """Decompose statevector to tensor network."""
+
+    @classmethod
+    def read_pickle(cls, filename):
+        """Read via pickle-module."""
+        ext = "pkl" + cls.extension
+        if not filename.endswith(ext):
+            raise Exception(
+                f"Filename {filename} not valid, extension should be {ext}."
+            )
+
+        with open(filename, "rb") as fh:
+            obj = pickle.load(fh)
+
+        if not isinstance(obj, cls):
+            raise TypeError(
+                f"Loading wrong tensor network ansatz: {type(obj)} vs {cls}."
+            )
+
+        return obj
+
+    @abc.abstractmethod
+    def to_dense(self, true_copy=False):
+        """Convert into a TN with dense tensors (without symmetries)."""
+
+    def copy(self, dtype=None, device=None):
         """
-        Calculate the norm of the state.
+        Make a copy of a TN.
+
+        **Details**
+
+        The following attributes have a special treatment and are not present
+        in the copied object.
+
+        * convergence_parameters
+        * log file (filehandle)
+        * MPI communicator
+
         """
-        raise NotImplementedError("This function has to be overwritten.")
+        # Store attributes which cannot be pickled, so also potential problems
+        # with deepcopy
+        storage = self._store_attr_for_pickle()
+        obj = deepcopy(self)
+        self._restore_attr_for_pickle(storage)
 
-    def normalize(self):
+        obj.convert(dtype, device)
+        return obj
+
+    @classmethod
+    @abc.abstractmethod
+    def read(cls, filename, tensor_backend, cmplx=True, order="F"):
+        """Read a TN from a formatted file."""
+
+    # --------------------------------------------------------------------------
+    #                            Checks and asserts
+    # --------------------------------------------------------------------------
+
+    # --------------------------------------------------------------------------
+    #                     Abstract methods to be implemented
+    # --------------------------------------------------------------------------
+
+    @abc.abstractmethod
+    def build_effective_operators(self, measurement_mode=False):
         """
-        Normalize the state depending on its current norm.
+        Build the complete effective operator on each
+        of the links. Now assumes `self.eff_op` is set.
         """
-        factor = 1.0 / self.norm()
-        self.scale(factor)
 
-    def site_canonize(self, idx, keep_singvals=False):
+    @abc.abstractmethod
+    def _convert_singvals(self, dtype, device):
+        """Convert the singular values of the tensor network to dtype/device."""
+
+    @abc.abstractmethod
+    def get_bipartition_link(self, pos_src, pos_dst):
+        """
+        Returns two sets of sites forming the bipartition of the system for
+        a loopless tensor network. The link is specified via two positions
+        in the tensor network.
         """
-        Shift the isometry center to the tensor containing the
-        corresponding site, i.e., move the isometry to a specific
-        Hilbert space. This method can be implemented independent
-        of the tensor network structure.
 
-        Parameters
-        ----------
-        idx : int
-            Index of the physical site which should be isometrized.
-        keep_singvals : bool, optional
-            If True, keep the singular values even if shifting the iso with a
-            QR decomposition. Default to False.
+    @abc.abstractmethod
+    def get_pos_links(self, pos):
+        """
+        Return a list of positions where all links are leading to. Number
+        of entries is equal to number of links. Each entry contains the position
+        as accessible in the actual tensor network.
         """
-        raise NotImplementedError("This function has to be overwritten.")
 
+    @abc.abstractmethod
     def get_rho_i(self, idx):
         """
         Get the reduced density matrix of the site at index idx
 
         Parameters
         ----------
         idx : int
             Index of the site
         """
-        raise NotImplementedError("This function has to be overwritten.")
 
+    @abc.abstractmethod
+    def get_tensor_of_site(self, idx):
+        """
+        Generic function to retrieve the tensor for a specific site. Compatible
+        across different tensor network geometries.
+
+        Parameters
+        ----------
+        idx : int
+            Return tensor containin the link of the local
+            Hilbert space of the idx-th site.
+        """
+
+    @abc.abstractmethod
     def iso_towards(self, new_iso, keep_singvals=False, trunc=False, conv_params=None):
         """
         Shift the isometry center to the tensor at the
         corresponding position, i.e., move the isometry to a
         specific tensor, that might not be a physical.
 
         Parameters
@@ -377,435 +425,349 @@
             Default to `False`.
         conv_params : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters to use for the SVD. If `None`, convergence
             parameters are taken from the TTN.
             Default to `None`.
 
         """
-        raise NotImplementedError("This function has to be overwritten.")
 
+    @abc.abstractmethod
+    def _iter_tensors(self):
+        """Iterate over all tensors forming the tensor network (for convert etc)."""
+
+    @abc.abstractmethod
+    def norm(self):
+        """
+        Calculate the norm of the state.
+        """
+
+    @abc.abstractmethod
     def scale(self, factor):
         """
         Multiply the tensor network state by a scalar factor.
 
         Parameters
         ----------
         factor : float
             Factor for multiplication of current tensor network state.
         """
-        raise NotImplementedError("This function has to be overwritten.")
 
-    @staticmethod
-    def tensordot_diagonal(tensor, diagonal, contr_legs):
+    @abc.abstractmethod
+    def set_singvals_on_link(self, pos_a, pos_b, s_vals):
+        """Update or set singvals on link via two positions."""
+
+    @abc.abstractmethod
+    def site_canonize(self, idx, keep_singvals=False):
         """
-        Optimally contract a diagonal matrix represented as a vector
-        with a tensor along the `contr_legs`.
-        Instead of a matrix-matrix multiplication we perform a
-        elementwise multiplication.
+        Shift the isometry center to the tensor containing the
+        corresponding site, i.e., move the isometry to a specific
+        Hilbert space. This method can be implemented independent
+        of the tensor network structure.
 
         Parameters
         ----------
-        tensor : xp.ndarray
-            Tensor to which the diagonal is contract
-        diagonal : xp.ndarray
-            Vector representing the diagonal matrix to contract
-        contr_legs : list of ints
-            Legs of the tensor along which you contract the diagonal
+        idx : int
+            Index of the physical site which should be isometrized.
+        keep_singvals : bool, optional
+            If True, keep the singular values even if shifting the iso with a
+            QR decomposition. Default to False.
+        """
 
-        Returns
-        -------
-        xp.ndarray
-            Output tensor after the contraction
+    @abc.abstractmethod
+    def _update_eff_ops(self, id_step):
         """
-        if np.isscalar(contr_legs):
-            contr_legs = [contr_legs]
+        Update the effective operators after the iso shift
 
-        t_shape = np.array(tensor.shape)
-        # Legs to be contracted (columns in the matrix representation)
-        contr_legs = list(contr_legs)
-        # Legs that are not going to be contracted (rows in the matrix rep)
-        not_contr_legs = [ss for ss in range(tensor.ndim) if ss not in contr_legs]
-        transposition = not_contr_legs + contr_legs
-        # Transpose and reshape in matrix
-        matrix = tensor.transpose(transposition).reshape(
-            -1, np.prod(t_shape[contr_legs])
-        )
-        # * is shorthand for xp.multiply
-        matrix = matrix * diagonal
+        Parameters
+        ----------
+        id_step : List[int]
+            List with information of the iso moving path
 
-        return matrix.reshape(t_shape[transposition]).transpose(
-            np.argsort(transposition)
-        )
+        Returns
+        -------
+        None
+            Updates the effective operators in place
+        """
 
-    def tSVD(
-        self,
-        tensor,
-        legs_left,
-        legs_right,
-        perm_left=None,
-        perm_right=None,
-        contract_singvals="N",
-        conv_params=None,
-    ):
-        """Perform a truncated Singular Value Decomposition by
-        first reshaping the tensor into a legs_left x legs_right
-        matrix, and permuting the legs of the ouput tensors if needed.
-        If the contract_singvals = ('L', 'R') it takes care of
-        renormalizing the output tensors such that the norm of
-        the MPS remains 1 even after a truncation.
+    @abc.abstractmethod
+    def _partial_iso_towards_for_timestep(self, pos, next_pos, no_rtens=False):
+        """
+        Move by hand the iso for the evolution backwards in time
 
         Parameters
         ----------
-        tensor : ndarray
-            Tensor upon which apply the SVD
-        legs_left : list of int
-            Legs that will compose the rows of the matrix
-        legs_right : list of int
-            Legs that will compose the columns of the matrix
-        perm_left : list of int, optional
-            permutations of legs after the SVD on left tensor
-        perm_right : list of int, optional
-            permutation of legs after the SVD on right tensor
-        contract_singvals: string, optional
-            How to contract the singular values.
-                'N' : no contraction
-                'L' : to the left tensor
-                'R' : to the right tensor
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters to use in the procedure. If None is given,
-            then use the default convergence parameters of the TN.
-            Default to None.
+        pos : Tuple[int] | int
+            Position of the tensor evolved
+        next_pos : Tuple[int] | int
+            Position of the next tensor to evolve
 
         Returns
         -------
-        tens_left: ndarray
-            left tensor after the SVD
-        tens_right: ndarray
-            right tensor after the SVD
-        singvals: ndarray
-            singular values kept after the SVD
-        singvals_cutted: ndarray
-            singular values cutted after the SVD, normalized with the biggest singval
+        QTeaTensor
+            The R tensor of the iso movement
+        Tuple[int]
+            The position of the partner (the parent in TTNs)
+        int
+            The link of the partner pointing towards pos
+        List[int]
+            The update path to pass to _update_eff_ops
         """
-        xp = self._device_checks(tensor=tensor)
 
-        if conv_params is None:
-            conv_params = self._convergence_parameters
-        elif not isinstance(conv_params, TNConvergenceParameters):
-            raise ValueError(
-                "conv_params must be TNConvergenceParameters or None, "
-                + f"not {type(conv_params)}."
-            )
+    @abc.abstractmethod
+    def default_sweep_order(self):
+        """
+        Default sweep order to be used in the ground state search/time evolution.
 
-        # Reshaping
-        matrix = xp.transpose(tensor, legs_left + legs_right)
-        shape_left = np.array(tensor.shape)[legs_left]
-        shape_right = np.array(tensor.shape)[legs_right]
-        matrix = matrix.reshape(np.prod(shape_left), np.prod(shape_right))
-
-        # SVD decomposition
-        try:
-            mat_left, singvals_tot, mat_right = xp.linalg.svd(
-                matrix, full_matrices=False
-            )
-        except np.linalg.LinAlgError:
-            warnings.warn("gesdd SVD decomposition failed. Resorting to gesvd.")
-            mat_left, singvals_tot, mat_right = sp.linalg.svd(
-                matrix, full_matrices=False, lapack_driver="gesvd"
-            )
-
-        # Truncation
-        cut, singvals, singvals_cutted = self._truncate_singvals(
-            singvals_tot, conv_params
-        )
-        mat_left = mat_left[:, :cut]
-        mat_right = mat_right[:cut, :]
-
-        # Contract singular values if requested
-        if contract_singvals.upper() == "L":
-            mat_left = xp.multiply(mat_left, singvals)
-        elif contract_singvals.upper() == "R":
-            mat_right = xp.multiply(singvals, mat_right.T).T
-        elif contract_singvals.upper() != "N":
-            raise ValueError(
-                f"Contract_singvals option {contract_singvals} is not "
-                + "implemented. Choose between right (R), left (L) or None (N)."
-            )
+        Returns
+        -------
+        List[int] | List[Tuple[int]]
+            The generator that you can sweep through
+        """
+        raise NotImplementedError("This method is ansatz-specific")
 
-        # Reshape back to tensors
-        tens_left = mat_left.reshape(list(shape_left) + [cut])
-        if perm_left is not None:
-            tens_left = xp.transpose(tens_left, perm_left)
-
-        tens_right = mat_right.reshape([cut] + list(shape_right))
-        if perm_right is not None:
-            tens_right = xp.transpose(tens_right, perm_right)
-
-        return tens_left, tens_right, singvals, singvals_cutted
-
-    def QR(self, tensor, legs_left, legs_right, perm_left=None, perm_right=None):
-        """Perform a QR Decomposition by
-        first reshaping the tensor into a legs_left x legs_right
-        matrix, and permuting the legs of the ouput tensors if needed.
+    def default_sweep_order_back(self):
+        """Default sweep order backwards, e.g., for second-order methods."""
+        return self.default_sweep_order()[::-1]
+
+    @abc.abstractmethod
+    def get_pos_partner_link_expansion(self, pos):
+        """
+        Get the position of the partner tensor to use in the link expansion
+        subroutine
 
         Parameters
         ----------
-        tensor : ndarray
-            Tensor upon which apply the QR
-        legs_left : list of int
-            Legs that will compose the rows of the matrix
-        legs_right : list of int
-            Legs that will compose the columns of the matrix
-        perm_left : list of int, optional
-            permutations of legs after the QR on left tensor
-        perm_right : list of int, optional
-            permutation of legs after the QR on right tensor
+        pos : int | Tuple[int]
+            Position w.r.t. which you want to compute the partner
 
         Returns
         -------
-        tens_left: ndarray
-            left tensor after the QR (orthogonal tensor)
-        tens_right: ndarray
-            right tensor after the QR (triangular tensor)
-        """
-        xp = self._device_checks(tensor=tensor)
-
-        # Reshaping
-        matrix = xp.transpose(tensor, legs_left + legs_right)
-        shape_left = np.array(tensor.shape)[legs_left]
-        shape_right = np.array(tensor.shape)[legs_right]
-        matrix = matrix.reshape(np.prod(shape_left), np.prod(shape_right))
-        k_dim = np.min([matrix.shape[0], matrix.shape[1]])
-
-        # QR decomposition
-        mat_left, mat_right = xp.linalg.qr(matrix)
-
-        # Reshape back to tensors
-        tens_left = mat_left.reshape(list(shape_left) + [k_dim])
-        if perm_left is not None:
-            tens_left = xp.transpose(tens_left, perm_left)
-
-        tens_right = mat_right.reshape([k_dim] + list(shape_right))
-        if perm_right is not None:
-            tens_right = xp.transpose(tens_right, perm_right)
-
-        return tens_left, tens_right
-
-    def tEQR(self, tens_left, tens_right, singvals_left, operator=None):
-        """
-        Perform an truncated ExpandedQR decomposition, generalizing the idea
-        of https://arxiv.org/pdf/2212.09782.pdf for a general bond expansion
-        given the isometry center of the network on  `tens_left`.
-        It should be rather general for three-legs tensors, and thus applicable
-        with any tensor network ansatz. Notice that, however, you do not have
-        full control on the approximation, since you know only a subset of the
-        singular values truncated.
+        int | Tuple[int]
+            Position of the partner
+        int
+            Link of pos pointing towards the partner
+        int
+            Link of the partner pointing towards pos
+        """
+
+    @abc.abstractmethod
+    def write(self, filename, cmplx=True):
+        """Write the TN in python format into a FORTRAN compatible format."""
+
+    # --------------------------------------------------------------------------
+    #                        Methods that can be inherited
+    # --------------------------------------------------------------------------
+
+    def checkpoint_copy_simulation_attr(self, src):
+        """Copy attributes linked to the simulation, like convergence parameters."""
+        self._log_file = src.log_file
+        self.convergence_parameters = src.convergence_parameters
+        self.solver = src.solver
 
-        Parameters
-        ----------
-        tens_left: xp.array
-            Left tensor
-        tens_right: xp.array
-            Right tensor
-        singvals_left: xp.array
-            Singular values array insisting on the link to the left of `tens_left`
-        operator: xp.array or None
-            Operator to contract with the tensors. If None, no operator is contracted
+        if src.comm is not None:
+            raise ValueError("Checkpoints and MPI are not yet enabled.")
 
-        Returns
-        -------
-        tens_left: ndarray
-            left tensor after the EQR
-        tens_right: ndarray
-            right tensor after the EQR
-        singvals: ndarray
-            singular values kept after the EQR
-        singvals_cutted: ndarray
-            subset of thesingular values cutted after the EQR,
-            normalized with the biggest singval
-        """
-        xp = self._device_checks()
-
-        # Trial bond dimension
-        eta = int(
-            np.ceil(
-                (1 + self._convergence_parameters.min_expansion_qr) * tens_left.shape[0]
-            )
-        )
+    def checkpoint_store(
+        self,
+        folder_name_output,
+        dyn_checkpoint_file,
+        int_str,
+        checkpoint_indicator_file,
+        is_dyn=False,
+        jdic=None,
+    ):
+        """
+        Store the tensor network as checkpoint.
 
-        # Contract the two tensors together
-        twotensors = xp.tensordot(tens_left, tens_right, (2, 0))
-        twotensors = xp.tensordot(np.diag(singvals_left), twotensors, (1, 0))
-
-        # Contract with the operator if present
-        if operator is not None:
-            twotensors = xp.tensordot(twotensors, operator, ([1, 2], [2, 3]))
-        # For simplicity, transpose in the same order as obtained
-        # after the application of the operator
-        else:
-            twotensors = twotensors.transpose(0, 3, 1, 2)
+        **Arguments**
+
+        folder_name_output : str
+            Name of the output folder, where we store checkpoints.
 
-        # Apply first phase in expanding the bond dimension
-        expansor = xp.eye(eta, np.prod(tens_left.shape[:2])).reshape(
-            eta, *tens_left.shape[:2]
+        dyn_checkpoint_file : str or `None`
+            Name of the previous checkpoint file, which can be deleted after
+            creating the new checkpoint.
+
+        int_str : str
+            Identifier containing integers as string to identify the checkpoint
+            when loading in a potential future run.
+
+        checkpoint_indicator_file: str
+            Path to file which indicates if checkpoints exists.
+
+        is_dyn : bool, optional
+            Flag to indicate if checkpoint is for statics (False) or
+            dynamics (True).
+            Default to `False`.
+
+        jdic : json-compatible structure or `None`, optional
+            Store additional information as json.
+            Default to `None` (store nothing).
+        """
+        prev_checkpoint_file = dyn_checkpoint_file
+        dyn_stat_switch = "dyn" if is_dyn else "stat"
+        dyn_checkpoint_file = os.path.join(
+            folder_name_output, f"TTN_{dyn_stat_switch}_{int_str}"
         )
-        expanded_y0 = xp.tensordot(expansor, twotensors, ([1, 2], [0, 2]))
-        expanded_y0 = xp.transpose(expanded_y0, [0, 2, 1])
+        self.save_pickle(dyn_checkpoint_file)
 
-        # Contract with the (i+1)th site dagger
-        first_qr = xp.tensordot(twotensors, xp.conj(expanded_y0), ([1, 3], [2, 1]))
-        first_q, _ = xp.linalg.qr(first_qr.reshape(-1, first_qr.shape[2]))
-        first_q = first_q.reshape(first_qr.shape)
+        if jdic is not None:
+            with open(dyn_checkpoint_file + ".json", "w+") as fh:
+                json.dump(jdic, fh)
 
-        # Contract the new q with the i-th site. The we would need a rq decomposition.
-        second_qr = xp.tensordot(twotensors, np.conj(first_q), ([0, 2], [0, 1]))
-        second_qr = second_qr.transpose(2, 1, 0)
-        second_q, second_r = xp.linalg.qr(second_qr.reshape(second_qr.shape[0], -1).T)
-        second_q = second_q.T.reshape(second_qr.shape)
-        # To get the real R matrix I would have to transpose, but to avoid a double
-        # transposition I simply avoid that
-        # second_r = second_r.T
+        # Delete previous checkpoint
+        if prev_checkpoint_file is not None:
+            ext = ".pkl" + self.extension
+            os.remove(prev_checkpoint_file + ext)
 
-        # Second phase in the expansor
-        eigvl, eigvc = xp.linalg.eigh(np.conj(second_r) @ second_r.T)
-        # Singvals are sqrt of eigenvalues, and sorted in the opposite order
-        singvals = np.sqrt(eigvl)[::-1]
+            if os.path.isfile(prev_checkpoint_file + ".json"):
+                os.remove(prev_checkpoint_file + ".json")
 
-        # Routine to select the bond dimension
-        cut, singvals, singvals_cutted = self._truncate_singvals(singvals)
-        tens_right = xp.tensordot(eigvc[:cut, ::-1], second_q, ([1], [0]))
+        if not os.path.isfile(checkpoint_indicator_file):
+            with open(checkpoint_indicator_file, "w+") as fh:
+                pass
 
-        # Get the last tensor
-        tens_left = xp.tensordot(twotensors, xp.conj(tens_right), ([1, 3], [2, 1]))
+        return dyn_checkpoint_file
 
-        return tens_left, tens_right, singvals, singvals_cutted
+    def convert(self, dtype, device):
+        """Convert data type and device inplace."""
+        if isinstance(dtype, str):
+            dtype = self.dtype_from_char(dtype)
 
-    def _truncate_singvals(self, singvals, conv_params=None):
-        """
-        Truncate the singular values followling the
-        strategy selected in the convergence parameters class
+        if (self.dtype == dtype) and (self.device == device):
+            # Fast return, nothing to do
+            self._convert_singvals(dtype, device)
+            return
 
-        Parameters
-        ----------
-        singvals : np.ndarray
-            Array of singular values
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters to use in the procedure. If None is given,
-            then use the default convergence parameters of the TN.
-            Default to None.
+        for tensor in self._iter_tensors():
+            tensor.convert(dtype, device)
 
-        Returns
-        -------
-        cut : int
-            Number of singular values kept
-        singvals_kept : np.ndarray
-            Normalized singular values kept
-        singvals_cutted : np.ndarray
-            Normalized singular values cutted
+        # Cannot update inplace in abstract class
+        self._convert_singvals(dtype, device)
+
+        if self.eff_op is not None:
+            self.eff_op.convert(dtype, device)
+
+    def dtype_from_char(self, dtype):
+        """Resolve data type from chars C, D, S, Z and optionally H."""
+        for tensor in self._iter_tensors():
+            return tensor.dtype_from_char(dtype)
+
+        raise Exception("Querying on empty tensor network.")
+
+    def normalize(self):
         """
-        xp = self._device_checks()
+        Normalize the state depending on its current norm.
+        """
+        factor = 1.0 / self.norm()
+        self.scale(factor)
 
-        if conv_params is None:
-            conv_params = self._convergence_parameters
-        elif not isinstance(conv_params, TNConvergenceParameters):
-            raise ValueError(
-                "conv_params must be TNConvergenceParameters or None, "
-                + f"not {type(conv_params)}."
-            )
+    def log_close(self):
+        """Close log file if open."""
+        self._log_file.close()
+        self._log_file = None
+
+    def log_open(self, filename, mode="auto"):
+        """Open a log file."""
+        if mode == "auto":
+            mode = "a" if os.path.isfile(filename) else "w+"
+
+        # pylint: disable-next=consider-using-with
+        self._log_file = open(filename, mode)
+
+        if mode == "a":
+            self.log_print("\n\n" + "=" * 80)
+            self.log_print("APPENDING TO EXISTING LOG FILE")
+            self.log_print("=" * 80 + "\n\n")
+
+    def log_set_verbosity(self, verbosity):
+        """Set the verbosity for print statements."""
+        self._log_verbosity = verbosity
+
+    def log_print(self, *args, verbosity_level=0):
+        """Write to stdout or log file depending on setting."""
+        if verbosity_level >= self._log_verbosity:
+            return
 
-        if conv_params.trunc_method == "R":
-            cut = self._truncate_sv_ratio(singvals, conv_params)
-        elif conv_params.trunc_method == "N":
-            cut = self._truncate_sv_norm(singvals, conv_params)
+        if self._log_file is None:
+            print(*args)
         else:
-            raise Exception(f"Unkown trunc_method {conv_params.trunc_method}")
+            self._log_file.write(str(args))
+            self._log_file.write("\n")
 
-        # Divide singvals in kept and cut
-        singvals_kept = singvals[:cut]
-        singvals_cutted = singvals[cut:]
-        # Renormalizing the singular values vector to its norm
-        # before the truncation
-        norm_kept = xp.sum(singvals_kept**2)
-        norm_trunc = xp.sum(singvals_cutted**2)
-        normalization_factor = np.sqrt(norm_kept) / np.sqrt(norm_kept + norm_trunc)
-        singvals_kept /= normalization_factor
+    def _store_attr_for_pickle(self):
+        """Return dictionary with attributes that cannot be pickled and unset them."""
+        storage = {
+            "conv_params": self._convergence_parameters,
+            "log_file": self._log_file,
+            "comm": self.comm,
+            "solver": self._solver,
+        }
+
+        self._convergence_parameters = None
+        self.comm = None
+        self._log_file = None
+        self._solver = None
 
-        # Renormalize cut singular values to track the norm loss
-        singvals_cutted /= np.sqrt(norm_trunc + norm_kept)
+        return storage
 
-        return cut, singvals_kept, singvals_cutted
+    def _restore_attr_for_pickle(self, storage):
+        """Restore attributed removed for pickle from dictionary."""
+        # Reset temporary removed attributes
+        self._convergence_parameters = storage["conv_params"]
+        self.comm = storage["comm"]
+        self._log_file = storage["log_file"]
+        self._solver = storage["solver"]
 
-    def _truncate_sv_ratio(self, singvals, conv_params):
+    def save_pickle(self, filename):
         """
-        Truncate the singular values based on the ratio
-        with the bigger one
+        Save class via pickle-module.
 
-        Parameters
-        ----------
-        singvals : np.ndarray
-            Array of singular values
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters to use in the procedure.
+        **Details**
 
-        Returns
-        -------
-        cut : int
-            Number of singular values kept
+        The following attributes have a special treatment and are not present
+        in the copied object.
+
+        * convergence_parameters
+        * log file (filehandle)
+        * MPI communicator
         """
-        xp = self._device_checks()
+        # Temporary remove objects which cannot be pickled which
+        # included convergence parameters for lambda function and
+        # parameterized variables, the log file as file handle and
+        # the MPI communicator
+        storage = self._store_attr_for_pickle()
 
-        # Truncation
-        lambda1 = singvals[0]
-        cut = xp.nonzero(singvals / lambda1 < conv_params.cut_ratio)[0]
-        if xp == cp:
-            cut = cut.get()
-
-        # Confront the cut w.r.t the maximum bond dimension
-        if len(cut) > 0:
-            cut = min(conv_params.max_bond_dimension, cut[0])
-        else:
-            cut = conv_params.max_bond_dimension
-        cut = min(cut, len(singvals))
+        device = self.device
+        if device != "cpu":
+            # Assume pickle needs to be on host
+            self.convert(None, "cpu")
 
-        return cut
+        ext = "pkl" + self.extension
+        if not filename.endswith(ext):
+            filename += "." + ext
 
-    def _truncate_sv_norm(self, singvals, conv_params):
-        """
-        Truncate the singular values based on the
-        total norm cut
+        with open(filename, "wb") as fh:
+            pickle.dump(self, fh)
 
-        Parameters
-        ----------
-        singvals : np.ndarray
-            Array of singular values
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters to use in the procedure.
+        # Check if we move back to the device where TN
+        # was stored originally
+        if device != "cpu":
+            self.convert(None, device)
 
-        Returns
-        -------
-        cut : int
-            Number of singular values kept
-        """
-        xp = self._device_checks()
+        self._restore_attr_for_pickle(storage)
 
-        norm = xp.cumsum(singvals[::-1] ** 2) / xp.sum(singvals**2)
-        # You get the first index where the constraint is broken,
-        # so you need to stop an index before
-        cut = xp.nonzero(norm > conv_params.cut_ratio)[0]
-        if xp == cp:
-            cut = cut.get()
-
-        # Confront the cut w.r.t the maximum bond dimension
-        if len(cut) > 0:
-            cut = len(singvals) - cut[0]
-            cut = min(conv_params.max_bond_dimension, cut)
-        else:
-            cut = conv_params.max_bond_dimension
+    # pylint: disable-next=unused-argument
+    def permute_spo_for_two_tensors(self, spo_list, theta, link_partner):
+        """Returns permuted SPO list, permuted theta, and the inverse permutation."""
+        return spo_list, theta, None
 
-        return cut
+    # --------------------------------------------------------------------------
+    #                                  Unsorted
+    # --------------------------------------------------------------------------
 
     def _postprocess_singvals_cut(self, singvals_cut, conv_params=None):
         """
         Postprocess the singular values cut after the application of a
         tSVD based on the convergence parameters. Either take the sum of
         the singvals (if `conv_params.trunc_tracking_mode` is `"C"`) or the maximum
         (if `conv_params.trunc_tracking_mode` is `"M"`).
@@ -834,83 +796,14 @@
         elif conv_params.trunc_tracking_mode == "C":
             singvals_cut = (singvals_cut**2).sum()
         else:
             raise Exception(f"Unkown trunc_tracking_mode {conv_params.trunc_method}")
 
         return singvals_cut
 
-    def to_device(self, device):
-        """
-        Move the TN class to the new device.
-        Should be implemented by the derived class
-
-        Parameters
-        ----------
-        device : string
-            Device where to move the tensor network
-        """
-        if not device in self.implemented_devices:
-            raise ValueError(
-                f"Device {device} is not implemented. Select from "
-                + f"{self.implemented_devices}"
-            )
-        return NotImplementedError("to_device must be implemented by the class")
-
-    def _device_checks(self, return_sla=False, **kwargs):
-        """
-        Check if all the arguments of the function where
-        _device_checks is called are on the correct device,
-        select the correct
-
-        Parameters
-        ----------
-        device : str
-            Device where the computation should take place.
-            If called inside an emulator it should be the
-            emulator device
-        return_sla : bool, optional
-            If True, returns the handle to the sparse linear algebra.
-            Either sp.sparse.linalg or cp.scipy.sparse.linalg.
-            Default to False.
-        **kwargs : array-like
-            Array-like inputs to the function. If they are
-            on the wrong device an exception is raised.
-            The keyword is the identifier used in the raise
-            statement
-
-        Returns
-        -------
-        module handle
-            cp if the device is GPU
-            np if the device is CPU
-        """
-        if not GPU_AVAILABLE:
-            xp = np
-            xsla = ssla
-        else:
-            if self.device == "gpu":
-                xp = cp
-                xsla = csla
-            elif self.device == "cpu":
-                xp = np
-                xsla = ssla
-
-            for key, value in kwargs.items():
-                xp_arg = cp.get_array_module(value)
-                if xp_arg != xp:
-                    raise ValueError(
-                        f"Argument {key} is not "
-                        + f"on the correct device. Should be {xp} but is {xp_arg}."
-                    )
-
-        if return_sla:
-            return xp, xsla
-        else:
-            return xp
-
     #########################################
     ########## MEASUREMENT METHODS ##########
     #########################################
 
     def meas_local(self, op):
         """
         Measure a local observable along all sites of the MPS
@@ -922,29 +815,34 @@
 
         Return
         ------
         measures : ndarray, shape (num_sites)
             Measures of the local operator along each site
         """
         self.check_obs_input(op)
-        xp = self._device_checks()
+        if op.ndim == 4:
+            if op.shape[0] == 1 and op.shape[3] == 1:
+                # Need copy, otherwise input tensor is modified ("passed-by-pointer")
+                op = op.copy()
+                op = op.remove_dummy_link(3).remove_dummy_link(0)
 
-        measures = xp.zeros(self.num_sites)
+        # Always store on host
+        measures = np.zeros(self.num_sites)
 
         # This subroutine can be parallelized if the singvals are stored using
         # joblib
         for ii in range(self.num_sites):
             rho_i = self.get_rho_i(ii)
-
-            expectation = xp.trace(rho_i @ op)
-            measures[ii] = xp.real(expectation)
-
-        # Come back to CPU if on GPU
-        if xp == cp:
-            measures = measures.get()
+            if op.ndim == 2:
+                expectation = rho_i.tensordot(op, ([0, 1], [1, 0]))
+            else:
+                tmp = deepcopy(op)
+                tmp.trace_one_dim_pair([0, 3])
+                expectation = rho_i.tensordot(tmp, ([0, 1], [1, 0]))
+            measures[ii] = np.real(expectation.get_entry())
 
         return measures
 
     def meas_magic(
         self, renyi_idx=2, num_samples=1000, return_probabilities=False, precision=14
     ):
         """
@@ -1051,50 +949,60 @@
             occurrences. The keys are separated by a comma if local_dim > 9.
         """
         if nmeas == 0:
             return {}
 
         if seed is not None and isinstance(seed, int):
             np.random.seed(seed)
-        xp = self._device_checks()
+
         # Put in canonic form
         self.site_canonize(0)
 
         measures = []
         probabilities = []
         # Loop over number of measurements
         for _ in range(nmeas):
             state = np.zeros(self.num_sites, dtype=int)
             temp_tens = deepcopy(self.get_tensor_of_site(0))
             # Loop over tensors
             cumulative_prob = 1.0
             for ii in range(self.num_sites):
-                target_prob = xp.random.rand()
+                target_prob = np.random.rand()
                 measured_idx, temp_tens, prob_ii = self._get_child_prob(
                     temp_tens, ii, target_prob, unitary_setup, state, qiskit_convention
                 )
                 cumulative_prob *= prob_ii
 
                 # Save the measured state either with qiskit or
                 # theoretical convention
                 if qiskit_convention:
                     state[self.num_sites - 1 - ii] = measured_idx
                 else:
                     state[ii] = measured_idx
 
-            if self._local_dim.max() < 10:
-                measures.append(xp.array2string(state, separator="")[1:-1])
+            if isinstance(self._local_dim, list):
+                max_local_dim = np.max(self._local_dim)
+            else:
+                max_local_dim = self._local_dim.max()
+
+            if max_local_dim < 10:
+                measure_ii = np.array2string(
+                    state, separator="", max_line_width=2 * self.num_sites
+                )[1:-1]
             else:
-                measures.append(xp.array2string(state, separator=",")[1:-1])
+                measure_ii = np.array2string(
+                    state, separator=",", max_line_width=2 * self.num_sites
+                )[1:-1]
 
             probabilities.append(cumulative_prob)
 
-        # Come back to CPU if on GPU
-        if xp == cp:
-            measures = cp.asnumpy(measures)
+            # Come back to CPU if on GPU for list in measures (not needed since it is string)
+            measures.append(measure_ii)
+
+        measures = np.array(measures)
         states, counts = np.unique(measures, return_counts=True)
         probabilities = dict(zip(measures, probabilities))
         measures = dict(zip(states, counts))
 
         if do_return_probabilities:
             return measures, probabilities
         else:
@@ -1178,15 +1086,16 @@
         if mode == "projection_z":
             local_dim = self.local_dim
             get_children_prob = self._get_children_prob
             initial_tensor = self.get_tensor_of_site(0)
         elif mode == "magic":
             local_dim = np.repeat(4, self.num_sites)
             get_children_prob = self._get_children_magic
-            initial_tensor = np.ones((1, 1))
+            tmp = self.get_tensor_of_site(0)
+            initial_tensor = tmp.eye_like(tmp.links[0])
         else:
             raise ValueError(f"mode {mode} not available for unbiased sampling")
 
         # ==== Initialize variables ====
         # all_probs is a structure to keep track of already-visited nodes in
         # the probability tree. The i-th dictionary of the list correspond to
         # a state measured up to the i-th site. Each dictionary has the states
@@ -1458,281 +1367,790 @@
             in ``curr_state[-1]``. Passing ``False`` means indices are
             equal and not reversed.
         """
         # Cannot implement it here, it highly depends on the TN
         # geometry
         raise NotImplementedError("This function has to be overwritten.")
 
-    def _contr_to_eff_op(self, tensor, ops_list, idx_list, idx_out):
+    def compute_energy(self, pos=None):
         """
-        Contract operators lists with tensor T and its dagger. Return effective
-        Hamiltonian operators along idx_out (relative to T),
-        resulting from contraction.
+        Compute the energy of the TTN through the effective operator
+        at position pos.
 
         Parameters
         ----------
-        T: np.ndarray
-                Tensor of the TTN to contract
-        ops_list: list of lists of Operator
-            list of local operator lists, each corresponding to a
-            specific link.
-        idx_list:   list of ints
-            link indices (relative to T), each corresponding to
-            a local operator list in ops_list.
+        pos : list, optional
+            If a position is provided, the isometry is first shifted to
+            that position and then the energy is computed. If None,
+            the current isometry center is computed, by default None
 
         Returns
-        ---------
-        list
-            list of Operators after contractions
-        """
-        xp = self._device_checks(tensor=tensor)
-
-        # Put everything in the correct order
-        sorting = np.argsort(idx_list)
-        ops_list = np.array(ops_list, dtype=object)
-        idx_list = np.array(idx_list)
-        ops_list = ops_list[sorting]
-        idx_list = idx_list[sorting]
-
-        # Retrieve the ID of all the operator passed
-        ops_ids = np.array(
-            [[opjj.op_id for opjj in opii] for opii in ops_list], dtype=object
-        )
-        ops_ids_flattened = [op for ops_list in ops_ids for op in ops_list]
-        # Get a list of unique IDs
-        ids = np.sort(np.unique(ops_ids_flattened))
-
-        tensor_len = len(tensor.shape)
-        avail_idx = np.arange(tensor_len, dtype=int)
-        avail_idx = np.delete(avail_idx, idx_out)
-
-        new_ops = []
-        # We could run this for cycle in parallel
-        for op_id in ids:
-            idxs = [np.nonzero(ops_id == op_id)[0] for ops_id in ops_ids]
-            temp = deepcopy(tensor)
-            entered = False
-            for ii, common_id in enumerate(idxs):
-                # If that ID is present in the list
-                if len(common_id) == 1:
-                    # Perform the contraction
-                    temp = xp.tensordot(
-                        temp, ops_list[ii][common_id[0]].op, ([idx_list[ii]], [1])
-                    )
-                    temp = temp.transpose(_transpose_idx(tensor_len, idx_list[ii]))
-                    # Record the coefficient
-                    coeff = ops_list[ii][common_id[0]].coeff
-                    entered = True
+        -------
+        float
+            Energy of the TTN
+        """
+
+        if self.eff_op is None:
+            warn("Tried to compute energy with no effective operators. Returning nan")
+            return np.nan
+        # Move the iso center if needed
+        if pos is not None:
+            self.iso_towards(pos)
+        else:
+            pos = self.iso_center
+            if not np.isscalar(pos):
+                pos = tuple(pos)
+
+        # Retrieve the tensor at the isometry
+        tens = self[self.iso_center]
+
+        # Get the list of operators to contract
+        pos_links = self.get_pos_links(pos)
+
+        # Contract the tensor with the effective operators around
+        vec = self.eff_op.contract_tensor_lists(tens, pos, pos_links)
 
-            if entered:
-                # Perform the contraction with the complex conjugate
-                # This order avoids an extra transposition
-                new_t = xp.tensordot(xp.conj(tensor), temp, (avail_idx, avail_idx))
+        energy = tens.dot(vec)
 
-                # Append to the new operators
-                new_ops.append(IndexedOperator(new_t, op_id, coeff))
+        # Update internal storage
+        self._prev_energy = energy
 
-        return new_ops
+        return np.real(tens.get_of(energy))
+
+    #########################################################################
+    ######################### Optimization methods ##########################
+    #########################################################################
 
-    def _contract_tensor_lists(self, vector, pos, ops_list, idx_list):
+    def optimize_single_tensor(self, pos):
         """
-        Linear operator to contract all the effective operators
-        around the tensor in position `pos`. Used in the optimization.
+        Optimize the tensor at position `pos` based on the
+        effective operators loaded in the TTN
 
         Parameters
         ----------
-        vector : np.ndarray
-            tensor in position pos in vector form
-        pos : list of int
-            list of [layer_idx, tensor_idx]
+        pos : list of ints or int
+            Position of the tensor in the TN
 
         Returns
         -------
-        np.ndarray
-            vector after the contraction of the effective operators
+        float
+            Computed energy
         """
-        if pos != self._iso_center:
-            raise RuntimeError(
-                "Tried efficient operators contraction not at the iso_center"
-            )
-        xp = self._device_checks()
-
-        tensor_shape = self[pos].shape
-        tensor_len = len(tensor_shape)
-        tensor = vector.reshape(tensor_shape)
-
-        # Put everything in the correct order
-        sorting = np.argsort(idx_list)
-        ops_list = np.array(ops_list, dtype=object)
-        idx_list = np.array(idx_list)
-        ops_list = ops_list[sorting]
-        idx_list = idx_list[sorting]
-
-        # Retrieve the ID of all the operator passed
-        ops_ids = np.array(
-            [[opjj.op_id for opjj in opii] for opii in ops_list], dtype=object
-        )
-        # Get a list of unique IDs
-        ops_ids_flattened = [op for ops_list_id in ops_ids for op in ops_list_id]
-        ids = np.sort(np.unique(ops_ids_flattened))
-
-        new_tens = xp.zeros_like(tensor, dtype=complex)
-        # We could run this for cycle in parallel
-        for op_id in ids:
-            idxs = [np.nonzero(ops_id == op_id)[0] for ops_id in ops_ids]
-            temp = deepcopy(tensor)
-            entered = False
-            for ii, common_id in enumerate(idxs):
-                # If that ID is present in the list
-                if len(common_id) == 1:
-                    # Perform the contraction
-                    temp = xp.tensordot(
-                        temp, ops_list[ii][common_id[0]].op, ([idx_list[ii]], [1])
-                    )
-                    temp = temp.transpose(_transpose_idx(tensor_len, idx_list[ii]))
-                    # Record the coefficient
-                    coeff = ops_list[ii][common_id[0]].coeff
-                    entered = True
-            # Update the tensor
-            if entered:
-                new_tens += coeff * temp
+        tic = tictoc()
+        self.log_print("-" * 50, verbosity_level=2)
+        self.log_print(f"Optimizing tensor {pos}", verbosity_level=2)
 
-        return new_tens.reshape(-1)
+        # Isometrise towards the desired tensor
+        self.iso_towards(pos)
+        pos_links = self.get_pos_links(pos)
 
-    def _get_eff_op_on_pos(self, pos):
+        dim_problem = np.product(self[pos].shape)
+        if dim_problem == 1:
+            # Nothing to do - ARPACK will fail
+            eigenvalue = self.compute_energy()
+            return eigenvalue
+
+        # Retrieve the tensor
+        eigenvalues, tensor = self[pos].eig_api(
+            self.eff_op.contract_tensor_lists,
+            self[pos].shape,
+            self._convergence_parameters,
+            args_func=(pos, pos_links),
+        )
+
+        self.log_print(f"New energy is E={np.real(eigenvalues[0])}", verbosity_level=2)
+        self.log_print(f"Computational time {tictoc()-tic}", verbosity_level=2)
+        self.log_print("-" * 50, verbosity_level=2)
+
+        self[pos] = tensor
+
+        # Update internal storage
+        self._prev_energy = eigenvalues[0]
+
+        return np.real(tensor.get_of(eigenvalues[0]))
+
+    def optimize_link_expansion(
+        self,
+        pos,
+        pos_partner,
+        link_self,
+        link_partner,
+    ):
         """
-        Obtain the list of effective operators adjacent
-        to the position pos and the index where they should
-        be contracted
+        Optimize a tensor pair via a space-link expansion.
 
-        Parameters
-        ----------
-        pos :
-            key to the desired tensor
+        **Arguments**
+
+        pos : int, tuple of ints (depending on TN)
+            position of tensor to be optimized
+
+        pos_partner : int, tuple of ints (depending on TN)
+            position of partner tensor, where link between
+            tensor and partner tensor will be randomly
+            expandend.
+
+        link_self : int
+            Link connecting to partner tensor (in tensor at `pos`)
+
+        link_partner : int
+            Link connecting to optimized tensors (in partner tensor).
+
+        requires_singvals : bool
+            Flag if calling methods upstream need singular values, i.e.,
+            want to replace QR with SVDs
 
         Returns
         -------
-        list of IndexedOperators
-            List of effective operators
-        list of ints
-            Indexes where the operators should be contracted
+        float
+            Computed energy
         """
-        raise NotImplementedError("This function has to be overwritten")
+        if isinstance(pos, list):
+            raise Exception("Passing list as position")
+        if isinstance(pos_partner, list):
+            raise Exception("Passing list as partner position")
+
+        # Here it would be beneficial to implement the skip_exact_rgtensors, but
+        # we would need to add a data structure to flag which tensors are converged.
+        # After that, when moving the iso with svd we can easily understand if there
+        # is truncation
+        # _ = self._convergence_parameters.sim_params["skip_exact_rgtensors"]
+        self.iso_towards(pos_partner)
+
+        tensor = self[pos].copy()
+        tensor_partner = self[pos_partner].copy()
+
+        # If energy goes up and we want to reinstall original tensor
+        if self._prev_energy is None:
+            self._prev_energy = self.compute_energy()
+        prev_tensor = tensor.copy()
+        prev_tensor_partner = tensor_partner.copy()
+
+        new_dim = (
+            tensor.shape[link_self]
+            + self._convergence_parameters.sim_params["min_expansion"]
+        )
 
-    def compute_energy(self, pos=None):
+        self[pos], self[pos_partner] = tensor.expand_link_tensorpair(
+            tensor_partner,
+            link_self,
+            link_partner,
+            new_dim,
+        )
+
+        # Ideal implementation would be ...
+        # First iso_towards to pos_partner, as well as pos_partner
+        # after decision.
+
+        # Update of eff operators (internal iso_towards in space link
+        # expansion cannot truncate or update singvals)
+        self.iso_towards(pos)
+
+        # Random entries destroyed normalization, to get valid
+        # eigenvalue in these intermediate steps, need to renormalize
+        self.normalize()
+
+        # Expansion cycles
+        # ----------------
+
+        # Same here, use QR as otherwise truncation kicks in potentially]
+        # undoing the expansion. Final iso_towards with QR or SVD follows
+        # after expansion cycles.
+        requires_singvals = self._requires_singvals
+        self._requires_singvals = False
+
+        for _ in range(self._convergence_parameters.sim_params["expansion_cycles"]):
+            self.iso_towards(pos_partner)
+            energy = self.optimize_single_tensor(pos_partner)
+
+            self.iso_towards(pos)
+            energy = self.optimize_single_tensor(pos)
+
+        # Reset value
+        self._requires_singvals = requires_singvals
+
+        # Decision on accepting update
+        # ----------------------------
+
+        expansion_drop = self._convergence_parameters.sim_params["expansion_drop"]
+
+        if energy <= self._prev_energy or expansion_drop in ["f"]:
+            # We improved in energy or accept higher energies to escape local
+            # minima in this sweep
+            self.iso_towards(
+                pos_partner,
+                keep_singvals=requires_singvals,
+                trunc=True,
+                conv_params=self._convergence_parameters,
+            )
+        elif expansion_drop in ["o"]:
+            # Energy did not improve, but optimize locally
+            self[pos] = prev_tensor
+            self[pos_partner] = prev_tensor_partner
+
+            # Iso center before copy was at pos_partner
+            self.iso_center = pos_partner
+
+            self.iso_towards(
+                pos, trunc=requires_singvals, keep_singvals=requires_singvals
+            )
+            energy = self.optimize_single_tensor(pos)
+
+        elif expansion_drop in ["d"]:
+            # Energy did not improve, reinstall previous tensors, discard
+            # step and do not optimize even locally
+            self[pos] = prev_tensor
+            self[pos_partner] = prev_tensor_partner
+
+            # Iso center before copy was at pos_partner
+            self.iso_center = pos_partner
+
+        # iso_towards does not normalize (maybe it does inside the truncate methods ...)
+        self.normalize()
+
+        return energy
+
+    #########################################################################
+    ######################## Time evolution methods #########################
+    #########################################################################
+
+    def timestep_single_tensor(self, pos, next_pos, sc):
         """
-        Compute the energy of the TTN through the effective operator
-        at position pos.
+        Time step for a single-tensor update on a single tensor `exp(sc*Heff*dt)`.
 
         Parameters
         ----------
-        pos : list, optional
-            If a position is provided, the isometry is first shifted to
-            that position and then the energy is computed. If None,
-            the current isometry center is computed, by default None
+        pos : Tuple[int] | int
+            Position in the TN of the tensor to time-evolve
+        next_pos: Tuple[int] | int
+            Position in the TN of the next tensor to time-evolve
+        sc : complex
+            Multiplicative factor in the exponent `exp(sc*Heff*dt)`
+
+        Return
+        ------
+        None
+            Acts in place
 
-        Returns
-        -------
-        float
-            Energy of the TTN
         """
-        xp = self._device_checks()
-        if self.eff_op is None:
-            raise RuntimeError("Tried to compute energy with no effective operators")
-        # Move the iso center if needed
-        if pos is not None:
-            self.iso_towards(pos)
+        self.log_print("Time-step at tensor", pos, next_pos, verbosity_level=3)
+        self.log_print(
+            "Time step at tensor's norm, scalar", self.norm(), sc, verbosity_level=5
+        )
 
-        # Retrieve the tensor at the isometry
-        tens = self[self._iso_center]
-        # Get the list of operators to contract
-        ops_list, ops_idxs = self._get_eff_op_on_pos(self._iso_center)
-        # Contract the tensor with the effective operators around
-        vec = self._contract_tensor_lists(
-            tens.reshape(-1), self._iso_center, ops_list, ops_idxs
+        # Isometrize towards the desired tensor
+        self.iso_towards(pos)
+        pos_links = self.get_pos_links(pos)
+
+        krylov_solver = self._solver(
+            self[pos],
+            sc,
+            self.eff_op.contract_tensor_lists,
+            self._convergence_parameters,
+            args_func=(pos, pos_links),
         )
 
-        # Contract the obtained tensor with the complex conjugate of the tree
-        cidxs = np.arange(len(tens.shape))
-        energy = xp.tensordot(vec.reshape(tens.shape), np.conj(tens), (cidxs, cidxs))
-        if xp == cp:
-            energy = energy.get()
+        self[pos] = krylov_solver.solve()
+
+        if next_pos is not None:
+            # Have to evolve backwards
+            # ------------------------
+            #
+            # This is a bit inconvenient, because we have to shift the isometry
+            # center by hand as the r-tensor has to be evolved backwards in time.
+            (
+                rtens,
+                pos_partner,
+                link_partner,
+                path_elem,
+            ) = self._partial_iso_towards_for_timestep(pos, next_pos)
+
+            # Retrieve operator from partner to iso center
+            ops_a = self.eff_op[(pos_partner, pos)]
+
+            # Path elem src layer-tensor-link, dst layer-tensor-link
+            self._update_eff_ops(path_elem)
+
+            # Needing just one operators, no idxs needed
+            ops_b = self.eff_op[(pos, pos_partner)]
+
+            # Assumed to be in the order of links
+            ops_list_reverse = [ops_b, ops_a]
+
+            krylov_solver = self._solver(
+                rtens,
+                -sc,
+                self.eff_op.contract_tensor_lists,
+                self._convergence_parameters,
+                args_func=(None, None),
+                kwargs_func={"custom_ops": ops_list_reverse},
+            )
 
-        return np.real(energy)
+            rtens = krylov_solver.solve()
 
-    #########################################################################
-    ######################### Optimization methods ##########################
-    #########################################################################
+            tmp = rtens.tensordot(self[pos_partner], ([1], [link_partner]))
+            if link_partner == 0:
+                self[pos_partner] = tmp
+            else:
+                nn = self[pos_partner].ndim
+                perm = (
+                    list(range(1, link_partner + 1))
+                    + [0]
+                    + list(range(link_partner + 1, nn))
+                )
+                self[pos_partner] = tmp.transpose(perm)
+
+            self.iso_center = pos_partner
+
+        return
 
-    def optimize_single_tensor(self, pos, verbose=False):
+    def timestep_two_tensors(self, pos, next_pos, sc, skip_back):
         """
-        Optimize the tensor at position `pos` based on the
-        effective operators loaded in the TTN
+        Time step for a single-tensor update on two tensors `exp(sc*Heff*dt)`.
 
         Parameters
         ----------
-        pos : list of ints or int
-            Position of the tensor in the TN
-        verbose : bool, optional
-            If True, prints informations about the diagonalization.
-            Default to False.
+        pos : Tuple[int] | int
+            Position in the TN of the tensor to time-evolve
+        next_pos: Tuple[int] | int
+            Position in the TN of the next tensor to time-evolve
+        sc : complex
+            Multiplicative factor in the exponent `exp(sc*Heff*dt)`
+        skip_back : bool
+            Flag if backwards propagation of partner tensor can be skipped;
+            used for last two tensors, partner tensor must be next position
+            as well.
+
+        Return
+        ------
+        None
+            Acts in place
+
         """
-        xp, xsla = self._device_checks(return_sla=True)
-        if verbose:
-            print("-" * 50)
-            print(f"Optimizing tensor {pos[1]} in layer {pos[0]}")
-        # Isometrise towards the desired tensor
+        self.log_print("Time-step at tensor", pos, verbosity_level=3)
+
+        # Isometrize towards the desired tensor
         self.iso_towards(pos)
-        # Retrieve the tensor
-        tensor = self[pos]
-        ham_dim = int(np.prod(tensor.shape))
 
-        # Get the list of operators to contract
-        ops_list, ops_idxs = self._get_eff_op_on_pos(self._iso_center)
-        # perform the diagonalization of the effective Hamiltonian
-        # with the ARNOLDI method of ARPACK (in Scipy), by using
-        # the LinearOperator strategy
-        # ------------------------------- IMPORTANT ---------------------------------
-        # | We put a - sign in the linear operator in order to use the              |
-        # | Largest Amplitude search (LA) instead of Smallest Amplitude search (SA) |
-        # | in eigsh routine, since the latter is not available for the GPU.        |
-        # ---------------------------------------------------------------------------
-        lin_op = xsla.LinearOperator(
-            (ham_dim, ham_dim),
-            matvec=lambda v: -self._contract_tensor_lists(v, pos, ops_list, ops_idxs),
-        )
-
-        tolerance = self._convergence_parameters.sim_params["arnoldi_min_tolerance"]
-        if xp == np:
-            eigenvalues, eigenvectors = xsla.eigsh(
-                lin_op,
-                k=1,
-                which="LA",
-                v0=tensor.reshape(-1),
-                ncv=None,
-                maxiter=None,
-                tol=tolerance,
-                return_eigenvectors=True,
+        # pos_partner, link_pos, link_partner = self.get_pos_partner_link_expansion(pos)
+        (
+            link_pos,
+            pos_partner,
+            link_partner,
+            path_elem,
+        ) = self._partial_iso_towards_for_timestep(pos, next_pos, no_rtens=True)
+
+        tens_a = self[pos]
+        tens_b = self[pos_partner]
+        is_a_outgoing = tens_a.are_links_outgoing[link_pos]
+
+        theta = tens_a.tensordot(tens_b, ([link_pos], [link_partner]))
+
+        # Build custom eff ops list
+        custom_ops = []
+        for ii, elem in enumerate(self.get_pos_links(pos)):
+            if ii == link_pos:
+                continue
+
+            if elem is None:
+                custom_ops.append(None)
+            else:
+                custom_ops.append(self.eff_op[(elem, pos)])
+
+        for ii, elem in enumerate(self.get_pos_links(pos_partner)):
+            if ii == link_partner:
+                continue
+
+            if elem is None:
+                custom_ops.append(None)
+            else:
+                custom_ops.append(self.eff_op[(elem, pos_partner)])
+
+        custom_ops, theta, inv_perm = self.permute_spo_for_two_tensors(
+            custom_ops, theta, link_partner
+        )
+        krylov_solver = self._solver(
+            theta,
+            sc,
+            self.eff_op.contract_tensor_lists,
+            self._convergence_parameters,
+            args_func=(None, None),
+            kwargs_func={"custom_ops": custom_ops},
+        )
+
+        theta = krylov_solver.solve()
+
+        if inv_perm is not None:
+            theta.transpose_update(inv_perm)
+
+        links_a = list(range(tens_a.ndim - 1))
+        links_b = list(range(tens_a.ndim - 1, theta.ndim))
+
+        tens_a, tens_b, svals, svals_cut = theta.split_svd(
+            links_a,
+            links_b,
+            contract_singvals="R",
+            conv_params=self._convergence_parameters,
+            is_link_outgoing_left=is_a_outgoing,
+        )
+
+        svals_cut = self._postprocess_singvals_cut(
+            singvals_cut=svals_cut, conv_params=self._convergence_parameters
+        )
+        svals_cut = theta.get_of(svals_cut)
+
+        self.set_singvals_on_link(pos, pos_partner, svals)
+
+        nn = tens_a.ndim
+        perm_a = list(range(link_pos)) + [nn - 1] + list(range(link_pos, nn - 1))
+        self[pos] = tens_a.transpose(perm_a)
+
+        nn = tens_b.ndim
+        perm_b = (
+            list(range(1, link_partner + 1)) + [0] + list(range(link_partner + 1, nn))
+        )
+        self[pos_partner] = tens_b.transpose(perm_b)
+
+        self._update_eff_ops(path_elem)
+        self.iso_center = pos_partner
+
+        if not skip_back:
+            # Have to evolve backwards
+            # ------------------------
+
+            pos_links = self.get_pos_links(pos_partner)
+
+            krylov_solver = self._solver(
+                self[pos_partner],
+                -sc,
+                self.eff_op.contract_tensor_lists,
+                self._convergence_parameters,
+                args_func=(pos_partner, pos_links),
             )
+
+            self[pos_partner] = krylov_solver.solve()
+        elif pos_partner != next_pos:
+            raise Exception("Sweep order incompatible with two-tensor update.")
+
+        return
+
+    def timestep_single_tensor_link_expansion(self, pos, next_pos, sc):
+        """
+        Time step for a single-tensor update on two tensors `exp(sc*Heff*dt)`.
+
+        Parameters
+        ----------
+        pos : Tuple[int] | int
+            Position in the TN of the tensor to time-evolve
+        next_pos: Tuple[int] | int
+            Position in the TN of the next tensor to time-evolve
+        sc : complex
+            Multiplicative factor in the exponent `exp(sc*Heff*dt)`
+
+        Return
+        ------
+        None
+            Acts in place
+
+        """
+        requires_singvals = True
+        self.log_print(
+            "Time-step with link expansion at tensor", pos, verbosity_level=3
+        )
+
+        if next_pos is None:
+            self.timestep_single_tensor(pos, next_pos, sc)
+            return
+
+        self.iso_towards(
+            next_pos, trunc=requires_singvals, keep_singvals=requires_singvals
+        )
+
+        (
+            link_self,
+            pos_partner,
+            link_partner,
+            _,
+        ) = self._partial_iso_towards_for_timestep(pos, next_pos, no_rtens=True)
+
+        tensor = self[pos].copy()
+        tensor_partner = self[pos_partner].copy()
+
+        # Expand the tensors
+        new_dim = max(
+            tensor.shape[link_self]
+            + self._convergence_parameters.sim_params["min_expansion"],
+            np.delete(list(tensor.shape), link_self).prod(),
+        )
+
+        self[pos], self[pos_partner] = tensor.expand_link_tensorpair(
+            tensor_partner, link_self, link_partner, new_dim, ctrl="Z"
+        )
+        # Update of eff operators (internal iso_towards in space link
+        # expansion cannot truncate or update singvals)
+        self.iso_towards(pos)
+
+        # Expansion cycles
+        # ----------------
+
+        # Same here, use QR as otherwise truncation kicks in potentially]
+        # undoing the expansion. Final iso_towards with QR or SVD follows
+        # after expansion cycles.
+        exp_cycles = self._convergence_parameters.sim_params["expansion_cycles"]
+
+        sc_e = sc / exp_cycles
+        for ii in range(exp_cycles):
+            self.iso_towards(pos)
+            self.timestep_single_tensor(pos, pos_partner, sc_e)
+
+            if exp_cycles > 1:
+                next_pos_partner = pos if ii < exp_cycles - 1 else None
+                self.timestep_single_tensor(pos_partner, next_pos_partner, sc_e)
+
+        # Evolve back the tensor at pos_partner
+        if exp_cycles > 1:
+            self.timestep_single_tensor(pos_partner, None, -sc)
+            self.iso_towards(
+                pos, trunc=requires_singvals, keep_singvals=requires_singvals
+            )
+            self.iso_towards(
+                pos_partner, trunc=requires_singvals, keep_singvals=requires_singvals
+            )
+
+        return
+
+    def timestep(self, dt, mode, sweep_order=None, sweep_order_back=None):
+        """
+        Evolve the Tensor network for one timestep.
+
+        Parameters
+        ----------
+        mode : int
+            Currently encoded are single-tensor TDVP first order (1), two-tensor
+            TDVP first order (2), two-tensor TDVP second order (3), and single-tensor
+            TDVP second order (4). A flex-TDVP as (5) is pending.
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+        sweep_order_back : List[int] | None
+            Order in which we iterate backwards through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()[::-1]`
+        dt : float
+            Timestep
+
+        Returns
+        -------
+        None
+            Acts in place
+
+        Details
+        -------
+
+        Flex-TDVP in the fortran implementation was using two-tensor updates
+        as long as the maximal bond dimension is not reached and then a ratio
+        of 9 single-tensor updates to 1 two-tensor update step.
+        """
+        if mode == 1:
+            self.timestep_mode_1(dt, sweep_order=sweep_order)
+        elif mode == 2:
+            self.timestep_mode_2(dt, sweep_order=sweep_order)
+        elif mode == 3:
+            self.timestep_mode_3(
+                dt,
+                sweep_order=sweep_order,
+                sweep_order_back=sweep_order_back,
+            )
+        elif mode == 4:
+            self.timestep_mode_4(
+                dt,
+                sweep_order=sweep_order,
+                sweep_order_back=sweep_order_back,
+            )
+        elif mode == 5:
+            self.timestep_mode_5(dt, sweep_order=sweep_order)
         else:
-            eigenvalues, eigenvectors = xsla.eigsh(
-                lin_op,
-                k=1,
-                which="LA",
-                ncv=None,
-                maxiter=None,
-                tol=tolerance,
-                return_eigenvectors=True,
+            raise ValueError(f"Time evolution mode {mode} not available.")
+
+    def timestep_mode_1(self, dt, sweep_order=None):
+        """
+        Evolve the Tensor network for one timestep (single-tensor update
+        1st order).
+
+        Parameters
+        ----------
+        dt : float
+            Timestep
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+
+        Returns
+        -------
+        None
+            Acts in place
+        """
+        if sweep_order is None:
+            sweep_order = self.default_sweep_order()
+
+        for ii, pos in enumerate(sweep_order):
+            # 1st order update
+            next_pos = None if (ii + 1 == len(sweep_order)) else sweep_order[ii + 1]
+            self.timestep_single_tensor(pos, next_pos, -1j * dt)
+
+    def timestep_mode_2(self, dt, sweep_order=None):
+        """
+        Evolve the Tensor network for one timestep (two-tensor update
+        1st order).
+
+        Parameters
+        ----------
+        dt : float
+            Timestep
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+
+        Returns
+        -------
+        None
+            Acts in place
+        """
+        if sweep_order is None:
+            sweep_order = self.default_sweep_order()
+
+        for ii, pos in enumerate(sweep_order):
+            # 1st order update
+            next_pos = None if (ii + 1 == len(sweep_order)) else sweep_order[ii + 1]
+            skip_back = ii + 2 == len(sweep_order)
+            self.timestep_two_tensors(pos, next_pos, -1j * dt, skip_back)
+
+            if skip_back:
+                break
+
+    def timestep_mode_3(self, dt, sweep_order=None, sweep_order_back=None):
+        """
+        Evolve the Tensor network for one timestep (two-tensor update
+        2nd order).
+
+        Parameters
+        ----------
+        dt : float
+            Timestep
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+        sweep_order_back : List[int] | None
+            Order in which we iterate backwards through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()[::-1]`
+
+        Returns
+        -------
+        None
+            Acts in place
+        """
+        self.timestep_mode_2(0.5 * dt, sweep_order=sweep_order)
+
+        if sweep_order_back is None:
+            sweep_order_back = self.default_sweep_order_back()
+
+        self.timestep_mode_2(0.5 * dt, sweep_order=sweep_order_back)
+
+    def timestep_mode_4(self, dt, sweep_order=None, sweep_order_back=None):
+        """
+        Evolve the Tensor network for one timestep (single-tensor update
+        2nd order).
+
+        Parameters
+        ----------
+        dt : float
+            Timestep
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+        sweep_order_back : List[int] | None
+            Order in which we iterate backwards through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()[::-1]`
+
+        Returns
+        -------
+        None
+            Acts in place
+        """
+        self.timestep_mode_1(0.5 * dt, sweep_order=sweep_order)
+
+        if sweep_order_back is None:
+            sweep_order_back = self.default_sweep_order_back()
+
+        self.timestep_mode_1(0.5 * dt, sweep_order=sweep_order_back)
+
+    def timestep_mode_5(self, dt, sweep_order=None, stride_two_tensor=10):
+        """
+        Evolve the Tensor network for one timestep (mixed two-tensor and
+        one-tensor update, first order).
+
+        Parameters
+        ----------
+        dt : float
+            Timestep
+        sweep_order : List[int] | None
+            Order in which we iterate through the network for the timestep.
+            If None, use the default in `self.default_sweep_order()`
+        stride_two_tensor: int
+            If maximum bond dimension is reached, do a two-tensor update
+            every `stride_two_tensor` steps.
+
+        Returns
+        -------
+        None
+            Acts in place
+        """
+        if sweep_order is None:
+            sweep_order = self.default_sweep_order()
+
+        idx = self._timestep_mode_5_counter
+        self._timestep_mode_5_counter += 1
+
+        # For the main loop, we always evolve the R-tensor back in time
+        skip_back = False
+
+        for ii, pos in enumerate(sweep_order[:-2]):
+            # Everything but the last two
+            next_pos = sweep_order[ii + 1]
+
+            link_pos, _, _, _ = self._partial_iso_towards_for_timestep(
+                pos, next_pos, no_rtens=True
             )
 
-        # Substitute old tensor with new optimized tensor
-        self[pos] = eigenvectors.reshape(tensor.shape)
-        if verbose:
-            print(f"New energy is E={np.real(eigenvalues[0])}")
-            print("-" * 50)
+            is_link_full = self[pos].is_link_full(link_pos)
+            enforce_two_tensor = idx % stride_two_tensor == 0
+            do_two_tensor = (not is_link_full) or enforce_two_tensor
+
+            if do_two_tensor:
+                self.timestep_two_tensors(pos, next_pos, -1j * dt, skip_back)
+            else:
+                self.timestep_single_tensor(pos, next_pos, -1j * dt)
+
+        # Treat the last two tensors (cannot decide individually on update-scheme)
+        pos = sweep_order[-2]
+        next_pos = sweep_order[-1]
+        link_pos, pos_partner, link_partner, _ = self._partial_iso_towards_for_timestep(
+            pos, next_pos, no_rtens=True
+        )
+
+        is_link_full_a = self[pos].is_link_full(link_pos)
+        is_link_full_b = self[pos_partner].is_link_full(link_partner)
+        is_link_full = is_link_full_a or is_link_full_b
+        enforce_two_tensor = idx % stride_two_tensor == 0
+        do_two_tensor = (not is_link_full) or enforce_two_tensor
+
+        if do_two_tensor:
+            skip_back = True
+            self.timestep_two_tensors(pos, next_pos, -1j * dt, True)
+        else:
+            self.timestep_single_tensor(pos, next_pos, -1j * dt)
+            self.timestep_single_tensor(next_pos, None, -1j * dt)
 
     #########################################################################
     ########################## Observables methods ##########################
     #########################################################################
     def check_obs_input(self, ops, idxs=None):
         """
         Check if the observables are in the right
@@ -1749,25 +2167,25 @@
         ------
         None
         """
         if np.isscalar(self.local_dim):
             local_dim = np.repeat(self.local_dim, self.num_sites)
         else:
             local_dim = self.local_dim
-        if not np.all(local_dim == local_dim[0]):
+        if not np.all(np.array(local_dim) == local_dim[0]):
             raise RuntimeError("Measurement not defined for non-constant local_dim")
 
         if idxs is None:
             ops = [ops]
 
-        for op in ops:
-            if list(op.shape) != [local_dim[0]] * 2:
-                raise ValueError(
-                    "Input operator should be of shape (local_dim, local_dim)"
-                )
+        # for op in ops:
+        #    if list(op.shape) != [local_dim[0]] * 2:
+        #        raise ValueError(
+        #            "Input operator should be of shape (local_dim, local_dim)"
+        #        )
 
         if idxs is not None:
             if len(idxs) != len(ops):
                 raise ValueError(
                     "The number of indexes must match the number of operators"
                 )
 
@@ -1790,21 +2208,15 @@
         to_ : int
             Index of the process where to send the tensor
 
         Returns
         -------
         None
         """
-        # Send the dim of the shape
-        self.comm.send(tensor.ndim, to_)
-        shape = np.array(list(tensor.shape), dtype=int)
-        # Send the shape first
-        self.comm.Send([shape, TN_MPI_TYPES["<i8"]], to_)
-        # Send the tensor
-        self.comm.Send([tensor, TN_MPI_TYPES[tensor.dtype.str]], to_)
+        tensor.mpi_send(to_, self.comm, TN_MPI_TYPES)
 
     def mpi_receive_tensor(self, from_):
         """
         Receive the tensor from the process `from_`.
 
 
         Parameters
@@ -1813,26 +2225,103 @@
             Index of the process that sent the tensor
 
         Returns
         -------
         xp.ndarray
             Received tensor
         """
-        # Receive the number of legs
-        ndim = self.comm.recv(source=from_)
+        return self._tensor_backend.tensor_cls.mpi_recv(
+            from_, self.comm, TN_MPI_TYPES, self._tensor_backend
+        )
+
+    def reinstall_isometry_parallel(self, *args, **kwargs):
+        """
+        Reinstall the isometry in a parallel TN parallely
+        """
+        # Empty on porpouse: depends on TN ansatz and
+        # it is used ONLY for MPI-distributed ansatzes
+
+    def reinstall_isometry_serial(self, *args, **kwargs):
+        """
+        Reinstall the isometry in a parallel TN serially
+        """
+        # Empty on porpouse: depends on TN ansatz and
+        # it is used ONLY for MPI-distributed ansatzes
+
+    @staticmethod
+    def matrix_to_tensorlist(
+        matrix, n_sites, dim, conv_params, tensor_backend=TensorBackend()
+    ):
+        """
+        For a given matrix returns dense MPO form decomposing with SVDs
 
-        # Receive the shape
-        shape = np.empty(ndim, dtype=int)
-        self.comm.Recv([shape, TN_MPI_TYPES["<i8"]], from_)
-
-        # Receive the tensor
-        tens = np.empty(shape, dtype=self.dtype)
-        self.comm.Recv([tens, TN_MPI_TYPES[np.dtype(self.dtype).str]], from_)
+        Parameters
+        ----------
+        matrix : ndarray
+            Matrix to write in LPTN(MPO) format
+        n_sites : int
+            Number of sites
+        dim : int
+            Local Hilbert space dimension
+        conv_params : :py:class:`TNConvergenceParameters`
+            Input for handling convergence parameters.
+            In particular, in the LPTN simulator we
+            are interested in:
+            - the maximum bond dimension (max_bond_dimension)
+            - the cut ratio (cut_ratio) after which the
+            singular values in SVD are neglected, all
+            singular values such that
+            :math:`\\lambda` /:math:`\\lambda_max`
+            <= :math:`\\epsilon` are truncated
+        tensor_backend : instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
+        Return
+        ------
+        List[QteaTensor]
+            List of tensor, the MPO decomposition of the matrix
+        """
+
+        if not isinstance(matrix, tensor_backend.tensor_cls):
+            matrix = tensor_backend.tensor_cls.from_elem_array(matrix)
+
+        bond_dim = 1
+        tensorlist = []
+        work = matrix
+        for ii in range(0, n_sites - 1):
+            #                dim  dim**(n_sites-1)
+            #  |                 ||
+            #  O  --[unfuse]-->  O   --[fuse upper and lower legs]-->
+            #  |                 ||
+            #
+            # ==O==  --[SVD, truncating]-->  ==O-o-O==
+            #
+            #                 | |
+            #  --[unfuse]-->  O-O           ---iterate
+            #                 | |
+            #             dim   dim**(n_sites-1)
+            work = np.reshape(
+                work,
+                (
+                    bond_dim,
+                    dim,
+                    dim ** (n_sites - 1 - ii),
+                    dim,
+                    dim ** (n_sites - 1 - ii),
+                ),
+            )
+            tens_left, work, _, _ = work.split_svd(
+                [0, 1, 3], [2, 4], contract_singvals="R", conv_params=conv_params
+            )
+            tensorlist.append(tens_left)
+            bond_dim = deepcopy(work.shape[0])
+        work = work.reshape((work.shape[0], dim, dim, 1))
+        tensorlist.append(work)
 
-        return tens
+        return tensorlist
 
 
 def postprocess_statedict(state_dict, local_dim=2, qiskit_convention=False):
     """
     Remove commas from the states defined as keys of statedict
     and, if `qiskit_convention=True` invert the order of the
     digits following the qiskit convention
@@ -1969,44 +2458,43 @@
 
     # Sort the array
     samples = np.sort(samples)
 
     return samples, bound_probabilities
 
 
-def _transpose_idx(num_legs, contracted_idx):
+def _projector(idxs, shape, xp=np):
     """
-    Transpose in the original order the indexes
-    of a n-legs tensor contracted over the
-    index `contracted_idx`
+    Generate a projector of a given shape on the
+    subspace identified by the indexes idxs
 
     Parameters
     ----------
-    contracted_idx : int
-        Index over which there has been a contraction
-
-    Returns
-    -------
-    tuple
-        Indexes for the transposition
+    idxs : int or array-like of ints
+        Indexes where the diagonal of the projector is 1,
+        i.e. identifying the projector subspace
+    shape : int or array-like of ints
+        Dimensions of the projector. If an int, it is
+        assumed a square matrix
+    xp : module handle
+        Module handle for the creation of the projector.
+        Possible are np (cpu) or cp (cpu). Default to np.
     """
-    if contracted_idx > num_legs - 1:
-        raise ValueError(
-            f"Cannot contract leg {contracted_idx} of tensor with {num_legs} legs"
-        )
-    # Until the contracted idx the ordering is correct
-    idxs = np.arange(contracted_idx)
-    # Then the last
-    idxs = np.append(idxs, num_legs - 1)
-    idxs = np.hstack((idxs, np.arange(contracted_idx, num_legs - 1)))
+    if np.isscalar(idxs):
+        idxs = [idxs]
+    if np.isscalar(shape):
+        shape = (shape, shape)
 
-    return idxs
+    idxs = np.array(idxs, dtype=int)
+    projector = xp.zeros(shape)
+    projector[idxs, idxs] = 1
+    return projector
 
 
-def _projector(idxs, shape, xp=np):
+def _projector_for_rho_i(idxs, rho_i):
     """
     Generate a projector of a given shape on the
     subspace identified by the indexes idxs
 
     Parameters
     ----------
     idxs : int or array-like of ints
@@ -2017,20 +2505,19 @@
         assumed a square matrix
     xp : module handle
         Module handle for the creation of the projector.
         Possible are np (cpu) or cp (cpu). Default to np.
     """
     if np.isscalar(idxs):
         idxs = [idxs]
-    if np.isscalar(shape):
-        shape = (shape, shape)
 
-    idxs = np.array(idxs, dtype=int)
-    projector = xp.zeros(shape)
-    projector[idxs, idxs] = 1
+    projector = rho_i.zeros_like()
+    for ii in idxs:
+        projector.set_diagonal_entry(ii, 1.0)
+
     return projector
 
 
 def _mp_precision_check(precision):
     """
     Based on the precision selected, gives
     a wrapper around the initialization of
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/ed_simulation.py` & `qtealeaves-1.1.1/qtealeaves/emulator/ed_simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,33 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
+# pylint: disable=too-many-branches
+# pylint: disable=too-many-statements
+
 """
 The module contains a light-weight execution of an exact state simulation.
 """
 import os
+
+# pylint: disable-next=no-member, no-name-in-module
 import os.path
 from copy import deepcopy
 import numpy as np
 import scipy.linalg as sla
 
+from qtealeaves.tensors import TensorBackend
+
 from .state_simulator import StateVector
 from .ttn_simulator import TTN
-
+from ..solvers.krylovexp_solver import KrylovSolverH
 
 __all__ = ["run_ed_simulation"]
 
 
 def run_ed_simulation(simulation, params):
     """
     Run a full simulation with the exact state vector.
@@ -69,41 +76,71 @@
     else:
         state = StateVector.from_groundstate(ham, num_sites, local_dim)
 
     # Measurements
     folder_name_output = simulation.observables.get_folder_trajectories(
         simulation.folder_name_output, params
     )
-
+    # pylint: disable-next=no-member
     full_file_path = os.path.join(folder_name_output, "static_obs.dat")
 
     observables = run_ed_measurements(state, ham, simulation, params)
     observables.write_results(full_file_path, state.is_measured, params)
 
     # Dynamics
     # --------
 
     quench_list = params["Quenches"] if ("Quenches" in params) else []
-    time_now = 0.0
 
+    # convert the dtype of the initial state to complex
+    if len(quench_list) > 0:
+        state.state = state.state.astype(np.complex128)
+
+    time_now = 0.0
     idx = 0
     for ii, quench in enumerate(quench_list):
+        time_evolution_mode = quench.time_evolution_mode
+        if time_evolution_mode not in [0, 10, 11]:
+            raise Exception(
+                f"""Exact diagonalisation requires
+                time_evolution_mode 0, 10 or 11, got {time_evolution_mode}."""
+            )
+        # automatic time_evolution_mode selection depending on the system size
+        if time_evolution_mode == 0:
+            if num_sites < 10:
+                time_evolution_mode = 10
+            else:
+                time_evolution_mode = 11
+
         for dt in quench.iter_params_dts(params):
             if dt > 0.0:
                 # Time step
                 time_mid = time_now + 0.5 * dt
 
                 params_tt = deepcopy(params)
                 for key, func in quench.items():
                     params_tt[key] = func(time_mid, params)
 
-                ham = simulation.model.build_ham(simulation.operators, params_tt)
-
-                propagator = sla.expm(-1j * dt * ham)
-                state.apply_global_operator(propagator)
+                # by default construct the full H matrix
+                if time_evolution_mode == 10:
+                    ham = simulation.model.build_ham(simulation.operators, params_tt)
+
+                    propagator = sla.expm(-1j * dt * ham)
+                    state.apply_global_operator(propagator)
+
+                # or do the Krylov expansion
+                elif time_evolution_mode == 11:
+                    # update the state
+                    state = KrylovSolverH(
+                        vec0=state,
+                        prefactor=-1j * dt,
+                        matvec_func=simulation.model.apply_ham_to_state,
+                        conv_params=simulation.convergence,
+                        args_func=[simulation.operators, params_tt],
+                    ).solve()
 
                 # Increase evolution time and index
                 time_now += dt
                 idx += 1
 
             elif np.isclose(dt, 0.0):
                 # Measurement
@@ -115,14 +152,15 @@
 
                 postfix = "_%08d_%08d" % (ii, idx)
                 observables = run_ed_measurements(
                     state, ham, simulation, params, postfix=postfix, time=time_now
                 )
 
                 file_name = "dyn_obs%08d_%08d.dat" % (1, idx)
+                # pylint: disable-next=no-member
                 full_file_path = os.path.join(folder_name_output, file_name)
                 observables.write_results(full_file_path, state.is_measured, params)
 
             else:
                 # Skipped measurement
                 pass
 
@@ -226,15 +264,15 @@
     # --------------------
 
     dist_obs = observables.obs_list["TNDistance2Pure"]
 
     for jj, name_jj in enumerate(dist_obs.name):
         path_jj = dist_obs.path_to_state[jj]
 
-        psi_ttn = TTN.read(path_jj)
+        psi_ttn = TTN.read(path_jj, TensorBackend())
         psi_vec = psi_ttn.to_statevector()
 
         dist_obs.results_buffer[name_jj] = state.dot(psi_vec)
 
     # State2File measurement
     # ----------------------
     #
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/lptn_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/lptn_simulator.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,30 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 This module contains a light-weight LPTN emulator.
 """
+
+# pylint: disable=protected-access
+# pylint: disable=too-many-lines
+# pylint: disable=too-many-branches
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-locals
+# pylint: disable=too-many-public-methods
+
 from copy import deepcopy
+import warnings
 import numpy as np
 import numpy.linalg as nla
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from ..fortran_interfaces import write_tensor, read_tensor
+from qtealeaves.tensors import _AbstractQteaTensor
 from .abstract_tn import _AbstractTN
+from .mps_simulator import MPS
 
 
 class LPTN(_AbstractTN):
     """
     LOCALLY PURIFIED TENSOR NETWORK CLASS - operator
     order of legs: 0 - left bond, 1 - lower (physical) leg,
     2 - upper leg, 3 - right bond
@@ -41,23 +51,22 @@
         :math:`\\lambda` /:math:`\\lambda_max`
         <= :math:`\\epsilon` are truncated
 
     local_dim : int, optional
         Dimension of Hilbert space of single site
         (defined as the same for each site).
         Default is 2
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
     iso_center : None or list of two ints, optional
         Isometry center is between the two sites
         specified in a list. The counting starts at 1.
         If the LPTN has no
         isometry center, iso_center = None.
         Default is None
-    dtype : dtype, optional
-        Type of entries for the tensor.
-        Default is np.complex128
 
     Initialization
     --------------
 
     |000...000><000---000|
 
     Tensor representation
@@ -90,25 +99,38 @@
     LPTN.iso_center : None or list of int, optional
         Isometry center is between the two sites
         specified in a list. The counting starts at 1.
         If the LPTN has no
         isometry center, iso_center = None.
     """
 
+    extension = "lptn"
+
     def __init__(
-        self, num_sites, conv_params, local_dim=2, iso_center=None, dtype=np.complex128
+        self,
+        num_sites,
+        conv_params,
+        local_dim=2,
+        tensor_backend=None,
+        iso_center=None,
+        **kwargs,
     ):
-        super().__init__(num_sites, conv_params, local_dim=local_dim)
+        if "initialize" in kwargs:
+            raise Exception("Input ignored.")
+        if "sectors" in kwargs:
+            raise Exception("Input ignored.")
 
-        self.dtype = dtype
+        super().__init__(
+            num_sites, conv_params, local_dim=local_dim, tensor_backend=tensor_backend
+        )
 
         # initialize tensors as |00...0>
-        one_site = np.zeros((1, local_dim, local_dim, 1), dtype=dtype)
-        one_site[0, 0, 0, 0] = 1
-        default = [one_site for ii in np.repeat(None, num_sites)]
+        shape = [1, local_dim, local_dim, 1]
+        tensor_backend = self._tensor_backend
+        default = [tensor_backend(shape, ctrl="ground") for _ in range(num_sites)]
         self.tensors = default
 
         if isinstance(iso_center, (np.ndarray, list)):
             if not all(isinstance(element, int) for element in iso_center) or (
                 len(iso_center) != 2
             ):
                 raise TypeError(
@@ -119,24 +141,45 @@
                 )
 
         elif iso_center is not None:
             raise TypeError(
                 f"iso_center must be None or list of two ints, not {type(iso_center)}."
             )
 
-        self.iso_center = iso_center
+        self._iso_center = iso_center
+
+        # LPTN initializetion not aware of device or data type
+        self.convert(self._tensor_backend.dtype, self._tensor_backend.device)
+
+    # --------------------------------------------------------------------------
+    #                               Properties
+    # --------------------------------------------------------------------------
+
+    @property
+    def default_iso_pos(self):
+        """
+        Returns default isometry center position, e.g., for initialziation
+        of effective operators.
+        """
+        raise NotImplementedError(
+            "Default should be similar to MPS, but here it is a list."
+        )
 
     @property
     def cc_tensors(self):
         """
         complex conjugate part of LPTN, returns complex conjugate tensors
         """
-        c_conj = [np.conjugate(x) for x in self.tensors]
+        c_conj = [elem.conj() for elem in self.tensors]
         return c_conj
 
+    # --------------------------------------------------------------------------
+    #                          Overwritten operators
+    # --------------------------------------------------------------------------
+
     def __len__(self):
         """
         Provide number of sites in the LPTN
         """
         return self.num_sites
 
     def __getitem__(self, key):
@@ -174,45 +217,482 @@
         value : np.array
             value of the new tensor
 
         Return
         ------
         None
         """
-        if not isinstance(value, np.ndarray):
-            raise TypeError("New tensor must be a numpy array, not {type(value)}")
+        if not isinstance(value, _AbstractQteaTensor):
+            raise TypeError(
+                "New tensor must be a _AbstracQteaTensor, not {type(value)}"
+            )
         self.tensors[key] = value
 
         return None
 
+    # --------------------------------------------------------------------------
+    #                       classmethod, classmethod like
+    # --------------------------------------------------------------------------
+
+    @classmethod
+    def from_statevector(
+        cls, statevector, local_dim=2, conv_params=None, tensor_backend=None
+    ):
+        """Decompose statevector to tensor network."""
+        psi = MPS.from_statevector(
+            statevector,
+            local_dim=local_dim,
+            conv_params=conv_params,
+            tensor_backend=tensor_backend,
+        )
+
+        return cls.from_tensor_list_mps(psi.to_tensor_list())
+
+    @classmethod
+    def from_tensor_list(
+        cls, tensor_list, conv_params=None, iso_center=None, tensor_backend=None
+    ):
+        """
+        Initialize the LPTN tensors using a list of correctly
+        shaped tensors
+
+        Parameters
+        ----------
+        tensor_list : list of ndarrays
+            List of tensors for initializing the LPTN
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Input for handling convergence parameters.
+            In particular, in the LPTN simulator we
+            are interested in:
+            - the maximum bond dimension (`max_bond_dimension`)
+            - the cut ratio (`cut_ratio`) after which the
+            singular values in SVD are neglected, all
+            singular values such that :math:`\\lambda` /
+            :math:`\\lambda_max` <= :math:`\\epsilon` are truncated
+        iso_center : None or list of int, optional
+            Isometry center is between the two sites
+            specified in a list. If the LPTN has no
+            isometry center, iso_center = None.
+            Default is None
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
+        Return
+        ------
+        obj : :py:class:`LPTN`
+            The LPTN class composed of the given tensors
+        --------------------------------------------------------------------
+        """
+        local_dim = tensor_list[0].shape[1]
+        max_bond_dim = deepcopy(local_dim)
+        for tens in enumerate(tensor_list):
+            t_shape = tens[1].shape
+            max_bond_dim = max(max_bond_dim, t_shape[0])
+
+        if conv_params is None:
+            conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
+        obj = cls(
+            len(tensor_list),
+            conv_params=conv_params,
+            local_dim=local_dim,
+            tensor_backend=tensor_backend,
+        )
+        obj.tensors = tensor_list
+        obj.iso_center = iso_center
+
+        # Ensure we have _AbstractQteaTensors from here on
+        tensor_cls = obj._tensor_backend.tensor_cls
+        for ii, elem in enumerate(obj.tensors):
+            if not isinstance(elem, _AbstractQteaTensor):
+                obj.tensors[ii] = tensor_cls.from_elem_array(elem)
+
+        obj.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
+        return obj
+
+    @classmethod
+    def from_tensor_list_mps(cls, tensor_list, conv_params=None, iso_center=None):
+        """
+        Initialize the LPTN tensors using a list of MPS
+        shaped tensors. A dummy leg is added and then the function
+        from_tensor_list is called.
+
+        Parameters
+        ----------
+        tensor_list : list of ndarrays
+            List of tensors for initializing the LPTN
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Input for handling convergence parameters.
+            In particular, in the LPTN simulator we
+            are interested in:
+            - the maximum bond dimension (`max_bond_dimension`)
+            - the cut ratio (`cut_ratio`) after which the
+            singular values in SVD are neglected, all
+            singular values such that :math:`\\lambda` /
+            :math:`\\lambda_max` <= :math:`\\epsilon` are truncated
+        iso_center : None or list of int, optional
+            Isometry center is between the two sites
+            specified in a list. If the LPTN has no
+            isometry center, iso_center = None.
+            Default is None
+
+        Return
+        ------
+        obj : :py:class:`LPTN`
+            The LPTN class composed of the given tensors
+        --------------------------------------------------------------------
+        """
+        if iso_center is not None:
+            if len(iso_center) != 2:
+                raise ValueError(
+                    "Iso-center for LPTN has to be of length two (f90-index)."
+                )
+
+        # reshape to rank 4
+        new_tensor_list = []
+        for tens in tensor_list:
+            new_tensor_list.append(
+                tens.reshape((tens.shape[0], tens.shape[1], 1, tens.shape[2]))
+            )
+
+        obj = cls.from_tensor_list(
+            tensor_list=new_tensor_list, conv_params=conv_params, iso_center=iso_center
+        )
+
+        # Ensure we have _AbstractQteaTensors from here on
+        for ii, elem in enumerate(obj.tensors):
+            if not isinstance(elem, _AbstractQteaTensor):
+                obj.tensors[ii] = obj._tensor_backend.tensor_cls.from_elem_array(elem)
+
+        obj.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
+        return obj
+
+    @classmethod
+    def dm_to_lptn(
+        cls, rho, n_sites, dim, conv_params, tensor_backend=None, prob=False
+    ):
+        """
+        For a given density matrix in matrix form returns LPTN form
+
+        Parameters
+        ----------
+        rho : ndarray
+            Density matrix
+        n_sites : int
+            Number of sites
+        dim : int
+            Local Hilbert space dimension
+        conv_params : :py:class:`TNConvergenceParameters`
+            Input for handling convergence parameters.
+            In particular, in the LPTN simulator we
+            are interested in:
+            - the maximum bond dimension (max_bond_dimension)
+            - the cut ratio (cut_ratio) after which the
+            singular values in SVD are neglected, all
+            singular values such that
+            :math:`\\lambda` /:math:`\\lambda_max`
+            <= :math:`\\epsilon` are truncated
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+        prob : Boolean, optional
+            If True, returns eigenvalues of initial eigenvalue
+            decomposition. If everything is correct, should
+            correspond to mixed state probabilities
+
+        Return
+        ------
+        rho_lptn : :py:class::`LPTN`
+            Density matrix in LPTN form
+        (if prob==True) :
+        val : 1D np.ndarray
+            Eigenvalues of initial EVD
+            = mixed state probabilities
+        """
+        if not isinstance(n_sites, int):
+            raise TypeError(
+                "Input number of sites must be an integer, not {type(n_sites)}"
+            )
+        if not isinstance(dim, int):
+            raise TypeError(
+                "Input local Hilbert space dimension must be an integer, "
+                "not {type(dim)}"
+            )
+        rho_lptn = cls(
+            n_sites,
+            local_dim=dim,
+            conv_params=conv_params,
+            tensor_backend=tensor_backend,
+        )
+
+        # --O--   --[EVD, no truncating]--> --O--o--O--
+        val, vec = nla.eigh(rho)
+        val, vec = val[::-1], vec[:, ::-1]
+
+        # absorb the eigenvalues,    | --> dimension dim**n_sites
+        # square root to each side,  O
+        # and take only one side:    | --> physical legs, dimension dim**n_sites
+        work = vec * np.sqrt(val)
+        tensorlist = LPTN.matrix_to_tensorlist(
+            work, n_sites, dim, conv_params, tensor_backend=rho_lptn._tensor_backend
+        )
+        rho_lptn.tensors = tensorlist
+        rho_lptn.iso_center = [n_sites - 1, n_sites - 1]
+
+        # Ensure we have _AbstractQteaTensors from here on
+        tensor_cls = rho_lptn._tensor_backend.tensor_cls
+        for ii, elem in enumerate(rho_lptn.tensors):
+            if not isinstance(elem, _AbstractQteaTensor):
+                rho_lptn.tensors[ii] = tensor_cls.from_elem_array(elem)
+
+        rho_lptn.convert(
+            rho_lptn._tensor_backend.dtype, rho_lptn._tensor_backend.device
+        )
+
+        if prob:
+            return rho_lptn, val
+
+        return rho_lptn
+
+    def to_dense(self, true_copy=False):
+        """Convert into a TN with dense tensors (without symmetries)."""
+        if self.has_symmetry:
+            raise NotImplementedError("Cannot convert LPTN with symmetry to dense yet.")
+
+        # Cases without symmetry
+
+        if true_copy:
+            return self.copy()
+
+        return self
+
+    @classmethod
+    def read(cls, filename, tensor_backend, cmplx=True, order="F"):
+        """
+        Read the LPTN written by FORTRAN in a formatted way on file.
+        Reads in column-major order but the output is in row-major.
+
+        Parameters
+        ----------
+        filename: str
+            PATH to the file
+        tensor_backend : :class:`TensorBackend`
+            Setup which tensor class to create.
+        cmplx: bool, optional
+            If True the LPTN is complex, real otherwise. Default to True
+        order: str, optional
+            If 'F' the tensor is transformed from column-major to row-major, if 'C'
+            it is left as read.
+
+        Returns
+        -------
+        obj: py:class:`LPTN`
+            LPTN class read from file
+        """
+        tensors = []
+        with open(filename, "r") as fh:
+            # read real/complex datatype stored in file
+            _ = fh.readline()
+
+            # total number of sites
+            num_sites = int(fh.readline())
+
+            # isometry
+            iso = fh.readline().split()
+            iso_center = [int(iso[0]), int(iso[1])]
+
+            # ds, bc, sr N-N and sr N-N+1
+            for _ in range(num_sites):
+                _ = fh.readline()
+            _ = fh.readline()
+
+            # reading tensors
+            for _ in range(num_sites):
+                tens = tensor_backend.tensor_cls.read(
+                    fh,
+                    tensor_backend.dtype,
+                    tensor_backend.device,
+                    tensor_backend.base_tensor_cls,
+                    cmplx=cmplx,
+                    order=order,
+                )
+                # skip empty lines
+                if not fh.readline():
+                    continue
+                tensors.append(tens)
+
+        obj = cls.from_tensor_list(
+            tensors, iso_center=iso_center, tensor_backend=tensor_backend
+        )
+
+        return obj
+
+    # --------------------------------------------------------------------------
+    #                            Checks and asserts
+    # --------------------------------------------------------------------------
+
+    # --------------------------------------------------------------------------
+    #                     Abstract methods to be implemented
+    # --------------------------------------------------------------------------
+
+    def build_effective_operators(self, measurement_mode=False):
+        """
+        Build the complete effective operator on each
+        of the links. Now assumes `self.eff_op` is set.
+        """
+
+    def _convert_singvals(self, dtype, device):
+        """Convert the singular values of the tensor network to dtype/device."""
+        # No singvals stored
+
+    def get_bipartition_link(self, pos_src, pos_dst):
+        """
+        Returns two sets of sites forming the bipartition of the system for
+        a loopless tensor network. The link is specified via two positions
+        in the tensor network.
+
+        **Arguments**
+
+        pos_src : tuple of two ints
+            Specifies the first tensor and source of the link.
+
+        pos_dst : tuple of two ints
+            Specifies the second tensor and destination of the link.
+
+        **Returns**
+
+        sites_src : list of ints
+            Hilbert space indices when looking from the link towards
+            source tensor and following the links therein.
+
+        sites_dst : list of ints
+            Hilbert space indices when looking from the link towards
+            destination tensor and following the links therein.
+        """
+        if pos_src < pos_dst:
+            return list(range(pos_src + 1)), list(range(pos_src + 1, self.num_sites))
+
+        # pos_src > pos_dst
+        return list(range(pos_dst + 1, self.num_sites)), list(range(pos_dst + 1))
+
+    def get_pos_links(self, pos):
+        """List where links are leading to."""
+        raise NotImplementedError("pos links.")
+
+    def get_rho_i(self, idx):
+        """
+        Calculate the reduced density matrix for a single site.
+
+        Parameters
+        ----------
+        idx : integer
+            Calculate the reduced density matrix of site ``idx``.
+            Recall python indices start at zero.
+
+        Returns
+        -------
+        2D np.ndarray :
+            Reduced density matrix.
+        """
+        return self.reduced_dm(sites=[idx])
+
     def get_tensor_of_site(self, idx):
         """
         Generic function to retrieve the tensor for a specific site. Compatible
         across different tensor network geometries.
 
         Parameters
         ----------
         idx : int
             Return tensor containin the link of the local
             Hilbert space of the idx-th site.
         """
         return self[idx]
 
+    def iso_towards(self, new_iso, keep_singvals=False, trunc=False, conv_params=None):
+        """Shift the isometry center to the tensor"""
+        raise NotImplementedError("iso towards.")
+
+    def _update_eff_ops(self, id_step):
+        """Update the effective operators after isometry movement."""
+        raise NotImplementedError("Easy given MPS function, requires iso_towards first")
+
+    def _partial_iso_towards_for_timestep(self, pos, next_pos, no_rtens=False):
+        """
+        Move by hand the iso for the evolution backwards in time
+        """
+        raise NotImplementedError("Easy given MPS function, requires iso_towards first")
+
+    def default_sweep_order(self):
+        """
+        Default sweep order to be used in the ground state search/time evolution.
+
+        Returns
+        -------
+        List[int]
+            The generator that you can sweep through
+        """
+        return list(range(self.num_sites))
+
+    def get_pos_partner_link_expansion(self, pos):
+        """
+        Get the position of the partner tensor to use in the link expansion
+        subroutine. It is the tensor towards the center, that is supposed to
+        be more entangled w.r.t. the tensor towards the edge
+
+        Parameters
+        ----------
+        pos : int
+            Position w.r.t. which you want to compute the partner
+
+        Returns
+        -------
+        int
+            Position of the partner
+        int
+            Link of pos pointing towards the partner
+        int
+            Link of the partner pointing towards pos
+        """
+        pos_partner = pos + 1 if pos < self.num_sites / 2 else pos - 1
+        link_self = 2 if pos < pos_partner else 0
+        link_partner = 0 if pos < pos_partner else 2
+
+        return pos_partner, link_self, link_partner
+
+    def _iter_tensors(self):
+        """Iterate over all tensors forming the tensor network (for convert etc)."""
+        for tensor in self.tensors:
+            yield tensor
+
     def norm(self):
         """
         Calculate the norm of the state, where the state is X of
         rho = X Xdagger.
         """
         if self.iso_center is None:
             self.install_gauge_center()
 
-        tensor = self[self.iso_center[0]]
-        norm = np.sum(np.real(tensor * np.conj(tensor)))
+        return self[self.iso_center[0]].norm_sqrt()
 
-        return np.sqrt(norm)
+    def scale(self, factor):
+        """
+        Multiply the tensor network state by a scalar factor.
+
+        Parameters
+        ----------
+        factor : float
+            Factor for multiplication of current tensor network state.
+        """
+        if self.iso_center is None:
+            self.install_gauge_center()
+
+        self[self.iso_center[0]] *= factor
+
+    def set_singvals_on_link(self, pos_a, pos_b, s_vals):
+        """Update or set singvals on link via two positions."""
+        warnings.warn("LPTN cannot store singular values yet.")
 
     def site_canonize(self, idx, keep_singvals=False):
         """
         Shift the isometry center to the tensor containing the
         corresponding site, i.e., move the isometry to a specific
         Hilbert space. This method can be implemented independent
         of the tensor network structure.
@@ -226,27 +706,21 @@
             QR decomposition. Default to False.
         """
         if keep_singvals:
             raise ValueError("keep_singvals not implemented for LPTN `site_canonize`")
 
         self.shift_gauge_center([idx, idx + 2])
 
-    def scale(self, factor):
-        """
-        Multiply the tensor network state by a scalar factor.
-
-        Parameters
-        ----------
-        factor : float
-            Factor for multiplication of current tensor network state.
-        """
-        if self.iso_center is None:
-            self.install_gauge_center()
-
-        self[self.iso_center[0]] *= factor
+    # --------------------------------------------------------------------------
+    #                   Choose to overwrite instead of inheriting
+    # --------------------------------------------------------------------------
+
+    # --------------------------------------------------------------------------
+    #                                  Unsorted
+    # --------------------------------------------------------------------------
 
     def print_tensors(self, how_many=None):
         """
         Prints the tensors in LPTN together with their shape
 
         Parameters
         ----------
@@ -325,16 +799,22 @@
                 " for performing Kronecker product with LPTN"
                 " with boundary bond dimension "
                 f"{self.tensors[-1].shape[3]}"
             )
 
         # concatenates the tensors from both LPTN's to one list
         tensor_list = self.tensors + other.tensors
-        max_bond_dim = max(self.max_bond_dim, other.max_bond_dim)
-        cut_ratio = min(self.cut_ratio, other.cut_ratio)
+        max_bond_dim = max(
+            self._convergence_parameters.max_bond_dim,
+            other._convergence_parameters.max_bond_dim,
+        )
+        cut_ratio = min(
+            self._convergence_parameters.cut_ratio,
+            other._convergence_parameters.cut_ratio,
+        )
         conv_params = TNConvergenceParameters(
             max_bond_dimension=max_bond_dim, cut_ratio=cut_ratio
         )
 
         lptn_kron = LPTN.from_tensor_list(
             tensor_list=tensor_list, conv_params=conv_params
         )
@@ -397,15 +877,20 @@
 
         if np.any(np.array(sites[:-1]) > np.array(sites[1:])):
             raise ValueError(
                 "Remaining sites must be ordered from the"
                 " smallest to the largest value."
             )
 
-        if np.log2(self.local_dim ** len(sites)) > max_qubits:
+        if np.isscalar(self.local_dim):
+            dim = self.local_dim ** len(sites)
+        else:
+            dim = np.product(self.local_dim)
+
+        if np.log2(dim) > max_qubits:
             raise RuntimeError(
                 "Cannot generate a density matrix of"
                 f" {len(sites)} qubits. Maximal"
                 " number of qubits a reduced density"
                 f" matrix can have is set to {max_qubits}."
             )
 
@@ -437,54 +922,37 @@
         #  ---O---O---               |   |            ||          |
         #     |   |
 
         # step:            [1]                  [2]         [3]
 
         if len(sites) > 1:
             # step [1]
-            tens_left = np.tensordot(
-                self[sites[0]], np.conj(self[sites[0]]), axes=[[0, 2], [0, 2]]
+            tens_left = self[sites[0]].tensordot(
+                self[sites[0]].conj(), [[0, 2], [0, 2]]
             )
-            tens_right = np.tensordot(
-                self[sites[1]], np.conj(self[sites[1]]), axes=[[2, 3], [2, 3]]
+            tens_right = self[sites[1]].tensordot(
+                self[sites[1]].conj(), [[2, 3], [2, 3]]
             )
+
             # step [2]
-            dm_red = np.tensordot(tens_left, tens_right, axes=[[1, 3], [0, 2]])
-            dm_red = np.transpose(dm_red, axes=[0, 2, 1, 3])
+            dm_red = tens_left.tensordot(tens_right, [[1, 3], [0, 2]])
+            dm_red.transpose_update([0, 2, 1, 3])
             # step [3]
-            dm_red = np.reshape(
-                dm_red,
+            dm_red.reshape_update(
                 (dm_red.shape[0] * dm_red.shape[1], dm_red.shape[2] * dm_red.shape[3]),
             )
 
         # analog procedure with the one tensor, now only step [1] is needed
         else:
-            dm_red = np.tensordot(
-                self[sites[0]], np.conj(self[sites[0]]), axes=[[0, 2, 3], [0, 2, 3]]
+            dm_red = self[sites[0]].tensordot(
+                self[sites[0]].conj(), [[0, 2, 3], [0, 2, 3]]
             )
 
         return dm_red
 
-    def get_rho_i(self, idx):
-        """
-        Calculate the reduced density matrix for a single site.
-
-        Parameters
-        ----------
-        idx : integer
-            Calculate the reduced density matrix of site ``idx``.
-            Recall python indices start at zero.
-
-        Returns
-        -------
-        2D np.ndarray :
-            Reduced density matrix.
-        """
-        return self.reduced_dm(sites=[idx])
-
     def get_rho_ij(self, idx):
         """
         Calculate the reduced density matrix for two
         neighbour sites.
 
         Parameters
         ----------
@@ -525,32 +993,18 @@
         # --(contract R with tensor on the right)->  --Q--O--O--
         #           (Q is now unitary)                 |  |  |
 
         # - repeat the same for the next tensor, and so on until all
         #   the tensors except the last one are unitary.
 
         for ii in range(0, self.num_sites - 1):
-            work = np.reshape(
-                self[ii],
-                (
-                    self[ii].shape[0] * self[ii].shape[1] * self[ii].shape[2],
-                    self[ii].shape[3],
-                ),
-            )
-            q_mat, r_mat = nla.qr(work)
-            self[ii + 1] = np.tensordot(r_mat, self[ii + 1], axes=[[1], [0]])
-            self[ii] = np.reshape(
-                q_mat,
-                (
-                    self[ii].shape[0],
-                    self[ii].shape[1],
-                    self[ii].shape[2],
-                    q_mat.shape[1],
-                ),
-            )
+            q_mat, r_mat = self[ii].split_qr([0, 1, 2], [3])
+
+            self[ii] = q_mat
+            self[ii + 1] = r_mat @ self[ii + 1]
 
         self.iso_center = [self.num_sites - 1, self.num_sites + 1]
         return None
 
     def shift_gauge_center(self, ind_final):
         """
         Shift a gauge center of the LPTN.
@@ -615,155 +1069,29 @@
             return None
         direction = np.sign(center_final - center_init)
 
         # two separate cases for shifting to the left and to the right
 
         if direction > 0:
             for ii in range(center_init, center_final):
-                work = np.reshape(
-                    self[ii],
-                    (
-                        self[ii].shape[0] * self[ii].shape[1] * self[ii].shape[2],
-                        self[ii].shape[3],
-                    ),
-                )
-                q_mat, r_mat = nla.qr(work)
-                self[ii + 1] = np.tensordot(r_mat, self[ii + 1], axes=[[1], [0]])
-                self[ii] = np.reshape(
-                    q_mat,
-                    (
-                        self[ii].shape[0],
-                        self[ii].shape[1],
-                        self[ii].shape[2],
-                        q_mat.shape[1],
-                    ),
-                )
+                q_mat, r_mat = self[ii].split_qr([0, 1, 2], [3])
+
+                self[ii] = q_mat
+                self[ii + 1] = r_mat @ self[ii + 1]
 
         else:
             for ii in range(center_init, center_final, -1):
-                work = np.reshape(
-                    self[ii],
-                    (
-                        self[ii].shape[0],
-                        self[ii].shape[1] * self[ii].shape[2] * self[ii].shape[3],
-                    ),
-                )
-                work = np.transpose(work, axes=[1, 0])
-                q_mat, r_mat = nla.qr(work)
-                q_mat = np.transpose(q_mat, axes=[1, 0])
-                r_mat = np.transpose(r_mat, axes=[1, 0])
-                self[ii - 1] = np.tensordot(self[ii - 1], r_mat, axes=[[3], [0]])
-                self[ii] = np.reshape(
-                    q_mat,
-                    (
-                        q_mat.shape[0],
-                        self[ii].shape[1],
-                        self[ii].shape[2],
-                        self[ii].shape[3],
-                    ),
-                )
+                q_mat, r_mat = self[ii].split_qr([1, 2, 3], [0], perm_left=[3, 0, 1, 2])
+
+                self[ii] = q_mat
+                self[ii - 1] = self[ii - 1].tensordot(r_mat, ([3], [1]))
 
         self.iso_center = [center_final, center_final + 2]
         return None
 
-    @classmethod
-    def from_tensor_list(cls, tensor_list, conv_params=None, iso_center=None):
-        """
-        Initialize the LPTN tensors using a list of correctly
-        shaped tensors
-
-        Parameters
-        ----------
-        tensor_list : list of ndarrays
-            List of tensors for initializing the LPTN
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Input for handling convergence parameters.
-            In particular, in the LPTN simulator we
-            are interested in:
-            - the maximum bond dimension (`max_bond_dimension`)
-            - the cut ratio (`cut_ratio`) after which the
-            singular values in SVD are neglected, all
-            singular values such that :math:`\\lambda` /
-            :math:`\\lambda_max` <= :math:`\\epsilon` are truncated
-        iso_center : None or list of int, optional
-            Isometry center is between the two sites
-            specified in a list. If the LPTN has no
-            isometry center, iso_center = None.
-            Default is None
-
-        Return
-        ------
-        obj : :py:class:`LPTN`
-            The LPTN class composed of the given tensors
-        --------------------------------------------------------------------
-        """
-        local_dim = tensor_list[0].shape[1]
-        max_bond_dim = deepcopy(local_dim)
-        for tens in enumerate(tensor_list):
-            t_shape = tens[1].shape
-            max_bond_dim = max(max_bond_dim, t_shape[0])
-
-        if conv_params is None:
-            conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
-        obj = cls(len(tensor_list), conv_params=conv_params, local_dim=local_dim)
-        obj.tensors = tensor_list
-        obj.iso_center = iso_center
-
-        return obj
-
-    @classmethod
-    def from_tensor_list_mps(cls, tensor_list, conv_params=None, iso_center=None):
-        """
-        Initialize the LPTN tensors using a list of MPS
-        shaped tensors. A dummy leg is added and then the function
-        from_tensor_list is called.
-
-        Parameters
-        ----------
-        tensor_list : list of ndarrays
-            List of tensors for initializing the LPTN
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Input for handling convergence parameters.
-            In particular, in the LPTN simulator we
-            are interested in:
-            - the maximum bond dimension (`max_bond_dimension`)
-            - the cut ratio (`cut_ratio`) after which the
-            singular values in SVD are neglected, all
-            singular values such that :math:`\\lambda` /
-            :math:`\\lambda_max` <= :math:`\\epsilon` are truncated
-        iso_center : None or list of int, optional
-            Isometry center is between the two sites
-            specified in a list. If the LPTN has no
-            isometry center, iso_center = None.
-            Default is None
-
-        Return
-        ------
-        obj : :py:class:`LPTN`
-            The LPTN class composed of the given tensors
-        --------------------------------------------------------------------
-        """
-        if iso_center is not None:
-            if len(iso_center) != 2:
-                raise ValueError(
-                    "Iso-center for LPTN has to be of length two (f90-index)."
-                )
-
-        # reshape to rank 4
-        new_tensor_list = []
-        for tens in tensor_list:
-            new_tensor_list.append(
-                tens.reshape((tens.shape[0], tens.shape[1], 1, tens.shape[2]))
-            )
-
-        obj = cls.from_tensor_list(
-            tensor_list=new_tensor_list, conv_params=conv_params, iso_center=iso_center
-        )
-        return obj
-
     def to_tensor_list_mps(self):
         """
         Return the tensor list representation of the LPTN
         as MPS. If the upper link has dimension one, the tensors
         are reshaped to rank 3.
 
         Return
@@ -773,175 +1101,23 @@
         """
         # check if link of complex conjugate has dimension 1
         for tens in self.tensors:
             if tens.shape[2] != 1:
                 raise Exception(
                     "Tensor with upper leg dimension other than 1 found in the list."
                 )
-
         # reshape to rank 3
         new_tensors = []
         for tens in self.tensors:
             new_tensors.append(
                 tens.reshape((tens.shape[0], tens.shape[1], tens.shape[3]))
             )
 
         return new_tensors
 
-    @classmethod
-    def dm_to_lptn(cls, rho, n_sites, dim, conv_params, prob=False):
-        """
-        For a given density matrix in matrix form returns LPTN form
-
-        Parameters
-        ----------
-        rho : ndarray
-            Density matrix
-        n_sites : int
-            Number of sites
-        dim : int
-            Local Hilbert space dimension
-        conv_params : :py:class:`TNConvergenceParameters`
-            Input for handling convergence parameters.
-            In particular, in the LPTN simulator we
-            are interested in:
-            - the maximum bond dimension (max_bond_dimension)
-            - the cut ratio (cut_ratio) after which the
-            singular values in SVD are neglected, all
-            singular values such that
-            :math:`\\lambda` /:math:`\\lambda_max`
-            <= :math:`\\epsilon` are truncated
-        prob : Boolean, optional
-            If True, returns eigenvalues of initial eigenvalue
-            decomposition. If everything is correct, should
-            correspond to mixed state probabilities
-
-        Return
-        ------
-        rho_lptn : :py:class::`LPTN`
-            Density matrix in LPTN form
-        (if prob==True) :
-        val : 1D np.ndarray
-            Eigenvalues of initial EVD
-            = mixed state probabilities
-        """
-        if not isinstance(n_sites, int):
-            raise TypeError(
-                "Input number of sites must be an integer, not {type(n_sites)}"
-            )
-        if not isinstance(dim, int):
-            raise TypeError(
-                "Input local Hilbert space dimension must be an integer, "
-                "not {type(dim)}"
-            )
-
-        rho_lptn = cls(n_sites, local_dim=dim, conv_params=conv_params)
-        rho_lp = []
-
-        """
-        --O--   --[EVD, no truncating]--> --O--o--O--
-        """
-        val, vec = nla.eigh(rho)
-        val, vec = val[::-1], vec[:, ::-1]
-        """
-        absorb the eigenvalues,    | --> dimension dim**n_sites
-        square root to each side,  O
-        and take only one side:    | --> physical legs, dimension dim**n_sites
-        """
-        work = vec * np.sqrt(val)
-        bond_dim = 1
-        for ii in range(0, n_sites - 1):
-            """
-                           dim  dim**(n_sites-1)
-            |                 ||
-            O  --[unfuse]-->  O   --[fuse upper and lower legs]-->
-            |                 ||
-
-            ==O==  --[SVD, truncating]-->  ==O-o-O==
-
-                           | |
-            --[unfuse]-->  O-O           ---iterate
-                           | |
-                        dim   dim**(n_sites-1)
-            """
-            work = np.reshape(
-                work,
-                (
-                    bond_dim,
-                    dim,
-                    dim ** (n_sites - 1 - ii),
-                    dim,
-                    dim ** (n_sites - 1 - ii),
-                ),
-            )
-            tens_left, work, _, _ = rho_lptn.tSVD(
-                work, [0, 1, 3], [2, 4], contract_singvals="R", conv_params=conv_params
-            )
-            rho_lp.append(tens_left)
-            bond_dim = deepcopy(work.shape[0])
-        work = np.reshape(work, (work.shape[0], dim, dim, 1))
-        rho_lp.append(work)
-
-        rho_lptn.tensors = rho_lp
-
-        if prob:
-            return rho_lptn, val
-
-        return rho_lptn
-
-    @classmethod
-    def read(cls, filename, cmplx=True, order="F"):
-        """
-        Read the LPTN written by FORTRAN in a formatted way on file.
-        Reads in column-major order but the output is in row-major.
-
-        Parameters
-        ----------
-        filename: str
-            PATH to the file
-        cmplx: bool, optional
-            If True the LPTN is complex, real otherwise. Default to True
-        order: str, optional
-            If 'F' the tensor is transformed from column-major to row-major, if 'C'
-            it is left as read.
-
-        Returns
-        -------
-        obj: py:class:`LPTN`
-            LPTN class read from file
-        """
-        tensors = []
-        with open(filename, "r") as fh:
-            # read real/complex datatype stored in file
-            _ = fh.readline()
-
-            # total number of sites
-            num_sites = int(fh.readline())
-
-            # isometry
-            iso = fh.readline().split()
-            iso_center = [int(iso[0]), int(iso[1])]
-
-            # ds, bc, sr N-N and sr N-N+1
-            for _ in range(num_sites):
-                _ = fh.readline()
-            _ = fh.readline()
-
-            # reading tensors
-            for _ in range(num_sites):
-                tens = read_tensor(fh, cmplx=cmplx, order=order)
-                # skip empty lines
-                if not fh.readline():
-                    continue
-                tensors.append(tens)
-
-        obj = cls.from_tensor_list(tensors, iso_center=iso_center)
-
-        return obj
-
     def write(self, filename, cmplx=True):
         """
         Write an LPTN in python format into a FORTRAN format, i.e.
         transforms row-major into column-major
 
         Parameters
         ----------
@@ -969,22 +1145,27 @@
             # local dim, kappa, bond dimension to the left for each site (this
             # information refers to the maximum allowed for kappa and the bond
             # dimension, not to the current one. Usually, this should be overwritten
             # or set from the simulations reading the LPTN, but set it to sensbile
             # value derived from the convergence parameters stored)
             for tens in self.tensors:
                 fh.write(
-                    "%d %d %d\n" % (tens.shape[1], self.max_bond_dim, self.max_bond_dim)
+                    "%d %d %d\n"
+                    % (
+                        tens.shape[1],
+                        self._convergence_parameters.max_bond_dimension,
+                        self._convergence_parameters.max_bond_dimension,
+                    )
                 )
 
             # bond dimension to the right for the last site
             fh.write("%d\n" % (self.tensors[-1].shape[3]))
 
             for tens in self.tensors:
-                write_tensor(tens, fh, cmplx=cmplx)
+                tens.write(fh, cmplx=cmplx)
 
         return None
 
     def _get_children_prob(self, tensor, site_idx, curr_state, do_clear_cache):
         """
         Compute the probability and the relative tensor state of all the
         children of site `site_idx` in the probability tree
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/mpi_mps_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/mpi_mps_simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,28 +48,31 @@
         - the *cut ratio* :math:`\\epsilon` after which the singular
             values are neglected, i.e. if :math:`\\lamda_1` is the
             bigger singular values then after an SVD we neglect all the
             singular values such that :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`
     local_dim: int or list of ints, optional
         Local dimension of the degrees of freedom. Default to 2.
         If a list is given, then it must have length num_sites.
-    dtype: type, optional
-        Type of the entries of the tensors. Default to np.complex128.
+    initialize: str, optional
+        The method for the initialization. Default to "vacuum"
+        Available:
+        - "vacuum", for the |000...0> state
+        - "random", for a random state at given bond dimension
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
 
     """
 
-    implemented_devices = "cpu"
-
     def __init__(
         self,
         num_sites,
         convergence_parameters,
         local_dim=2,
-        dtype=np.complex128,
-        device="cpu",
+        initialize="vacuum",
+        tensor_backend=None,
     ):
         if MPI is None:
             raise ImportError("No module mpi4py found in python environment")
         # MPI variables
         self.comm = MPI.COMM_WORLD
         self.size = self.comm.Get_size()
         self.rank = self.comm.Get_rank()
@@ -79,17 +82,21 @@
         modulus = num_sites % self.size
         local_num_size = int(np.floor(num_sites // self.size))
         self.indexes = [0] + [
             local_num_size + 1 if ii < modulus else local_num_size
             for ii in range(self.size)
         ]
         local_num_size = self.indexes[self.rank + 1]
+
         # indexes takes into account which indexes are in each core
         self.indexes = np.cumsum(self.indexes)
 
+        # The par_map is a dicrionary where the index is the position of the
+        # sites in the full chain, while the value the position on the
+        # subchain in this process
         self.par_map = dict(
             zip(
                 np.arange(
                     self.indexes[self.rank], self.indexes[self.rank + 1], dtype=int
                 ),
                 np.arange(local_num_size, dtype=int),
             )
@@ -100,23 +107,30 @@
             local_num_size += 1
 
         if not np.isscalar(local_dim):
             local_dim = local_dim[
                 self.indexes[self.rank] : self.indexes[self.rank + 1]
                 + int(self.rank != (self.size - 1))
             ]
-        # Only CPU available at the moment with MPI
+
         super().__init__(
-            local_num_size, convergence_parameters, local_dim, dtype, device
+            local_num_size,
+            convergence_parameters,
+            local_dim=local_dim,
+            initialize=initialize,
+            tensor_backend=tensor_backend,
         )
 
+        # MPS initializetion not aware of device
+        self.convert(self._tensor_backend.dtype, self._tensor_backend.device)
+
     @property
     def mpi_dtype(self):
-        """Return the MPI version of the MPS dtype"""
-        return TN_MPI_TYPES[np.dtype(self.dtype).str]
+        """Return the MPI version of the MPS dtype (going via first tensor)"""
+        return TN_MPI_TYPES[np.dtype(self[0].dtype).str]
 
     def apply_one_site_operator(self, op, pos):
         """
         Applies a one operator `op` to the site `pos` of the MPIMPS.
         Instead of communicating the changes on the boundaries we
         perform an additional contraction.
 
@@ -129,15 +143,15 @@
         """
         # Apply the gate on the right MPS
         if pos in self.par_map:
             super().apply_one_site_operator(op, self.par_map[pos])
 
         # For one-qubit gates it is more convenient to apply them both to
         # the real and auxiliary qubits if they are on the boundaries
-        if pos == self.indexes[self.rank] - 1:
+        elif pos - 1 in self.par_map:
             super().apply_one_site_operator(op, self.num_sites - 1)
 
         return None
 
     def apply_two_site_operator(self, op, pos, swap=False, svd=None, parallel=None):
         """
         Applies a two-site operator `op` to the site `pos`, `pos+1` of the MPS.
@@ -164,14 +178,21 @@
 
         Returns
         -------
         singular_values_cutted: ndarray
             Array of singular values cutted, normalized to the biggest singular value
 
         """
+        if not np.isscalar(pos) and len(pos) == 2:
+            pos = min(pos[0], pos[1])
+        elif not np.isscalar(pos):
+            raise ValueError(
+                f"pos should be only scalar or len 2 array-like, not len {len(pos)}"
+            )
+
         # Hardcoded but necessary for compatibility
         svd = True
         parallel = True
 
         if pos in self.par_map:
             res = super().apply_two_site_operator(
                 op, self.par_map[pos], swap, svd=svd, parallel=parallel
@@ -186,44 +207,43 @@
                         TN_MPI_TYPES[self.singvals[1].dtype.str],
                     ],
                     self.rank - 1,
                 )
 
             # Send the information towards the next if it was the last site
             elif self.par_map[pos] == self.num_sites - 2 and self.rank < self.size - 1:
-
                 self.mpi_send_tensor(self[self.num_sites - 1], to_=self.rank + 1)
                 self.comm.Send(
                     [
-                        self.singvals[self.num_sites - 2],
+                        self.singvals[self.num_sites - 1],
                         TN_MPI_TYPES[self.singvals[self.num_sites - 1].dtype.str],
                     ],
                     self.rank + 1,
                 )
 
         else:
-            res = None
-
+            res = []
             # Receive the information from the MPS on the right
             if pos == self.indexes[self.rank + 1] and self.rank < self.size - 1:
                 tens = self.mpi_receive_tensor(from_=self.rank + 1)
+
                 self[self.num_sites - 1] = tens
 
                 singvals = np.empty(tens.shape[2], self.singvals[self.num_sites].dtype)
                 self.comm.Recv(
                     [
                         singvals,
                         TN_MPI_TYPES[self.singvals[self.num_sites].dtype.str],
                     ],
                     self.rank + 1,
                 )
                 self._singvals[self.num_sites] = singvals
 
             # Receive the information from the MPS from the left
-            elif pos == self.indexes[self.rank] - 1 and self.rank > 0:
+            if pos == self.indexes[self.rank] - 1 and self.rank > 0:
                 tens = self.mpi_receive_tensor(from_=self.rank - 1)
                 self[0] = tens
 
                 singvals = np.empty(tens.shape[0], self.singvals[0].dtype)
                 self.comm.Recv(
                     [
                         singvals,
@@ -254,28 +274,29 @@
         Returns
         -------
         meas_state: int
             Measured state
         state_prob : float
             Probability of measuring the output state
         """
-        self.reinstall_isometry()
+        self.reinstall_isometry_serial()
         if site in self.par_map:
             res = super().apply_projective_operator(
                 self.par_map[site], selected_output, remove
             )
 
         # Move informations to further right
-        self.reinstall_isometry(left=False, from_site=site)
+        self.reinstall_isometry_serial(left=False, from_site=site)
         # Move information to the left
-        self.reinstall_isometry()
+        self.reinstall_isometry_serial()
 
         return res
 
-    def reinstall_isometry(self, left=True, from_site=None):
+    # pylint: disable-next=arguments-differ
+    def reinstall_isometry_serial(self, left=True, from_site=None):
         """
         Reinstall the isometry center on position 0 of the full MPS.
 
         This step is serial because we have to serially pass the information
         along the MPS. It cannot be parallelized.
 
         Parameters
@@ -319,14 +340,46 @@
                 self.mpi_send_tensor(self[tidx], to_=to_)
 
             elif self.rank == ii - 1:
                 # Receive tensor
                 tens = self.mpi_receive_tensor(from_=from_)
                 self[self.num_sites - 1 - tidx] = tens
 
+    # pylint: disable-next=arguments-differ
+    def reinstall_isometry_parallel(self, num_cycles):
+        """
+        Reinstall the isometry by applying identities to all even sites and
+        to all odd sites, and repeating for `num_cycles` cycles.
+        The reinstallation is exact for `num_cycles=num_sites/2`.
+        Method from https://arxiv.org/abs/2312.02667
+
+        This step is serial because we have to serially pass the information
+        along the MPS. It cannot be parallelized.
+
+        Parameters
+        ----------
+        num_cycles: int
+            Number of cycles for reinstalling the isometry
+
+        Returns
+        -------
+        None
+        """
+        for _ in range(num_cycles):
+            # Apply on all even sites
+            for ii in range(0, self.tot_sites - 1, 2):
+                self.apply_two_site_operator(
+                    self[0].eye_like(4), ii, svd=True, parallel=True
+                )
+            # Apply on all odd sites
+            for ii in range(1, self.tot_sites - 1, 2):
+                self.apply_two_site_operator(
+                    self[0].eye_like(4), ii, svd=True, parallel=True
+                )
+
     def mpi_gather_tn(self):
         """
         Gather the tensors on process 0.
         We do not use MPI.comm.Gather because we would gather lists of np.arrays
         without using the np.array advantages, making it slower than the single
         communications.
 
@@ -337,18 +390,16 @@
         """
         self.comm.Barrier()
         if self.rank != 0:
             num_tensors = (
                 self.num_sites if self.rank == self.size - 1 else self.num_sites - 1
             )
             for jj in range(num_tensors):
-                self.mpi_send_tensor(np.ascontiguousarray(self[jj]), to_=0)
-
+                self.mpi_send_tensor(self[jj], to_=0)
             tensor_list = None
-
         else:
             tensor_list = [None for _ in range(self.tot_sites)]
             tensor_list[: self.num_sites - 1] = self.tensors[:-1]
 
             tidx = self.num_sites - 1
             for ii in range(1, self.size):
                 num_tensors = self.indexes[ii + 1] - self.indexes[ii]
@@ -378,15 +429,15 @@
         list on np.ndarray or None
             List of tensors on the rank 0 process, None on the others
         """
         self.comm.Barrier()
         if self.rank == 0:
             for ridx, sub_tensorlist in enumerate(tensor_list[1:]):
                 for idx, tens in enumerate(sub_tensorlist):
-                    self.mpi_send_tensor(np.ascontiguousarray(tens), to_=ridx + 1)
+                    self.mpi_send_tensor(tens, to_=ridx + 1)
 
             tensor_list = tensor_list[0]
         else:
             num_tensors = len(tensor_list[self.rank])
             tensor_list = [None for _ in range(num_tensors)]
             for idx in range(num_tensors):
                 tens = self.mpi_receive_tensor(from_=0)
@@ -439,31 +490,32 @@
         else:
             statevect = None
 
         return statevect
 
     @classmethod
     def from_tensor_list(
-        cls, tensor_list, conv_params=None, device="cpu", dtype=np.complex128
+        cls,
+        tensor_list,
+        conv_params=None,
+        tensor_backend=None,
     ):
         """
         Initialize the MPS tensors using a list of correctly shaped tensors
 
         Parameters
         ----------
         tensor_list : list of ndarrays or cupy arrays
             List of tensor for initializing the MPS
         conv_params : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters for the new MPS. If None, the maximum bond
             bond dimension possible is assumed, and a cut_ratio=1e-9.
             Default to None.
-        device : str
-            Computational device. Available 'cpu', 'gpu'. Default to 'cpu'
-        dtype : data type preferably numpy
-            Data type for constructing MPS.
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
 
         Returns
         -------
         obj : :py:class:`MPIMPS`
             The MPIMPS class
         """
         local_dim = []
@@ -473,20 +525,25 @@
             local_dim.append(t_shape[1])
             max_bond_dim = max(max_bond_dim, t_shape[0])
             if ii > 0 and t_shape[0] != tensor_list[ii - 1].shape[2]:
                 raise ValueError(
                     f"The dimension of the left leg of tensor {ii} and "
                     + f"the right leg of tensor {ii-1} must be equal"
                 )
-            tensor_list[ii] = tens.astype(dtype)
 
         if conv_params is None:
             conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
 
-        obj = cls(len(tensor_list), conv_params, local_dim, dtype=dtype, device=device)
+        obj = cls(
+            len(tensor_list), conv_params, local_dim, tensor_backend=tensor_backend
+        )
+
+        # Convert data type (lateron device if GPU enabled?)
+        for elem in tensor_list:
+            elem.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
 
         if obj.rank == 0:
             tensorlist = [
                 tensor_list[
                     obj.indexes[rank] : obj.indexes[rank + 1]
                     + int(rank != obj.size - 1)
                 ]
@@ -506,24 +563,23 @@
 
     @classmethod
     def from_statevector(
         cls,
         statevector,
         local_dim=2,
         conv_params=None,
-        device="cpu",
-        dtype=np.complex128,
+        tensor_backend=None,
     ):
         """Serially decompose the statevector and then initialize the MPS"""
         mps = MPS.from_statevector(
-            statevector, local_dim, conv_params, dtype=dtype, device=device
+            statevector, local_dim, conv_params, tensor_backend=tensor_backend
         )
 
         return cls.from_tensor_list(
-            mps.to_tensor_list(), conv_params, dtype=dtype, device=device
+            mps.to_tensor_list(), conv_params, tensor_backend=tensor_backend
         )
 
     # ---------------------------
     # ----- MEASURE METHODS -----
     # ---------------------------
 
     def meas_local(self, op):
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/mps_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/mps_simulator.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,32 +11,17 @@
 """
 The module contains a light-weight MPS emulator.
 """
 from copy import deepcopy
 from warnings import warn
 from joblib import delayed, Parallel
 import numpy as np
-from numpy import double, linalg as nla
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from ..fortran_interfaces import write_tensor, read_tensor
-from .abstract_tn import _AbstractTN, postprocess_statedict, _projector
-
-# Try to import cupy
-try:
-    import cupy as cp
-    from cupy_backends.cuda.api.runtime import CUDARuntimeError
-
-    try:
-        _ = cp.cuda.Device()
-        GPU_AVAILABLE = True
-    except CUDARuntimeError:
-        GPU_AVAILABLE = False
-except ImportError:
-    cp = None
-    GPU_AVAILABLE = False
+from qtealeaves.tensors import _AbstractQteaTensor
+from .abstract_tn import _AbstractTN, postprocess_statedict, _projector_for_rho_i
 
 __all__ = ["MPS"]
 
 
 class MPS(_AbstractTN):
     """Matrix product states class
 
@@ -51,79 +36,169 @@
         - the *cut ratio* :math:`\\epsilon` after which the singular
             values are neglected, i.e. if :math:`\\lamda_1` is the
             bigger singular values then after an SVD we neglect all the
             singular values such that :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`
     local_dim: int or list of ints, optional
         Local dimension of the degrees of freedom. Default to 2.
         If a list is given, then it must have length num_sites.
-    dtype: type, optional
-        Type of the entries of the tensors. Default to np.complex128.
-    device: string, optional
-        Device where to create the MPS. Default to 'cpu'.
-        Implemented devices:
-        - 'cpu'
-        - 'gpu'
-
+    initialize: str, optional
+        The method for the initialization. Default to "vacuum"
+        Available:
+        - "vacuum", for the |000...0> state
+        - "random", for a random state at given bond dimension
+    requires_singvals : boolean, optional
+        Allows to enforce SVD to have singular values on each link available
+        which might be useful for measurements, e.g., bond entropy (the
+        alternative is traversing the whole TN again to get the bond entropy
+        on each link with an SVD).
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+    sectors : dict, optional
+        Can restrict symmetry sector and/or bond dimension in initialization.
+        If empty, no restriction.
+        Default to None
     """
 
-    implemented_devices = ("cpu", "gpu")
+    extension = "mps"
 
     def __init__(
         self,
         num_sites,
         convergence_parameters,
         local_dim=2,
-        dtype=np.complex128,
-        device="cpu",
+        initialize="vacuum",
+        requires_singvals=False,
+        tensor_backend=None,
+        sectors=None,
+        **kwargs,
     ):
-        _AbstractTN.__init__(
-            self,
+        super().__init__(
             num_sites,
             convergence_parameters,
             local_dim=local_dim,
-            device=device,
-            dtype=dtype,
+            requires_singvals=requires_singvals,
+            tensor_backend=tensor_backend,
         )
 
-        if np.isscalar(local_dim):
-            if local_dim < 2:
-                raise ValueError(
-                    "The local dimension must be at least 2 to show quantum behavior"
-                )
-            self._local_dim = np.repeat(local_dim, num_sites)
-        elif len(local_dim) == self._num_sites:
-            self._local_dim = np.array(local_dim)
-        else:
-            raise ValueError(
-                "An array-like local dimension must have length equal to num_sites"
-            )
-
         # Set orthogonality tracker for left/right-orthogonal form
         self._first_non_orthogonal_left = 0
         self._first_non_orthogonal_right = num_sites - 1
 
+        # We can set numpy double, will be converted
+        self._singvals = [None for _ in range(num_sites + 1)]
+
         # Initialize the tensors to the |000....0> state
         self._tensors = []
-        for ii in range(num_sites):
-            state0 = np.zeros((1, self._local_dim[ii], 1), dtype=dtype)
-            state0[0, 0, 0] = 1
-            self._tensors.append(state0)
-        self._singvals = [np.ones(1, dtype=double) for _ in range(num_sites + 1)]
-
-        # Save device
-        self._device = "cpu"
-        self.to_device(device)
+        self._initialize_mps(initialize)
 
         # Attribute used for computing probabilities. See
         # meas_probabilities for further details
         self._temp_for_prob = {}
 
         # Variable to save the maximum bond dimension reached at any moment
         self.max_bond_dim_reached = 1
 
+        # Each tensor has 3 links, but all tensors share links. So effectively
+        # we have 2 links per tensor, plus one at the beginning and one at the end
+        self.num_links = 2 + 2 * num_sites
+        self.sectors = sectors
+        # Contains the index of the neighboring effective operator in
+        # a 1-d vector of operators. Each vector op_neighbors(:, ii)
+        # contains the index of a link for the ii-th tensor in this layer.
+        # 0-o-2-o-4-o-6-o-8  --->   i -o- i+2
+        #   |1  |3  |4  |5             | i+1
+        self.op_neighbors = np.zeros((3, num_sites), dtype=int)
+        self.op_neighbors[0, :] = np.arange(0, 2 * num_sites, 2)
+        self.op_neighbors[1, :] = np.arange(1, 2 * num_sites, 2)
+        self.op_neighbors[2, :] = np.arange(2, 2 * num_sites + 1, 2)
+
+        #########################################################
+        ## OBSERVABLES THE SIMULATOR IS ABLE TO MEASURE IN THE ##
+        ## SAME ORDER OF THE ARRAY IN TNObservables            ##
+        #########################################################
+        self.is_measured = [
+            True,  # TNObsLocal
+            True,  # TNObsCorr
+            True,  # TNDistance2Pure
+            True,  # TnState2File
+            True,  # TNObsTensorProduct
+            True,  # TNObsWeightedSum
+            True,  # TNPbsProjective
+            True,  # TNObsProbabilities
+            True,  # TNObsBondEntropy
+            False,  # TNObsTZeroCorr
+            False,  # TNObsCorr4
+            False,  # TNObsCustom
+        ]
+        # MPS initializetion not aware of device
+        self.convert(self._tensor_backend.dtype, self._tensor_backend.device)
+
+    # --------------------------------------------------------------------------
+    #                               Properties
+    # --------------------------------------------------------------------------
+
+    @property
+    def default_iso_pos(self):
+        """
+        Returns default isometry center position, e.g., for initialziation
+        of effective operators.
+        """
+        return self.num_sites - 1
+
+    @property
+    def tensors(self):
+        """List of tensors componing the MPS"""
+        return self._tensors
+
+    @property
+    def singvals(self):
+        """List of singular values in the bonds"""
+        return self._singvals
+
+    @property
+    def first_non_orthogonal_left(self):
+        """First non orthogonal tensor starting from the left"""
+        return self._first_non_orthogonal_left
+
+    @property
+    def first_non_orthogonal_right(self):
+        """First non orthogonal tensor starting from the right"""
+        return self._first_non_orthogonal_right
+
+    @property
+    def iso_center(self):
+        """
+        Output the gauge center if it is well defined, otherwise None
+        """
+        if self.first_non_orthogonal_left == self.first_non_orthogonal_right:
+            center = self.first_non_orthogonal_right
+        else:
+            center = None
+        return center
+
+    @iso_center.setter
+    def iso_center(self, value):
+        self._first_non_orthogonal_left = value
+        self._first_non_orthogonal_right = value
+
+    @property
+    def physical_idxs(self):
+        """Physical indices property"""
+        return self.op_neighbors[1, :].reshape(-1)
+
+    @property
+    def current_max_bond_dim(self):
+        """Maximum bond dimension of the mps"""
+        max_bond_dims = [tt.shape for tt in self]
+        return np.max(max_bond_dims)
+
+    # --------------------------------------------------------------------------
+    #                          Overwritten operators
+    # --------------------------------------------------------------------------
+
     def __repr__(self):
         """
         Return the class name as representation.
         """
         return self.__class__.__name__
 
     def __len__(self):
@@ -163,17 +238,16 @@
         Parameters
         ----------
         key : int
             index of the array
         value : np.array
             value of the new tensor. Must have the same shape as the old one
         """
-        xp = self._device_checks()
-        if not isinstance(value, xp.ndarray):
-            raise TypeError("New tensor must be a numpy array")
+        if not isinstance(value, _AbstractQteaTensor):
+            raise TypeError("New tensor must be an _AbstractQteaTensor.")
         self._tensors[key] = value
 
         return None
 
     def __iter__(self):
         """Iterator protocol"""
         return iter(self.tensors)
@@ -198,44 +272,40 @@
         if not isinstance(other, MPS):
             raise TypeError("Only two MPS classes can be summed")
         elif self.num_sites != other.num_sites:
             raise ValueError("Number of sites must be the same to concatenate MPS")
         elif np.any(self.local_dim != other.local_dim):
             raise ValueError("Local dimension must be the same to concatenate MPS")
 
-        xp = self._device_checks()
-
-        max_bond_dim = max(self.max_bond_dim, other.max_bond_dim)
-        cut_ratio = min(self.cut_ratio, other.cut_ratio)
+        max_bond_dim = max(
+            self.convergence_parameters.max_bond_dimension,
+            other.convergence_parameters.max_bond_dimension,
+        )
+        cut_ratio = min(
+            self._convergence_parameters.cut_ratio,
+            other._convergence_parameters.cut_ratio,
+        )
         convergence_params = TNConvergenceParameters(
             max_bond_dimension=int(max_bond_dim), cut_ratio=cut_ratio
         )
 
         tensor_list = []
         idx = 0
         for tens_a, tens_b in zip(self, other):
             shape_c = np.array(tens_a.shape) + np.array(tens_b.shape)
             shape_c[1] = tens_a.shape[1]
             if idx == 0 and [tens_a.shape[0], tens_b.shape[0]] == [1, 1]:
-                shape_c[0] = 1
-                tens_c = xp.zeros(shape_c, dtype=self.dtype)
-                tens_c[:, :, : tens_a.shape[2]] = tens_a
-                tens_c[:, :, tens_a.shape[2] :] = tens_b
+                tens_c = tens_a.stack_link(tens_b, 2)
             elif idx == self.num_sites - 1 and [tens_a.shape[2], tens_b.shape[2]] == [
                 1,
                 1,
             ]:
-                shape_c[2] = 1
-                tens_c = xp.zeros(shape_c, dtype=self.dtype)
-                tens_c[: tens_a.shape[0], :, :] = tens_a
-                tens_c[tens_a.shape[0] :, :, :] = tens_b
+                tens_c = tens_a.stack_link(tens_b, 0)
             else:
-                tens_c = xp.zeros(shape_c, dtype=self.dtype)
-                tens_c[: tens_a.shape[0], :, : tens_a.shape[2]] = tens_a
-                tens_c[tens_a.shape[0] :, :, tens_a.shape[2] :] = tens_b
+                tens_c = tens_a.stack_first_and_last_link(tens_b)
 
             tensor_list.append(tens_c)
             idx += 1
 
         addMPS = MPS.from_tensor_list(tensor_list, conv_params=convergence_params)
 
         return addMPS
@@ -296,134 +366,350 @@
         the conjugation of the left-term
         """
         if not isinstance(other, MPS):
             raise TypeError("Only two MPS classes can be contracted")
 
         return other.contract(self)
 
-    @property
-    def tensors(self):
-        """List of tensors componing the MPS"""
-        return self._tensors
+    def dot(self, other):
+        """
+        Calculate the dot-product or overlap between two MPSs, i.e.,
+        <self | other>.
 
-    @property
-    def singvals(self):
-        """List of singular values in the bonds"""
-        return self._singvals
+        Parameters
+        ----------
 
-    @property
-    def first_non_orthogonal_left(self):
-        """First non orthogonal tensor starting from the left"""
-        return self._first_non_orthogonal_left
+        other : :class:`MPS`
+            Measure the overlap with this other MPS.
 
-    @property
-    def first_non_orthogonal_right(self):
-        """First non orthogonal tensor starting from the right"""
-        return self._first_non_orthogonal_right
+        Returns
+        -------a
 
-    @property
-    def iso_center(self):
+        Scalar representing the overlap.
         """
-        Output the gauge center if it is well defined, otherwise None
+        return other.contract(self)
+
+    # --------------------------------------------------------------------------
+    #                       classmethod, classmethod like
+    # --------------------------------------------------------------------------
+
+    @classmethod
+    def from_statevector(
+        cls,
+        statevector,
+        local_dim=2,
+        conv_params=None,
+        tensor_backend=None,
+    ):
         """
-        if self.first_non_orthogonal_left == self.first_non_orthogonal_right:
-            center = self.first_non_orthogonal_right
+        Initialize the MPS tensors by decomposing a statevector into MPS form.
+        All the degrees of freedom must have the same local dimension
+
+        Parameters
+        ----------
+        statevector : ndarray of shape( local_dim^num_sites, )
+            Statevector describing the interested state for initializing the MPS
+        local_dim : int, optional
+            Local dimension of the degrees of freedom. Default to 2.
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters for the new MPS. If None, the maximum bond
+            bond dimension possible is assumed, and a cut_ratio=1e-9.
+            Default to None.
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
+        Returns
+        -------
+        obj : :py:class:`MPS`
+            MPS simulator class
+
+        Examples
+        --------
+        >>> -U1 - U2 - U3 - ... - UN-
+        >>>  |    |    |          |
+        # For d=2, N=7 and chi=5, the tensor network is as follows:
+        >>> -U1 -2- U2 -4- U3 -5- U4 -5- U5 -4- U6 -2- U7-
+        >>>  |      |      |      |      |      |      |
+        # where -x- denotes the bounds' dimension (all the "bottom-facing" indices
+        # are of dimension d=2). Thus, the shapes
+        # of the returned tensors are as follows:
+        >>>      U1         U2         U3         U4         U5         U6         U7
+        >>> [(1, 2, 2), (2, 2, 4), (4, 2, 5), (5, 2, 5), (5, 2, 4), (4, 2, 2), (2, 2, 1)]
+        """
+        if not isinstance(statevector, np.ndarray):
+            raise TypeError("Statevector must be numpy array")
         else:
-            center = None
-        return center
+            statevector = statevector.reshape(-1)
+        num_sites = int(np.log(len(statevector)) / np.log(local_dim))
 
-    def get_tensor_of_site(self, idx):
+        max_bond_dim = local_dim ** (num_sites // 2)
+        if conv_params is None:
+            conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
+        obj = cls(num_sites, conv_params, local_dim, tensor_backend=tensor_backend)
+
+        state_tensor = statevector.reshape([1] + [local_dim] * num_sites + [1])
+        tensor_cls = obj._tensor_backend.tensor_cls
+        state_tensor = tensor_cls.from_elem_array(state_tensor)
+        for ii in range(num_sites - 1):
+            legs = list(range(len(state_tensor.shape)))
+            tens_left, tens_right, singvals, _ = state_tensor.split_svd(
+                legs[:2], legs[2:], contract_singvals="R", conv_params=conv_params
+            )
+
+            obj._tensors[ii] = tens_left
+            obj._singvals[ii + 1] = singvals
+            state_tensor = tens_right
+        obj._tensors[-1] = tens_right
+
+        # After this procedure the state is in left canonical form
+        obj._first_non_orthogonal_left = obj.num_sites - 1
+        obj._first_non_orthogonal_right = obj.num_sites - 1
+
+        obj.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
+
+        return obj
+
+    def _initialize_mps(self, initialize):
         """
-        Generic function to retrieve the tensor for a specific site. Compatible
-        across different tensor network geometries. This function does not
-        shift the gauge center before returning the tensor.
+        Initialize the MPS with a given structure. Available are:
+        - "vacuum", initializes the MPS in |00...0>
+        - "random", initializes the MPS in a random state at fixed bond dimension
 
         Parameters
         ----------
-        idx : int
-            Return tensor containin the link of the local
-            Hilbert space of the idx-th site.
+        initialize : str
+            Type of initialization.
+
+        Returns
+        -------
+        None
         """
-        return self[idx]
+        kwargs = self._tensor_backend.tensor_cls_kwargs()
+        tensor_cls = self._tensor_backend.tensor_cls
+
+        if initialize.lower() == "vacuum":
+            for ii in range(self.num_sites):
+                state0 = tensor_cls(
+                    [1, self._local_dim[ii], 1], ctrl="ground", **kwargs
+                )
+                self._tensors.append(state0)
+        elif initialize.lower() == "random":
+            # Works only for qubits right now
+            chi_ini = self._convergence_parameters.ini_bond_dimension
+            chis = [1] + [chi_ini] * (self.num_sites - 1) + [1]
+
+            chi_tmp = 1
+            for ii in range(self.num_sites):
+                chi_tmp *= self._local_dim[ii]
+                if chi_tmp < chis[ii + 1]:
+                    chis[ii + 1] = chi_tmp
+                    chis[-ii - 2] = chi_tmp
+                else:
+                    break
+
+            for ii in range(self.num_sites):
+                bd_left = chis[ii]
+                bd_right = chis[ii + 1]
+
+                mat = np.random.rand(bd_left, self._local_dim[ii], bd_right)
+
+                self._tensors.append(
+                    tensor_cls.from_elem_array(
+                        mat,
+                        kwargs.get("dtype", np.double),
+                        kwargs.get("device", "cpu"),
+                    )
+                )
+
+            self.site_canonize(self.num_sites - 1, normalize=True)
+            self.normalize()
+
+    def to_dense(self, true_copy=False):
+        """
+        Return MPS without symmetric tensors.
+
+        Parameters
+        ----------
+
+        true_copy : bool, optional
+            The function can be forced to return an actual copy with
+            `true_copy=True`, while otherwise `self` can be returned
+            if the MPS is already without symmetries.
+            Default to `False`
+
+        Returns
+        -------
+
+        dense_mps : :class:`MPS`
+            MPS representation without symmetric tensors.
+        """
+        if self.has_symmetry:
+            # Have to convert
+            tensor_list = [elem.to_dense() for elem in self]
+
+            obj = self.from_tensor_list(
+                tensor_list,
+                conv_params=self.convergence_parameters,
+                tensor_backend=self._tensor_backend,
+            )
+
+            for ii, s_vals in enumerate(self.singvals):
+                # Tensor list is shorter, still choose tensor belonging to singvals.
+                jj = min(ii, len(self) - 1)
+                obj._singvals[ii] = self[jj].to_dense_singvals(
+                    s_vals, true_copy=true_copy
+                )
+
+            obj.iso_center = self.iso_center
+
+            return obj
+
+        # Cases without symmetry
+
+        if true_copy:
+            return self.copy()
+
+        return self
+
+    # --------------------------------------------------------------------------
+    #                            Checks and asserts
+    # --------------------------------------------------------------------------
+
+    # --------------------------------------------------------------------------
+    #                     Abstract methods to be implemented
+    # --------------------------------------------------------------------------
+
+    def _convert_singvals(self, dtype, device):
+        """Convert the singular values of the tensor network to dtype/device."""
+        if len(self) == 0:
+            return
+
+        # Take any example tensor
+        tensor = self[0]
+
+        singvals_list = []
+        for elem in self._singvals:
+            if elem is None:
+                singvals_list.append(None)
+            else:
+                singvals_ii = tensor.convert_singvals(elem, dtype, device)
+                singvals_list.append(singvals_ii)
+
+        self._singvals = singvals_list
+
+    def get_bipartition_link(self, pos_src, pos_dst):
+        """
+        Returns two sets of sites forming the bipartition of the system for
+        a loopless tensor network. The link is specified via two positions
+        in the tensor network.
+
+        **Arguments**
+
+        pos_src : tuple of two ints
+            Specifies the first tensor and source of the link.
+
+        pos_dst : tuple of two ints
+            Specifies the second tensor and destination of the link.
+
+        **Returns**
+
+        sites_src : list of ints
+            Hilbert space indices when looking from the link towards
+            source tensor and following the links therein.
+
+        sites_dst : list of ints
+            Hilbert space indices when looking from the link towards
+            destination tensor and following the links therein.
+        """
+        if pos_src < pos_dst:
+            return list(range(pos_src + 1)), list(range(pos_src + 1, self.num_sites))
+
+        # pos_src > pos_dst
+        return list(range(pos_dst + 1, self.num_sites)), list(range(pos_dst + 1))
+
+    def get_pos_links(self, pos):
+        """
+        List of tensor position where links are leading to.
+
+        Parameters
+        ----------
+        pos : int
+            Index of the tensor in the MPS
+
+        Returns
+        -------
+        Tuple[int]
+            Index of the tensor connected through links to pos.
+            None if they are open links.
+        """
+        return [
+            pos - 1 if pos > 0 else None,
+            -pos - 2,
+            pos + 1 if pos < self.num_sites - 1 else None,
+        ]
 
     def get_rho_i(self, idx):
         """
         Get the reduced density matrix of the site at index idx
 
         Parameters
         ----------
         idx : int
             Index of the site
 
         Returns
         -------
-        xp.ndarray
+        :class:`_AbstractQteaTensor`
             Reduced density matrix of the site
         """
-        xp = self._device_checks()
-
         s_idx = 1 if self.iso_center > idx else 0
         if self.singvals[idx + s_idx] is None:
             self.iso_towards(idx, keep_singvals=True)
             tensor = self[idx]
         else:
             tensor = self[idx]
             if self.iso_center > idx:
-                tensor = xp.tensordot(
-                    tensor, xp.diag(self.singvals[idx + s_idx]), ([2], [1])
-                )
+                tensor = tensor.scale_link(self.singvals[idx + s_idx], 2)
             elif self.iso_center < idx:
-                tensor = xp.tensordot(
-                    xp.diag(self.singvals[idx + s_idx]), tensor, ([1], [0])
-                )
+                tensor = tensor.scale_link(self.singvals[idx + s_idx], 0)
 
-        rho = xp.tensordot(tensor, np.conj(tensor), [[0, 2], [0, 2]])
+        rho = tensor.tensordot(tensor.conj(), [[0, 2], [0, 2]])
 
-        return rho
+        trace = rho.trace(return_real_part=True, do_get=True)
+        if abs(1 - trace) > 10 * rho.dtype_eps:
+            warn("Renormalizing reduced density matrix.")
+            rho /= trace
 
-    def _get_eff_op_on_pos(self, pos):
-        """
-        Obtain the list of effective operators adjacent
-        to the position pos and the index where they should
-        be contracted
-
-        Parameters
-        ----------
-        pos : int
-            Index of the tensor w.r.t. which we have to retrieve
-            the effective operators
-
-        Returns
-        -------
-        list of IndexedOperators
-            List of effective operators
-        list of ints
-            Indexes where the operators should be contracted
-        """
-        raise NotImplementedError("This function has to be overwritten")
+        return rho
 
-    def site_canonize(self, idx, keep_singvals=False):
+    def get_tensor_of_site(self, idx):
         """
-        Apply the gauge transformation to shift the isoemtry
-        center to a specific site `idx`.
+        Generic function to retrieve the tensor for a specific site. Compatible
+        across different tensor network geometries. This function does not
+        shift the gauge center before returning the tensor.
 
         Parameters
         ----------
-        idx: int
-            index of the tensor up to which the canonization
-            occurs from the left and right side.
-        keep_singvals : bool, optional
-            If True, keep the singular values even if shifting the iso with a
-            QR decomposition. Default to False.
+        idx : int
+            Return tensor containin the link of the local
+            Hilbert space of the idx-th site.
         """
-        self.iso_towards(idx, keep_singvals=keep_singvals)
+        return self[idx]
 
-    def iso_towards(self, new_iso, keep_singvals=False, trunc=False, conv_params=None):
+    # pylint: disable-next=arguments-differ
+    def iso_towards(
+        self,
+        new_iso,
+        keep_singvals=False,
+        trunc=False,
+        conv_params=None,
+        normalize=False,
+    ):
         """
-        Apply yhe gauge transformation to shift the isometry
+        Apply the gauge transformation to shift the isometry
         center to a specific site `new_iso`.
         The method might be different for
         other TN structure, but for the MPS it is the same.
 
         Parameters
         ----------
         new_iso : int
@@ -435,146 +721,294 @@
             If `True`, the shifting is done via truncated SVD.
             If `False`, the shifting is done via QR.
             Default to `False`.
         conv_params : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters to use for the SVD. If `None`, convergence
             parameters are taken from the TTN.
             Default to `None`.
+        normalize : bool, optional
+            Flag if intermediate steps should normalize.
+            Default to `False`
+        """
+
+        self.left_canonize(
+            new_iso,
+            trunc=trunc,
+            keep_singvals=keep_singvals,
+            conv_params=conv_params,
+            normalize=normalize,
+        )
+        self.right_canonize(
+            new_iso,
+            trunc=trunc,
+            keep_singvals=keep_singvals,
+            conv_params=conv_params,
+            normalize=normalize,
+        )
+
+    def _iter_tensors(self):
+        """Iterate over all tensors forming the tensor network (for convert etc)."""
+        for elem in self._tensors:
+            yield elem
+
+    def norm(self):
+        """
+        Returns the norm of the MPS as sqrt(<self|self>)
+
+        Return
+        ------
+        norm: float
+            norm of the MPS
+        """
+        idx = self.first_non_orthogonal_right
+
+        if self.first_non_orthogonal_left != self.first_non_orthogonal_right:
+            self.left_canonize(self.first_non_orthogonal_right, keep_singvals=True)
+
+        return self[idx].norm_sqrt()
+
+    def scale(self, factor):
+        """
+        Scale the MPS state by a scalar constant using the gauge center.
+
+        Parameters
+        ----------
+
+        factor : scalar
+             Factor is multiplied to the MPS at the gauge center.
+        """
+        self._tensors[self.iso_center] *= factor
+
+    def set_singvals_on_link(self, pos_a, pos_b, s_vals):
+        """Update or set singvals on link via two positions."""
+        if pos_a < pos_b:
+            self._singvals[pos_b] = s_vals
+        else:
+            self._singvals[pos_a] = s_vals
+
+    # pylint: disable-next=arguments-differ
+    def site_canonize(self, idx, keep_singvals=False, normalize=False):
+        """
+        Apply the gauge transformation to shift the isoemtry
+        center to a specific site `idx`.
+
+        Parameters
+        ----------
+        idx: int
+            index of the tensor up to which the canonization
+            occurs from the left and right side.
+        keep_singvals : bool, optional
+            If True, keep the singular values even if shifting the iso with a
+            QR decomposition. Default to False.
+        normalize : bool, optional
+            Flag if intermediate steps should normalize.
+            Default to `False`
         """
-        if conv_params is not None:
-            raise ValueError("conv_params not yet supported for MPS.")
+        self.iso_towards(idx, keep_singvals=keep_singvals, normalize=normalize)
+
+    # --------------------------------------------------------------------------
+    #                   Choose to overwrite instead of inheriting
+    # --------------------------------------------------------------------------
 
-        self.left_canonize(new_iso, svd=trunc, keep_singvals=keep_singvals)
-        self.right_canonize(new_iso, svd=trunc, keep_singvals=keep_singvals)
+    # --------------------------------------------------------------------------
+    #                                  Unsorted
+    # --------------------------------------------------------------------------
 
-    def right_canonize(self, idx, svd=False, keep_singvals=False):
+    def _iter_all_links(self, pos):
+        """
+        Iterate through all the links of
+        a given position of the MPS
+
+        Parameters
+        ----------
+        pos : int
+            Index of the tensor
+
+        Yields
+        ------
+        int
+            Index of the tensor. The order is
+            left-physical-right
+        """
+        yield pos - 1, 2
+        yield -pos - 2, 1
+        yield pos + 1, 0
+
+    def _iter_physical_links(self):
+        """
+        Gives an iterator through the physical links.
+        In the MPS, the physical links are connected to nothing,
+        i.e. we assign the tensor index -2
+
+        Return
+        ------
+        Tuple[int]
+            The identifier from_tensor, to_tensor
+        """
+        for pos in range(self.num_sites):
+            yield -pos - 2, pos
+
+    def right_canonize(
+        self, idx, trunc=False, keep_singvals=False, conv_params=None, normalize=False
+    ):
         """
         Apply a gauge transformation to all bonds between
         :py:method:`MPS.num_sites` and `idx`, so that all
         sites between the last (rightmost one) and idx
         are set to (semi)-unitary tensors.
 
         Parameters
         ----------
         idx: int
             index of the tensor up to which the canonization occurs
-        svd: bool, optional
+        trunc: bool, optional
             If True, use the SVD instead of the QR for the canonization.
             It might be useful to reduce the bond dimension. Default to False.
         keep_singvals : bool, optional
             If True, keep the singular values even if shifting the iso with a
             QR decomposition. Default to False.
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters to use for the SVD in the procedure.
+            If `None`, convergence parameters are taken from the TTN.
+            Default to `None`.
+        normalize : bool, optional
+            Flag if intermediate steps should normalize.
+            Default to `False`
         """
+        # Get functions for elemtary arrays
+        mysum, sqrt = self[0].get_attr("sum", "sqrt")
+
+        do_svd = self._requires_singvals or trunc
+
         if idx > self.num_sites - 1 or idx < 0:
             raise ValueError(
                 "The canonization index must be between the "
                 + "number of sites-1 and 0"
             )
+        if conv_params is None:
+            conv_params = self._convergence_parameters
 
-        xp = self._device_checks()
         for ii in range(self.first_non_orthogonal_right, idx, -1):
-            tensor = self[ii]
-            tensor_shape = tensor.shape
-            matrix = tensor.reshape(tensor_shape[0], np.prod(tensor_shape[1:])).T
-            # We want (left) - (right) => (left) - R - Q =
-            # So we need R before Q. That is why we transpose:
-            # (right).T = Q R => (right) = R.T Q.T (and rename R.T => R and Q.T => Q)
-            if svd:
-                RR, tensor, singvals, _ = self.tSVD(
-                    tensor, [0], [1, 2], contract_singvals="L"
+            if do_svd:
+                rr_mat, tensor, singvals, _ = self[ii].split_svd(
+                    [0],
+                    [1, 2],
+                    contract_singvals="L",
+                    conv_params=conv_params,
+                    no_truncation=not trunc,
                 )
+                if normalize:
+                    norm = sqrt(mysum(singvals**2))
+                    singvals /= norm
+                    rr_mat /= norm
+
                 self._singvals[ii] = singvals
             else:
-                QQ, RR = xp.linalg.qr(matrix)
-                RR = RR.T
-                QQ = QQ.T
+                tensor, rr_mat = self[ii].split_qr(
+                    [1, 2], [0], perm_left=[2, 0, 1], perm_right=[1, 0]
+                )
+
+                if normalize:
+                    norm = rr_mat.norm()
+                    rr_mat /= norm
 
-                # Reshape back
-                tensor = QQ.reshape(-1, *tensor_shape[1:])
                 if not keep_singvals:
                     self._singvals[ii] = None
-
             # Update the tensors in the MPS
             self._tensors[ii] = tensor
-            self._tensors[ii - 1] = xp.tensordot(self[ii - 1], RR, ([2], [0]))
+            self._tensors[ii - 1] = self[ii - 1].tensordot(rr_mat, ([2], [0]))
+            if self.eff_op is not None:
+                self._update_eff_ops([ii, ii - 1])
 
         self._first_non_orthogonal_left = min(self.first_non_orthogonal_left, idx)
         self._first_non_orthogonal_right = idx
 
-    def left_canonize(self, idx, svd=False, keep_singvals=False):
+    def left_canonize(
+        self, idx, trunc=False, keep_singvals=False, conv_params=None, normalize=False
+    ):
         """
         Apply a gauge transformation to all bonds between 0 and `idx`,
         so that all sites between the first (òeftmpst one) and idx
         are set to (semi)-unitary tensors.
 
         Parameters
         ----------
         idx: int
             index of the tensor up to which the canonization occurs
-        svd: bool, optional
+        trunc: bool, optional
             If True, use the SVD instead of the QR for the canonization.
             It might be useful to reduce the bond dimension. Default to False.
         keep_singvals : bool, optional
             If True, keep the singular values even if shifting the iso with a
             QR decomposition. Default to False.
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters to use for the SVD in the procedure.
+            If `None`, convergence parameters are taken from the TTN.
+            Default to `None`.
+        normalize : bool, optional
+            Flag if singular values should be normalized.
+            Default to `False`
         """
+        # Get functions for elemtary arrays
+        mysum, sqrt = self[0].get_attr("sum", "sqrt")
+
+        do_svd = self._requires_singvals or trunc
+
         if idx > self.num_sites - 1 or idx < 0:
             raise ValueError(
                 "The canonization index must be between the "
                 + "number of sites-1 and 0"
             )
+        if conv_params is None:
+            conv_params = self._convergence_parameters
 
-        xp = self._device_checks()
         for ii in range(self.first_non_orthogonal_left, idx):
             tensor = self[ii]
-            tensor_shape = tensor.shape
-            matrix = tensor.reshape(np.prod(tensor_shape[:2]), tensor_shape[2])
-
-            if svd:
-                tensor, RR, singvals, _ = self.tSVD(
-                    tensor, [0, 1], [2], contract_singvals="R"
+            if do_svd:
+                tensor, rr_mat, singvals, _ = self[ii].split_svd(
+                    [0, 1],
+                    [2],
+                    contract_singvals="R",
+                    conv_params=conv_params,
+                    no_truncation=not trunc,
                 )
+                if normalize:
+                    norm = sqrt(mysum(singvals**2))
+                    singvals /= norm
+                    rr_mat /= norm
+
                 self._singvals[ii + 1] = singvals
             else:
-                QQ, RR = xp.linalg.qr(matrix)
+                tensor, rr_mat = self[ii].split_qr([0, 1], [2])
+
+                if normalize:
+                    norm = rr_mat.norm()
+                    rr_mat /= norm
 
-                # Reshape back
-                tensor = QQ.reshape(*tensor_shape[:2], -1)
                 if not keep_singvals:
                     self._singvals[ii + 1] = None
 
             # Update the tensors in the MPS
             self._tensors[ii] = tensor
-            self._tensors[ii + 1] = xp.tensordot(self[ii + 1], RR, ([0], [1]))
-            self._tensors[ii + 1] = xp.transpose(self._tensors[ii + 1], [2, 0, 1])
-
+            self._tensors[ii + 1] = self[ii + 1].tensordot(rr_mat, ([0], [1]))
+            self._tensors[ii + 1] = self._tensors[ii + 1].transpose([2, 0, 1])
+            if self.eff_op is not None:
+                self._update_eff_ops([ii, ii + 1])
         self._first_non_orthogonal_left = idx
         self._first_non_orthogonal_right = max(self.first_non_orthogonal_right, idx)
 
     def normalize(self):
         """
         Normalize the MPS state, by dividing by :math:`\\sqrt{<\\psi|\\psi>}`.
         """
         # Compute the norm. Internally, it set the gauge center
         norm = self.norm()
         # Update the norm
         self._tensors[self.iso_center] /= norm
 
-    def scale(self, factor):
-        """
-        Scale the MPS state by a scalar constant using the gauge center.
-
-        Parameters
-        ----------
-
-        factor : scalar
-             Factor is multiplied to the MPS at the gauge center.
-        """
-        self._tensors[self.iso_center] *= factor
-
     def modify_local_dim(self, value, idxs=None):
         """
         Modify the local dimension of sites `idxs` to the value `value`.
         By default modify the local dimension of all the sites. If `value` is
         a vector then it must have the same length of `idxs`.
         Notice that there may be loss of information, it is up to the
         user to be sure no error is done in this procedure.
@@ -608,34 +1042,49 @@
             )
         elif len(value) != len(idxs):
             raise ValueError(
                 "value and idxs must have the same length, but "
                 + f"{len(value)} != {len(idxs)}"
             )
 
-        xp = self._device_checks()
-
         # Quick return
         if len(idxs) == 0:
             return
         # Sort arguments to avoid moving the gauge back and forth
         value = value[np.argsort(idxs)]
         idxs = np.sort(idxs)
 
         for ii, idx in enumerate(idxs):
             initial_local_dim = self.local_dim[idx]
             new_local_dim = value[ii]
-            self.site_canonize(idx, keep_singvals=True)
 
-            modify_tens = xp.eye(new_local_dim, initial_local_dim)
+            if initial_local_dim == new_local_dim:
+                # Already right dimension
+                continue
+
+            self.site_canonize(idx, keep_singvals=True)
             initial_norm = self.norm()
 
-            # Modify the local dimension
-            res = xp.tensordot(self[idx], modify_tens, ([1], [1]))
-            self._tensors[idx] = res.transpose(0, 2, 1)
+            if new_local_dim < initial_local_dim:
+                # Get subtensor along link
+                res = self[idx].subtensor_along_link(1, 0, new_local_dim)
+            else:
+                shape = [
+                    self[idx].shape[0],
+                    new_local_dim - initial_local_dim,
+                    self[idx].shape[2],
+                ]
+                kwargs = self._tensor_backend.tensor_cls_kwargs()
+
+                # Will fail for symmetric tensors
+                pad = self._tensor_backend.tensor_cls(shape, **kwargs)
+
+                res = self[idx].stack_link(pad, 1)
+
+            self._tensors[idx] = res
 
             final_norm = self.norm()
             self._tensors[self.iso_center] *= initial_norm / final_norm
 
             self._local_dim[idx] = new_local_dim
 
     def add_site(self, idx, state=None):
@@ -653,32 +1102,37 @@
 
         Details
         -------
         To insert a new site in the MPS we first insert an identity on a link,
         then add a dimension-1 link to the identity and lastly contract the
         new link with the initial state, usually a |0>
         """
-        xp = self._device_checks()
         if idx < 0 or idx > self.num_sites:
             raise ValueError(f"idx must be between 0 and N+1, not {idx}")
         if state is None:
-            state = xp.zeros(int(np.min(self.local_dim)), dtype=self.dtype)
-            state[0] = 1
+            local_dim = int(np.min(self.local_dim))
+            kwargs = self._tensor_backend.tensor_cls_kwargs()
+            state = self._tensor_backend.tensor_cls(
+                [1, local_dim, 1], ctrl="ground", **kwargs
+            )
+
         old_norm = self.norm()
 
         # Insert an identity on link idx
         if idx == 0:
             id_dim = self[0].shape[0]
         else:
             id_dim = self[idx - 1].shape[2]
-        identity = xp.eye(id_dim, dtype=self.dtype).reshape(id_dim, 1, id_dim)
+
+        identity = state.eye_like(id_dim)
+        identity.reshape_update([id_dim, 1, id_dim])
 
         # Contract the identity with the desired state of the new tensor
-        state = state.reshape(len(state), 1)
-        new_site = xp.tensordot(identity, state, ([1], [1]))
+        state = state.reshape([np.product(state.shape), 1])
+        new_site = identity.tensordot(state, ([1], [1]))
         new_site = new_site.transpose([0, 2, 1])
 
         # Insert it in the data structure
         self._tensors.insert(idx, new_site)
         self._local_dim = np.insert(self._local_dim, idx, new_site.shape[1])
         self._num_sites += 1
         self._singvals.insert(idx + 1, None)
@@ -689,51 +1143,14 @@
             self._first_non_orthogonal_left += 1
 
         # Renormalize
         new_norm = self.norm()
 
         self._tensors[self.iso_center] *= old_norm / new_norm
 
-    def to_device(self, device):
-        """
-        Move the MPS class to the new device.
-
-        Parameters
-        ----------
-        device : string
-            Device where to move the MPS
-        """
-        if device not in self.implemented_devices:
-            raise ValueError(
-                f"Device {device} is not implemented. Select from"
-                + f" {self.implemented_devices}"
-            )
-        # We already are in the correct device
-        elif device == self.device:
-            return
-        # We go to the cpu to gpu
-        elif device == "gpu":
-            if not GPU_AVAILABLE:
-                raise ImportError("CUDA GPU is not available")
-            self._tensors = [cp.asarray(tens) for tens in self._tensors]
-            self._singvals = [
-                cp.asarray(singv) if singv is not None else None
-                for singv in self._singvals
-            ]
-        # We go from gpu to cpu
-        elif device == "cpu":
-            self._tensors = [cp.asnumpy(tens) for tens in self._tensors]
-            self._singvals = [
-                cp.asnumpy(singv) if singv is not None else None
-                for singv in self._singvals
-            ]
-        self._device = device
-
-        return
-
     def to_statevector(self, qiskit_order=False, max_qubit_equivalent=20):
         """
         Given a list of N tensors *MPS* [U1, U2, ..., UN] , representing
         a Matrix Product State, perform the contraction in the Examples,
         leading to a single tensor of order N, representing a dense state.
 
         The index ordering convention is from left-to-right.
@@ -759,23 +1176,22 @@
             N-order tensor representing the dense state.
 
         Examples
         --------
         >>> U1 - U2 - ... - UN
         >>>  |    |          |
         """
-        xp = self._device_checks()
         if np.prod(self.local_dim) > 2**max_qubit_equivalent:
             raise RuntimeError(
                 "Maximum number of sites for the statevector is "
                 + f"fixed to the equivalent of {max_qubit_equivalent} qubit sites"
             )
         psi = self[0]
         for tensor in self[1:]:
-            psi = xp.tensordot(psi, tensor, axes=(-1, 0))
+            psi = psi.tensordot(tensor, ([-1], [0]))
 
         if qiskit_order:
             order = "F"
         else:
             order = "C"
 
         return psi.reshape(np.prod(self.local_dim), order=order)
@@ -807,216 +1223,144 @@
         The order of the legs is always left-child, right-child, parent with
         the exception of the left top tensor. The left top tensor has an
         additional link, i.e., the symmetry selector; the order is left-child,
         right-child, parent, symmetry-selector.
 
         Also see :py:func:ttn_simulator:`from_tensor_list`.
         """
-        self.to_device("cpu")
         nn = len(self)
         if abs(np.log2(nn) - int(np.log2(nn))) > 1e-15:
             raise Exception(
                 "A conversion to a binary tree requires 2**n "
                 "sites; but having %d sites." % (nn)
             )
 
         if nn == 4:
             # Special case: iterations will not work
-            left_tensor = np.tensordot(self[0], self[1], [[2], [0]])
-            right_tensor = np.tensordot(self[2], self[3], [[2], [0]])
+            left_tensor = self[0].tensordot(self[1], [[2], [0]])
+            right_tensor = self[2].tensordot(self[3], [[2], [0]])
 
             # Use left link of dimension 1 as symmetry selector
-            left_tensor = np.transpose(left_tensor, [1, 2, 3, 0])
+            left_tensor.transpose_update([1, 2, 3, 0])
 
             # Eliminate one link
-            right_tensor = np.reshape(right_tensor, right_tensor.shape[:-1])
+            right_tensor.reshape_update(right_tensor.shape[:-1])
 
             return [[left_tensor, right_tensor]]
 
         # Initial iteration
         theta_list = []
         for ii in range(nn // 2):
             ii1 = 2 * ii
             ii2 = ii1 + 1
 
-            theta_list.append(np.tensordot(self[ii1], self[ii2], [[2], [0]]))
+            theta_list.append(self[ii1].tensordot(self[ii2], [[2], [0]]))
 
         child_list = []
         parent_list = []
         for ii, theta in enumerate(theta_list):
-            dims = theta.shape
-            tmp = np.transpose(theta, [1, 2, 0, 3])
-            tmp = np.reshape(tmp, [np.prod(tmp.shape[:2]), np.prod(tmp.shape[2:])])
-            qmat, rmat = nla.qr(tmp)
-            qmat = np.reshape(qmat, [dims[1], dims[2], rmat.shape[0]])
-            rmat = np.reshape(rmat, [qmat.shape[2], dims[0], dims[3]])
-            rmat = np.transpose(rmat, [1, 0, 2])
+            qmat, rmat = theta.split_qr([1, 2], [0, 3], perm_right=[1, 0, 2])
 
             child_list.append(qmat)
             parent_list.append(rmat)
 
         layer_list = [child_list]
         while len(parent_list) > 4:
             theta_list = []
             for ii in range(len(parent_list) // 2):
                 ii1 = 2 * ii
                 ii2 = ii1 + 1
 
                 theta_list.append(
-                    np.tensordot(parent_list[ii1], parent_list[ii2], [[2], [0]])
+                    parent_list[ii1].tensordot(parent_list[ii2], [[2], [0]])
                 )
 
             child_list = []
             parent_list = []
             for ii, theta in enumerate(theta_list):
-                dims = theta.shape
-                tmp = np.transpose(theta, [1, 2, 0, 3])
-                tmp = np.reshape(tmp, [np.prod(tmp.shape[:2]), np.prod(tmp.shape[2:])])
-                qmat, rmat = nla.qr(tmp)
-                qmat = np.reshape(qmat, [dims[1], dims[2], rmat.shape[0]])
-                rmat = np.reshape(rmat, [qmat.shape[2], dims[0], dims[3]])
-                rmat = np.transpose(rmat, [1, 0, 2])
+                qmat, rmat = theta.split_qr([1, 2], [0, 3], perm_right=[1, 0, 2])
 
                 child_list.append(qmat)
                 parent_list.append(rmat)
 
             layer_list.append(child_list)
 
         # Last iteration
-        left_tensor = np.tensordot(parent_list[0], parent_list[1], [[2], [0]])
-        right_tensor = np.tensordot(parent_list[2], parent_list[3], [[2], [0]])
+        left_tensor = parent_list[0].tensordot(parent_list[1], [[2], [0]])
+        right_tensor = parent_list[2].tensordot(parent_list[3], [[2], [0]])
 
         # The fourth-link is the symmetry selector, i.e., for tensor
         # networks without symmetries a link of dimension one. The link
         # to the left of the MPS fulfills this purpose
-        left_tensor = np.transpose(left_tensor, [1, 2, 3, 0])
+        left_tensor.transpose_update([1, 2, 3, 0])
 
-        right_tensor = np.reshape(right_tensor, right_tensor.shape[:-1])
-        right_tensor = np.transpose(right_tensor, [1, 2, 0])
+        right_tensor.reshape_update(right_tensor.shape[:-1])
+        right_tensor.transpose_update([1, 2, 0])
 
         layer_list.append([left_tensor, right_tensor])
 
         return layer_list
 
     @classmethod
     def from_tensor_list(
-        cls, tensor_list, conv_params=None, device="cpu", dtype=np.complex128
+        cls,
+        tensor_list,
+        conv_params=None,
+        tensor_backend=None,
     ):
         """
         Initialize the MPS tensors using a list of correctly shaped tensors
 
         Parameters
         ----------
         tensor_list : list of ndarrays or cupy arrays
             List of tensor for initializing the MPS
         conv_params : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters for the new MPS. If None, the maximum bond
             bond dimension possible is assumed, and a cut_ratio=1e-9.
             Default to None.
-        device : str
-            Computational device. Available 'cpu', 'gpu'. Default to 'cpu'
-        dtype : data type preferably numpy
-            Data type for constructing MPS.
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
 
         Returns
         -------
         obj : :py:class:`MPS`
             The MPS class
         """
         local_dim = []
         max_bond_dim = 2
         for ii, tens in enumerate(tensor_list):
             t_shape = tens.shape
             local_dim.append(t_shape[1])
             max_bond_dim = max(max_bond_dim, t_shape[0])
             if ii > 0 and t_shape[0] != tensor_list[ii - 1].shape[2]:
                 raise ValueError(
-                    f"The dimension of the left leg of tensor {ii} and "
-                    + f"the right leg of tensor {ii-1} must be equal"
+                    f"Dimension mismatch of the left leg of tensor {ii} and "
+                    + f"the right leg of tensor {ii-1}: "
+                    + f"{t_shape[0]} vs {tensor_list[ii - 1].shape[2]}"
                 )
 
         if conv_params is None:
             conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
-        obj = cls(len(tensor_list), conv_params, local_dim, dtype=dtype, device=device)
-        obj._tensors = tensor_list
-        obj.to_device(device)
-
-        return obj
-
-    @classmethod
-    def from_statevector(
-        cls,
-        statevector,
-        local_dim=2,
-        conv_params=None,
-        device="cpu",
-        dtype=np.complex128,
-    ):
-        """
-        Initialize the MPS tensors by decomposing a statevector into MPS form.
-        All the degrees of freedom must have the same local dimension
-
-        Parameters
-        ----------
-        statevector : ndarray of shape( local_dim^num_sites, )
-            Statevector describing the interested state for initializing the MPS
-        local_dim : int, optional
-            Local dimension of the degrees of freedom. Default to 2.
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters for the new MPS. If None, the maximum bond
-            bond dimension possible is assumed, and a cut_ratio=1e-9.
-            Default to None.
-        device : str
-            Computational device. Available 'cpu', 'gpu'. Default to 'cpu'
-        dtype : data type preferably numpy
-            Data type for constructing MPS.
-
-        Returns
-        -------
-        obj : :py:class:`MPS`
-            MPS simulator class
-
-        Examples
-        --------
-        >>> -U1 - U2 - U3 - ... - UN-
-        >>>  |    |    |          |
-        # For d=2, N=7 and chi=5, the tensor network is as follows:
-        >>> -U1 -2- U2 -4- U3 -5- U4 -5- U5 -4- U6 -2- U7-
-        >>>  |      |      |      |      |      |      |
-        # where -x- denotes the bounds' dimension (all the "bottom-facing" indices
-        # are of dimension d=2). Thus, the shapes
-        # of the returned tensors are as follows:
-        >>>      U1         U2         U3         U4         U5         U6         U7
-        >>> [(1, 2, 2), (2, 2, 4), (4, 2, 5), (5, 2, 5), (5, 2, 4), (4, 2, 2), (2, 2, 1)]
-        """
-        if not isinstance(statevector, np.ndarray):
-            raise TypeError("Statevector must be numpy array")
-        num_sites = int(np.log(len(statevector)) / np.log(local_dim))
-
-        max_bond_dim = local_dim ** (num_sites // 2)
-        if conv_params is None:
-            conv_params = TNConvergenceParameters(max_bond_dimension=int(max_bond_dim))
-        obj = cls(num_sites, conv_params, local_dim, dtype=dtype)
+        obj = cls(
+            len(tensor_list), conv_params, local_dim, tensor_backend=tensor_backend
+        )
 
-        state_tensor = statevector.reshape([1] + [local_dim] * num_sites + [1])
-        for ii in range(num_sites - 1):
-            legs = list(range(len(state_tensor.shape)))
-            tens_left, tens_right, singvals, _ = obj.tSVD(
-                state_tensor, legs[:2], legs[2:], contract_singvals="R"
-            )
+        qtea_tensor_list = []
+        for elem in tensor_list:
+            if not isinstance(elem, _AbstractQteaTensor):
+                qtea_tensor_list.append(
+                    obj._tensor_backend.tensor_cls.from_elem_array(elem)
+                )
+            else:
+                qtea_tensor_list.append(elem)
 
-            obj._tensors[ii] = tens_left
-            obj._singvals[ii + 1] = singvals
-            state_tensor = tens_right
-        obj._tensors[-1] = tens_right
+        obj._tensors = qtea_tensor_list
 
-        # After this procedure the state is in left canonical form
-        obj._first_non_orthogonal_left = obj.num_sites - 1
-        obj._first_non_orthogonal_right = obj.num_sites - 1
-        obj.to_device(device)
+        obj.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
 
         return obj
 
     def apply_one_site_operator(self, op, pos):
         """
         Applies a one operator `op` to the site `pos` of the MPS.
 
@@ -1028,24 +1372,17 @@
             Position of the qubit where to apply `op`.
 
         """
         if pos < 0 or pos > self.num_sites - 1:
             raise ValueError(
                 "The position of the site must be between 0 and (num_sites-1)"
             )
-        # elif not isinstance(op, np.ndarray):
-        #    raise TypeError('Input operator must be a ndarray')
-        elif list(op.shape) != [self._local_dim[pos]] * 2:
-            raise ValueError(
-                "Shape of the input operator must be (local_dim, local_dim)"
-            )
 
-        xp = self._device_checks(operator=op)
-        res = xp.tensordot(self[pos], op, (1, 1))
-        self._tensors[pos] = res.transpose(0, 2, 1)
+        res = self[pos].tensordot(op, ([1], [1]))
+        self._tensors[pos] = res.transpose([0, 2, 1])
 
     def apply_two_site_operator(self, op, pos, swap=False, svd=True, parallel=False):
         """
         Applies a two-site operator `op` to the site `pos`, `pos+1` of the MPS.
 
         Parameters
         ----------
@@ -1081,74 +1418,154 @@
               -P-M-       -P-M-
               2| |2       2| |2
               3| |4       4| |3
                GGG         GGG
               1| |2       2| |1
         """
         if not np.isscalar(pos) and len(pos) == 2:
+            if max(pos[0], pos[1]) - min(pos[0], pos[1]) > 1:
+                warn("Using non-local gates. Errors might increase.")
+                return self.apply_nonlocal_two_site_operator(op, pos[0], pos[1], swap)
             pos = min(pos[0], pos[1])
         elif not np.isscalar(pos):
             raise ValueError(
                 f"pos should be only scalar or len 2 array-like, not len {len(pos)}"
             )
 
         if pos < 0 or pos > self.num_sites - 1:
             raise ValueError(
                 "The position of the site must be between 0 and (num_sites-1)"
             )
-        elif list(op.shape) != [self._local_dim[pos], self._local_dim[pos + 1]] * 2:
-            raise ValueError(
-                "Shape of the input operator must be (local_dim, "
-                + "local_dim, local_dim, local_dim)"
-            )
+        op = op.reshape([self._local_dim[pos], self._local_dim[pos + 1]] * 2)
 
-        xp = self._device_checks(operator=op)
         if swap:
-            op = xp.transpose(op, [1, 0, 3, 2])
+            op = op.transpose([1, 0, 3, 2])
 
         if parallel:
-            self[pos] = self.tensordot_diagonal(self[pos], self.singvals[pos], 0)
+            self[pos].scale_link_update(self.singvals[pos], 0)
+            contract_singvals = "L"
         else:
             # Set orthogonality center
             self.site_canonize(pos, keep_singvals=True)
+            contract_singvals = "R"
 
         # Perform SVD
         if svd:
             # Contract the two qubits
-            twoqubit = xp.tensordot(self[pos], self[pos + 1], (2, 0))
+            twoqubit = self[pos].tensordot(self[pos + 1], ([2], [0]))
 
             # Contract with the gate
-            twoqubit = xp.tensordot(twoqubit, op, ([1, 2], [2, 3]))
-            twoqubit = xp.transpose(twoqubit, [0, 2, 3, 1])
-            tens_left, tens_right, singvals, singvals_cutted = self.tSVD(
-                twoqubit, [0, 1], [2, 3], contract_singvals="R"
+            twoqubit = twoqubit.tensordot(op, ([1, 2], [2, 3]))
+            twoqubit.transpose_update([0, 2, 3, 1])
+            tens_left, tens_right, singvals, singvals_cutted = twoqubit.split_svd(
+                [0, 1],
+                [2, 3],
+                contract_singvals=contract_singvals,
+                conv_params=self._convergence_parameters,
             )
         else:
-            tens_left, tens_right, singvals, singvals_cutted = self.tEQR(
-                self[pos], self[pos + 1], self.singvals[pos], op
+            tens_left, tens_right, singvals, singvals_cutted = self[pos].split_qrte(
+                self[pos + 1],
+                self.singvals[pos],
+                op,
+                conv_params=self._convergence_parameters,
             )
 
         # Update state
         self._tensors[pos] = tens_left
         self._tensors[pos + 1] = tens_right
         self._singvals[pos + 1] = singvals
 
         if parallel:
-            self[pos] = self.tensordot_diagonal(self[pos], 1 / self.singvals[pos], 0)
+            self[pos].scale_link_update(1 / self.singvals[pos], 0)
 
         else:
             self._first_non_orthogonal_left = pos + 1
             self._first_non_orthogonal_right = pos + 1
 
         # Update maximum bond dimension reached
         if self[pos].shape[2] > self.max_bond_dim_reached:
             self.max_bond_dim_reached = self[pos].shape[2]
 
         return singvals_cutted
 
+    def swap_qubits(self, sites, conv_params=None, trunc=True):
+        """
+        This function applies a swap gate to sites in an MPS,
+        i.e. swaps these two qubits
+
+        Parameters
+        ----------
+        sites : Tuple[int]
+            The qubits on site sites[0] and sites[1] are swapped
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters to use for the SVD in the procedure.
+            If `None`, convergence parameters are taken from the TTN.
+            Default to `None`.
+
+        Return
+        ------
+        np.ndarray
+            Singualr values cut in the process of shifting the isometry center.
+            None if moved through the QR.
+        """
+        if conv_params is None:
+            conv_params = self._convergence_parameters
+        # transform input into np array just in case the
+        # user passes the list
+        sites = np.sort(sites)
+        singvals_cut_tot = []
+        self.iso_towards(sites[0], True, False, conv_params)
+        # Move sites[0] in sites[1] position
+        for pos in range(sites[0], sites[1]):
+            # Contract the two sites
+            two_sites = self[pos].tensordot(self[pos + 1], ([2], [0]))
+            # Swap the qubits
+            two_sites.transpose_update([0, 2, 1, 3])
+            if trunc:
+                left, right, singvals, singvals_cut = two_sites.split_svd(
+                    [0, 1], [2, 3], contract_singvals="R", conv_params=conv_params
+                )
+                self._singvals[pos + 1] = singvals
+                singvals_cut_tot.append(singvals_cut)
+            else:
+                left, right = two_sites.split_qr([0, 1], [2, 3])
+
+            # Update tensor and iso center
+            self._tensors[pos] = left
+            self._tensors[pos + 1] = right
+            self._first_non_orthogonal_left += 1
+            self._first_non_orthogonal_right += 1
+
+        self.iso_towards(sites[1] - 1, True, False, conv_params)
+        # Move sites[1] in sites[0] position
+        for pos in range(sites[1] - 1, sites[0], -1):
+            # Contract the two sites
+            two_sites = self[pos - 1].tensordot(self[pos], ([2], [0]))
+            # Swap the qubits
+            two_sites.transpose_update([0, 2, 1, 3])
+            if trunc:
+                left, right, singvals, singvals_cut = two_sites.split_svd(
+                    [0, 1], [2, 3], contract_singvals="L", conv_params=conv_params
+                )
+                self._singvals[pos] = singvals
+                singvals_cut_tot.append(singvals_cut)
+            else:
+                right, left = two_sites.split_qr(
+                    [2, 3], [0, 1], perm_left=[2, 0, 1], perm_right=[1, 2, 0]
+                )
+
+            # Update tensor and iso center
+            self._tensors[pos - 1] = left
+            self._tensors[pos] = right
+            self._first_non_orthogonal_left -= 1
+            self._first_non_orthogonal_right -= 1
+
+        return singvals_cut_tot
+
     def apply_projective_operator(self, site, selected_output=None, remove=False):
         """
         Apply a projective operator to the site **site**, and give the measurement as output.
         You can also decide to select a given output for the measurement, if the probability is
         non-zero. Finally, you have the possibility of removing the site after the measurement.
 
         .. warning::
@@ -1176,68 +1593,70 @@
         Returns
         -------
         meas_state: int
             Measured state
         state_prob : float
             Probability of measuring the output state
         """
+
         if selected_output is not None and selected_output > self._local_dim[site] - 1:
             raise ValueError("The seleted output must be at most local_dim-1")
-        xp = self._device_checks()
 
         # Set the orthogonality center
         self.site_canonize(site, keep_singvals=True)
 
         # Normalize
         old_norm = self.norm()
         self._tensors[site] = self._tensors[site] / old_norm
 
         # Measure
-        cum_prob = 0
         random_u = np.random.rand()
         rho_i = self.get_rho_i(site)
-        for ii in range(self._local_dim[site]):
+
+        probabilities = rho_i.diag(real_part_only=True, do_get=True)
+        cumul_probs = np.cumsum(probabilities)
+
+        meas_state = None
+        for ii, cprob_ii in enumerate(cumul_probs):
             if selected_output is not None and ii != selected_output:
                 continue
 
-            projector = _projector(ii, self._local_dim[site], xp)
-            prob_ii = xp.trace(rho_i @ projector)
-            cum_prob += prob_ii
-            if cum_prob >= random_u or selected_output == ii:
+            if cprob_ii >= random_u or selected_output == ii:
                 meas_state = ii
-                state_prob = prob_ii
+                state_prob = probabilities[ii]
                 break
 
+        if meas_state is None:
+            raise Exception("Did not run into measurement.")
+
         # Renormalize and come back to previous norm
         if remove:
-            projector_vect = xp.zeros(int(self._local_dim[site]))
-            projector_vect[meas_state] = 1
-            # Project the state in the measured one
-            tens_to_remove = xp.tensordot(
-                self._tensors[site], projector_vect, ([1], [0])
-            )
+            ii = meas_state
+            tens_to_remove = self._tensors[site].subtensor_along_link(1, ii, ii + 1)
+            tens_to_remove.remove_dummy_link(1)
 
             if site < self.num_sites - 1:
                 # contract the measured tensor in the next tensor
-                self._tensors[site + 1] = xp.tensordot(
-                    tens_to_remove, self[site + 1], ([1], [0])
+                self._tensors[site + 1] = tens_to_remove.tensordot(
+                    self[site + 1], ([1], [0])
                 )
             else:
-                self._tensors[site - 1] = xp.tensordot(
-                    self[site - 1], tens_to_remove, ([2], [0])
+                self._tensors[site - 1] = self[site - 1].tensordot(
+                    tens_to_remove, ([2], [0])
                 )
 
             self._tensors.pop(site)
             self._singvals.pop(site)
             self._local_dim = np.delete(self._local_dim, site)
             self._num_sites -= 1
             site = min(site, self._num_sites - 1)
             self._first_non_orthogonal_left = site
             self._first_non_orthogonal_right = site
         else:
+            projector = _projector_for_rho_i(meas_state, rho_i)
             self.apply_one_site_operator(projector, site)
 
         # Renormalize
         self._tensors[site] = self._tensors[site] / self.norm()
         self._tensors[site] = self._tensors[site] * old_norm
 
         # Set to None all the singvals
@@ -1280,69 +1699,179 @@
             )
         elif list(op.shape) != [self._local_dim[control], self._local_dim[target]] * 2:
             raise ValueError(
                 "Shape of the input operator must be (local_dim, "
                 + "local_dim, local_dim, local_dim)"
             )
         if swap:
-            op = op.transpose(1, 0, 3, 2)
-
-        xp = self._device_checks()
+            op = op.transpose([1, 0, 3, 2])
 
         min_site = min(control, target)
         max_site = max(control, target)
-        left_gate, right_gate, _, _ = self.tSVD(
-            op,
+        left_gate, right_gate, _, _ = op.split_svd(
             [0, 2],
             [1, 3],
             perm_left=[0, 2, 1],
             perm_right=[1, 0, 2],
-            contract_singvals="R",
+            contract_singvals="L",
+            no_truncation=True,
+            conv_params=self._convergence_parameters,
         )
 
-        test = xp.tensordot(left_gate, left_gate.conj(), ([0, 1], [0, 1]))
-        if not xp.isclose(xp.identity(test.shape[0]), test):
+        test = right_gate.tensordot(right_gate.conj(), ([0, 1], [0, 1]))
+        if not test.is_close_identity():
             warn(
-                "Left-tensor is not unitary. Thus, the contraction is not optimal. We"
+                "Right-tensor is not unitary. Thus, the contraction is not optimal. We"
                 " suggest"
                 + " to linearize the circuit instead of using non-local operators",
-                RuntimeWarning(),
+                RuntimeWarning,
             )
 
         self.site_canonize(min_site, keep_singvals=True)
-        self._tensors[min_site] = xp.tensordot(
-            self[min_site], left_gate / np.sqrt(2), ([1], [2])
+        self._tensors[min_site] = self[min_site].tensordot(
+            left_gate / np.sqrt(2), ([1], [2])
         )
 
-        self._tensors[min_site] = self._tensors[min_site].transpose(0, 2, 3, 1)
+        self._tensors[min_site] = self._tensors[min_site].transpose([0, 2, 3, 1])
 
         for idx in range(min_site, max_site):
-            double_site = xp.tensordot(self[idx], self[idx + 1], ([3], [0]))
-            # if np.isnan(double_site).any(): print(op)
-            self._tensors[idx], self._tensors[idx + 1], _, singvals_cut = self.tSVD(
-                double_site,
-                [0, 1],
-                [2, 3, 4],
-                perm_right=[0, 2, 1, 3],
-                contract_singvals="R",
+            double_site = self[idx].tensordot(self[idx + 1], ([3], [0]))
+            (self._tensors[idx], self._tensors[idx + 1]) = double_site.split_qr(
+                [0, 1], [2, 3, 4], perm_right=[0, 2, 1, 3]
             )
 
-        self._tensors[max_site] = xp.tensordot(
-            self[max_site], right_gate * np.sqrt(2), ([1, 2], [2, 1])
+        self._tensors[max_site] = self[max_site].tensordot(
+            right_gate * np.sqrt(2), ([1, 2], [2, 1])
         )
-        self._tensors[max_site] = self._tensors[max_site].transpose(0, 2, 1)
+        self._tensors[max_site] = self._tensors[max_site].transpose([0, 2, 1])
 
         # double_site = np.tensordot(self[max_site-1], self[max_site], ([3, 2], [0, 2]) )
         # self._tensors[max_site-1], self._tensors[max_site], _, singvals_cut = \
         #        self.tSVD(double_site, [0, 1], [2, 3], contract_singvals='R' )
 
         self._first_non_orthogonal_left = max_site
         self._first_non_orthogonal_right = max_site
+        self.iso_towards(min_site, keep_singvals=True, trunc=True)
+
+        return []
+
+    def apply_mpo(self, mpo):
+        """
+        Apply an MPO to the MPS on the sites `sites`.
+        The MPO should have the following convention for the links:
+        0 is left link. 1 is physical link pointing downwards.
+        2 is phisical link pointing upwards. 3 is right link.
+
+        The sites are encoded inside the DenseMPO class.
+
+        Parameters
+        ----------
+        mpo : DenseMPO
+            MPO to be applied
 
-        return singvals_cut
+        Returns
+        -------
+        np.ndarray
+            Singular values cutted when the gate link is contracted
+        """
+        # Sort sites
+        # mpo.sort_sites()
+        sites = np.array([mpo_site.site for mpo_site in mpo])
+        if not np.isclose(sites, np.sort(sites)).all():
+            raise RuntimeError("MPO sites are not sorted")
+
+        # transform input into np array just in case the
+        # user passes the list
+        operators = [site.operator * site.weight for site in mpo]
+        if mpo[0].strength is not None:
+            operators[0] *= mpo[0].strength
+
+        self.site_canonize(sites[0], keep_singvals=True)
+
+        tot_singvals_cut = []
+        # Operator index
+        oidx = 0
+        next_site = self[sites[0]].eye_like(self[sites[0]].shape[0])
+        for sidx in range(sites[0], sites[-1] + 1):
+            tens = self[sidx]
+            if sidx in sites:
+                # i -o- k
+                #    |j     = T(i,k,l,m,n) -> T(i,l,m, k,n)
+                # l -o- n
+                #    |m
+                tens = tens.tensordot(operators[oidx], ([1], [2]))
+                tens.transpose_update((0, 2, 3, 1, 4))
+                # T(i,l,m, k,n) -> T(il, m, kn)
+                tens.reshape_update((np.prod(tens.shape[:2]), tens.shape[2], -1))
+
+                # The matrix next, from the second cycle, is bringing the isometry center in tens
+                # next = next.reshape(-1, tens.shape[0])
+                # x -o- il -o- kn = x -o- kn
+                #           |m         |m
+                tens = next_site.tensordot(tens, ([1], [0]))
+                oidx += 1
+
+                if sidx + 1 in sites:
+                    # Move the isometry when the next site has an MPO (and thus left-dimension kn)
+                    # x -o- kn -->  x -o- y -o- kn
+                    #    |m            |m
+                    self._tensors[sidx], next_site, _, singvals_cut = tens.split_svd(
+                        [0, 1],
+                        [2],
+                        contract_singvals="R",
+                        conv_params=self._convergence_parameters,
+                        no_truncation=True,
+                    )
+
+                    tot_singvals_cut += list(singvals_cut)
+                elif sidx == sites[-1]:
+                    # End of the procedure
+                    self._tensors[sidx] = tens
+                else:
+                    # Move the isometry when the next site does not have an MPO
+                    # x -o- kn -->  x -o- y -o- kn
+                    #    |m
+                    self._tensors[sidx], next_site = tens.split_qr([0, 1], [2])
+                    #                n|
+                    # y -o- kn --> y -o- k
+                    # T(y,kn) -> T(y, k, n) -> T(y, n, k)
+                    next_site.reshape_update(
+                        (next_site.shape[0], -1, operators[oidx - 1].shape[3])
+                    )
+                    next_site.transpose_update((0, 2, 1))
+
+            else:
+                # Site does not have an operator, just bring the isometry here
+                #   n|
+                # y -o- i -o- k -> T(y, n, j, k) -> T(y, j, n, k)
+                #          | j
+                tens = next_site.tensordot(tens, ([2], [0]))
+                tens.transpose_update((0, 2, 1, 3))
+
+                if sidx + 1 in sites:
+                    tens.reshape_update((tens.shape[0], tens.shape[1], -1))
+                    self._tensors[sidx], next_site, _, singvals_cut = tens.split_svd(
+                        [0, 1],
+                        [2],
+                        contract_singvals="R",
+                        conv_params=self._convergence_parameters,
+                        no_truncation=True,
+                    )
+                    tot_singvals_cut += list(singvals_cut)
+                else:
+                    #   n|                 |n
+                    # y -o- k --> y -o- s -o- k
+                    #    |j          |j
+                    self._tensors[sidx], next_site = tens.split_qr([0, 1], [2, 3])
+
+        self._first_non_orthogonal_left = sites[-1]
+        self._first_non_orthogonal_right = sites[-1]
+        self.iso_towards(sites[0], trunc=True, keep_singvals=True)
+
+        return tot_singvals_cut
 
     def reset(self, idxs=None):
         """
         Reset the states of the sites idxs to the |0> state
 
         Parameters
         ----------
@@ -1361,36 +1890,132 @@
         for idx in idxs:
             state, _ = self.apply_projective_operator(idx)
             if state != 0:
                 new_projector = np.zeros((self._local_dim[idx], self._local_dim[idx]))
                 new_projector[0, state] = 1
                 self.apply_one_site_operator(new_projector, idx)
 
-        self.left_canonize(self.num_sites - 1, svd=True)
-        self.right_canonize(0, svd=True)
+        self.left_canonize(self.num_sites - 1, trunc=True)
+        self.right_canonize(0, trunc=True)
 
-    def norm(self):
+    #########################################################################
+    ######################### Optimization methods ##########################
+    #########################################################################
+
+    def default_sweep_order(self):
         """
-        Returns the norm of the MPS <self|self>
+        Default sweep order to be used in the ground state search/time evolution.
+        Default for MPS is left-to-right.
 
-        Return
-        ------
-        norm: float
-            norm of the MPS
+        Returns
+        -------
+        List[int]
+            The generator that you can sweep through
         """
-        xp = self._device_checks()
-        idx = self.first_non_orthogonal_right
+        return list(range(self.num_sites))
 
-        if self.first_non_orthogonal_left == self.first_non_orthogonal_right:
-            norm = xp.tensordot(self[idx], xp.conj(self[idx]), ([0, 1, 2], [0, 1, 2]))
+    def get_pos_partner_link_expansion(self, pos):
+        """
+        Get the position of the partner tensor to use in the link expansion
+        subroutine. It is the tensor towards the center, that is supposed to
+        be more entangled w.r.t. the tensor towards the edge
+
+        Parameters
+        ----------
+        pos : int
+            Position w.r.t. which you want to compute the partner
+
+        Returns
+        -------
+        int
+            Position of the partner
+        int
+            Link of pos pointing towards the partner
+        int
+            Link of the partner pointing towards pos
+        """
+        pos_partner = pos + 1 if pos < self.num_sites / 2 else pos - 1
+        link_self = 2 if pos < pos_partner else 0
+        link_partner = 0 if pos < pos_partner else 2
+
+        return pos_partner, link_self, link_partner
+
+    #########################################################################
+    ######################## Time evolution methods #########################
+    #########################################################################
+
+    def _partial_iso_towards_for_timestep(self, pos, next_pos, no_rtens=False):
+        """
+        Move by hand the iso for the evolution backwards in time
+
+        Parameters
+        ----------
+        pos : Tuple[int]
+            Position of the tensor evolved
+        next_pos : Tuple[int]
+            Position of the next tensor to evolve
+
+        Returns
+        -------
+        QTeaTensor | link_self
+            The R tensor of the iso movement
+            link_self in no_rtens=True mode
+        Tuple[int]
+            The position of the partner (pos+-1 in MPSs)
+        int
+            The link of the partner pointing towards pos
+        List[int]
+            The update path to pass to _update_eff_ops
+        """
+        requires_singvals = self._requires_singvals
+
+        # Needed in other TN geometries
+        link_partner = 0 if pos < next_pos else 2
+        pos_partner = pos + 1 if pos < next_pos else pos - 1
+
+        path_elem = [pos, next_pos]
+        if no_rtens:
+            link_self = 2 if pos < next_pos else 0
+            return link_self, pos_partner, link_partner, path_elem
+
+        if (pos < next_pos) and requires_singvals:
+            # Going left-to-right, SVD
+            qtens, rtens, s_vals, _ = self[pos].split_svd(
+                [0, 1],
+                [2],
+                no_truncation=True,
+                conv_params=self._convergence_parameters,
+                contract_singvals="R",
+            )
+            self.set_singvals_on_link(pos, pos_partner, s_vals)
+
+        elif pos < next_pos:
+            # Going left-to-right, QR
+            qtens, rtens = self[pos].split_qr([0, 1], [2])
+            self.set_singvals_on_link(pos, pos_partner, None)
+        elif requires_singvals:
+            # Going right-to-left, SVD
+            qtens, rtens, s_vals, _ = self[pos].split_svd(
+                [1, 2],
+                [0],
+                no_truncation=True,
+                conv_params=self._convergence_parameters,
+                contract_singvals="R",
+                perm_left=[2, 0, 1],
+            )
+            self.set_singvals_on_link(pos, pos_partner, s_vals)
         else:
-            self.left_canonize(self.first_non_orthogonal_right, keep_singvals=True)
-            norm = xp.tensordot(self[idx], xp.conj(self[idx]), ([0, 1, 2], [0, 1, 2]))
+            # Going right-to-left, RQ. Need to permute Q tensor (this is called
+            # also by abstractTN where R cannot be permuted, always the first
+            # link needs to go to the Q-tensor.)
+            qtens, rtens = self[pos].split_qr([1, 2], [0], perm_left=[2, 0, 1])
+            self.set_singvals_on_link(pos, pos_partner, None)
+        self[pos] = qtens
 
-        return np.sqrt(np.real(norm))
+        return rtens, pos_partner, link_partner, path_elem
 
     def contract(self, other, boundaries=None):
         """
         Contract the MPS with another MPS other <other|self>.
         By default it is a full contraction, but also a partial
         contraction is possible
 
@@ -1419,30 +2044,27 @@
         if boundaries is None:
             full_contraction = True
             boundaries = (0, self.num_sites, 1)
         else:
             full_contraction = False
             boundaries = (*boundaries, np.sign(boundaries[1] - boundaries[0]))
 
-        xp = self._device_checks()
-
         idx = 0 if boundaries[1] > boundaries[0] else 2
-        transfer_mat = xp.eye(self[boundaries[0]].shape[idx])
+        transfer_mat = self[boundaries[0]].eye_like(self[boundaries[0]].links[idx])
         for ii in range(*boundaries):
             if boundaries[2] > 0:
-                transfer_mat = xp.tensordot(transfer_mat, self[ii], ([0], [idx]))
+                transfer_mat = transfer_mat.tensordot(self[ii], ([0], [idx]))
             else:
-                transfer_mat = xp.tensordot(self[ii], transfer_mat, ([idx], [0]))
+                transfer_mat = self[ii].tensordot(transfer_mat, ([idx], [0]))
 
-            transfer_mat = xp.tensordot(
-                transfer_mat, xp.conj(other[ii]), ([idx, 1], [idx, 1])
+            transfer_mat = transfer_mat.tensordot(
+                other[ii].conj(), ([idx, 1], [idx, 1])
             )
         if full_contraction:
-            transfer_mat = transfer_mat.flatten()
-            contraction = transfer_mat[0]
+            contraction = transfer_mat.get_entry()
         else:
             new_shape = (
                 (1, *transfer_mat.shape)
                 if boundaries[1] > boundaries[0]
                 else (*transfer_mat.shape, 1)
             )
             contraction = transfer_mat.reshape(new_shape)
@@ -1470,28 +2092,35 @@
         if not isinstance(other, MPS):
             raise TypeError("Only two MPS classes can be concatenated")
         elif self[-1].shape[2] != 1 and other[0].shape[0] != 1:
             raise ValueError(
                 "Head and tail of the MPS not compatible. Last "
                 + "and first dimensions of the tensors must be the same"
             )
-        elif self.device != other.device:
+        elif self._tensor_backend.device != other._tensor_backend.device:
             raise RuntimeError(
                 "MPS to be kron multiplied must be on the same "
-                + f"device, not {self.device} and {other.device}"
+                + f"device, not {self._tensor_backend.device} and "
+                + f"{other._tensor_backend.device}."
             )
-        max_bond_dim = max(self.max_bond_dim, other.max_bond_dim)
-        cut_ratio = min(self.cut_ratio, other.cut_ratio)
+        max_bond_dim = max(
+            self._convergence_parameters.max_bond_dimension,
+            other._convergence_parameters.max_bond_dimension,
+        )
+        cut_ratio = min(
+            self._convergence_parameters.cut_ratio,
+            other._convergence_parameters.cut_ratio,
+        )
         convergence_params = TNConvergenceParameters(
             max_bond_dimension=int(max_bond_dim), cut_ratio=cut_ratio
         )
         tensor_list = self.tensors + other.tensors
 
         addMPS = MPS.from_tensor_list(
-            tensor_list, convergence_params, device=self.device
+            tensor_list, convergence_params, tensor_backend=self._tensor_backend
         )
         addMPS._singvals[: self.num_sites + 1] = self.singvals
         addMPS._singvals[self.num_sites + 1 :] = other.singvals[1:]
 
         if inplace:
             self.__dict__.update(addMPS.__dict__)
             return None
@@ -1500,15 +2129,17 @@
 
     # ---------------------------
     # ----- MEASURE METHODS -----
     # ---------------------------
 
     def meas_tensor_product(self, ops, idxs):
         """
-        Measure the tensor products of n operators `ops` acting on the indexes `idxs`
+        Measure the tensor products of n operators `ops` acting on the indexes `idxs`.
+        The operators should be MPOs, i.e. rank-4 tensors of shape (left, up, down, right).
+        To retrieve the tensor product operators, left=right=1.
 
         Parameters
         ----------
         ops : list of ndarrays
             List of numpy arrays which are one-site operators
         idxs : list of int
             Indexes where the operators are applied
@@ -1518,60 +2149,62 @@
         measure : float
             Result of the measurement
         """
         self.check_obs_input(ops, idxs)
 
         if len(idxs) == 0:
             return 1
-        xp = self._device_checks()
+
         order = np.argsort(idxs)
         idxs = np.array(idxs)[order]
-        ops = xp.array(ops)
-        ops = ops[order]
         self.site_canonize(idxs[0], keep_singvals=True)
 
-        transfer_mat = xp.eye(self[idxs[0]].shape[0], dtype=xp.complex64)
+        transfer_mat = (
+            self[idxs[0]].eye_like(self[idxs[0]].links[0]).attach_dummy_link(1)
+        )
         jj = 0
         closed = False
         for ii in range(idxs[0], self.num_sites):
             if closed:
                 break
 
             # Case of finished tensors
             if jj == len(idxs):
                 # close with transfer matrix of correct size
-                closing_transfer_mat = xp.eye(self[ii].shape[0])
-                measure = xp.tensordot(
-                    transfer_mat, closing_transfer_mat, ([0, 1], [0, 1])
+                closing_transfer_mat = (
+                    self[ii].eye_like(self[ii].links[0]).attach_dummy_link(1)
+                )
+                measure = transfer_mat.tensordot(
+                    closing_transfer_mat, ([0, 1, 2], [0, 1, 2])
                 )
                 closed = True
             # Case of operator inside
             elif idxs[jj] == ii:
-                transfer_mat = xp.tensordot(transfer_mat, self[ii], ([0], [0]))
-                transfer_mat = xp.tensordot(transfer_mat, ops[jj], ([1], [1]))
-                transfer_mat = xp.transpose(transfer_mat, [0, 2, 1])
-                transfer_mat = xp.tensordot(
-                    transfer_mat, xp.conj(self[ii]), ([0, 1], [0, 1])
-                )
+                op_jj = ops[order[jj]]
+                transfer_mat = transfer_mat.tensordot(self[ii], ([0], [0]))
+                transfer_mat = transfer_mat.tensordot(op_jj, ([0, 2], [0, 2]))
+                transfer_mat = transfer_mat.tensordot(self[ii].conj(), ([0, 2], [0, 1]))
                 jj += 1
             # Case of no operator between the sites
             else:
-                transfer_mat = xp.tensordot(transfer_mat, self[ii], ([0], [0]))
-                transfer_mat = xp.tensordot(
-                    transfer_mat, xp.conj(self[ii]), ([0, 1], [0, 1])
-                )
+                transfer_mat = transfer_mat.tensordot(self[ii], ([0], [0]))
+                transfer_mat = transfer_mat.tensordot(self[ii].conj(), ([1, 2], [0, 1]))
+                transfer_mat.transpose_update([1, 0, 2])
 
         if not closed:
             # close with transfer matrix of correct size
-            closing_transfer_mat = xp.eye(self[-1].shape[2])
-            measure = xp.tensordot(transfer_mat, closing_transfer_mat, ([0, 1], [0, 1]))
+            closing_transfer_mat = (
+                self[-1].eye_like(self[-1].links[2]).attach_dummy_link(1)
+            )
+            measure = transfer_mat.tensordot(
+                closing_transfer_mat, ([0, 1, 2], [0, 1, 2])
+            )
             closed = True
 
-        if xp == cp:
-            measure = measure.get()
+        measure = measure.get_entry()
 
         return np.real(measure)
 
     def meas_weighted_sum(self, op_strings, idxs_strings, coefs):
         """
         Measure the weighted sum of tensor product operators.
         See :py:func:`meas_tensor_product`
@@ -1616,21 +2249,22 @@
 
         Return
         ------
         measures : dict
             Keys are the range of the bipartition from 0 to which the entanglement
             (value) is relative
         """
-        xp = self._device_checks()
         measures = {}
         for ii, ss in enumerate(self.singvals[1:-1]):
+            if hasattr(ss, "get"):
+                ss = ss.get()
             if ss is None:
                 s_von_neumann = None
             else:
-                s_von_neumann = -xp.sum(ss**2 * xp.log(ss**2))
+                s_von_neumann = -2 * (ss**2 * np.log(ss)).sum()
 
             measures[(0, ii + 1)] = s_von_neumann
 
         return measures
 
     def meas_even_probabilities(self, threshold, qiskit_convention=False):
         """
@@ -1857,50 +2491,50 @@
         -------
         probabilities : list of floats
             Probabilities of the children
         tensor_list : list of ndarray
             Child tensors, already contracted with the next site
             if not last site.
         """
-        xp = self._device_checks()
         local_dim = self.local_dim[site_idx]
         if tensor is None:
-            return xp.zeros(local_dim), np.repeat(None, local_dim)
+            tmp = tensor.vector_with_dim_like(local_dim)
+            tmp *= 0.0
+            return tmp, np.repeat(None, local_dim)
 
-        conjg_tens = xp.conj(tensor)
-        probabilities = []
+        conjg_tens = tensor.conj()
         tensors_list = []
 
         # Construct rho at effort O(chi_l * chi_r * d^2) which is
         # equal to contracting one projector to one tensor
-        reduced_rho = xp.diag(xp.tensordot(tensor, conjg_tens, ([0, 2], [0, 2])))
+        reduced_rho = tensor.tensordot(conjg_tens, ([0, 2], [0, 2]))
+
+        # Convert to array on host/CPU with real values; select diagonal elements
+        probabilities = reduced_rho.diag(real_part_only=True, do_get=True)
 
         # Loop over basis states
-        for jj, prob_jj in enumerate(reduced_rho):
+        for jj, prob_jj in enumerate(probabilities):
             # Compute probabilities of the state; projecting always to
             # one index `j`, we can read the diagonal entries of the
             # reduced density matrix
-            probabilities.append(np.real(prob_jj))
+            # --> we have it already due to the trace
 
             # Create list of updated tensors after the projection
             if prob_jj > 0 and site_idx < self.num_sites - 1:
                 # Extract the rank-2 tensor without tensordot as we operator
                 # on a diagonal projector with a single index
-                temp_tens = tensor[:, jj, :]
+                temp_tens = tensor.subtensor_along_link(1, jj, jj + 1)
+                temp_tens.remove_dummy_link(1)
 
                 # Contract with the next site in the MPS
-                temp_tens = xp.tensordot(temp_tens, self[site_idx + 1], ([1], [0]))
+                temp_tens = temp_tens.tensordot(self[site_idx + 1], ([1], [0]))
                 tensors_list.append(temp_tens * (prob_jj ** (-0.5)))
             else:
                 tensors_list.append(None)
 
-        probabilities = xp.array(probabilities)
-        if xp == cp:
-            probabilities = probabilities.get()
-
         return probabilities, tensors_list
 
     def _get_children_magic(self, transfer_matrix, site_idx, *args):
         """
         Compute the probability and the relative tensor state of all the
         children of site `site_idx` in the tensor tree
 
@@ -1918,49 +2552,59 @@
         -------
         probabilities : list of floats
             Probabilities of the children
         tensor_list : list of ndarray
             Child tensors, already contracted with the next site
             if not last site.
         """
-        xp = self._device_checks()
+        tensor = deepcopy(self.get_tensor_of_site(site_idx))
 
         if transfer_matrix is None:
-            return xp.zeros(4), np.repeat(None, 4)
+            tmp = tensor.vector_with_dim_like(4)
+            tmp *= 0.0
+            return tmp, np.repeat(None, 4)
 
-        tensor = deepcopy(self.get_tensor_of_site(site_idx))
-        probabilities = xp.zeros(4)
+        sqrt, real = tensor.get_attr("sqrt", "real")
+        probabilities = tensor.vector_with_dim_like(4)
         tensors_list = []
 
-        paulis = [
-            xp.identity(2),
-            xp.array([[0, 1], [1, 0]]),
-            xp.array([[0, -1j], [1j, 0]]),
-            xp.array([[1, 0], [0, -1]]),
-        ]
+        rho_i = tensor.tensordot(tensor.conj(), ([0, 2], [0, 2]))
+        pauli_1 = rho_i.zeros_like()
+        pauli_x = rho_i.zeros_like()
+        pauli_y = rho_i.zeros_like()
+        pauli_z = rho_i.zeros_like()
+
+        pauli_1.set_diagonal_entry(0, 1)
+        pauli_1.set_diagonal_entry(1, 1)
+        pauli_x.set_matrix_entry(0, 1, 1)
+        pauli_x.set_matrix_entry(1, 0, 1)
+        pauli_y.set_matrix_entry(0, 1, -1j)
+        pauli_y.set_matrix_entry(1, 0, 1j)
+        pauli_z.set_diagonal_entry(0, 1)
+        pauli_z.set_diagonal_entry(1, -1)
+        paulis = [pauli_1, pauli_x, pauli_y, pauli_z]
+
         original_transfer_matrix = deepcopy(transfer_matrix)
         for ii, pauli in enumerate(paulis):
-            temp_tens = xp.tensordot(tensor, pauli, ([1], [1]))
-            transfer_matrix = xp.tensordot(
-                original_transfer_matrix, temp_tens, ([0], [0])
-            )
-            transfer_matrix = xp.tensordot(
-                transfer_matrix, tensor.conj(), ([0, 2], [0, 1])
-            )
-            probabilities[ii] = np.real(
-                xp.tensordot(transfer_matrix, transfer_matrix.conj(), ([0, 1], [0, 1]))
-                / 2
-            )
-            if probabilities[ii] > 0 and site_idx < self.num_sites - 1:
-                tensors_list.append(transfer_matrix / np.sqrt(probabilities[ii] * 2))
+            temp_tens = tensor.tensordot(pauli, ([1], [1]))
+            transfer_matrix = original_transfer_matrix.tensordot(temp_tens, ([0], [0]))
+            transfer_matrix = transfer_matrix.tensordot(tensor.conj(), ([0, 2], [0, 1]))
+
+            probability_as_tensor = transfer_matrix.tensordot(
+                transfer_matrix.conj(), ([0, 1], [0, 1])
+            )
+            probabilities[ii] = real(probability_as_tensor.flatten() / 2)
+            prob_host = np.real(probability_as_tensor.get_entry()) / 2
+            if prob_host > 0 and site_idx < self.num_sites - 1:
+                tensors_list.append(transfer_matrix / sqrt(real(probabilities[ii] * 2)))
             else:
                 tensors_list.append(None)
 
-        if xp == cp:
-            probabilities = probabilities.get()
+        probabilities = tensor.get_of(probabilities)
+        probabilities = np.real(probabilities)
 
         return probabilities, tensors_list
 
     def _get_child_prob(self, tensor, site_idx, target_prob, unitary_setup, *args):
         """
         Compute which child has to be selected for a given target probability
         and return the index and the tensor of the next site to be measured.
@@ -1980,48 +2624,51 @@
             If `None`, no local unitaries are applied. Otherwise,
             unitary for local transformations are provided and applied
             to the local sites.
         args : list
             Other argument are not needed for the MPS implementation
             and stored in `*args`.
         """
-        xp = self._device_checks()
+        # Get functions for elemtary arrays
+        cumsum, sqrt = tensor.get_attr("cumsum", "sqrt")
+
         local_dim = self.local_dim[site_idx]
 
         if unitary_setup is not None:
             # Have to apply local unitary
             unitary = unitary_setup.get_unitary(site_idx)
 
             # Contract and permute back
-            tensor = np.tensordot(unitary, tensor, ([1], [1]))
-            tensor = np.transpose(tensor, [1, 0, 2])
+            tensor = unitary.tensordot(tensor, ([1], [1]))
+            tensor.transpose_update([1, 0, 2])
 
-        conjg_tens = xp.conj(tensor)
+        conjg_tens = tensor.conj()
 
         # Calculate the cumulated probabilities via the reduced
         # density matrix
-        reduced_rho = xp.tensordot(tensor, conjg_tens, ([0, 2], [0, 2]))
-        probs = xp.real(xp.diag(reduced_rho))
-        cumul_probs = xp.cumsum(probs)
+        reduced_rho = tensor.tensordot(conjg_tens, ([0, 2], [0, 2]))
 
+        probs = reduced_rho.diag(real_part_only=True)
+        cumul_probs = cumsum(probs)
         measured_idx = None
 
         for jj in range(local_dim):
             if cumul_probs[jj] < target_prob:
                 continue
 
             prob_jj = probs[jj]
 
             # Reached interval with target probability ... project
             measured_idx = jj
-            temp_tens = tensor[:, jj, :]
-            temp_tens /= probs[jj] ** 0.5
+            temp_tens = tensor.subtensor_along_link(1, jj, jj + 1)
+            temp_tens.remove_dummy_link(1)
+            temp_tens /= sqrt(probs[jj])
 
             if site_idx < self.num_sites - 1:
-                temp_tens = xp.tensordot(temp_tens, self[site_idx + 1], ([1], [0]))
+                temp_tens = temp_tens.tensordot(self[site_idx + 1], ([1], [0]))
             else:
                 temp_tens = None
 
             break
 
         return measured_idx, temp_tens, prob_jj
 
@@ -2041,61 +2688,161 @@
         cmplx: bool, optional
             If True the MPS is complex, real otherwise. Default to True
 
         Returns
         -------
         None
         """
-        self.to_device("cpu")
+        self.convert(None, "cpu")
+
         with open(filename, "w") as fh:
             fh.write(str(len(self)) + " \n")
             for tens in self:
-                write_tensor(tens, fh, cmplx=cmplx)
+                tens.write(fh, cmplx=cmplx)
 
         return None
 
     @classmethod
-    def read(cls, filename, cmplx=True, order="F", device="cpu"):
+    def read(cls, filename, tensor_backend, cmplx=True, order="F"):
         """
         Read an MPS written by FORTRAN in a formatted way on file.
         Reads in column-major order but the output is in row-major.
         This is the only method that overrides the number of sites,
         since you may not know before reading.
 
         Parameters
         ----------
         filename: str
             PATH to the file
+        tensor_backend : :class:`TensorBackend`
+            Setup which tensor class to create.
         cmplx: bool, optional
             If True the MPS is complex, real otherwise. Default to True
         order: str, optional
             If 'F' the tensor is transformed from column-major to row-major, if 'C'
             it is left as read.
-        device: str, optional
-            Device where the MPS is stored
-
 
         Returns
         -------
         obj: py:class:`MPS`
             MPS class read from file
         """
         tensors = []
         with open(filename, "r") as fh:
             num_sites = int(fh.readline())
 
             for _ in range(num_sites):
-                tens = read_tensor(fh, cmplx=cmplx, order=order)
+                tens = tensor_backend.tensor_cls.read(
+                    fh,
+                    tensor_backend.dtype,
+                    tensor_backend.device,
+                    tensor_backend.base_tensor_cls,
+                    cmplx=cmplx,
+                    order=order,
+                )
                 tensors.append(tens)
 
-        obj = cls.from_tensor_list(tensors)
-        obj.to_device(device)
+        obj = cls.from_tensor_list(tensors, tensor_backend=tensor_backend)
 
         return obj
 
+    # --------------------------------------
+    # ---- Effective operators methods -----
+    # --------------------------------------
+
+    # pylint: disable-next=unused-argument
+    def build_effective_operators(self, measurement_mode=False):
+        """
+        Build the complete effective operator on each
+        of the links. It assumes `self.eff_op` is set.
+
+        Parameters
+        ----------
+        measurement_mode : bool, optional
+            If True, enable measurement mode of effective operators
+        """
+        self.iso_towards(self.num_sites - 1, keep_singvals=True)
+
+        if self.eff_op is None:
+            raise Exception("Trying to build eff_op without attribute being set.")
+
+        for pos, tens in enumerate(self[:-1]):
+            # Retrieve the index of the operators for the left link
+            # and the physical link
+            idx_out = 2
+            pos_links = self.get_pos_links(pos)
+            self.eff_op.contr_to_eff_op(tens, pos, pos_links, idx_out)
+
+            if measurement_mode:
+                # pylint: disable-next=unsubscriptable-object
+                self.eff_op[pos, pos_links[idx_out]].run_measurements(
+                    tens, idx_out, self.singvals[pos + 1]
+                )
+
+        if measurement_mode:
+            # To finish measurements, we keep going through the last site as
+            # well
+            pos = self.num_sites - 1
+            idx_out = 2
+            pos_links = self.get_pos_links(pos)
+            self.eff_op.contr_to_eff_op(self[-1], pos, pos_links, idx_out)
+
+            # Last center must be isometry center
+            link_weights = None
+            # pylint: disable-next=unsubscriptable-object
+            self.eff_op[(pos, pos_links[idx_out])].run_measurements(
+                self[-1], idx_out, link_weights
+            )
+
+    def _update_eff_ops(self, id_step):
+        """
+        Update the effective operators after the iso shift
+
+        Parameters
+        ----------
+        id_step : list of ints
+            List with the iso path, i.e. `[src_tensor, dst_tensor]`
+
+        Returns
+        -------
+        None
+            Updates the effective operators in place
+        """
+        # Get info on the source tensor
+        tens = self[id_step[0]]
+        src_link = 0 if id_step[0] > id_step[1] else 2
+        links = self.get_pos_links(id_step[0])
+
+        # Perform the contraction
+        self.eff_op.contr_to_eff_op(tens, id_step[0], links, src_link)
+
+    def deprecated_get_eff_op_on_pos(self, pos):
+        """
+        Obtain the list of effective operators adjacent
+        to the position pos and the index where they should
+        be contracted
+
+        Parameters
+        ----------
+        pos : list
+            list of [layer, tensor in layer]
+
+        Returns
+        -------
+        list of IndexedOperators
+            List of effective operators
+        list of ints
+            Indexes where the operators should be contracted
+        """
+        # pylint: disable-next=unsubscriptable-object
+        eff_ops = [self.eff_op[oidx] for oidx in self.op_neighbors[:, pos]]
+        idx_list = np.arange(3)
+
+        return eff_ops, idx_list
+
     # ------------------------
     # ---- ML Operations -----
     # ------------------------
     def ml_get_gradient_tensor(self, idx, data_sample, true_label):
         """
         Get the gradient w.r.t. the tensors at position `idx`, `idx+1`
         of the MPS following the procedure explained in
@@ -2112,44 +2859,46 @@
             True label of the datasample
 
         Returns
         -------
         xp.ndarray
             Gradient tensor
         """
-        xp = self._device_checks()
+        real = self[0].get_attr("real")
+
         self.site_canonize(idx, True)
 
         if idx == 0:
-            left_effective_feature = np.ones(1).reshape(1, 1)
+            left_effective_feature = self[0].eye_like(1)
         else:
-            left_effective_feature = xp.squeeze(
-                self.contract(data_sample, (0, idx)), axis=0
-            )
+            left_effective_feature = self.contract(data_sample, (0, idx))
+            left_effective_feature.remove_dummy_link(0)
+
         if idx == self.num_sites - 2:
-            right_effective_feature = np.ones(1).reshape(1, 1)
+            right_effective_feature = self[0].eye_like(1)
         else:
-            right_effective_feature = xp.squeeze(
-                self.contract(data_sample, (self.num_sites - 1, idx + 1)), axis=2
+            right_effective_feature = self.contract(
+                data_sample, (self.num_sites - 1, idx + 1)
             )
+            right_effective_feature.remove_dummy_link(2)
 
         # Compute the label efficiently
         label = left_effective_feature
         for ii in (idx, idx + 1):
-            label = xp.tensordot(label, self[ii], ([0], [0]))
-            label = xp.tensordot(label, xp.conj(data_sample[ii]), ([0, 1], [0, 1]))
-        label = xp.tensordot(label, right_effective_feature, ([0, 1], [0, 1]))
+            label = label.tensordot(self[ii], ([0], [0]))
+            label = label.tensordot(data_sample[ii].conj(), ([0, 1], [0, 1]))
+        label = label.tensordot(right_effective_feature, ([0, 1], [0, 1])).get_entry()
 
         # Compute the loss function
-        loss = true_label - xp.real(label)
+        loss = true_label - real(label)
 
         # Compute the gradient
-        grad = xp.tensordot(left_effective_feature.conj(), data_sample[idx], ([1], [0]))
-        grad = xp.tensordot(grad, data_sample[idx + 1], ([2], [0]))
-        grad = xp.tensordot(grad, right_effective_feature.conj(), ([3], [1]))
+        grad = left_effective_feature.conj().tensordot(data_sample[idx], ([1], [0]))
+        grad = grad.tensordot(data_sample[idx + 1], ([2], [0]))
+        grad = grad.tensordot(right_effective_feature.conj(), ([3], [1]))
         grad *= loss
 
         return grad, loss
 
     def ml_optmize_tensor(
         self, idx, data_samples, true_labels, learning_rate, n_jobs=1, direction=1
     ):
@@ -2172,40 +2921,43 @@
         Returns
         -------
         xp.ndarray
             Singular values cut in the optimization
         float
             Value of the loss function
         """
-        xp = self._device_checks()
+        array = self[0].get_attr("array")
 
         # Canonize to idx
         self.site_canonize(idx, True)
 
         # Run in parallel the data batch
-        res = xp.array(
+        res = array(
             Parallel(n_jobs=n_jobs)(
                 delayed(self.ml_get_gradient_tensor)(idx, ds, tl)
                 for ds, tl in zip(data_samples, true_labels)
             ),
             dtype=object,
         )
 
         # Sum the values for computing gradient and loss
-        grad = xp.sum(res[:, 0])
-        loss = xp.sum(res[:, 1])
+        grad = res[:, 0].sum()
+        loss = res[:, 1].sum()
 
         # Compute the two_tensor of site idx, idx+1 for the update
-        two_tensors = xp.tensordot(self[idx], self[idx + 1], ([2], [0]))
+        two_tensors = self[idx].tensordot(self[idx + 1], ([2], [0]))
         two_tensors += learning_rate * grad
 
         # Split the tensor back and update the MPS
         direction = "R" if direction > 0 else "L"
-        left, right, singvals, singval_cut = self.tSVD(
-            two_tensors, [0, 1], [2, 3], contract_singvals=direction
+        left, right, singvals, singval_cut = two_tensors.split_svd(
+            [0, 1],
+            [2, 3],
+            contract_singvals=direction,
+            conv_params=self._convergence_parameters,
         )
         self[idx] = left
         self[idx + 1] = right
         self.singvals[idx + 1] = singvals
         # self.normalize()
 
         return singval_cut, loss
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/state_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/state_simulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -337,17 +337,25 @@
         """
         return self._global_dim
 
     @property
     def state(self):
         """
         State property.
+        The state vector in the shape of a N-legged tensor for N sites.
         """
         return self._state
 
+    @state.setter
+    def state(self, value):
+        """
+        Setter for state, used to update the state vector.
+        """
+        self._state = value
+
     def apply_global_operator(self, global_op):
         """
         Applies a global operator to the state; the state is updated
         in-place.
 
         **Arguments**
 
@@ -365,33 +373,90 @@
             raise Exception(
                 "Global operator must match the " + "Hilbert space dimension."
             )
 
         state = np.reshape(self.state, [global_op.shape[0]])
         self._state = np.reshape(global_op.dot(state), self.local_dim)
 
+    def apply_two_site_operator(self, twosite_op, sites):
+        """
+        Applies a two-site operator to the state; the state is updated
+        in-place.
+
+        **Arguments**
+
+        twosite_op : np.array, rank-4
+            Two-site operator to apply. The contraction with the state
+            is done over the links [2,3] of the operator.
+
+        sites : list/np.array of len 2
+            Sites indices on which to apply the operator.
+
+        **Returns**
+
+        Return ``None``; instance of class is updated in-place.
+        """
+        sites = np.array(sites)
+        if len(sites) != 2:
+            raise Exception(f"{len(sites)} sites passed for a two-site operator.")
+
+        if np.max(sites) >= self._num_sites or any(site < 0 for site in sites):
+            raise Exception(
+                "Site index out of range. Cannot apply operator"
+                f" on sites {sites} to {self._num_sites}-site system."
+            )
+        if twosite_op.ndim != 4:
+            raise Exception("Two-site operator must be rank-4.")
+
+        if (
+            twosite_op.shape[0] != twosite_op.shape[2]
+            or twosite_op.shape[1] != twosite_op.shape[3]
+        ):
+            raise Exception(
+                "Shape mismatch, two-site operator cannot change local Hilbert"
+                " space dimension."
+            )
+
+        if (
+            twosite_op.shape[2] != self._local_dim[sites[0]]
+            or twosite_op.shape[3] != self._local_dim[sites[1]]
+        ):
+            raise Exception(
+                "Shape mismatch: local dimension in two-site operator"
+                " doesn't match the state's local Hilbert space dimension."
+            )
+
+        # apply the operator
+        self._state = np.tensordot(self._state, twosite_op, [sites, [2, 3]])
+
+        # permute the legs into the original order
+        permutation = np.arange(self._num_sites - 2)
+        permutation = np.insert(permutation, sites[0], self._num_sites - 2)
+        permutation = np.insert(permutation, sites[1], self._num_sites - 1)
+        self._state = np.transpose(self._state, permutation)
+
     def dot(self, other):
         """
         Calculate the dot-product or overlap between two state vectors, i.e.,
-        <other | self>.
+        <self | other>.
 
         **Arguments**
 
         other : :class:`StateVector`, numpy ndarray
             Measure the overlap with this other state vector..
 
         **Returns**
 
         Scalar representing the overlap; complex valued.
         """
         if isinstance(other, np.ndarray):
-            return np.conj(other.flatten()).dot(self._state.flatten())
+            return np.conj(self.state.flatten()).dot(other.flatten())
 
         if isinstance(other, StateVector):
-            return np.conj(other.state.flatten()).dot(self._state.flatten())
+            return np.conj(self.state.flatten()).dot(other.state.flatten())
 
         raise Exception("Unknown type for other")
 
     def meas_global_operator(self, global_op):
         """
         Measure the expectation value of a global operator.
 
@@ -414,14 +479,55 @@
         **Returns**
 
         norm : float
             Real-valued scalar with the norm.
         """
         return np.real(np.sum(np.conj(self._state) * self._state))
 
+    def norm_sqrt(self):
+        """
+        Calculate the square root of the norm of the state.
+
+        **Returns**
+
+        norm_sqrt : float
+            The square root of the norm.
+        """
+        return np.sqrt(self.norm())
+
+    def add_update(self, other, factor_this=None, factor_other=None):
+        """
+        Inplace addition as `self = factor_this * self + factor_other * other`.
+        Exactly copied from the QteaTensor class (Feb 2024).
+
+        **Arguments**
+
+        other : same instance as `self`
+            Will be added to `self`. Unmodified on exit.
+
+        factor_this : scalar
+            Scalar weight for tensor `self`.
+
+        factor_other : scalar
+            Scalar weight for tensor `other`
+        """
+        if (factor_this is None) and (factor_other is None):
+            self.state += other.state
+            return
+
+        if factor_this is not None:
+            self.state *= factor_this
+            return
+
+        if factor_other is None:
+            self.state += other.state
+            return
+
+        self.state += factor_other * other.state
+
     def normalize(self):
         """
         Normalize the current state in-place.
 
         **Returns**
 
         psi : :class:`StateVector`
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/ttn_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/ttn_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,52 +7,33 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 The module contains a light-weight TTN class.
 """
-import os
 import warnings
 from copy import deepcopy
 import numpy as np
 
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 from matplotlib import colors
 import matplotlib.cm as cmx
 
 from qtealeaves.convergence_parameters import TNConvergenceParameters
-from qtealeaves.hilbert_curvature import map_selector
-from qtealeaves.modeling import TensorProductOperator
-from .abstract_tn import _AbstractTN, TNnode, _projector, _transpose_idx
-from ..fortran_interfaces import write_tensor, read_tensor
-
-# Try to import cupy
-try:
-    import cupy as cp
-    from cupy_backends.cuda.api.runtime import CUDARuntimeError
-
-    try:
-        _ = cp.cuda.Device()
-        GPU_AVAILABLE = True
-    except CUDARuntimeError:
-        GPU_AVAILABLE = False
-except ImportError:
-    cp = None
-    GPU_AVAILABLE = False
+from qtealeaves.tooling.hilbert_curvature import map_selector
+from qtealeaves.tooling.permutations import _transpose_idx
+from qtealeaves.tensors import _AbstractQteaTensor
+from qtealeaves.mpos import SparseMatrixOperatorPy
 
-__all__ = ["TTN"]
+from .tnnode import TNnode
+from .abstract_tn import _AbstractTN, _projector_for_rho_i
 
-# Enable fast switch, previously use sys.getsizeof had trouble
-# in resolving size, numpy attribute is only for array without
-# metadata, but metadata like dimensions is only small overhead.
-# (fast switch if we want to use another approach for estimating
-# the size of a numpy array)
-getsizeof = lambda arg: arg.nbytes
+__all__ = ["TTN"]
 
 
 class TTNLayer(list):
     """
     One layer of the TTN.
 
     Parameters
@@ -91,15 +72,14 @@
     def __init__(
         self,
         layer_idx,
         local_dim,
         max_bond_dimension,
         max_num_links=4,
         num_tensors=1,
-        device="cpu",
     ):
         super().__init__()
 
         self.layer_idx = layer_idx
         self.local_dim = local_dim
         self.max_bond_dimension = max_bond_dimension
         self.num_tensors = num_tensors
@@ -135,33 +115,29 @@
         #########################################################
         self.is_measured = [
             True,  # TNObsLocal
             True,  # TNObsCorr
             True,  # TNDistance2Pure
             True,  # TnState2File
             True,  # TNObsTensorProduct
-            False,  # TNObsWeightedSum
-            False,  # TNPbsProjective
+            True,  # TNObsWeightedSum
+            True,  # TNObsProjective
             True,  # TNObsProbabilities
             True,  # TNObsBondEntropy
             False,  # TNObsTZeroCorr
             False,  # TNObsCorr4
             False,  # TNObsCustom
         ]
 
-        self.device = device
-
     @property
     def cc_tensors(self):
         """
         complex conjugate part of TTO layer, returns complex conjugated tensors
         """
-        xp = self._device_checks()
-
-        c_conj = [xp.conjugate(x) for x in self]
+        c_conj = [elem.conj() for elem in self]
         return c_conj
 
     @property
     def is_ttn_toplayer(self):
         """
         True if it is a top layer of the TTN ansatz
         """
@@ -196,113 +172,180 @@
         if max_bond_dimension is None:
             max_bond_dimension = np.max([tens.shape for tens in tensor_list])
         max_num_links = np.max([tens.ndim for tens in tensor_list])
         layer_idx = int(np.log2(len(tensor_list)))
 
         obj = cls(layer_idx, local_dim, max_bond_dimension, max_num_links, num_tensors)
         obj[:] = tensor_list
-        obj.to_device(device)
+
+        obj.convert(None, device)
+
+        return obj
+
+    def to_dense(self, true_copy=False):
+        """Return layer without symmetric tensors."""
+        tensor_list = []
+        for elem in self:
+            tensor_list.append(elem.to_dense(true_copy=true_copy))
+
+        obj = self.from_tensorlist(
+            tensor_list,
+            local_dim=self.local_dim,
+            max_bond_dimension=self.max_bond_dimension,
+        )
+
+        for ii, elem in enumerate(self.singvals):
+            if elem is None:
+                continue
+
+            s_vals = self[ii].to_dense_singvals(elem, true_copy=true_copy)
+            obj.singvals[ii] = s_vals
 
         return obj
 
     def initialize_layer(
         self,
         tensor_shape,
+        tensor_backend,
         initialization="random",
         isometry=True,
-        dtype=np.complex128,
-        device="cpu",
+        sectors={},
     ):
         """
         Initialize the layer with random tensor of shape tensor_shape.
         The only exception is the first tensor of the first layer,
         that has shape (*tensor_shape, 1) to encode the symmetry
 
         Parameters
         ----------
         tensor_shape : list
             shape of the tensor
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
         initialization : str, optional
             Strategy for the initialization. Available strategies are:
             - "random", all tensors initialized at random
             - "empty", layer initialized with no tensors
             - "ground", layer initialized in the state |00....0>
             Default to "random".
         isometry : bool, optional
             If True, the tree is initialized as isometry, by default True
-        device: str, optional
-            Device where the computation is done
-        dtype : dtype, optional
-            Type of the tensors in the layer
+        sectors : dict, optional
+            Can restrict symmetry sector and/or bond dimension in initialization.
+            If empty, no restriction.
+            Default to empty dictionary.
         """
-        xp = self._device_checks()
         if initialization == "empty":
             return
 
-        for ii in range(self.num_tensors):
-            if self.is_ttn_toplayer and ii == 0:
-                tshape = tensor_shape + [1]
-                rows = np.prod(tshape[:-2])
-                cols = tshape[-2]
-            else:
-                tshape = tensor_shape
-                rows = np.prod(tshape[:-1])
-                cols = tshape[-1]
-
-            if initialization == "random":
-                tensor = xp.random.rand(*tshape) + 1j * xp.random.rand(*tshape)
-                tensor = tensor.astype(dtype)
-
-            elif initialization == "ground":
-                tensor = xp.zeros(np.prod(tshape), dtype=dtype)
-                tensor[0] = 1
-                tensor = tensor.reshape(tshape)
+        link_dirs = [False, False, True]
 
-            else:
-                raise ValueError(f"{initialization} initialization not implemented")
+        # For symmetries, we need to handle TTN top layer manually (completely)
+        if self.is_ttn_toplayer and self.layer_idx == 0:
+            # Right tensor first
+            tshape = tensor_shape
+            sector = sectors.get((0, 1), None)
+            if sector is not None:
+                tshape[-1].restrict_irreps(sector)
+            rows = list(range(len(tshape)))[:-1]
+            cols = list(range(len(tshape)))[-1:]
+
+            tensor = tensor_backend.tensor_cls(
+                tshape,
+                ctrl=initialization,
+                are_links_outgoing=link_dirs,
+                **tensor_backend.tensor_cls_kwargs(),
+            )
 
             if isometry:
-                qmat, _ = xp.linalg.qr(tensor.reshape(rows, cols))
-                tensor = qmat.reshape(tshape)
+                tensor, _ = tensor.split_qr(rows, cols)
 
-            # Normalize if top left tensor
-            if self.layer_idx == 0 and ii == 0:
-                cidxs = np.arange(len(tshape))
-                norm = xp.tensordot(tensor, tensor.conj(), (cidxs, cidxs))
-                tensor /= xp.sqrt(xp.real(norm))
+            tensor_1 = tensor
+
+            # Left tensor (last link is global symmetry sector!)
+            link_dirs = [False, False, False, True]
+            ini_bond_dimension = tshape[-1].shape if tensor.has_symmetry else 1
+            links = tensor_backend.tensor_cls.set_missing_link(
+                [tshape[0], tshape[1], tshape[2], None],
+                ini_bond_dimension,
+                are_links_outgoing=[False, False, False, True],
+            )
+
+            sector = sectors.get((0, 0), None)
+            if sector is not None:
+                # pylint: disable-next=no-member
+                links[-1].restrict_irreps(sector)
+
+            tensor = tensor_backend.tensor_cls(
+                links,
+                ctrl=initialization,
+                are_links_outgoing=link_dirs,
+                **tensor_backend.tensor_cls_kwargs(),
+            )
+
+            if isometry:
+                # Normalization only make sense if other tensors are isometrized
+                tensor.normalize()
 
             self.append(tensor)
+            self.append(tensor_1)
+        else:
+            for ii in range(self.num_tensors):
+                tshape = tensor_shape
+                sector = sectors.get((self.layer_idx, ii), None)
+                if sector is not None:
+                    tshape[-1].restrict_irreps(sector)
+                rows = list(range(len(tshape)))[:-1]
+                cols = list(range(len(tshape)))[-1:]
+
+                tensor = tensor_backend.tensor_cls(
+                    tshape,
+                    ctrl=initialization,
+                    are_links_outgoing=link_dirs,
+                    **tensor_backend.tensor_cls_kwargs(),
+                )
 
-        self.device = device
+                if isometry:
+                    if self.layer_idx == 0:
+                        # Must be TTO
+                        tensor.normalize()
+                    else:
+                        # Some lower layers
+                        tensor, _ = tensor.split_qr(rows, cols)
+
+                self.append(tensor)
+
+        # initializetion not aware of device
+        self.convert(tensor_backend.dtype, tensor_backend.device)
+
+    def convert(self, dtype, device, singvals_only=False):
+        """Convert layer towards specified data type and device."""
+        if len(self) == 0:
+            return
 
-    def _device_checks(self, **kwargs):
-        """
-        Check if all the arguments of the function where
-        _device_checks is called are on the correct device,
-        select the correct
+        if singvals_only:
+            tensor = self[0]
+        else:
+            for tensor in self:
+                tensor.convert(dtype, device)
 
-        Parameters
-        ----------
-        device : str
-            Device where the computation should take place.
-            If called inside an emulator it should be the
-            emulator device
-        **kwargs : array-like
-            Array-like inputs to the function. If they are
-            on the wrong device an exception is raised.
-            The keyword is the identifier used in the raise
-            statement
+        singvals_list = []
+        for elem in self.singvals:
+            if elem is None:
+                singvals_list.append(None)
+            else:
+                singvals_ii = tensor.convert_singvals(elem, dtype, device)
+                singvals_list.append(singvals_ii)
 
-        Returns
-        -------
-        module handle
-            cp if the device is GPU
-            np if the device is CPU
-        """
-        return _AbstractTN._device_checks(self, **kwargs)
+        self.singvals = singvals_list
+
+    def _iter_tensors(self):
+        """Iterate over all tensors forming the tensor network (for convert etc)."""
+        for elem in self:
+            yield elem
 
     def extend_local_hilbert_space(self, number_levels):
         """
         Extend the local Hilbert by a certain number of levels without
         population. For use on lowest layer with physical Hilbert space.
 
         Parameters
@@ -347,57 +390,74 @@
             on the level of a TTN layer.
         """
         if not isinstance(other, TTNLayer):
             raise TypeError("Only two TTNLayer classes can be the input.")
 
         if len(self) != len(other):
             raise ValueError("Layers must have the same length.")
-        xp = self._device_checks()
 
         sandwich_list = []
         for ii, ket in enumerate(self):
             bra = other[ii]
 
-            new_tens = xp.tensordot(xp.conj(bra), ket, [[0, 1], [0, 1]])
+            new_tens = bra.conj().tensordot(ket, [[0, 1], [0, 1]])
             sandwich_list.append(new_tens)
 
         return sandwich_list
 
-    def qr_towards_top(self):
+    def qr_towards_top(self, requires_singvals, conv_params):
         """
         Iterating over QR decompositions for the complete layer, where
         the q-tensors remain in the layer and the r-tensors have to
         be contracted with the parent links.
 
         One use-case is the initial isometrization.
 
+        Arguments
+        ---------
+
+        requires_singvals : bool
+            Flag if singular values should be calculated; then, SVDs are
+            used instead of QRs.
+
+        conv_params : :class:`TNConvergenceParameters`
+            For SVD, settings with convergence parameters have to be
+            passed.
+
         Returns
         -------
 
         List of r-tensors (rank-2, 1st link to this layer, 2nd link
         to parent)
         """
         if len(self) == 2 and self.layer_idx == 0:
             raise Exception("Looks like this is already the top layer.")
-        xp = self._device_checks()
 
         r_list = []
         for ii in range(len(self)):
-            shape = list(self[ii].shape)
+            d1 = list(range(self[ii].ndim))[:-1]
+            d2 = list(range(self[ii].ndim))[-1:]
 
-            d1 = shape[0] * shape[1]
-            d2 = shape[2]
-
-            tmp = self[ii].reshape([d1, d2])
-            qmat, rmat = xp.linalg.qr(tmp)
-
-            self[ii] = qmat.reshape([shape[0], shape[1], qmat.shape[1]])
+            if requires_singvals:
+                self[ii], rmat, lambdas, _ = self[ii].split_svd(
+                    d1,
+                    d2,
+                    contract_singvals="R",
+                    conv_params=conv_params,
+                    no_truncation=True,
+                )
+                norm = np.sum(lambdas**2)
+                if abs(norm - 1.0) > 1e-12:
+                    raise Exception("normalization")
+                self.singvals[ii] = lambdas
+            else:
+                self[ii], rmat = self[ii].split_qr(d1, d2)
 
-            # Unset the singular values
-            self.unset_singvals(ii)
+                # Unset the singular values
+                self.unset_singvals(ii)
 
             r_list.append(rmat)
 
         return r_list
 
     def contr_rmats(self, r_list):
         """
@@ -421,25 +481,24 @@
         Details
         -------
 
         One use-case is the initial isometrization.
         """
         if len(r_list) != 2 * len(self):
             raise Exception("Dimension of self and r_list do not match.")
-        xp = self._device_checks()
 
         for ii in range(len(self)):
             # indices of r-tensors
             i1 = 2 * ii
             i2 = i1 + 1
 
             # Contract over the second child first avoids
             # permutations
-            tmp = xp.tensordot(r_list[i2], self[ii], [[1], [1]])
-            self[ii] = xp.tensordot(r_list[i1], tmp, [[1], [1]])
+            tmp = r_list[i2].tensordot(self[ii], [[1], [1]])
+            self[ii] = r_list[i1].tensordot(tmp, [[1], [1]])
 
         return
 
     def fuse_all_children(self):
         """
         Fuse the links towards the children and return a list
         of matrices.
@@ -447,35 +506,62 @@
         fused = []
         for elem in self:
             new_dim = [elem.shape[0] * elem.shape[1], elem.shape[2]]
             fused.append(elem.reshape(new_dim))
 
         return fused
 
-    def qr_top_right(self):
+    def qr_top_right(self, requires_singvals, conv_params):
         """
         Do QR decomposition on top layer with two tensors. R-tensor
         is moved into the left tensor.
 
+        Arguments
+        ---------
+
+        requires_singvals : bool
+            Flag if singular values should be calculated; then, SVDs are
+            used instead of QRs.
+
+        conv_params : :class:`TNConvergenceParameters`
+            For SVD, settings with convergence parameters have to be
+            passed.
+
         Returns
         -------
 
         None
         """
         if len(self) != 2 and self.layer_idx != 0:
             raise Exception("Only available for top layer.")
-        xp = self._device_checks()
 
-        mat = self[1].reshape([self[1].shape[0] * self[1].shape[1], self[1].shape[2]])
-        qmat, rmat = xp.linalg.qr(mat)
+        d1 = list(range(self[1].ndim))[:-1]
+        d2 = list(range(self[1].ndim))[-1:]
+
+        if requires_singvals:
+            self[1], rmat, s_vals, _ = self[1].split_svd(
+                d1,
+                d2,
+                contract_singvals="R",
+                conv_params=conv_params,
+                no_truncation=True,
+            )
 
-        self[1] = qmat.reshape([self[1].shape[0], self[1].shape[1], rmat.shape[0]])
+            self.singvals[0] = s_vals
+            self.singvals[1] = s_vals
+        else:
+            self[1], rmat = self[1].split_qr(d1, d2)
+
+            # Unset the singular values
+            self.unset_singvals(0)
+            self.unset_singvals(1)
+
+        tmp = self[0].tensordot(rmat, [[2], [1]])
+        self[0] = tmp.transpose([0, 1, 3, 2])
 
-        tmp = xp.tensordot(self[0], rmat, [[2], [1]])
-        self[0] = xp.transpose(tmp, [0, 1, 3, 2])
         self.unset_singvals(0)
 
         return
 
     def write(self, filehandle, f90_ttn_version, num_layers, cmplx=True):
         """
         Get string of the TTN layer which is compatible with the
@@ -502,23 +588,26 @@
         None
 
         Details
         -------
 
         We assume a binary tree.
         """
-        self.to_device("cpu")
+        self.convert(None, device="cpu")
 
         filehandle.write(f90_ttn_version + "\n")
         filehandle.write("%d\n" % (len(self)))
         dim_n2 = 3 if (self.layer_idx != 0) else 4
         filehandle.write("%d\n" % (dim_n2))
 
         for elem in self:
-            write_tensor(elem, filehandle, cmplx=cmplx)
+            if elem.has_symmetry:
+                raise Exception("Cannot write symmetric tensors so far.")
+
+            elem.write(filehandle, cmplx=cmplx)
 
         # Cutoff (integer)
         filehandle.write("%d\n" % (self.max_bond_dimension))
 
         # is_truncated (vector of logicals)
         # We take the safe path and assume it is not truncated only
         # if the dimension are smaller than the maximal bond dimension
@@ -723,135 +812,102 @@
         for ii in range(0, how_many):
             print("Tensor", ii, ":")
             print("Shape: ", self[ii].shape)
         print("\n")
 
         return None
 
-    def to_device(self, device):
-        """
-        Move the TTNLayer class to the new device.
-
-        Parameters
-        ----------
-        device : string
-            Device where to move the TTNLayer
-        """
-        device = device.lower()
-        if device not in self.implemented_devices:
-            raise ValueError(
-                f"Device {device} is not implemented. Select from"
-                + f" {self.implemented_devices}"
-            )
-        # We already are in the correct device
-        if device == self.device:
-            return
-        # We go to the cpu to gpu
-        if device == "gpu":
-            if not GPU_AVAILABLE:
-                raise ImportError("CUDA GPU is not available")
-            self[:] = [cp.asarray(tens) for tens in self]
-            self.singvals = [
-                cp.asarray(singv) if singv is not None else None
-                for singv in self.singvals
-            ]
-        # We go from gpu to cpu
-        elif device == "cpu":
-            self[:] = [cp.asnumpy(tens) for tens in self]
-            self.singvals = [
-                cp.asnumpy(singv) if singv is not None else None
-                for singv in self.singvals
-            ]
-        self.device = device
-
-        return
-
 
 class TTN(_AbstractTN):
     """
     Tree tensor network class.
 
     Parameters
     ----------
 
     num_sites: int
         Number of sites
 
-    local_dim: int, optional
-        Local dimension of the degrees of freedom. Default to 2.
-
     convergence_parameters: :py:class:`TNConvergenceParameters`
         Class for handling convergence parameters. In particular,
         in the TTN simulator we are interested in:
         - the *maximum bond dimension* :math:`\\chi`;
         - the *cut ratio* :math:`\\epsilon` after which the singular
             values are neglected, i.e. if :math:`\\lamda_1` is the
             bigger singular values then after an SVD we neglect all the
             singular values such that
             :math:`\\frac{\\lambda_i}{\\lambda_1}\\leq\\epsilon`
 
-    initialise: string, optional
+    local_dim: int, optional
+        Local dimension of the degrees of freedom. Default to 2.
+
+    requires_singvals : boolean, optional
+        Allows to enforce SVD to have singular values on each link available
+        which might be useful for measurements, e.g., bond entropy (the
+        alternative is traversing the whole TN again to get the bond entropy
+        on each link with an SVD).
+
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
+    network : str, optional
+        Default to "binary" (probably only option right now).
+
+    initialize: string, optional
         Define the initialization method. For random entries use
         'random', for empty TTN use 'empty'.
         Default to 'random'.
 
-    dtype : dtype, optional
-        Type of entries for the tensor.
-        Default is np.complex128.
-
-    device : str, optional
-        Device where the computations are done.
-        Default to "cpu".
+    sectors : dict, optional
+        Can restrict symmetry sector and/or bond dimension in initialization.
+        If empty, no restriction.
+        Default to empty dictionary.
 
     Details
     -------
 
     The last layer contains the local Hilbert spaces and the
     most tensors.
     """
 
     is_ttn = True
+    extension = "ttn"
 
     def __init__(
         self,
         num_sites,
         convergence_parameters,
         local_dim=2,
+        requires_singvals=False,
+        tensor_backend=None,
         network="binary",
         initialize="random",
-        dtype=np.complex128,
-        device="cpu",
+        sectors={},
+        **kwargs,
     ):
         # Pre-process local_dim to be a vector
         if np.isscalar(local_dim):
             local_dim = np.repeat(int(local_dim), num_sites)
         else:
-            local_dim = np.array(local_dim, dtype=int)
-
-        if np.min(local_dim) < 2:
-            raise ValueError("Local dimension cannot be smaller than 2.")
-
-        if len(local_dim) != num_sites:
-            raise ValueError(
-                f"Length of local_dim {len(local_dim)} differs "
-                + f"from num_sites {num_sites}."
-            )
+            pass
+            # local_dim = np.array(local_dim, dtype=int)
 
         super().__init__(
             num_sites,
             convergence_parameters,
             local_dim=local_dim,
-            device=device,
-            dtype=dtype,
+            requires_singvals=requires_singvals,
+            tensor_backend=tensor_backend,
         )
 
         # The number of links is defined in the network definition, i.e. at the
         # moment insite _generate_binary_network
         self.num_links = 0
 
+        self._network = network
         if network == "binary":
             self.num_layers = int(np.log2(num_sites)) - int(self.is_ttn)
             network = self._generate_binary_network()
 
             if abs(np.log2(num_sites) - int(self.is_ttn) - self.num_layers) > 1e-14:
                 raise Exception(
                     "Cannot construct TTN; num_sites is "
@@ -860,29 +916,61 @@
         else:
             raise NotImplementedError("Only binary tree is implemented")
 
         # Layer and tree initialization
         self.layers = []
         for ii in range(self.num_layers):
             layer = TTNLayer(
-                ii, self.local_dim, self.max_bond_dim, 4, len(network[ii]), device
+                ii,
+                self.local_links,
+                self._convergence_parameters.max_bond_dimension,
+                4,
+                len(network[ii]),
             )
             layer.initialize_quantities(network[ii])
             self.layers.append(layer)
         self._initialize_sites_range(network)
-        self._initialize_tree(initialize)
+        self._initialize_tree(initialize, sectors=sectors)
 
         # Caching of sampling steps
         self._cache_get_children_prob = {}
         self._cachesize_bytes_get_children_prob = 0
         self._cachelimit_bytes_get_children_prob = None
         self._cache_clearing_strategy = "num_qubits"
 
         self.is_measured = self[0].is_measured
 
+        # TTN initializetion not aware of device
+        self.convert(self._tensor_backend.dtype, self._tensor_backend.device)
+
+    # --------------------------------------------------------------------------
+    #                               Properties
+    # --------------------------------------------------------------------------
+
+    @property
+    def default_iso_pos(self):
+        """
+        Returns default isometry center position, e.g., for initialziation
+        of effective operators.
+        """
+        return [0, 0]
+
+    @property
+    def current_max_bond_dim(self):
+        """Current maximum bond dimension of the TTN"""
+        max_chi = 0
+        for tensor in self._iter_tensors():
+            max_chi = max(max_chi, np.max(tensor.shape))
+
+        return max_chi
+
+    # --------------------------------------------------------------------------
+    #                          Overwritten operators
+    # --------------------------------------------------------------------------
+
     def __getitem__(self, idx):
         """
         Overwrite calls to get element in list, which refers to the layer
         in a TTN.
 
         Parameters
         ----------
@@ -920,24 +1008,732 @@
             Tensor to be set in place of the old
         """
         if np.isscalar(idx):
             self.layers[idx] = value
         else:
             self.layers[idx[0]][idx[1]] = value
 
+    def __matmul__(self, other):
+        """
+        Implement the contraction between two TTNs overloading the operator
+        @. It is equivalent to doing <self|other>. It already takes into account
+        the conjugation of the left-term
+        """
+        if not isinstance(other, TTN):
+            raise TypeError("Only two TTN classes can be contracted")
+
+        return other.dot(self)
+
+    # --------------------------------------------------------------------------
+    #                       classmethod, classmethod like
+    # --------------------------------------------------------------------------
+    #
+    # Inheriting:
+    #
+    # * read_pickle
+
+    @classmethod
+    def from_statevector(
+        cls, statevector, local_dim=2, conv_params=None, tensor_backend=None
+    ):
+        """
+        Initialize the TTN by decomposing a statevector into TTN form.
+
+        Parameters
+        ----------
+
+        statevector : ndarray of shape( [local_dim]*num_sites, )
+            Statevector describing the interested state for initializing the TTN
+
+        device : str, optional
+            Device where the computation is done. Either "cpu" or "gpu".
+
+        tensor_cls : type for representing tensors.
+            Default to :class:`QteaTensor`
+        """
+
+        # At the moment, no truncation is implemented in the code
+        num_sites = len(statevector.shape)
+
+        if local_dim != statevector.shape[0]:
+            raise Exception("Mismatch local dimension (passed and one in array).")
+
+        if np.any(local_dim != np.array(statevector.shape)):
+            raise Exception(
+                "from_statevector requires equal local dim " + "across the system."
+            )
+
+        num_layers = int(np.log2(num_sites) - 1)
+        state_tensor = statevector
+        tensor_list = []
+        singvals_list = []
+        p0 = 1
+        p1 = 2
+
+        for ll in range(num_layers):
+            tensor_layer_list = []
+            singvals_layer_list = []
+            i0 = p0
+            i1 = p1
+
+            if ll == (num_layers - 1):
+                num_svd = 1
+            else:
+                num_svd = num_sites // p1
+
+            for _ in range(num_svd):
+                d0 = local_dim ** (p1 // 2)
+                d1 = local_dim**p1
+                d2 = np.prod(state_tensor.shape[2:])
+                umat, s_tot, vhmat = np.linalg.svd(
+                    state_tensor.reshape([d1, d2]), full_matrices=False
+                )
+                singvals_layer_list.append(s_tot)
+                s_tot = np.diag(s_tot)
+
+                umat = umat.reshape([d0, d0, d1])
+                new_shape = (
+                    [d1] + [d0] * ((num_sites - i1) // (p1 // 2)) + [d1] * (i0 - 1)
+                )
+                state_tensor = np.dot(s_tot, vhmat).reshape(new_shape)
+
+                perm = [jj + 1 for jj in range(len(state_tensor.shape) - 1)] + [0]
+                state_tensor = np.transpose(state_tensor, perm)
+
+                i0 += 1
+                i1 += p1
+                tensor_layer_list.append(umat)
+
+                if ll == (num_layers - 1):
+                    tensor_layer_list.append(state_tensor)
+
+            p1 *= 2
+            tensor_list.append(tensor_layer_list)
+            singvals_list.append(singvals_layer_list)
+
+        tensor_list[-1][0] = np.reshape(
+            tensor_list[-1][0], list(tensor_list[-1][0].shape) + [1]
+        )
+        # The two top links are the same link
+        singvals_list[-1].append(singvals_list[-1][0])
+
+        obj = cls.from_tensor_list(
+            tensor_list,
+            singvals_list=singvals_list,
+            tensor_backend=tensor_backend,
+            conv_params=conv_params,
+        )
+
+        obj.iso_center = (0, 1)
+        obj.iso_towards([0, 0], keep_singvals=True)
+        obj._requires_singvals = True
+
+        return obj
+
+    @classmethod
+    def product_state_from_local_states_2d(
+        cls,
+        mat_2d,
+        padding=None,
+        mapping="HilbertCurveMap",
+        return_map=False,
+        conv_params=None,
+        tensor_backend=None,
+    ):
+        """
+        Construct a product (separable) state in 1d TTN form for a 2d system
+        by mapping it to 1d, given the local states of each of the sites.
+
+        Parameters
+        ----------
+        mat_2d : np.array of rank 2
+            Array with third axis being a (normalized) local state of
+            the (ii,jj)-th site (where ii and jj are indices of the
+            first and second axes).
+            Product of first two axes' dimensions is therefore equal
+            to the total number of sites, and third axis dimension
+            corresponds to the local dimension.
+
+        padding : np.array of length 2 or `None`, optional
+            Used to enable the growth of bond dimension in TDVP algorithms
+            for TTN (necessary as well for two tensor updates).
+            If not `None`, all the TTN tensors are padded such that the bond
+            dimension is equal to `padding[0]`. The value `padding[1]`
+            tells with which value are we padding the tensors. Note that
+            `padding[1]` should be very small, as it plays the role of
+            numerical noise.
+            If False, the bond dimensions are equal to 1.
+            Default to None.
+
+        mapping : string or instance of :py:class:`HilbertCurveMap`,
+                  optional
+            Which 2d to 1d mapping to use. Possible inputs are:
+            'HilbertCurveMap', 'SnakeMap', and 'ZigZagMap'.
+            Default is 'HilbertCurveMap'.
+
+        return_map : boolean, optional
+            If True, the function returns array `map` with indices
+            of 2d to 1d mapping.
+            Default to False.
+
+        convergence_parameters : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters for the new TTN.
+
+        Return
+        ------
+        prod_ttn : :py:class:`TTN`
+            Corresponding product state TTN.
+        map : np.array, returned only if return_map==True
+            Nx2 Matrix, where N is a total number of particles.
+            The values in the ii-th row of the matrix denote
+            particle's position in a corresponding 2d grid.
+
+        """
+        if len(mat_2d.shape) != 3:
+            raise Exception("numpy ndarray must be of rank-3.")
+        for ii in range(0, mat_2d.shape[0]):
+            for jj in range(0, mat_2d.shape[1]):
+                norm = np.linalg.norm(mat_2d[ii, jj, :])
+                if abs(norm - 1) > 10e-5:
+                    raise ValueError(
+                        f"Local state on site ({ii+1},{jj+1}) "
+                        f"not normalized. Norm = {norm}."
+                    )
+
+        dim = 2  # define that we are in 2d
+        num_sites_x, num_sites_y, local_dim = mat_2d.shape
+        size = [num_sites_x, num_sites_y]
+        num_sites_tot = num_sites_x * num_sites_y
+
+        # f ind the corresponding indices of 2d points in 1d
+        map_indices = map_selector(dim, size, mapping)
+        if return_map:
+            # will be same as map_indices, just in np.ndarray form
+            map_array = np.zeros((num_sites_tot, 2))
+
+        # compute the corresponding array with local states for 1d
+        mat_1d = np.zeros((num_sites_tot, local_dim))
+        ii = 0
+        for ind in map_indices:
+            n_x, n_y = ind
+            mat_1d[ii, :] = mat_2d[n_x, n_y, :]
+            if return_map:
+                map_array[ii] = ind
+            ii += 1
+
+        prod_ttn = TTN.product_state_from_local_states(
+            mat_1d,
+            padding=padding,
+            convergence_parameters=conv_params,
+            tensor_backend=tensor_backend,
+        )
+
+        if return_map:
+            return prod_ttn, map_array
+        return prod_ttn
+
+    def to_dense(self, true_copy=False):
+        """Return TTN without symmetric tensors."""
+        if self.has_symmetry:
+            obj = type(self)(
+                self.num_sites,
+                self.convergence_parameters,
+                local_dim=self.local_dim,
+                initialize="empty",
+                tensor_backend=self._tensor_backend,
+            )
+
+            for ii, layer in enumerate(self.layers):
+                layer_dense = layer.to_dense(true_copy=true_copy)
+
+                obj[ii] = layer_dense
+
+            return obj
+
+        # Cases without symmetry
+
+        if true_copy:
+            return self.copy()
+
+        return self
+
+    # --------------------------------------------------------------------------
+    #                            Checks and asserts
+    # --------------------------------------------------------------------------
+
+    # --------------------------------------------------------------------------
+    #                     Abstract methods to be implemented
+    # --------------------------------------------------------------------------
+
+    def _convert_singvals(self, dtype, device):
+        """Convert the singular values of the tensor network to dtype/device."""
+        for layer in self.layers:
+            layer.convert(dtype, device, singvals_only=True)
+
+    def get_bipartition_link(self, pos_src, pos_dst):
+        """
+        Returns two sets of sites forming the bipartition of the system for
+        a loopless tensor network. The link is specified via two positions
+        in the tensor network.
+
+        **Arguments**
+
+        pos_src : tuple of two ints
+            Specifies the first tensor and source of the link.
+
+        pos_dst : tuple of two ints
+            Specifies the second tensor and destination of the link.
+
+        **Returns**
+
+        sites_src : list of ints
+            Hilbert space indices when looking from the link towards
+            source tensor and following the links therein.
+
+        sites_dst : list of ints
+            Hilbert space indices when looking from the link towards
+            destination tensor and following the links therein.
+        """
+        self.assert_binary_tree()
+
+        if pos_src[0] > pos_dst[0]:
+            # Use source tensor to start calculing
+            span_sites = 2 ** (self.num_layers - pos_src[0])
+            offset = span_sites * pos_src[1]
+
+            sites_src = list(range(offset, offset + span_sites))
+
+            sites_dst = list(range(offset))
+            sites_dst += list(range(offset + span_sites, self.num_sites))
+
+            return sites_src, sites_dst
+
+        # Use destination tensor to start calculating
+        span_sites = 2 ** (self.num_layers - pos_dst[0])
+        offset = span_sites * pos_dst[1]
+
+        sites_dst = list(range(offset, offset + span_sites))
+
+        sites_src = list(range(offset))
+        sites_src += list(range(offset + span_sites, self.num_sites))
+
+        return sites_src, sites_dst
+
+    def get_pos_links(self, pos):
+        """
+        Return a list of positions where all links are leading to. Number
+        of entries is equal to number of links. Each entry contains the position
+        as accessible in the actual tensor network.
+        """
+        pos_links = []
+        for i1, i2, _ in self._iter_all_links(pos):
+            if i2 is None:
+                pos_links.append(None)
+            else:
+                pos_links.append((i1, i2))
+
+        return pos_links
+
+    def get_rho_i(self, idx):
+        """
+        Calculate the reduced density matrix for a single site.
+        If the singular values are stored (i.e. not None) do not
+        move the isometry center, but use them to compute local
+        observables.
+
+        Parameters
+        ----------
+
+        idx : integer
+            Calculate the reduced density matrix of site ``idx``.
+            Recall python indices start at zero.
+
+        Returns
+        -------
+
+        numpy ndarray : rank-2 tensor with the reduced density
+        matrix.
+        """
+        self.assert_binary_tree()
+
+        layer_idx = self.num_layers - 1
+        tensor_idx = idx // 2
+
+        if (self.iso_center is None) or (self[layer_idx].singvals[tensor_idx] is None):
+            self.iso_towards([layer_idx, tensor_idx], keep_singvals=True)
+            tensor = self[layer_idx][tensor_idx]
+        elif list(self.iso_center) == [layer_idx, tensor_idx]:
+            tensor = self[layer_idx][tensor_idx]
+        else:
+            tensor = self[layer_idx][tensor_idx].scale_link(
+                self[layer_idx].singvals[tensor_idx], 2
+            )
+
+        if idx % 2 == 0:
+            contr_idx = [1, 2]
+        else:
+            contr_idx = [0, 2]
+
+        rho = tensor.tensordot(tensor.conj(), [contr_idx, contr_idx])
+
+        trace = rho.trace(return_real_part=True, do_get=True)
+        if abs(1 - trace) > 10 * rho.dtype_eps:
+            warnings.warn("Renormalizing reduced density matrix.")
+            rho /= trace
+
+        return rho
+
+    def get_tensor_of_site(self, idx):
+        """
+        Generic function to retrieve the tensor for a specific site. Compatible
+        across different tensor network geometries.
+
+        Parameters
+        ----------
+        idx : int
+            Return tensor containin the link of the local
+            Hilbert space of the idx-th site.
+        """
+        self.assert_binary_tree()
+
+        return self[-1][idx // 2]
+
+    def iso_towards(self, new_iso, keep_singvals=False, trunc=False, conv_params=None):
+        """
+        Shift isometry center towards a certain tensor.
+
+        Parameters
+        ----------
+
+        new_iso : list of two integers
+            New isometry center in terms of layer and tensor.
+
+        keep_singvals : bool, optional
+            If True, keep the singular values even if shifting the iso with a
+            QR decomposition. Default to False.
+
+        trunc : Boolean, optional
+            If `True`, the shifting is done via truncated SVD.
+            If `False`, the shifting is done via QR.
+            Default to `False`.
+
+        conv_params : :py:class:`TNConvergenceParameters`, optional
+            Convergence parameters to use for the SVD. If `None`, convergence
+            parameters are taken from the TTN.
+            Default to `None`.
+
+        Returns
+        -------
+
+        singvals_cut_tot : np.ndarray
+            Singualr values cut in the process of shifting the isometry center.
+            None if moved through the QR.
+
+        Details
+        -------
+
+        We introduce an overhead if the TTN has no
+        isometry center set up to now. This choice could
+        be further optimized.
+        """
+        if self.iso_center is not None:
+            if (self.iso_center[0] == new_iso[0]) and (
+                self.iso_center[1] == new_iso[1]
+            ):
+                # Return singular values cut, i.e., zeros in this case
+                return np.zeros(1)
+        else:
+            # Isometry center is not set; we install it first
+            # at [0, 0] and accept a small overhead
+            self.isometrize_all()
+
+        # Obtain the path
+        complete_path = self.get_path(new_iso)
+
+        singvals_cut_tot = []
+        for elem in complete_path:
+            # Get the tensor for the QR
+            src_layer_idx = elem[0]
+            src_tensor_idx = elem[1]
+            src = self[src_layer_idx][src_tensor_idx]
+
+            # Get the target/destination tensor
+            dst_layer_idx = elem[3]
+            dst_tensor_idx = elem[4]
+            dst = self[dst_layer_idx][dst_tensor_idx]
+
+            src_link = elem[2]
+            dst_link = elem[5]
+            src, dst, singvals_cut, singvals = self.shift_iso_to(
+                src, dst, src_link, dst_link, trunc=trunc, conv_params=conv_params
+            )
+            singvals_cut_tot.append(singvals_cut)
+            # Unset the singvals if the flag is not active, since the QRs might destroy
+            # the entanglement in the PATH.
+            if not keep_singvals:
+                lowest_layer = max(src_layer_idx, dst_layer_idx)
+                lowest_tensor = (
+                    dst_tensor_idx if dst_layer_idx > src_layer_idx else src_tensor_idx
+                )
+                self[lowest_layer].unset_singvals(lowest_tensor)
+            if trunc or self._requires_singvals:
+                lowest_layer = max(src_layer_idx, dst_layer_idx)
+                lowest_tensor = (
+                    dst_tensor_idx if dst_layer_idx > src_layer_idx else src_tensor_idx
+                )
+                self[lowest_layer].singvals[lowest_tensor] = singvals
+
+            self[src_layer_idx][src_tensor_idx] = src
+            self[dst_layer_idx][dst_tensor_idx] = dst
+
+            if self.eff_op is not None:
+                self._update_eff_ops(elem)
+
+            # And reset iso center to new value
+            self.iso_center = elem[3:5]
+
+        return np.array(singvals_cut_tot)
+
+    def _iter_tensors(self):
+        """Iterate over all tensors forming the tensor network (for convert etc)."""
+        for layer in self.layers:
+            for tensor in layer._iter_tensors():
+                yield tensor
+
+    def norm(self):
+        """Return the norm of a TTN."""
+        if self.iso_center is None:
+            # We have to install isometry center, pick default
+            self.isometrize_all()
+
+        norm = self[self.iso_center[0]][self.iso_center[1]].norm()
+        # norm = np.sum(np.real(tensor * tensor.conj()))
+
+        return np.sqrt(norm)
+
+    def scale(self, factor):
+        """Scale a TTN with a scalar factor."""
+        if self.iso_center is None:
+            # We have to install isometry center, pick default
+            self.isometrize_all()
+
+        self[self.iso_center[0]][self.iso_center[1]] *= factor
+
+    def set_singvals_on_link(self, pos_a, pos_b, s_vals):
+        """Update or set singvals on link via two positions."""
+        if pos_a[0] > pos_b[0]:
+            # pos_a is in the lower layer
+            pos = pos_a
+        else:
+            pos = pos_b
+
+        if pos[0] == 0:
+            self.layers[pos[0]].singvals[0] = s_vals
+            self.layers[pos[0]].singvals[1] = s_vals
+        else:
+            self.layers[pos[0]].singvals[pos[1]] = s_vals
+
+    def site_canonize(self, idx, keep_singvals=False):
+        """
+        Shift the isometry center to the tensor containing the
+        corresponding site.
+
+        Parameters
+        ----------
+
+        idx : int
+            Index of the physical site which should be isometrized.
+
+        keep_singvals : bool, optional
+            If True, keep the singular values even if shifting the iso with a
+            QR decomposition. Default to False.
+
+        """
+        self.assert_binary_tree()
+
+        target_layer = self.num_layers - 1
+        target_tensor = idx // 2
+
+        self.iso_towards([target_layer, target_tensor], keep_singvals=keep_singvals)
+
+    # --------------------------------------------------------------------------
+    #                   Choose to overwrite instead of inheriting
+    # --------------------------------------------------------------------------
+
+    def permute_spo_for_two_tensors(self, spo_list, theta, link_partner):
+        """Incoming order Ta, Tb, Pa, Pb"""
+        if not isinstance(spo_list[0], SparseMatrixOperatorPy):
+            # Effective operator not affected
+            return spo_list, theta, None
+
+        if link_partner in [0, 2]:
+            return spo_list, theta, None
+
+        if (link_partner == 1) and (theta.ndim == 4):
+            spo_list = [spo_list[0], spo_list[1], spo_list[3], spo_list[2]]
+            theta.transpose_update([0, 1, 3, 2])
+            inv_permutation = [0, 1, 3, 2]
+
+            return spo_list, theta, inv_permutation
+
+        if (link_partner == 1) and (theta.ndim == 5):
+            spo_list = [spo_list[0], spo_list[1], spo_list[3], spo_list[2], spo_list[4]]
+            theta.transpose_update([0, 1, 3, 2, 4])
+            inv_permutation = [0, 1, 3, 2, 4]
+
+            return spo_list, theta, inv_permutation
+
+        raise Exception(f"Unknown link_partner being {link_partner}.")
+
+    # --------------------------------------------------------------------------
+    #                                  Unsorted
+    # --------------------------------------------------------------------------
+
+    def assert_binary_tree(self):
+        """Assert for methods requiring binary trees."""
+        if self._network != "binary":
+            raise Exception("Tree is not binary tree; no support yet.")
+
     @property
     def iso_center(self):
         """Isometry center property"""
         return self._iso_center
 
     @iso_center.setter
     def iso_center(self, value):
         """Change the value of the iso center"""
         self._iso_center = value
 
+    def _iter_all_links(self, pos):
+        """
+        Return an iterator over all the links of a position
+        `pos` in the TTN. It treats specially the tensor at `(0, 0)`
+
+        Parameters
+        ----------
+        pos : Tuple[int]
+            Position in the tree as `(layer_idx, tensor_idx)`
+
+        Returns
+        -------
+        Tuple[int]
+            Tuple of `(layer_link, tensor_link, leg_toward_link)`
+        """
+        for elem in self._iter_children_pos(pos):
+            yield elem
+
+        _, info = self._get_parent_info(pos)
+        yield info
+
+        if pos[0] == 0 and pos[1] == 0 and self.is_ttn:
+            yield None, None, None
+
+    def _iter_physical_links(self):
+        """
+        Returns an iterator over the physical links.
+        The physical links are represented as the tuple
+        `( (layer_idx+1, site_idx), (layer_idx, tensor_idx) )`,
+        where `layer_idx` is the physical (last) layer of the TTN.
+
+        Returns
+        -------
+        Tuple[int]
+            The extra physical layer and site index `(layer_idx+1, site_idx)`
+        Tuple[int]
+            The final TTN layer and the tensor index `(layer_idx, tensor_idx)`
+        """
+
+        # Relevant layer is the last layer
+        layer = self[-1]
+        lidx = layer.layer_idx
+
+        idx = -1
+        for ii, tens in enumerate(layer):
+            nn = tens.ndim - 1
+            if lidx == 0 and ii == 0:
+                # Top-tensor in four-body TTN
+                nn -= 1
+
+            for _ in range(nn):
+                idx += 1
+
+                yield (lidx + 1, idx), (lidx, ii)
+
+    def _iter_children_pos(self, pos):
+        """
+        Return an iterator over the tuple
+        giving informations about the children of
+        the tensor in position `pos`. The children are
+        the legs pointing downwards.
+        Works only for binary trees.
+
+        Parameters
+        ----------
+        pos : Tuple[int]
+            Position in the tree as `(layer_idx, tensor_idx)`
+
+        Returns
+        -------
+        Tuple[int]
+            Tuple of `(layer_child_1, tensor_child_1, leg_toward_parent)`
+        Tuple[int]
+            Tuple of `(layer_child_2, tensor_child_2, leg_toward_parent)`
+        """
+        self.assert_binary_tree()
+
+        # Works only for binary tree:
+        yield pos[0] + 1, 2 * pos[1], 2
+        yield pos[0] + 1, 2 * pos[1] + 1, 2
+
+    def _get_parent_info(self, pos):
+        """
+        Return informations about the parent of
+        the tensor in position `pos`. The parent is
+        the leg pointing upwards.
+        Works only for binary trees.
+
+        Parameters
+        ----------
+        pos : Tuple[int]
+            Position in the tree as `(layer_idx, tensor_idx)`
+
+        Returns
+        -------
+
+        link : int
+            Link index of the tensor at `pos` which connects to
+            the parent tensor.
+
+        info : list of three ints
+            Layer index of parent tensor, tensor index within
+            layer of parent tensor, link index in parent tensor
+            connecting to tensor at `pos`.
+        """
+        self.assert_binary_tree()
+
+        info = -np.ones(3, dtype=int)
+        link = 2
+
+        if np.any(info < 0):
+            # Works only for binary trees
+            if list(pos) == [0, 0]:
+                info[0] = 0
+                info[1] = 1
+                info[2] = 2
+            elif list(pos) == [0, 1]:
+                info[0] = 0
+                info[1] = 0
+                info[2] = 2
+            else:
+                info[0] = max(0, pos[0] - 1)
+                info[1] = pos[1] // 2
+                info[2] = pos[1] % 2
+
+        return link, list(info)
+
     def _generate_binary_network(self):
         """
         Generate the network structure for the binary tree.
         This function just generate the network structure, not
         the TTN itself.
 
         Returns
@@ -1024,36 +1820,75 @@
                     ]
                 # Upper link
                 layer.sites[:, len(node.link_idxs) - 1, tidx] = [
                     np.min(layer.sites[:, :, tidx][layer.sites[:, :, tidx] > 0]),
                     np.max(layer.sites[:, :, tidx]),
                 ]
 
-    def _initialize_tree(self, method="empty", isometry=True):
+    def _initialize_tree(self, method="empty", isometry=True, sectors={}):
         """
         Initialize the tree with random tensors
 
         Parameters
         ----------
         isometry : bool, optional
             If True, the tree is initialized as isometry, by default True
-        """
-        # Assuming all equal local dims
-        child_shape = self._local_dim[0]
-        parent_shape = min(self.max_bond_dim, child_shape**2)
-        for idx in range(self.num_layers - 1, -1, -1):
-            self[idx].initialize_layer(
-                [child_shape, child_shape, parent_shape],
-                initialization=method,
-                isometry=isometry,
-                dtype=self.dtype,
-                device=self.device,
+
+        sectors : dict, optional
+            Can restrict symmetry sector and/or bond dimension in initialization.
+            If empty, no restriction.
+            Default to empty dictionary.
+        """
+        isometrize = isometry or self._requires_singvals
+
+        if method == "vacuum":
+            matrix = np.zeros((self.num_sites, self.local_dim[0]))
+            matrix[:, 0] = 1
+            ttn = TTN.product_state_from_local_states(
+                matrix,
+                convergence_parameters=self._convergence_parameters,
+                tensor_backend=self._tensor_backend,
+            )
+            self.layers = ttn.layers
+        else:
+            # Assuming all equal local dims
+            child_link = self.local_links[0]
+            links = self._tensor_backend.tensor_cls.set_missing_link(
+                [child_link, child_link, None],
+                self._convergence_parameters.ini_bond_dimension,
+                are_links_outgoing=[False, False, True],
             )
-            child_shape = parent_shape
-            parent_shape = min(self.max_bond_dim, child_shape**2)
+
+            for idx in range(self.num_layers - 1, -1, -1):
+                self[idx].initialize_layer(
+                    links,
+                    self._tensor_backend,
+                    initialization=method,
+                    isometry=isometrize,
+                    sectors=sectors,
+                )
+
+                child_link = links[-1]
+                links = self._tensor_backend.tensor_cls.set_missing_link(
+                    [child_link, child_link, None],
+                    self._convergence_parameters.ini_bond_dimension,
+                    are_links_outgoing=[False, False, True],
+                )
+
+        if isometrize and (method != "empty"):
+            self.iso_center = (0, 0)
+
+        if self._requires_singvals:
+            # Cannot replace QR in initialize_layer with SVD as the values
+            # will be thrown a way, only way is to iterate through everything.
+            # So we skip QR in the first place, and do everything here.
+            for ii in range(self.num_sites):
+                self.site_canonize(ii)
+
+            self.iso_towards((0, 0))
 
     def dot(self, other):
         """
         Calculate the dot-product or overlap between two TTNs, i.e.,
         <other | self>.
 
         Parameters
@@ -1087,104 +1922,49 @@
         """
         if not isinstance(other, TTN):
             raise TypeError("Only two TTNs can be the input.")
 
         if self.num_sites != other.num_sites:
             raise ValueError("States must have the same number of sites.")
 
-        xp = self._device_checks()
-
         sandwich = self.layers[-1].dot(other.layers[-1])
 
         for ii in range(1, self.num_layers):
             ket = deepcopy(self.layers[-1 - ii])
 
             # contr_rmats will combine the tensors in the sandwich
             # list and the corresponding tensors in the ket, where
             # each ket tensor is contracted with two tensors in the
             # sandwich list
             ket.contr_rmats(sandwich)
 
             sandwich = ket.dot(other.layers[-1 - ii])
 
         if self.is_ttn:
-            final = xp.tensordot(sandwich[0], sandwich[1], [[0, 2], [0, 1]])
+            final = sandwich[0].tensordot(sandwich[1], [[0, 2], [0, 1]])
         else:
             final = sandwich[0]
 
         # It remain a 1x1 matrix with the links of the symmetry selector
-        return np.trace(final)
-
-    def get_tensor_of_site(self, idx):
-        """
-        Generic function to retrieve the tensor for a specific site. Compatible
-        across different tensor network geometries.
-
-        Parameters
-        ----------
-        idx : int
-            Return tensor containin the link of the local
-            Hilbert space of the idx-th site.
-        """
-        return self[-1][idx // 2]
-
-    def get_rho_i(self, idx):
-        """
-        Calculate the reduced density matrix for a single site.
-        If the singular values are stored (i.e. not None) do not
-        move the isometry center, but use them to compute local
-        observables.
-
-        Parameters
-        ----------
-
-        idx : integer
-            Calculate the reduced density matrix of site ``idx``.
-            Recall python indices start at zero.
-
-        Returns
-        -------
-
-        numpy ndarray : rank-2 tensor with the reduced density
-        matrix.
-        """
-        xp = self._device_checks()
-        layer_idx = self.num_layers - 1
-        tensor_idx = idx // 2
-
-        if self[layer_idx].singvals[tensor_idx] is None:
-            self.iso_towards([layer_idx, tensor_idx], keep_singvals=True)
-            tensor = self[layer_idx][tensor_idx]
-        else:
-            tensor = self[layer_idx][tensor_idx]
-            tensor = xp.tensordot(
-                tensor, xp.diag(self[layer_idx].singvals[tensor_idx]), ([2], [1])
-            )
-
-        if idx % 2 == 0:
-            contr_idx = [1, 2]
-        else:
-            contr_idx = [0, 2]
-
-        rho = xp.tensordot(tensor, tensor.conj(), [contr_idx, contr_idx])
-
-        return rho
+        return final.get_entry()
 
     @classmethod
-    def read(cls, filename, cmplx=True, order="F"):
+    def read(cls, filename, tensor_backend, cmplx=True, order="F"):
         """
         Read a TTN written by FORTRAN in a formatted way on file.
         Reads in column-major order but the output is in row-major.
         This is the only method that overrides the number of sites,
         since you may not know before reading.
 
         Parameters
         ----------
         filename: str
             PATH to the file
+        tensor_backend : :class:`TensorBackend`
+            Setup which tensor class to create.
         cmplx: bool, optional
             If True the MPS is complex, real otherwise. Default to True
         order: str, optional
             Format in which the tensors are saved. If 'F' column-major,
             if 'C' row major"
 
         Returns
@@ -1198,14 +1978,18 @@
         Many fields stored in a TTN for the fortran code are not kept
         as they can be easily retrieved on the python side.
 
         The performance can be improved if we consider converting
         the isometry center in fortran to python and ensure a
         conversion is always possible.
         """
+        ext = "pkl" + cls.extension
+        if filename.endswith(ext):
+            return cls.read_pickle(filename)
+
         tensor_list = []
 
         with open(filename, "r") as fh:
             # Version of tn_state_treenetwork
             _ = fh.readline().strip()
 
             # TTO flag
@@ -1230,15 +2014,22 @@
 
                 num_tensors_layer = int(fh.readline().strip())
 
                 # maximum number of links n2
                 _ = int(fh.readline().strip())
 
                 for _ in range(num_tensors_layer):
-                    tens_jj = read_tensor(fh, cmplx=cmplx, order=order)
+                    tens_jj = tensor_backend.tensor_cls.read(
+                        fh,
+                        tensor_backend.dtype,
+                        tensor_backend.device,
+                        tensor_backend.base_tensor_cls,
+                        cmplx=cmplx,
+                        order=order,
+                    )
                     layer_list.append(tens_jj)
 
                 # the cutoff
                 _ = int(fh.readline().strip())
                 truncated = [xx == "T" for xx in fh.readline().strip().split()]
                 tmp = list(map(int, fh.readline().strip().split()))
 
@@ -1274,25 +2065,27 @@
                 iso_f90 = list(map(int, fh.readline().strip().split()))
                 if len(iso_f90) == 2:
                     psi.iso_center = [iso_f90[0] - 1, iso_f90[1] - 1]
 
         return psi
 
     @classmethod
-    def read_v0_2_29(cls, filename, cmplx=True, order="F"):
+    def read_v0_2_29(cls, filename, tensor_backend, cmplx=True, order="F"):
         """
         Read a TTN written by FORTRAN in a formatted way on file.
         Reads in column-major order but the output is in row-major.
         This is the only method that overrides the number of sites,
         since you may not know before reading.
 
         Parameters
         ----------
         filename: str
             PATH to the file
+        tensor_backend : :class:`TensorBackend`
+            Setup which tensor class to create.
         cmplx: bool, optional
             If True the MPS is complex, real otherwise. Default to True
         order: str, optional
             Format in which the tensors are saved. If 'F' column-major,
             if 'C' row major"
 
         Returns
@@ -1329,15 +2122,22 @@
 
             for _ in range(num_layers):
                 layer_list = []
 
                 num_tensors_layer = int(fh.readline().strip())
 
                 for _ in range(num_tensors_layer):
-                    tens_jj = read_tensor(fh, cmplx=cmplx, order=order)
+                    tens_jj = tensor_backend.tensor_cls.read(
+                        fh,
+                        tensor_backend.dtype,
+                        tensor_backend.device,
+                        tensor_backend.base_tensor_cls,
+                        cmplx=cmplx,
+                        order=order,
+                    )
                     layer_list.append(tens_jj)
 
                 # the cutoff
                 _ = int(fh.readline().strip())
                 truncated = [xx == "T" for xx in fh.readline().strip().split()]
                 tmp = list(map(int, fh.readline().strip().split()))
 
@@ -1366,98 +2166,14 @@
             if has_iso:
                 # This would be the iso position, let's not trust it
                 # We prefer to instantiate upon need
                 _ = list(map(int, fh.readline().strip().split()))
 
         return cls.from_tensor_list(tensor_list)
 
-    @classmethod
-    def from_statevector(cls, statevector, device="cpu"):
-        """
-        Initialize the TTN by decomposing a statevector into TTN form.
-
-        Parameters
-        ----------
-
-        statevector : ndarray of shape( [local_dim]*num_sites, )
-            Statevector describing the interested state for initializing the TTN
-
-        device : str, optional
-            Device where the computation is done. Either "cpu" or "gpu".
-        """
-
-        # At the moment, no truncation is implemented in the code
-        num_sites = len(statevector.shape)
-        local_dim = statevector.shape[0]
-
-        if np.any(local_dim != np.array(statevector.shape)):
-            raise Exception(
-                "from_statevector requires equal local dim " + "across the system."
-            )
-
-        num_layers = int(np.log2(num_sites) - 1)
-        state_tensor = statevector
-        tensor_list = []
-        singvals_list = []
-        p0 = 1
-        p1 = 2
-
-        for ll in range(num_layers):
-            tensor_layer_list = []
-            singvals_layer_list = []
-            i0 = p0
-            i1 = p1
-
-            if ll == (num_layers - 1):
-                num_svd = 1
-            else:
-                num_svd = num_sites // p1
-
-            for _ in range(num_svd):
-                d0 = local_dim ** (p1 // 2)
-                d1 = local_dim**p1
-                d2 = np.prod(state_tensor.shape[2:])
-                umat, s_tot, vhmat = np.linalg.svd(
-                    state_tensor.reshape([d1, d2]), full_matrices=False
-                )
-                singvals_layer_list.append(s_tot)
-                s_tot = np.diag(s_tot)
-
-                umat = umat.reshape([d0, d0, d1])
-                new_shape = (
-                    [d1] + [d0] * ((num_sites - i1) // (p1 // 2)) + [d1] * (i0 - 1)
-                )
-                state_tensor = np.dot(s_tot, vhmat).reshape(new_shape)
-
-                perm = [jj + 1 for jj in range(len(state_tensor.shape) - 1)] + [0]
-                state_tensor = np.transpose(state_tensor, perm)
-
-                i0 += 1
-                i1 += p1
-                tensor_layer_list.append(umat)
-
-                if ll == (num_layers - 1):
-                    tensor_layer_list.append(state_tensor)
-
-            p1 *= 2
-            tensor_list.append(tensor_layer_list)
-            singvals_list.append(singvals_layer_list)
-
-        tensor_list[-1][0] = np.reshape(
-            tensor_list[-1][0], list(tensor_list[-1][0].shape) + [1]
-        )
-        # The two top links are the same link
-        singvals_list[-1].append(singvals_list[-1][0])
-
-        obj = cls.from_tensor_list(
-            tensor_list, singvals_list=singvals_list, device=device
-        )
-
-        return obj
-
     def to_statevector(self, qiskit_order=False, max_qubit_equivalent=20):
         """
         Decompose a given TTN into statevector form.
 
         Parameters
         ----------
         qiskit_order : bool, optional
@@ -1466,18 +2182,18 @@
         max_qubit_equivalent : int, optional
             Maximum number of qubits for which the statevector is computed.
             i.e. for a maximum hilbert space of 2**max_qubit_equivalent.
             Default to 20.
 
         Returns
         -------
-        xp.array
+
+        psi : instance of :class:`_AbstractQteaTensor`
             The statevector of the system
         """
-        xp = self._device_checks()
         if np.prod(self.local_dim) > 2**max_qubit_equivalent:
             raise Exception(
                 "Hilbert space %d**" % (self.local_dim)
                 + "%d is too large to " % (self.num_sites)
                 + "convert to statevector."
             )
 
@@ -1488,15 +2204,15 @@
 
             parent_layer = deepcopy(self[-2 - ii])
             parent_layer.contr_rmats(fused)
 
             current_layer = parent_layer
 
         # Top layer with two tensors
-        psi = xp.tensordot(current_layer[0], current_layer[1], [[2], [2]]).flatten()
+        psi = current_layer[0].tensordot(current_layer[1], [[2], [2]])
         if qiskit_order:
             order = "F"
         else:
             order = "C"
 
         return psi.reshape(self.local_dim).reshape(np.prod(self.local_dim), order=order)
 
@@ -1538,47 +2254,46 @@
         Returns
         -------
         list of numpy ndarray
             Tensors that will constitute the MPS
         numpy ndarray
             Singular values cut in the procedure
         """
-        xp = self._device_checks()
         # First, isometrize the top
         self.isometrize_all()
 
         # Start from uppermost layer
         curr_layer = self[0]  # Contains the current layer of tensors
         new_layer = []  # New layer being built
         cuts = []  # Approximation done in the procedure
 
         # Reshape first layer adding a dummy link for working with rank-4 tensors until the end
         # The convention is the following: links are numbered left to right, like in an MPS. This
         # means that, in the upper layer, we have [dummy, left_child, right_child, parent] on the
         # left tensor, while on the right we have [parent, left_child, right_child, dummy]
         # for curr_layer[0] we use only up to shpae[:-1] because we neglect the symmetry index
-        curr_layer[0] = curr_layer[0].reshape(1, *curr_layer[0].shape[:-1])
+        curr_layer[0] = curr_layer[0].reshape([1] + list(curr_layer[0].shape[:-1]))
         curr_layer[1] = curr_layer[1].transpose([2, 0, 1])
-        curr_layer[1] = curr_layer[1].reshape(*curr_layer[1].shape, 1)
+        curr_layer[1] = curr_layer[1].reshape(list(curr_layer[1].shape) + [1])
 
         # Cycle over the TTN layers, up to the last
         for idx in range(self.num_layers - 1):
             # print(f'Layer {idx} contracting into {idx+1} over {len(self[:])} layers')
             for tens_idx, tens in enumerate(curr_layer):
                 # First, divide the tensor with an SVD, such that each tensor in layer idx+1 has a
                 # corresponding layer in the upper tensor, instead of 1/2 of them
-                tens_left, tens_right, _, cut = self.tSVD(
-                    tens, [0, 1], [2, 3], contract_singvals="R", conv_params=conv_params
+                tens_left, tens_right, _, cut = tens.split_svd(
+                    [0, 1], [2, 3], contract_singvals="R", conv_params=conv_params
                 )
                 tens_left_next = self[idx + 1][tens_idx * 2]
                 tens_right_next = self[idx + 1][tens_idx * 2 + 1]
 
                 # Contract each tensor in layer idx with its correspondent in layer idx+1
-                new_tens_left = xp.tensordot(tens_left, tens_left_next, ([1], [2]))
-                new_tens_right = xp.tensordot(tens_right, tens_right_next, ([1], [2]))
+                new_tens_left = tens_left.tensordot(tens_left_next, ([1], [2]))
+                new_tens_right = tens_right.tensordot(tens_right_next, ([1], [2]))
                 # Transpose the legs in the correct format
                 new_tens_right = new_tens_right.transpose([0, 2, 3, 1])
                 new_tens_left = new_tens_left.transpose([0, 2, 3, 1])
 
                 # Save the new tensor in the next layer
                 new_layer.append(new_tens_left)
                 new_layer.append(new_tens_right)
@@ -1588,26 +2303,28 @@
             curr_layer = new_layer
             new_layer = []
 
         # Pass from a list of n/2 4-legs tensors to a list of n 3-legs tensors
         # that you can use to initialize an MPS
         tensor_list = []
         for tens in curr_layer:
-            tens_left, tens_right, _, cut = self.tSVD(
-                tens, [0, 1], [2, 3], contract_singvals="R"
+            tens_left, tens_right, _, cut = tens.split_svd(
+                [0, 1], [2, 3], contract_singvals="R", conv_params=conv_params
             )
 
             tensor_list.append(tens_left)
             tensor_list.append(tens_right)
             cuts.append(cut)
 
         return tensor_list, cuts
 
     @classmethod
-    def from_tensor_list(cls, tensor_list, singvals_list=None, device="cpu"):
+    def from_tensor_list(
+        cls, tensor_list, singvals_list=None, tensor_backend=None, conv_params=None
+    ):
         """
         Construct a TTN from a listed list of tensors. The outer list contains
         the layers, the inner list contains the tensors within a layer.
 
         The local Hilbert space is the first list entry and the uppermost
         layer in the TTN is the last list entry. The first list will have
         num_sites / 2 entries. The uppermost list has two entries.
@@ -1627,50 +2344,61 @@
         local_dim = []
         for elem in tensor_list[0]:
             local_dim.append(elem.shape[0])
             local_dim.append(elem.shape[1])
 
         # convergence parameters are hard-coded for now, find a meaningful
         # bond dimension
-        chi = 1 + int(
-            np.max(np.array([np.max(xx.shape) for sub in tensor_list for xx in sub]))
-        )
-        conv_param = TNConvergenceParameters(max_bond_dimension=chi)
+        if conv_params is None:
+            chi = 1 + int(
+                np.max(
+                    np.array([np.max(xx.shape) for sub in tensor_list for xx in sub])
+                )
+            )
+            conv_params = TNConvergenceParameters(max_bond_dimension=chi)
 
-        obj = cls(num_sites, conv_param, local_dim=local_dim, initialize="empty")
+        obj = cls(
+            num_sites,
+            conv_params,
+            local_dim=local_dim,
+            initialize="empty",
+            tensor_backend=tensor_backend,
+        )
+        tensor_cls = obj._tensor_backend.tensor_cls
 
         idx = obj.num_layers
         last_dim = num_sites
         for jdx, sub in enumerate(tensor_list):
             idx -= 1
 
             if last_dim / 2 != len(sub):
                 raise Exception("Length of tensor list not correct.")
 
             last_dim = len(sub)
 
             for kdx, elem in enumerate(sub):
+                if not isinstance(elem, _AbstractQteaTensor):
+                    elem = tensor_cls.from_elem_array(elem)
                 obj[idx].append(elem)
                 if singvals_list is None:
                     obj[idx].singvals[kdx] = None
                 else:
                     obj[idx].singvals[kdx] = singvals_list[jdx][kdx]
 
-        obj.to_device(device)
+        obj.convert(obj._tensor_backend.dtype, obj._tensor_backend.device)
 
         return obj
 
     @classmethod
     def product_state_from_local_states(
         cls,
         mat,
         padding=None,
         convergence_parameters=None,
-        dtype=np.complex128,
-        device="cpu",
+        tensor_backend=None,
     ):
         """
         Construct a product (separable) state in TTN form, given the local
         states of each of the sites.
 
         Parameters
         ----------
@@ -1690,14 +2418,17 @@
             numerical noise.
             If False, the bond dimensions are equal to 1.
             Default to None.
 
         convergence_parameters : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters for the new TTN.
 
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
         Return
         ------
         prod_ttn : :py:class:`TTN`
             Corresponding product state TTN.
         """
         if len(mat.shape) != 2:
             raise Exception("numpy ndarray must be of rank-2.")
@@ -1720,17 +2451,16 @@
             )
 
         # initialize the TTN
         prod_ttn = cls(
             num_sites,
             convergence_parameters,
             local_dim=local_dim,
+            tensor_backend=tensor_backend,
             initialize="empty",
-            dtype=dtype,
-            device=device,
         )
 
         # Bottom layer contains physical Hilbert space. We merge local states
         # into rank-2 tensors via Kronecker product.
         for ii in range(prod_ttn.num_sites // 2):
             # indices of states we want to merge into new rank-2 tensor
             i1 = 2 * ii
@@ -1742,27 +2472,28 @@
             theta = np.kron(mat[i1, :], mat[i2, :])
 
             theta = np.reshape(theta, [local_dim, local_dim, 1])
             if padding is not None:
                 theta = np.pad(
                     theta, ((0, 0), (0, 0), (0, pad - 1)), constant_values=pad_value
                 )
-            prod_ttn[-1].append(theta)
+            prod_ttn[-1].append(tensor_backend.tensor_cls.from_elem_array(theta))
         prod_ttn[-1].singvals = [np.ones(1) for _ in range(prod_ttn.num_sites // 2)]
 
         # Tensors in remaining layers are rank-3 tensor with all links
         # being of dimension 1, or `pad` in the case of padding
         # (symmetry sector is added in next step).
         tensor_fill = np.reshape(np.array([1], dtype=float), [1, 1, 1])
         if padding is not None:
             tensor_fill = np.pad(
                 tensor_fill,
                 ((0, pad - 1), (0, pad - 1), (0, pad - 1)),
                 constant_values=pad_value,
             )
+        tensor_fill = tensor_backend.tensor_cls.from_elem_array(tensor_fill)
         idx = prod_ttn.num_layers - 2
         last_dim = prod_ttn.num_sites // 2
         for ii in range(idx, -1, -1):
             last_dim = last_dim // 2
             for _ in range(last_dim):
                 prod_ttn[ii].append(tensor_fill)
             prod_ttn[ii].singvals = [np.ones(1) for _ in range(last_dim)]
@@ -1770,124 +2501,22 @@
         # Top layer has to be conform with symmetry sector even if
         # TTN has no symmetry.
         if prod_ttn.is_ttn:
             if padding is not None:
                 dims = [prod_ttn[0][0].shape[0], prod_ttn[0][0].shape[1], pad, 1]
             else:
                 dims = [prod_ttn[0][0].shape[0], prod_ttn[0][0].shape[1], 1, 1]
-            prod_ttn[0][0] = np.reshape(prod_ttn[0][0], dims)
+            prod_ttn[0][0] = prod_ttn[0][0].reshape(dims)
 
         prod_ttn[0].singvals = [np.ones(1) for _ in range(prod_ttn[0].num_tensors)]
 
-        prod_ttn.to_device(device)
-
-        return prod_ttn
-
-    @classmethod
-    def product_state_from_local_states_2d(
-        cls,
-        mat_2d,
-        padding=None,
-        mapping="HilbertCurveMap",
-        return_map=False,
-        conv_params=None,
-        dtype=np.complex128,
-        device="cpu",
-    ):
-        """
-        Construct a product (separable) state in 1d TTN form for a 2d system
-        by mapping it to 1d, given the local states of each of the sites.
-
-        Parameters
-        ----------
-        mat_2d : np.array of rank 2
-            Array with third axis being a (normalized) local state of
-            the (ii,jj)-th site (where ii and jj are indices of the
-            first and second axes).
-            Product of first two axes' dimensions is therefore equal
-            to the total number of sites, and third axis dimension
-            corresponds to the local dimension.
-
-        padding : np.array of length 2 or `None`, optional
-            Used to enable the growth of bond dimension in TDVP algorithms
-            for TTN (necessary as well for two tensor updates).
-            If not `None`, all the TTN tensors are padded such that the bond
-            dimension is equal to `padding[0]`. The value `padding[1]`
-            tells with which value are we padding the tensors. Note that
-            `padding[1]` should be very small, as it plays the role of
-            numerical noise.
-            If False, the bond dimensions are equal to 1.
-            Default to None.
-
-        mapping : string or instance of :py:class:`HilbertCurveMap`,
-                  optional
-            Which 2d to 1d mapping to use. Possible inputs are:
-            'HilbertCurveMap', 'SnakeMap', and 'ZigZagMap'.
-            Default is 'HilbertCurveMap'.
-
-        return_map : boolean, optional
-            If True, the function returns array `map` with indices
-            of 2d to 1d mapping.
-            Default to False.
-
-        convergence_parameters : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters for the new TTN.
-
-        Return
-        ------
-        prod_ttn : :py:class:`TTN`
-            Corresponding product state TTN.
-        map : np.array, returned only if return_map==True
-            Nx2 Matrix, where N is a total number of particles.
-            The values in the ii-th row of the matrix denote
-            particle's position in a corresponding 2d grid.
-
-        """
-        if len(mat_2d.shape) != 3:
-            raise Exception("numpy ndarray must be of rank-3.")
-        for ii in range(0, mat_2d.shape[0]):
-            for jj in range(0, mat_2d.shape[1]):
-                norm = np.linalg.norm(mat_2d[ii, jj, :])
-                if abs(norm - 1) > 10e-5:
-                    raise ValueError(
-                        f"Local state on site ({ii+1},{jj+1}) "
-                        f"not normalized. Norm = {norm}."
-                    )
-
-        dim = 2  # define that we are in 2d
-        num_sites_x, num_sites_y, local_dim = mat_2d.shape
-        size = [num_sites_x, num_sites_y]
-        num_sites_tot = num_sites_x * num_sites_y
-
-        # f ind the corresponding indices of 2d points in 1d
-        map_indices = map_selector(dim, size, mapping)
-        if return_map:
-            # will be same as map_indices, just in np.ndarray form
-            map_array = np.zeros((num_sites_tot, 2))
-
-        # compute the corresponding array with local states for 1d
-        mat_1d = np.zeros((num_sites_tot, local_dim))
-        ii = 0
-        for ind in map_indices:
-            n_x, n_y = ind
-            mat_1d[ii, :] = mat_2d[n_x, n_y, :]
-            if return_map:
-                map_array[ii] = ind
-            ii += 1
-
-        prod_ttn = TTN.product_state_from_local_states(
-            mat_1d,
-            padding=padding,
-            convergence_parameters=conv_params,
-            dtype=dtype,
-            device=device,
+        prod_ttn.convert(
+            prod_ttn._tensor_backend.dtype, prod_ttn._tensor_backend.device
         )
 
-        if return_map:
-            return prod_ttn, map_array
         return prod_ttn
 
     def extend_local_hilbert_space(self, number_levels):
         """
         Extend the local Hilbert by a certain number of levels without
         population. Extends the lowest layer with physical Hilbert space
         in the tree.
@@ -1912,19 +2541,21 @@
         None
         """
         if self.iso_center is not None:
             if (self.iso_center[0] == 0) and (self.iso_center[1] == 0):
                 return
 
         for ii in range(1, self.num_layers):
-            r_list = self[-ii].qr_towards_top()
+            r_list = self[-ii].qr_towards_top(
+                self._requires_singvals, self._convergence_parameters
+            )
             self[-ii - 1].contr_rmats(r_list)
 
         if self.is_ttn:
-            self[0].qr_top_right()
+            self[0].qr_top_right(self._requires_singvals, self._convergence_parameters)
 
         self.iso_center = [0, 0]
 
         return
 
     def get_path(self, target, start=None):
         """
@@ -2071,152 +2702,14 @@
             # QR from right to left
             path_up.append([0, 1, 2, 0, 0, 2])
 
         complete_path = path_up + path_down
 
         return complete_path
 
-    def norm(self):
-        if self.iso_center is None:
-            # We have to install isometry center, pick default
-            self.isometrize_all()
-
-        tensor = self[self.iso_center[0]][self.iso_center[1]]
-        norm = np.sum(np.real(tensor * tensor.conj()))
-
-        return np.sqrt(norm)
-
-    def normalize(self):
-        factor = 1.0 / self.norm()
-        self.scale(factor)
-
-    def scale(self, factor):
-        if self.iso_center is None:
-            # We have to install isometry center, pick default
-            self.isometrize_all()
-
-        self[self.iso_center[0]][self.iso_center[1]] *= factor
-
-    def site_canonize(self, idx, keep_singvals=False):
-        """
-        Shift the isometry center to the tensor containing the
-        corresponding site.
-
-        Parameters
-        ----------
-
-        idx : int
-            Index of the physical site which should be isometrized.
-
-        keep_singvals : bool, optional
-            If True, keep the singular values even if shifting the iso with a
-            QR decomposition. Default to False.
-
-        """
-        target_layer = self.num_layers - 1
-        target_tensor = idx // 2
-
-        self.iso_towards([target_layer, target_tensor], keep_singvals=keep_singvals)
-
-    def iso_towards(self, new_iso, keep_singvals=False, trunc=False, conv_params=None):
-        """
-        Shift isometry center towards a certain tensor.
-
-        Parameters
-        ----------
-
-        new_iso : list of two integers
-            New isometry center in terms of layer and tensor.
-
-        keep_singvals : bool, optional
-            If True, keep the singular values even if shifting the iso with a
-            QR decomposition. Default to False.
-
-        trunc : Boolean, optional
-            If `True`, the shifting is done via truncated SVD.
-            If `False`, the shifting is done via QR.
-            Default to `False`.
-
-        conv_params : :py:class:`TNConvergenceParameters`, optional
-            Convergence parameters to use for the SVD. If `None`, convergence
-            parameters are taken from the TTN.
-            Default to `None`.
-
-        Returns
-        -------
-
-        singvals_cut_tot : np.ndarray
-            Singualr values cut in the process of shifting the isometry center.
-            None if moved through the QR.
-
-        Details
-        -------
-
-        We introduce an overhead if the TTN has no
-        isometry center set up to now. This choice could
-        be further optimized.
-        """
-        if self.iso_center is not None:
-            if (self.iso_center[0] == new_iso[0]) and (
-                self.iso_center[1] == new_iso[1]
-            ):
-                # Return singular values cut, i.e., zeros in this case
-                return np.zeros(1)
-        else:
-            # Isometry center is not set; we install it first
-            # at [0, 0] and accept a small overhead
-            self.isometrize_all()
-
-        # Obtain the path
-        complete_path = self.get_path(new_iso)
-
-        singvals_cut_tot = []
-        for elem in complete_path:
-            # Get the tensor for the QR
-            src_layer_idx = elem[0]
-            src_tensor_idx = elem[1]
-            src = self[src_layer_idx][src_tensor_idx]
-
-            # Get the target/destination tensor
-            dst_layer_idx = elem[3]
-            dst_tensor_idx = elem[4]
-            dst = self[dst_layer_idx][dst_tensor_idx]
-
-            src_link = elem[2]
-            dst_link = elem[5]
-
-            src, dst, singvals_cut, singvals = self.shift_iso_to(
-                src, dst, src_link, dst_link, trunc=trunc, conv_params=conv_params
-            )
-            singvals_cut_tot.append(singvals_cut)
-            # Unset the singvals if the flag is not active, since the QRs might destroy
-            # the entanglement in the PATH.
-            if not keep_singvals:
-                lowest_layer = max(src_layer_idx, dst_layer_idx)
-                lowest_tensor = (
-                    dst_tensor_idx if dst_layer_idx > src_layer_idx else src_tensor_idx
-                )
-                self[lowest_layer].unset_singvals(lowest_tensor)
-            if trunc:
-                lowest_layer = max(src_layer_idx, dst_layer_idx)
-                lowest_tensor = (
-                    dst_tensor_idx if dst_layer_idx > src_layer_idx else src_tensor_idx
-                )
-                self[lowest_layer].singvals[lowest_tensor] = singvals
-            if self.eff_op is not None:
-                self._update_eff_ops(src, elem)
-
-            self[src_layer_idx][src_tensor_idx] = src
-            self[dst_layer_idx][dst_tensor_idx] = dst
-
-            # And reset iso center to new value
-            self.iso_center = elem[3:5]
-
-        return np.array(singvals_cut_tot)
-
     def _iso_towards_via_cache(
         self, tensor_jj, start, target, state_jj, trunc=False, conv_params=None
     ):
         """
         Run isometrization from a start site to a target site for given
         tensor using the tensors in the cache for specific states.
 
@@ -2372,17 +2865,15 @@
             does not come from previously contracting the
             2-qubit gate,`target_tens` represents a new iso
             center.
 
         singvals_cut : float or None
             Singular values cut (if trunc=True) or None
         """
-        xp = self._device_checks()
-        if not trunc:
-            conv_params = None
+        no_truncation = not trunc
 
         # define some useful variables
         sdim = source_tens.ndim
         leg = sdim - 1
         # get the links which go to the left and to the
         # right in QR
         links = np.arange(sdim)
@@ -2392,35 +2883,35 @@
         # define the correct permutation of the Q tensor for
         # after the QR based on the source_link position
         qperm = (
             list(range(source_link)) + [sdim - 2] + list(range(source_link, sdim - 2))
         )
         # if truncating, perform the splitting via truncated SVD
         if trunc:
-            q_tens, r_tens, _, singvals_cut = self.tSVD(
-                source_tens,
+            q_tens, r_tens, _, singvals_cut = source_tens.split_svd(
                 links_left,
                 links_right,
                 perm_left=qperm,
                 contract_singvals="R",
                 conv_params=conv_params,
+                no_truncation=no_truncation,
             )
             singvals_cut = self._postprocess_singvals_cut(
                 singvals_cut=singvals_cut, conv_params=conv_params
             )
         # otherwise split the tensor via QR
         else:
-            q_tens, r_tens = self.QR(
-                source_tens, links_left, links_right, perm_left=qperm
+            q_tens, r_tens = source_tens.split_qr(
+                links_left, links_right, perm_left=qperm
             )
             singvals_cut = None
 
         # contract the R tensor to the target_tensor
         # t_tens = np.tensordot(r_tens, target_tens, axes=[[1], [target_link]])
-        t_tens = xp.tensordot(target_tens, r_tens, axes=[[target_link], [1]])
+        t_tens = target_tens.tensordot(r_tens, [[target_link], [1]])
 
         # find the correct permutation of the new target tensor based
         # on the target_link position
         tdim = t_tens.ndim
         tperm = (
             list(range(target_link))
             + [tdim - 2]
@@ -2482,16 +2973,14 @@
 
         Return
         ------
         np.ndarray
             Singualr values cut in the process of shifting the isometry center.
             Array of None if moved through the QR.
         """
-        xp = self._device_checks()
-
         # TTN must have the isometry center installed on the starting tensor
         if any(self.iso_center != pos[0]):
             raise ValueError(
                 "Isometry center needs to be installed on"
                 f" the start tensor position {pos[0]}. Currently"
                 f" it is {self.iso_center}."
             )
@@ -2503,24 +2992,22 @@
                 "Initial shifting leg position can only be set for rank-3 tensor."
             )
 
         # if leg_start is defined, permute it to the end and add a dummy leg
         # of dimension 1 on its initial place
         if leg_start is not None:
             # add a dummy leg
-            self[pos[0, 0]][pos[0, 1]] = xp.expand_dims(
-                self[pos[0, 0]][pos[0, 1]], axis=leg_start
-            )
+            self[pos[0, 0]][pos[0, 1]].attach_dummy_link(leg_start, False)
 
             # permute the leg to the end
             perm = np.arange(self[pos[0, 0]][pos[0, 1]].ndim)
             perm = np.delete(perm, leg_start + 1)
             perm = np.append(perm, leg_start + 1)
 
-            self[pos[0, 0]][pos[0, 1]] = self[pos[0, 0]][pos[0, 1]].transpose(perm)
+            self[pos[0, 0]][pos[0, 1]].transpose_update(perm)
 
         # get path from initial to target position
         path = self.get_path(target=pos[1], start=pos[0])
 
         # for each step in the path, QR decompose the
         # source tensor and contract with the target tensor
         # to shift the extra leg.
@@ -2544,16 +3031,15 @@
             (
                 self[ind1[0]][ind1[1]],
                 self[ind2[0]][ind2[1]],
                 svals_trunc,
             ) = self.shift_leg_to(
                 tensor1, tensor2, link1, link2, trunc=trunc, conv_params=conv_params
             )
-            if xp == cp and svals_trunc is not None:
-                svals_trunc = svals_trunc.get()
+            svals_trunc = tensor1.get_of(svals_trunc)
             singvals_cut_tot.append(svals_trunc)
 
             # set the isometry center to the next tensor
             self.iso_center = ind2
 
         # if set, permute the extra leg to the desired position
         if leg_end is not None:
@@ -2581,15 +3067,16 @@
             If True the TTN is complex, real otherwise. Default to True
 
         Returns
         -------
 
         None
         """
-        self.to_device("cpu")
+        self.convert(None, "cpu")
+
         # Oldest compatible tn_state_treenetwork version (length must be 8)
         f90_ttn_version = "0.3.4   "
 
         num_tensors = 0
         for ii in range(self.num_layers):
             num_tensors += len(self[ii])
 
@@ -2627,15 +3114,16 @@
             tensor are printed for each layer. If array-like, you can individually
             select the number of tensors to be printed. By default None.
 
         Return
         ------
         None
         """
-        self.to_device("cpu")
+        self.convert(None, "cpu")
+
         if how_many_layers is None:
             how_many_layers = self.num_layers
         if how_many_layers > self.num_layers or how_many_layers < 0:
             raise ValueError("Invalid number of layers")
         if how_many is None or np.isscalar(how_many):
             how_many = np.repeat(how_many, self.num_layers)
         elif len(how_many) != self.num_layers:
@@ -2732,15 +3220,15 @@
 
         if self.num_layers - 1 == key[0]:
             self._cache_get_children_prob[key] = deepcopy(value)
         else:
             self._cache_get_children_prob[key] = value
 
         if self._cachelimit_bytes_get_children_prob is not None:
-            size_bytes = getsizeof(value)
+            size_bytes = value.getsizeof()
             self._cachesize_bytes_get_children_prob += size_bytes
 
     def _get_cache(self, key):
         """
         Internal function helping to retrieve tensors during projective
         measurements.
 
@@ -2848,15 +3336,14 @@
 
     def _clear_cache_by_state(self, all_probs, current_key, reduce_to=0.9):
         """
         Cleaning cache by identifying different states.
         """
         previously_deleted_keys = []
         for key in self._clear_cache_by_state_step(current_key, reduce_to):
-
             # Stored is not the length of the key, but the qubit where
             # we are at in py-index. Thus, at the (n-1)-th qubit, we have n
             # projective measurements and a length of n
             ii = len(key) - 1
 
             if all_probs is not None:
                 key_str = ",".join(map(str, key))
@@ -2912,15 +3399,15 @@
         for idx in inds:
             key2 = mapping[idx]
 
             for layer_idx, tensor_idx in keys_to_be_deleted[key2]:
                 key = (layer_idx, tensor_idx, key2)
 
                 if self._cachelimit_bytes_get_children_prob is not None:
-                    size_bytes = getsizeof(self._cache_get_children_prob[key])
+                    size_bytes = self._cache_get_children_prob[key].getsizeof()
                     self._cachesize_bytes_get_children_prob -= size_bytes
 
                 del self._cache_get_children_prob[key]
                 yield key[2]
 
             if (
                 self._cachesize_bytes_get_children_prob
@@ -2951,15 +3438,15 @@
         keys_to_delete = []
         for key in self._cache_get_children_prob:
             if len(key[2]) > num_qubits_keep:
                 keys_to_delete.append(key)
 
         for key in keys_to_delete:
             if self._cachelimit_bytes_get_children_prob is not None:
-                size_bytes = getsizeof(self._cache_get_children_prob[key])
+                size_bytes = self._cache_get_children_prob[key].getsizeof()
                 self._cachesize_bytes_get_children_prob -= size_bytes
 
             del self._cache_get_children_prob[key]
             yield key[2]
 
     def _clear_cache_by_num_qubits(self, all_probs, num_qubits_keep):
         """
@@ -3074,54 +3561,58 @@
         t_tens : np.ndarray
             New gauge center taking the place of `target_tens`
 
         singvals_cut : np.ndarray
             Singular values cut in moving the iso. If the iso is moved through the
             QR then it is None.
         """
-        if not GPU_AVAILABLE:
-            xp = np
-        else:
-            xp = cp.get_array_module(source_tens)
-        if not trunc:
-            conv_params = None
+        if conv_params is None:
+            conv_params = self._convergence_parameters
 
-        # Permute source_link to the end
+        no_truncation = not trunc
+        is_q_outgoing = source_tens.are_links_outgoing[source_link]
+
+        r_links = [source_link]
+        q_links = source_tens._invert_link_selection(r_links)
+
+        # Permute link back
         nn = len(source_tens.shape)
         lnk = source_link
-        s_perm = list(range(lnk)) + list(range(lnk + 1, nn)) + [lnk]
         q_perm = list(range(lnk)) + [nn - 1] + list(range(lnk, nn - 1))
 
-        tmp = source_tens.transpose(s_perm)
-        dim = list(np.arange(tmp.ndim))
-
-        # if truncating, perform the splitting via truncated SVD
-        if trunc:
-            left_mat, right_mat, singvals, singvals_cut = self.tSVD(
-                tmp,
-                dim[:-1],
-                [dim[-1]],
+        if trunc or self._requires_singvals:
+            # truncating, perform the splitting via truncated SVD
+            left_mat, right_mat, singvals, singvals_cut = source_tens.split_svd(
+                q_links,
+                r_links,
                 perm_left=q_perm,
                 contract_singvals="R",
                 conv_params=conv_params,
+                no_truncation=no_truncation,
+                is_link_outgoing_left=is_q_outgoing,
             )
             singvals_cut = self._postprocess_singvals_cut(
                 singvals_cut=singvals_cut, conv_params=conv_params
             )
-            if xp == cp:
-                singvals_cut = singvals_cut.get()
+            singvals_cut = left_mat.get_of(singvals_cut)
 
-        # Otherwise split the tensor via QR
         else:
-            left_mat, right_mat = self.QR(tmp, dim[:-1], [dim[-1]], perm_left=q_perm)
+            # Otherwise split the tensor via QR
+            # print("shift_iso_to", tmp.ndim, q_perm, len(tmp.links))
+            left_mat, right_mat = source_tens.split_qr(
+                q_links,
+                r_links,
+                perm_left=q_perm,
+                is_q_link_outgoing=is_q_outgoing,
+            )
             singvals_cut = None
             singvals = None
 
         # Contract rmat into target_tensor
-        tmp = xp.tensordot(target_tens, right_mat, ([target_link], [1]))
+        tmp = target_tens.tensordot(right_mat, ([target_link], [1]))
 
         nn = len(target_tens.shape)
         lnk = target_link
         t_perm = list(range(lnk)) + [nn - 1] + list(range(lnk, nn - 1))
 
         t_tens = tmp.transpose(t_perm)
 
@@ -3157,70 +3648,71 @@
         probabilities : list of floats
             Probabilities of the children
 
         tensor_list : list of ndarray
             Child tensors, already contracted with the next site
             if not last site.
         """
-        xp = self._device_checks()
+        # Get functions for elemtary arrays
+        sqrt = tensor.get_attr("sqrt")
+
         # New measurements clean up the cache
         if (site_idx == 0) and do_clear_cache:
             self.clear_cache(num_qubits_keep=0)
 
         link_site = site_idx % 2
         local_dim = self.local_dim[site_idx]
 
         if tensor is None:
             # Response to the end of the loop, I assume
-            return xp.zeros(local_dim), xp.repeat(None, local_dim)
+            tmp = tensor.vector_with_dim_like(local_dim)
+            tmp *= 0.0
+            return tmp, np.repeat(None, local_dim)
 
         # Build reduced density matrix
         if link_site == 0:
-            reduced_rho = xp.tensordot(tensor, tensor.conj(), ([1, 2], [1, 2]))
+            reduced_rho = tensor.tensordot(tensor.conj(), ([1, 2], [1, 2]))
         else:
-            reduced_rho = xp.tensordot(tensor, tensor.conj(), ([0, 2], [0, 2]))
+            reduced_rho = tensor.tensordot(tensor.conj(), ([0, 2], [0, 2]))
+
+        # Convert to array on host/CPU with real values
+        probabilities = reduced_rho.diag(real_part_only=True, do_get=True)
 
-        probabilities = []
         tensors_list = []
 
         # Loop over basis states
-        if np.abs(1 - np.trace(reduced_rho)) > 1e-12:
+        if np.abs(1 - probabilities.sum()) > tensor.dtype_eps * 1e2:
             print("reduced rho", site_idx, "#", curr_state)
-            raise Exception(
+            warnings.warn(
                 "Reduced density matrix is not normalized; error = "
-                + str(np.abs(1 - np.trace(reduced_rho)))
+                + str(np.abs(1 - probabilities.sum()))
             )
 
-        for jj in range(local_dim):
-            prob_jj = np.real(reduced_rho[jj, jj])
-            if xp == cp:
-                prob_jj = prob_jj.get()
-            probabilities.append(prob_jj)
-
+        for jj, prob_jj in enumerate(probabilities):
             if (prob_jj > 0) and (link_site == 0):
                 # link_site == 0 automatically fulfills site_idx < num_sites - 1
 
                 # Projector is diagonal with one entry - cut entry for efficient
                 # contractions (keep rank-3 structure)
-                tensor_jj = tensor[jj : jj + 1, :, :]
+                tensor_jj = tensor.subtensor_along_link(0, jj, jj + 1)
 
                 # After scaling, we are done, the next site is as well in
                 # this tensor
-                tensor_jj /= np.sqrt(prob_jj)
+                tensor_jj /= sqrt(prob_jj)
 
                 tensors_list.append(tensor_jj)
             elif (prob_jj > 0) and (site_idx < self.num_sites - 1):
                 # Projector is diagonal with one entry - cut entry for efficent
                 # QR (keep rank-3 structure)
-                tensor_jj = tensor[:, jj : jj + 1, :]
+                tensor_jj = tensor.subtensor_along_link(1, jj, jj + 1)
 
                 state_jj = list(map(int, curr_state.split(","))) + [jj]
 
                 # Scale tensor
-                tensor_jj /= np.sqrt(prob_jj)
+                tensor_jj /= sqrt(prob_jj)
 
                 # We are not done, we have to walk the TTN up and then down
                 # the right path
                 target_layer = self.num_layers - 1
                 target_tensor = (site_idx + 1) // 2
 
                 start = [target_layer, target_tensor - 1]
@@ -3229,16 +3721,14 @@
                 tensor_jj = self._iso_towards_via_cache(
                     tensor_jj, start, target, state_jj
                 )
                 tensors_list.append(tensor_jj)
             else:
                 tensors_list.append(None)
 
-        probabilities = np.array(probabilities)
-
         return probabilities, tensors_list
 
     def _get_children_magic(self, *args, **kwargs):
         raise NotImplementedError("Function not implemented yet")
 
     def _get_child_prob(
         self,
@@ -3278,43 +3768,47 @@
 
         qiskit_convention : bool
             Qiskit convention, i.e., ``True`` stores the projective
             measurement in reverse order, i.e., the first qubit is stored
             in ``curr_state[-1]``. Passing ``False`` means indices are
             equal and not reversed.
         """
-        xp = self._device_checks()
+        # Get functions for elemtary arrays
+        cumsum, sqrt = tensor.get_attr("cumsum", "sqrt")
+
         # New measurement clean up the cache
         if site_idx == 0:
             self.clear_cache(num_qubits_keep=0)
 
         link_site = site_idx % 2
         local_dim = self.local_dim[site_idx]
 
         if unitary_setup is not None:
             # Have to apply local unitary
             unitary = unitary_setup.get_unitary(site_idx)
 
-            tensor = xp.tensordot(unitary, tensor, ([1], [link_site]))
+            tensor = unitary.tensordot(tensor, ([1], [link_site]))
             if link_site == 1:
                 # Need to permute links back to original order
                 tensor = tensor.transpose([1, 0, 2])
 
         # Build reduced density matrix
         if link_site == 0:
-            reduced_rho = xp.tensordot(tensor, tensor.conj(), ([1, 2], [1, 2]))
+            reduced_rho = tensor.tensordot(tensor.conj(), ([1, 2], [1, 2]))
         else:
-            reduced_rho = xp.tensordot(tensor, tensor.conj(), ([0, 2], [0, 2]))
+            reduced_rho = tensor.tensordot(tensor.conj(), ([0, 2], [0, 2]))
 
-        probs = np.real(xp.diag(reduced_rho))
-        cumul_probs = np.cumsum(probs)
+        # Calculate the cumulated probabilities via the reduced
+        # density matrix
+        probs = reduced_rho.diag(real_part_only=True)
+        cumul_probs = cumsum(probs)
         measured_idx = None
 
         # Check norm
-        if np.abs(1 - cumul_probs[-1]) > 1e-12:
+        if np.abs(1 - cumul_probs[-1]) > tensor.dtype_eps * 1e2:
             raise Exception(
                 "Reduced density matrix is not normalized; norm"
                 + " is %2.6f." % (cumul_probs[-1])
             )
 
         for jj in range(local_dim):
             if cumul_probs[jj] < target_prob:
@@ -3326,34 +3820,38 @@
             measured_idx = jj
 
             if link_site == 0:
                 # link_site == 0 automatically fulfills site_idx < num_sites - 1
 
                 # Projector is diagonal with one entry - cut entry for efficient
                 # contractions (keep rank-3 structure)
-                temp_tens = tensor[jj : jj + 1, :, :]
+                temp_tens = tensor.subtensor_along_link(0, jj, jj + 1)
 
                 # After scaling, we are done, the next site is as well in
                 # this tensor
-                temp_tens /= np.sqrt(probs[jj])
+                temp_tens /= sqrt(probs[jj])
 
             elif site_idx < self.num_sites - 1:
                 # Projector is diagonal with one entry - cut entry for efficent
                 # QR (keep rank-3 structure)
-                temp_tens = tensor[:, jj : jj + 1, :]
+                temp_tens = tensor.subtensor_along_link(1, jj, jj + 1)
 
                 if qiskit_convention:
                     state_jj = list(curr_state[::-1][:site_idx]) + [jj]
                 else:
                     state_jj = list(curr_state[:site_idx]) + [jj]
 
                 # Scale tensor
-                temp_tens /= np.sqrt(probs[jj])
+                temp_tens /= sqrt(probs[jj])
 
-                if np.abs(1 - np.sum(temp_tens * np.conj(temp_tens))) > 1e-12:
+                norm_temp_tens = temp_tens.norm()
+                if (
+                    np.abs(1 - temp_tens.get_of(norm_temp_tens))
+                    > tensor.dtype_eps * 1e2
+                ):
                     raise Exception("Norm violation")
 
                 # We are not done, we have to walk the TTN up and then down
                 # the right path
                 target_layer = self.num_layers - 1
                 target_tensor = (site_idx + 1) // 2
 
@@ -3365,18 +3863,17 @@
                 )
             else:
                 temp_tens = None
 
             break
 
         if temp_tens is not None:
-            if np.abs(1 - np.sum(temp_tens * np.conj(temp_tens))) > 1e-12:
-                raise Exception(
-                    "Norm violation " + str(np.sum(temp_tens * np.conj(temp_tens)))
-                )
+            norm_temp_tens = temp_tens.norm()
+            if np.abs(1 - temp_tens.get_of(norm_temp_tens)) > tensor.dtype_eps * 1e2:
+                raise Exception("Norm violation")
 
         return measured_idx, temp_tens, prob_jj
 
     def unset_all_singvals(self):
         """
         Unset all the singvals in the TTN due to a
         local operation that is modifying the global
@@ -3387,113 +3884,97 @@
         -------
         None
         """
         for layer in self:
             for ii in range(layer.num_tensors):
                 layer.unset_singvals(ii)
 
-    def to_device(self, device):
-        """
-        Move the TTN class to the new device.
-
-        Parameters
-        ----------
-        device : string
-            Device where to move the TTN
-        """
-        device = device.lower()
-        if device not in self.implemented_devices:
-            raise ValueError(
-                f"Device {device} is not implemented. Select from"
-                + f" {self.implemented_devices}"
-            )
-        # We already are in the correct device
-        if device == self.device:
-            return
-
-        for layer in self.layers:
-            layer.to_device(device)
-        self._device = device
-
     #########################################################################
     ###################### Effective operators methods ######################
     #########################################################################
-    def build_effective_operators(self, eff_op):
+    def build_effective_operators(self, measurement_mode=False):
         """
         Build the complete effective operator on each
-        of the links
-
-        Parameters
-        ----------
-        eff_op : :class:`TensorProductOperator`
-            effective operator with the physical operators already initialized
+        of the links. Now assumes `self.eff_op` is set.
         """
-        self.isometrize_all()
+        if list(self.iso_center) != [0, 0]:
+            raise Exception(f"Need to isometrize to [0, 0], but at {self.iso_center}.")
+
+        if self.eff_op is None:
+            raise Exception("Trying to build eff_op without attribute being set.")
 
+        if not self.is_ttn:
+            raise Exception("Double-check measurement setup and continue statements.")
+
+        # loop over layers in TTN
         for layer in self.layers[::-1]:
-            for tidx, tens in enumerate(layer):
-                # Retrieve the index of the operators for the children
-                children_op_ldxs = layer.op_neighbors[:-2, tidx]
-                # Retrieve the index of the operator on the parent
-                parent_op_ldx = layer.op_neighbors[-2, tidx]
-                # Update the effective operator
-                eff_op[parent_op_ldx] = self._contr_to_eff_op(
-                    tens,
-                    [eff_op[ii] for ii in children_op_ldxs],
-                    np.arange(len(children_op_ldxs)),
-                    2,
-                )
+            lidx = layer.layer_idx
 
-        self.eff_op = eff_op
+            # loop over tensor index in a layer
+            for tidx in range(len(layer) - 1, -1, -1):
+                # tensor
+                tens = layer[tidx]
+                # position of a tensor: layer index, tensor index
+                pos = (lidx, tidx)
 
-    def _update_eff_ops(self, src_tensor, id_step):
+                idx_out = 2
+                pos_links = self.get_pos_links(pos)
+
+                if lidx == 0 and tidx == 0 and (not measurement_mode):
+                    # Would calculate entry towards (0, 1) and revert it again (TTN)
+                    continue
+
+                if lidx == 0 and tidx == 0:
+                    # Want to finalize measurements, use symmetry selector
+                    idx_out = 3
+                    pos_links[-1] = (None, None)
+
+                # get the effective operator for this tensor
+                self.eff_op.contr_to_eff_op(tens, pos, pos_links, idx_out)
+
+                if measurement_mode:
+                    singvals = layer.singvals[tidx]
+                    if lidx == 0 and tidx == 0:
+                        singvals = None
+                    elif singvals is None:
+                        raise Exception("Missing singvals.")
+                    self.eff_op[(pos, tuple(pos_links[idx_out]))].run_measurements(
+                        tens, idx_out, singvals
+                    )
+
+    def _update_eff_ops(self, id_step):
         """
-        Update the effective operators after the iso shift
+        Update the effective operators after the iso shift. Source tensor is
+        iso position.
 
         Parameters
         ----------
-        src_tensor : ndarray
-            Q tensor after the QR
+
         id_step : list of ints
             List with the iso path, i.e.
             [src_layer, src_tensor, src_link, dst_layer, dst_tensor, dst_link]
 
         Returns
         -------
         None
             Updates the effective operators in place
         """
-        if id_step[:2] != self.iso_center:
+        if tuple(id_step[:2]) != tuple(self.iso_center):
+            print("Error information", id_step, self.iso_center)
             raise RuntimeError("Tried effective operators update not at the iso_center")
-        # Get info on the source tensor
-        src_layer_idx = id_step[0]
-        src_tensor_idx = id_step[1]
-        src_link = id_step[2]
 
-        aval_links = []
-        eff_ops = []
-        # Link idx, operator idx
-        for ll_idx, op_idx in enumerate(
-            self[src_layer_idx].op_neighbors[:, src_tensor_idx]
-        ):
-            # Add all the necessary tensors, i.e. all but those in the QR link, or those
-            # that are not initialized (value=-1)
-            if op_idx != -1 and ll_idx != src_link:
-                aval_links.append(ll_idx)
-                eff_ops.append(self.eff_op[op_idx])
-            # This is the index of the new operator
-            elif ll_idx == src_link:
-                new_op_idx = op_idx
-
-        # Perform the contraction
-        self.eff_op[new_op_idx] = self._contr_to_eff_op(
-            src_tensor, eff_ops, aval_links, src_link
-        )
+        # Information extracted from source tensor
+        pos = (id_step[0], id_step[1])
+        idx_out = id_step[2]
+        tens = self[id_step[0]][id_step[1]]
 
-    def _get_eff_op_on_pos(self, pos):
+        pos_links = self.get_pos_links(pos)
+        self.eff_op.contr_to_eff_op(tens, pos, pos_links, idx_out)
+
+    def deprecated_get_eff_op_on_pos(self, pos):
         """
         Obtain the list of effective operators adjacent
         to the position pos and the index where they should
         be contracted
 
         Parameters
         ----------
@@ -3517,51 +3998,139 @@
                 idx_list.append(ll_idx)
 
         return eff_ops, idx_list
 
     #########################################################################
     ######################### Optimization methods ##########################
     #########################################################################
-
-    def optimize_tree(self, verbose=False):
+    def default_sweep_order(self):
         """
-        Optimize the TTN by optimizing each tensor
-        in the TTN a number of times equal to num_sweeps.
+        Default sweep order to be used in the ground state search/time evolution.
         The optimization is bottom-top optimization
          - left to right in layer with index even
          - right to left in layer with index odd
-        This order minimizes the QR needed to move
-        the isometrisation center.
-        The number of sweeps and the other details
-        are controlled in :py:class:`TNConvergenceParameters`
+
+        Returns
+        -------
+        List[Tuple[int]]
+            The generator that you can sweep through
+        """
+        opt_path = []
+        for ldx in range(self.num_layers - 1, -1, -1):
+            if ldx % 2 == 0:
+                opt_path += [(ldx, tdx) for tdx in range(self[ldx].num_tensors)]
+            else:
+                opt_path += [
+                    (ldx, tdx) for tdx in range(self[ldx].num_tensors - 1, -1, -1)
+                ]
+
+        return opt_path
+
+    def default_sweep_order_back(self):
+        """Default sweep order backwards."""
+        opt_path = []
+        for ldx in range(self.num_layers - 1, -1, -1):
+            opt_path_ii = []
+            if ldx % 2 == 0:
+                opt_path_ii += [(ldx, tdx) for tdx in range(self[ldx].num_tensors)]
+            else:
+                opt_path_ii += [
+                    (ldx, tdx) for tdx in range(self[ldx].num_tensors - 1, -1, -1)
+                ]
+
+            opt_path += opt_path_ii[::-1]
+
+        return opt_path
+
+    def get_pos_partner_link_expansion(self, pos):
+        """
+        Get the position of the partner tensor to use in the link expansion
+        subroutine.
+        In TTN, it is always the parent tensor.
 
         Parameters
         ----------
-        verbose : bool
-            If True, print a lot of stuff
+        pos : Tuple[int]
+            Position w.r.t. which you want to compute the partner
 
         Returns
         -------
-        float
-            Energy at the end of the optimization
+        Tuple[int]
+            Position of the partner
+        int
+            Link of pos pointing towards the partner
+        int
+            Link of the partner pointing towards pos
         """
+        link_self, tdx_info = self._get_parent_info(pos)
+        pos_partner = tuple(tdx_info[:2])
+        link_partner = tdx_info[2]
 
-        # Cycle over sweeps
-        for _ in range(self._convergence_parameters.max_iter):
-            # Cycle over layers
-            for ldx in range(self.num_layers - 1, -1, -1):
-                if ldx % 2 == 0:
-                    iterator = range(self[ldx].num_tensors)
-                else:
-                    iterator = range(self[ldx].num_tensors - 1, -1, -1)
-                # Cycle over tensors
-                for tdx in iterator:
-                    self.optimize_single_tensor([ldx, tdx], verbose=verbose)
+        return pos_partner, link_self, link_partner
+
+    def _partial_iso_towards_for_timestep(self, pos, next_pos, no_rtens=False):
+        """
+        Move by hand the iso for the evolution backwards in time
+
+        Parameters
+        ----------
+        pos : Tuple[int]
+            Position of the tensor evolved
+        next_pos : Tuple[int]
+            Position of the next tensor to evolve
+
+        Returns
+        -------
+        QTeaTensor | link_self
+            The R tensor of the iso movement
+            link_self in no_rtens=True model
+        Tuple[int]
+            The position of the partner (the parent in TTNs)
+        int
+            The link of the partner pointing towards pos
+        List[int]
+            The update path to pass to _update_eff_ops
+        """
+        requires_singvals = self._requires_singvals
+
+        # Needed in other TN geometries
+        _ = next_pos
+        link_self, tdx_info = self._get_parent_info(pos)
+
+        pos_partner = tuple(tdx_info[:2])
+        link_partner = tdx_info[2]
+
+        nn = self[pos].ndim
+        all_legs = np.array(range(nn))
+        qlegs = list(all_legs[all_legs != link_self])
+
+        path_elem = list(pos) + [link_self] + list(tdx_info)
+        if no_rtens:
+            return link_self, pos_partner, link_partner, path_elem
+
+        if requires_singvals:
+            qtens, rtens, s_vals, _ = self[pos].split_svd(
+                qlegs,
+                [link_self],
+                no_truncation=True,
+                conv_params=self._convergence_parameters,
+                contract_singvals="R",
+            )
+            self.set_singvals_on_link(pos, pos_partner, s_vals)
+        else:
+            qtens, rtens = self[pos].split_qr(qlegs, [link_self])
+            self.set_singvals_on_link(pos, pos_partner, None)
+        if link_self + 1 != nn:
+            # Have to permute
+            qperm = list(range(link_self)) + [nn - 1] + list(range(link_self, nn - 1))
+            self[pos] = qtens.transpose(qperm)
+        else:
+            self[pos] = qtens
 
-        return self.compute_energy()
+        return rtens, pos_partner, link_partner, path_elem
 
     #########################################################################
     ############################ Apply methods ##############################
     #########################################################################
 
     def apply_one_site_operator(self, op, pos):
         """
@@ -3575,32 +4144,30 @@
             Position of the qubit where to apply `op`.
 
         """
         if pos < 0 or pos > self.num_sites - 1:
             raise ValueError(
                 "The position of the site must be between 0 and (num_sites-1)"
             )
-        if list(op.shape) != [self._local_dim[pos]] * 2:
-            raise ValueError(
-                "Shape of the input operator must be (local_dim, local_dim)"
-            )
-
-        xp = self._device_checks(operator=op)
+        # if list(op.shape) != [self._local_dim[pos]] * 2:
+        #    raise ValueError(
+        #        "Shape of the input operator must be (local_dim, local_dim)"
+        #    )
 
         # The physical layer is always the last one
         physical_layer = self.num_layers - 1
         target_tensor = self[physical_layer][pos // 2]
 
-        # First index of the 3-legs tensor
         if pos % 2 == 0:
-            res = xp.tensordot(op, target_tensor, ([1], [0]))
-        # Second index of the 3-legs tensor
+            # First index of the 3-legs tensor
+            res = op.tensordot(target_tensor, ([1], [0]))
         else:
-            res = xp.tensordot(op, target_tensor, ([1], [1]))
-            res = res.transpose(1, 0, 2)
+            # Second index of the 3-legs tensor
+            res = op.tensordot(target_tensor, ([1], [1]))
+            res = res.transpose([1, 0, 2])
 
         self[physical_layer][pos // 2] = res
 
     def apply_projective_operator(self, site, selected_output=None, remove=False):
         """
         Apply a projective operator to the site **site**, and give the measurement as output.
         You can also decide to select a given output for the measurement, if the probability is
@@ -3634,15 +4201,15 @@
         meas_state: int
             Measured state
         state_prob : float
             Probability of measuring the output state
         """
         if selected_output is not None and selected_output > self._local_dim[site] - 1:
             raise ValueError("The seleted output must be at most local_dim-1")
-        xp = self._device_checks()
+
         physical_layer = self.num_layers - 1
 
         # Workaround in case we have an extra leg in the tensor due to a temporary site
         sites = np.cumsum([0] + [tens.ndim - 1 for tens in self[physical_layer]])
         tens_idx = np.nonzero(site < sites)[0][0] - 1
         leg_idx = site - sites[tens_idx]
         leg_dim = self[physical_layer][tens_idx].shape[leg_idx]
@@ -3661,50 +4228,48 @@
         # Measure
         cum_prob = 0
         random_u = np.random.rand()
         # We don't use get_rho_ii since it can handle only physical tensors with 2
         # sites, while here we possibly have 3 sites
         tens = self[physical_layer][tens_idx]
         contr_legs = [ii for ii in range(tens.ndim) if ii != leg_idx]
-        rho_ii = xp.tensordot(tens, tens.conj(), (contr_legs, contr_legs))
+        rho_ii = tens.tensordot(tens.conj(), (contr_legs, contr_legs))
 
         for ii in range(leg_dim):
             if selected_output is not None and ii != selected_output:
                 continue
-            projector = _projector(ii, leg_dim, xp)
-            prob_ii = xp.trace(rho_ii @ projector)
-            cum_prob += prob_ii
+            projector = _projector_for_rho_i(ii, rho_ii)
+            prob_ii = rho_ii.tensordot(projector, ([0, 1], [1, 0])).get_entry()
+            cum_prob += np.real(prob_ii)
             if cum_prob >= random_u or selected_output == ii:
                 meas_state = ii
                 state_prob = prob_ii
                 break
 
         # Remove the extra site or project into the correct
         # subspace
         if remove:
-            projector_vect = xp.zeros(leg_dim)
-            projector_vect[meas_state] = 1
+            projector_vect = rho_ii.zeros_like()
+            projector_vect.set_diagonal_entry(meas_state, 1)
+
             # Project the state in the measured one
-            tens_to_remove = xp.tensordot(tens, projector_vect, ([leg_idx], [0]))
+            tens_to_remove = tens.tensordot(projector_vect, ([leg_idx], [0]))
             self[physical_layer][tens_idx] = tens_to_remove
         else:
-            new_tens = xp.tensordot(tens, projector, ([leg_idx], [1]))
+            new_tens = tens.tensordot(projector, ([leg_idx], [1]))
             new_tens = new_tens.transpose(_transpose_idx(tens.ndim, leg_idx))
             self[physical_layer][tens_idx] = new_tens
 
         # Unset all singvals since they are now outdated
         self.unset_all_singvals()
 
         # Renormalize and come back to previous norm
         self.normalize()
         self.scale(old_norm)
 
-        if xp == cp:
-            state_prob = state_prob.get()
-
         return meas_state, state_prob
 
     def apply_two_site_operator(self, gate, sites, conv_params=None):
         """
         Applies a two-site operator `gate` to the TTN on sites `sites[0]`
         and `sites[1]`.
 
@@ -3722,18 +4287,17 @@
             Convergence parameters to use for the SVD in the procedure.
             If `None`, convergence parameters are taken from the TTN.
             Default to `None`.
 
         Return
         ------
         np.ndarray
-            Singualr values cut in the process of shifting the isometry center.
+            Singular values cut in the process of shifting the isometry center.
             None if moved through the QR.
         """
-        xp = self._device_checks()
         # first recast the site positions into tensors
         # and leg indices
 
         # transform input into np array just in case the
         # user passes the list
         sites = np.array(sites)
 
@@ -3747,55 +4311,141 @@
         # Split the gate into two operators
         gate = gate.reshape((2, 2, 2, 2))
         conv_params_gate = TNConvergenceParameters(
             max_bond_dimension=int(self.local_dim[0] ** 2),
             trunc_method="N",
             cut_ratio=0,
         )
-        op1, op2, _, _ = self.tSVD(
-            gate, [0, 2], [1, 3], contract_singvals="R", conv_params=conv_params_gate
+        op1, op2, _, _ = gate.split_svd(
+            [0, 2], [1, 3], contract_singvals="R", conv_params=conv_params_gate
         )
 
         # Install the isometry center at the left operator site
         self.iso_towards([self.num_layers - 1, pos[0, 0]])
 
         # Contract the left operator with a physical site and transpose so that
         # extra leg is at the end
-        self[-1][pos[0, 0]] = xp.tensordot(
-            self[-1][pos[0, 0]], op1, axes=[pos[0, 1], [1]]
-        )
-        self[-1][pos[0, 0]] = xp.transpose(
-            self[-1][pos[0, 0]], axes=[2 - 2 * pos[0, 1], 0 + 2 * pos[0, 1], 1, 3]
+        self[-1][pos[0, 0]] = self[-1][pos[0, 0]].tensordot(op1, [pos[0, 1], [1]])
+        self[-1][pos[0, 0]].transpose_update(
+            [2 - 2 * pos[0, 1], 0 + 2 * pos[0, 1], 1, 3]
         )
 
         # Shift the extra link towards the site of the other operator, isometry center
         # is shifted automatically
         self.leg_towards(
             np.array(
                 [[(self.num_layers - 1), pos[0, 0]], [(self.num_layers - 1), pos[1, 0]]]
             )
         )
 
         # Contract the right operator with the physical site. After this step,
         # the tensor network is in the shape of TTN.
-        self[-1][pos[1, 0]] = xp.tensordot(
-            self[-1][pos[1, 0]], op2, axes=[[3, pos[1, 1]], [0, 2]]
-        )
-        self[-1][pos[1, 0]] = xp.transpose(
-            self[-1][pos[1, 0]], axes=[2 - 2 * pos[1, 1], 0 + 2 * pos[1, 1], 1]
+        self[-1][pos[1, 0]] = self[-1][pos[1, 0]].tensordot(
+            op2, [[3, pos[1, 1]], [0, 2]]
         )
+        self[-1][pos[1, 0]].transpose_update([2 - 2 * pos[1, 1], 0 + 2 * pos[1, 1], 1])
 
         # Backpropagate the SVDs
         singvals_cut_tot = self.iso_towards(
-            [self.num_layers - 1, pos[0, 0]], trunc=True, conv_params=conv_params
+            [self.num_layers - 1, pos[0, 0]],
+            trunc=True,
+            conv_params=conv_params,
+            keep_singvals=True,
+        )
+
+        return singvals_cut_tot
+
+    def apply_mpo(self, mpo):
+        """
+        Apply an MPO to the TTN on the sites `sites`.
+        The MPO should have the following convention for the links:
+        0 is left link. 1 is physical link pointing downwards.
+        2 is phisical link pointing upwards. 3 is right link.
+
+        The sites are encoded inside the DenseMPO class.
+
+        Parameters
+        ----------
+        mpo : DenseMPO
+            MPO to be applied
+
+        Returns
+        -------
+        np.ndarray
+            Singular values cutted when the gate link is contracted
+        """
+        # Sort sites
+        # mpo.sort_sites()
+        sites = np.array([mpo_site.site for mpo_site in mpo])
+        if not np.isclose(sites, np.sort(sites)).all():
+            raise RuntimeError("MPO sites are not sorted")
+
+        # transform input into np array just in case the
+        # user passes the list
+
+        operators = [site.operator * site.weight for site in mpo]
+        if mpo[0].strength is not None:
+            operators[0] *= mpo[0].strength
+
+        # pos[0,:] indicates the position of the left site, and
+        # pos[1,:] indicates the position of the right site, such that
+        # pos[ii,:] = [tensor_index, leg_index]. Leg index can be 0 or 1.
+        pos = np.zeros((len(sites), 2), dtype=int)
+        pos[:, 0] = sites // 2
+        pos[:, 1] = sites % 2
+
+        # Install the isometry center at the left operator site
+        self.site_canonize(sites[0], keep_singvals=True)
+
+        # Contract the left operator with a physical site and transpose so that
+        # extra leg is at the end
+        op1 = operators[0].remove_dummy_link(0)
+        self[-1][pos[0, 0]] = self[-1][pos[0, 0]].tensordot(op1, [pos[0, 1], [1]])
+        self[-1][pos[0, 0]].transpose_update(
+            [2 - 2 * pos[0, 1], 0 + 2 * pos[0, 1], 1, 3]
         )
 
+        for idx, site in enumerate(pos[1:, 0]):
+            # Shift the extra link towards the site of the other operator, isometry center
+            # is shifted automatically
+            self.leg_towards(
+                np.array(
+                    [
+                        [(self.num_layers - 1), pos[idx, 0]],
+                        [(self.num_layers - 1), site],
+                    ]
+                )
+            )
+
+            # Contract the right operator with the physical site. After this step,
+            # the tensor network is in the shape of TTN.
+            op = operators[idx + 1]
+            if idx == len(pos) - 2:
+                op = op.remove_dummy_link(3)
+                transpose_idxs = [2 - 2 * pos[idx + 1, 1], 0 + 2 * pos[idx + 1, 1], 1]
+            else:
+                transpose_idxs = [
+                    2 - 2 * pos[idx + 1, 1],
+                    0 + 2 * pos[idx + 1, 1],
+                    1,
+                    3,
+                ]
+
+            self[-1][site] = self[-1][site].tensordot(op, [[3, pos[1, 1]], [0, 2]])
+            self[-1][site].transpose_update(transpose_idxs)
+
+        for site in pos[:-1, 0][::-1]:
+            # Backpropagate the SVDs
+            singvals_cut_tot = self.iso_towards(
+                [self.num_layers - 1, site], trunc=True, keep_singvals=True
+            )
+
         return singvals_cut_tot
 
-    def swap_qubits(self, sites, conv_params=None):
+    def swap_qubits(self, sites, conv_params=None, trunc=True):
         """
         This function applies a swap gate to sites in a TTN,
         i.e. swaps these two qubits.
 
         Parameters
         ----------
         sites : list/array of two int
@@ -3803,21 +4453,24 @@
             are swapped.
 
         conv_params : :py:class:`TNConvergenceParameters`, optional
             Convergence parameters to use for the SVD in the procedure.
             If `None`, convergence parameters are taken from the TTN.
             Default to `None`.
 
+        trunc: bool, optional
+            If True, move through SVDs, otherwise through QRs.
+            Default to True.
+
         Return
         ------
         np.ndarray
             Singualr values cut in the process of shifting the isometry center.
             None if moved through the QR.
         """
-        xp = self._device_checks()
         # first recast the site positions into tensors
         # and leg indices
 
         # transform input into np array just in case the
         # user passes the list
         sites = np.array(sites)
 
@@ -3848,18 +4501,18 @@
         # Shift the second leg from site 2 to site 1 and backpropagate the
         # SVD truncation
         singvals_cut_tot = self.leg_towards(
             np.array(
                 [[(self.num_layers - 1), pos[1, 0]], [(self.num_layers - 1), pos[0, 0]]]
             ),
             leg_end=pos[0, 1] + 1,
-            trunc=True,
+            trunc=trunc,
             conv_params=conv_params,
         )
-        self[-1][pos[0, 0]] = xp.squeeze(self[-1][pos[0, 0]], axis=pos[0, 1])
+        self[-1][pos[0, 0]].remove_dummy_link(pos[0, 1])
 
         return singvals_cut_tot
 
     #########################################################################
     ######################### Measurement methods ###########################
     #########################################################################
 
@@ -3874,29 +4527,29 @@
 
         Return
         ------
         measures : ndarray, shape (num_sites)
             Measures of the local operator along each site
         """
         self.check_obs_input(op)
-        xp = self._device_checks()
 
-        measures = xp.zeros(self.num_sites)
+        measures = np.zeros(self.num_sites)
 
         # This subroutine can be parallelized if the singvals are stored using
         # joblib
         for ii in range(self.num_sites):
             rho_i = self.get_rho_i(ii)
 
-            expectation = xp.trace(rho_i @ op)
-            measures[ii] = xp.real(expectation)
-
-        # Come back to CPU if on GPU
-        if xp == cp:
-            measures = measures.get()
+            if op.ndim == 2:
+                expectation = rho_i.tensordot(op, ([0, 1], [1, 0]))
+            else:
+                tmp = deepcopy(op)
+                tmp.trace_one_dim_pair([0, 3])
+                expectation = rho_i.tensordot(tmp, ([0, 1], [1, 0]))
+            measures[ii] = np.real(expectation.get_entry())
 
         return measures
 
     def meas_tensor_product(self, ops, idxs):
         """
         Measure the tensor products of n operators `ops` acting on the indexes `idxs`
 
@@ -3912,38 +4565,45 @@
         measure : float
             Result of the measurement
         """
         self.check_obs_input(ops, idxs)
         # No operator to measure, return expectation value of identity (which is always 1)
         if len(idxs) == 0:
             return 1
-        xp = self._device_checks()
+
         order = np.argsort(idxs)
         idxs = np.array(idxs)[order]
-        ops = xp.array(ops)
+        ops = np.array(ops)
         ops = ops[order]
 
         # Inefficient way without transfer matrix. For an efficient implementation
         # see the MPS method.
         temp_ttn = deepcopy(self)
 
         # Apply local operators to TTN
         for idx, op in zip(idxs, ops):
+            if op.ndim == 4:
+                if (op.shape[3] == 1) and (op.shape[0] == 1):
+                    op = op.copy().remove_dummy_link(3).remove_dummy_link(0)
+                else:
+                    raise RuntimeError(
+                        "Only bond dimension 1 MPOs implemented in TTN meas_tensor_product"
+                    )
             temp_ttn.apply_one_site_operator(op, idx)
 
         # Compute expectation  value through dot product.
         # It is inefficient, since if the observables are restricted to a subset of the
         # ttn we already know there are some contraction going to the identity for the
         # isometrization. For example, if the observable is only on the first quarter of
         # the tree, we know the remaining part contracts to the identity and we don't
         # need to compute it explicitely
-        measure = xp.real(temp_ttn.sandwich(self))
+        measure = temp_ttn.sandwich(self)
 
-        if xp == cp:
-            measure = measure.get()
+        # Move measure to host if necessary
+        measure = np.real(ops[0].get_of(measure))
 
         return measure
 
     def meas_weighted_sum(self, op_strings, idxs_strings, coefs):
         """
         Measure the weighted sum of tensor product operators.
         See :py:func:`meas_tensor_product`
@@ -3988,30 +4648,50 @@
 
         Return
         ------
         measures : dict
             Keys are the range of the smallest bipartition to which the entanglement
             (value) is relative
         """
-        xp = self._device_checks()
+        # Get functions for elemtary arrays
+        summ, log = self[0][0].get_attr("sum", "log")
+
         measures = {}
-        for layer in self:
+        for layer_idx, layer in enumerate(self):
             for idx, singvals in enumerate(layer.singvals):
                 # If the singvals are not present for some reason the bond entropy
                 # value for that bond is set to None
                 if singvals is None:
                     s_von_neumann = None
                 else:
                     # Remove 0s from the singvals (they might come from the from_statevector method)
                     singvals = singvals[singvals > 0]
-                    s_von_neumann = -xp.sum(singvals**2 * xp.log(singvals**2))
-                    if xp == cp:
-                        s_von_neumann = s_von_neumann.get()
+                    s_von_neumann = -summ(singvals**2 * log(singvals**2))
+                    s_von_neumann = self[0][0].get_of(s_von_neumann)
 
-                measures[tuple(layer.sites[:, 2, idx])] = s_von_neumann
+                pos_src = (layer_idx, idx)
+                _, pos_parent = self._get_parent_info(pos_src)
+                pos_parent = pos_parent[:2]
+                sites_src, sites_dst = self.get_bipartition_link(pos_src, pos_parent)
+
+                # Find the smaller bipartation and lower sites for equal bipartitions
+                if len(sites_src) < len(sites_dst):
+                    key = tuple([np.min(sites_src), np.max(sites_src)])
+                elif len(sites_src) > len(sites_dst):
+                    key = tuple([np.min(sites_dst), np.max(sites_dst)])
+                elif sites_src[0] < sites_dst[0] and sites_src[-1] < sites_dst[-1]:
+                    key = tuple([np.min(sites_src), np.max(sites_src)])
+                elif sites_src[0] > sites_dst[0] and sites_src[-1] > sites_dst[-1]:
+                    key = tuple([np.min(sites_dst), np.max(sites_dst)])
+                else:
+                    raise NotImplementedError(
+                        "No rule implemented to choose bipartition."
+                    )
+
+                measures[key] = s_von_neumann
 
         return measures
 
     #########################################################################
     ######################## Visualisation methods ##########################
     #########################################################################
 
@@ -4131,194 +4811,7 @@
                 which="both",  # both major and minor ticks are affected
                 bottom=False,  # ticks along the bottom edge are off
                 top=False,  # ticks along the top edge are off
                 labelbottom=False,
                 left=False,
                 labelleft=False,
             )  # labels along the bottom edge are off
-
-
-###########################################################################
-############## Function to run the code using the common tools ############
-###########################################################################
-
-
-def run_ttn_simulation(simulation, params):
-    """
-    Run a full simulation with the python ttn.
-
-    **Arguments**
-
-    simulation : instance of ``ATTNSimulation``
-        Represents all the information on the simulation.
-
-    params : dict
-        Dictionary containing the current parameters for the
-        simulation.
-    """
-
-    # Statics
-    # -------
-
-    # Collect some information
-    lvals = simulation.model.eval_lvals(params)
-    num_sites = np.prod(lvals)
-
-    # If `continue_file` is present, use it to initialize the state
-    if "continue_file" in params:
-        extension = params["continue_file"][-4:]
-        if extension != ".npy":
-            raise TypeError(
-                "The initial state for pyTTN must be in .npy array form. "
-                f"Current form is {extension}."
-            )
-        state = np.load(params["continue_file"], allow_pickle=True)
-        if len(state) != int(np.log2(num_sites)):
-            raise ValueError(
-                f"The number of layers in the inital state array "
-                f"({len(state)}) does not correspond "
-                "to the TTN number of layers "
-                f"({int(np.log2(num_sites))})."
-            )
-        state = TTN.from_tensor_list(state, device=params.get("device", "cpu"))
-    else:
-        state = TTN(
-            num_sites, simulation.convergence, device=params.get("device", "cpu")
-        )
-
-    # Initialize effective operators
-    _ = TensorProductOperator(
-        params,
-        simulation.model,
-        simulation.operators,
-        state,
-        device=params.get("device", "cpu"),
-    )
-
-    # Minimization of the energy
-    _ = state.optimize_tree(simulation.verbosity)
-
-    # Measurements
-    folder_name_output = simulation.observables.get_folder_trajectories(
-        simulation.folder_name_output, params
-    )
-
-    full_file_path = os.path.join(folder_name_output, "static_obs.dat")
-
-    observables = run_ttn_measurements(state, simulation, params)
-    observables.write_results(full_file_path, state.is_measured, params)
-
-    # Dynamics
-    # --------
-    if "Quenches" in params:
-        raise NotImplementedError("Dynamics is not implemented for python TTNs")
-
-    return
-
-
-def run_ttn_measurements(state, simulation, params, postfix=None, time=None):
-    """
-    Run all the measurements for a state.
-
-    **Arguments**
-
-    state : instance of TTN
-        State to be measured.
-
-    simulation : instance of ``ATTNSimulation``
-        Represents all the information on the simulation.
-
-    params : dict
-        Dictionary containing the current parameters for the
-        simulation.
-
-    postfix : str or ``None``, optional
-        Postfix to be attached to filename etc. If ``None``, no
-        postfix is attached.
-        Default to empty string via ``None``.
-
-    time : float or ``None``, optional
-        The current time during the evolution if float. If a
-        time cannot be specified, e.g., for statics, pass
-        ``None`` or do not pass argument.
-        Default to ``None``.
-
-    **Returns**
-
-    Instance of ``TNObservables``. If we run in parallel, we better
-    make a copy before using the buffer of the TNObservables.
-    """
-    # We probably need params in the future - avoid unused argument error
-    _ = len(params)
-
-    if postfix is None:
-        postfix = ""
-    if not isinstance(state, TTN):
-        raise TypeError()
-    observables = deepcopy(simulation.observables)
-
-    observables.results_buffer["energy"] = state.compute_energy()
-    observables.results_buffer["norm"] = state.norm()
-    if time is not None:
-        observables.results_buffer["time"] = time
-
-    # Local observables
-    # -----------------
-
-    local_obs = observables.obs_list["TNObsLocal"]
-
-    for jj, name_jj in enumerate(local_obs.name):
-        operator = simulation.operators.ops[local_obs.operator[jj]]
-
-        local_obs.results_buffer[name_jj] = state.meas_local(operator)
-
-    # Correlation measurements
-    # ------------------------
-    # Optmize correlators with either get_rho_ij or a better meas_tensor_product
-
-    corr_obs = observables.obs_list["TNObsCorr"]
-
-    for kk, name_kk in enumerate(corr_obs.name):
-        corr_mat = np.zeros((state.num_sites, state.num_sites), dtype=np.complex128)
-
-        op_a = simulation.operators.ops[corr_obs.operators[kk][0]]
-        op_b = simulation.operators.ops[corr_obs.operators[kk][1]]
-        op_ab = np.dot(op_a, op_b)
-
-        corr_mat += np.diag(state.meas_local(op_ab))
-
-        for ii in range(state.num_sites):
-            for jj in range(state.num_sites):
-                if ii == jj:
-                    continue
-                corr_mat[ii, jj] = state.meas_tensor_product([op_a, op_b], [ii, jj])
-                corr_mat[jj, ii] = state.meas_tensor_product([op_a, op_b], [jj, ii])
-
-        corr_obs.results_buffer[name_kk] = corr_mat
-
-    # Distance measurement (TNDistance2Pure)
-    # --------------------
-
-    dist_obs = observables.obs_list["TNDistance2Pure"]
-
-    for jj, name_jj in enumerate(dist_obs.name):
-        path_jj = dist_obs.path_to_state[jj]
-
-        psi_ttn = TTN.read(path_jj)
-
-        dist_obs.results_buffer[name_jj] = state.dot(psi_ttn)
-
-    # State2File measurement
-    # ----------------------
-    # we will store numpy arrays now independent of the flag
-
-    file_obs = observables.obs_list["TNState2File"]
-
-    for jj, name_jj in enumerate(file_obs.name):
-        full_name = name_jj + postfix + ".npy"
-        np.save(
-            full_name, np.array(state.to_tensor_list(), dtype=object), allow_pickle=True
-        )
-
-        file_obs.results_buffer[name_jj] = full_name
-
-    return observables
```

### Comparing `qtealeaves-0.5.14/qtealeaves/emulator/tto_simulator.py` & `qtealeaves-1.1.1/qtealeaves/emulator/tto_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,14 @@
 import scipy.optimize as scop
 import numpy as np
 import numpy.linalg as nla
 from qtealeaves.emulator.lptn_simulator import LPTN
 from qtealeaves.convergence_parameters import TNConvergenceParameters
 from .ttn_simulator import TTN, TTNLayer
 
-# Try to import cupy
-try:
-    import cupy as cp
-    from cupy_backends.cuda.api.runtime import CUDARuntimeError
-
-    try:
-        _ = cp.cuda.Device()
-        GPU_AVAILABLE = True
-    except CUDARuntimeError:
-        GPU_AVAILABLE = False
-except ImportError:
-    cp = None
-    GPU_AVAILABLE = False
-
 
 class TTO(TTN):
     r"""
     TREE TENSOR OPERATOR - represents a density matrix
 
     Parameters
     ----------
@@ -57,32 +43,29 @@
         are truncated
 
     local_dim : int, optional
         Dimension of Hilbert space of single site
         (defined as the same for each site).
         Default is 2.
 
+    tensor_backend : `None` or instance of :class:`TensorBackend`
+        Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
     iso_center : None or np.ndarray/list of two ints, optional
         Position of the gauge center. [i,j] means j-th
         tensor of i-th layer, i=0 is uppermost, j=0 is
         the leftmost tensor. If TTO has no gauge
         center, iso_center = None.
         Default is None.
 
-    dtype : dtype
-        Type of entries for the tensor.
-        Default is np.complex128.
-
-    device : str, optional
-        Device where the computations are done.
-        Default to "cpu".
-
     Initialization
     --------------
-    |000...000><000---000|
+
+    Maximally mixed state is initialized, which may lead to memory issues for large system sizes.
+    The option to initialize a (pure) product state will be included in the future.
 
     Tensor representation
     ---------------------
     .. codeblock::
     \ / \ /
      O   O
       \ /            } --> complex conjugates of tensors below,
@@ -134,34 +117,40 @@
 
         [ uppermost layer is indexed with i = 0 ]
     - access to [i,j]-th tensor with TTO[i][j]
 
         [ leftmost tensor is indexed with j = 0 ]
     - order of legs in tensor
 
-        [ left leg - upper leg - right leg ]
+        [ left leg - right leg - upper leg]
     """
+
+    extension = "tto"
     is_ttn = False
 
     def __init__(
         self,
         num_sites,
         conv_params,
         local_dim=2,
+        tensor_backend=None,
         iso_center=None,
-        dtype=np.complex128,
-        device="cpu",
+        **kwargs,
     ):
+        if "initialize" in kwargs:
+            raise Exception("Input ignored.")
+        if "sectors" in kwargs:
+            raise Exception("Input ignored.")
+
         super().__init__(
             num_sites,
             conv_params,
             local_dim=local_dim,
+            tensor_backend=None,
             initialize="ground",
-            dtype=dtype,
-            device=device,
         )
 
         self._probabilities = None
 
         if iso_center is not None and not isinstance(iso_center, (list, np.ndarray)):
             raise TypeError(
                 "The iso_center must be None or list or np.ndarray,"
@@ -184,23 +173,29 @@
                 raise ValueError(
                     "Invalid input for iso_center."
                     f" The {iso_center[0]}-th layer does not contain"
                     f" {iso_center[1]} tensors."
                 )
         self.iso_center = iso_center
 
+        # TTO initializetion not aware of device
+        self.convert(self._tensor_backend.dtype, self._tensor_backend.device)
+
     @property
     def cc_layers(self):
         """
         complex conjugate part of LPTN, returns complex conjugate tensors
         stored in TTOLayers
         """
         c_conj = [
             TTNLayer.from_tensorlist(
-                x.cc_tensors, self.local_dim, self.max_bond_dim, self.device
+                x.cc_tensors,
+                self.local_dim,
+                self._convergence_parameters.max_bond_dim,
+                self._tensor_backend.device,
             )
             for x in self.layers
         ]
         return c_conj
 
     @property
     def local_dim(self):
@@ -223,15 +218,17 @@
         prob : np.ndarray
             Mixed state probabilities in
             descending order.
         """
         if self._probabilities is not None:
             # Probabilities have been calculated before
             return self._probabilities
-        xp = self._device_checks()
+
+        # Get functions for elemtary arrays
+        sort = self[0][0].get_attr("sort")
 
         if self.iso_center is None:
             warn(
                 "Mixed state probabilities can be extracted"
                 " only from TTO with gauge center at the"
                 " uppermost tensor. Installing a gauge center"
                 " to the TTO."
@@ -243,17 +240,18 @@
                 " only from TTO with gauge center at the"
                 " uppermost tensor. Shifting a gauge center"
                 f" from {self.iso_center} to [0,0]."
             )
             self.shift_gauge_center([0, 0])
 
         top = self[0][0]
-        top = top.reshape((top.shape[0] * top.shape[1], top.shape[2]))
-        sing_val = xp.linalg.svd(top, compute_uv=False)
-        prob = np.sort(sing_val**2)
+        _, _, sing_val, _ = top.split_svd(
+            [0, 1], [2], no_truncation=True, conv_params=self._convergence_parameters
+        )  # compute_uv=False)
+        prob = sort(sing_val**2)
         prob = prob[::-1]
 
         self._probabilities = prob
         return self._probabilities
 
     def trunc_probabilities(self, k_0, cut_ratio=1e-6, norm_track=False):
         """
@@ -274,20 +272,18 @@
         norm_loss : float, returned if `norm_track`==True
             Norm loss due to the truncation.
         """
         root = self[0][0]
         conv_params = TNConvergenceParameters(
             max_bond_dimension=k_0, cut_ratio=cut_ratio
         )
-        root, _, _, norm_loss = self.tSVD(
-            root,
-            [0, 2],
-            [1],
+        root, _, _, norm_loss = root.split_svd(
+            [0, 1],
+            [2],
             contract_singvals="L",
-            perm_left=[0, 2, 1],
             conv_params=conv_params,
         )
         norm_loss = 1 - np.sum(norm_loss**2)
         self[0][0] = deepcopy(root)
         self._probabilities = None
         self.iso_center = [0, 0]
 
@@ -394,39 +390,39 @@
             warn(
                 "Negativity can be computed only for TTO"
                 " with gauge center at the uppermost tensor."
                 f" Shifting a gauge center from {self.iso_center}"
                 " to [0,0]."
             )
             self.shift_gauge_center([0, 0])
-        xp = self._device_checks()
 
-        root_rho = xp.tensordot(self[0][0], self[0][0].conj(), axes=[[2], [2]])
+        root_rho = self[0][0].tensordot(self[0][0].conj(), [[2], [2]])
 
         # partial transpose with respect to one subsystem (half of
         # the system in this case)
         # the resulting negativity is independent of the
         # choice of which from the two subsystems we transpose
         part_transpose = root_rho.transpose((2, 1, 0, 3))
         dims = part_transpose.shape
         part_transpose = part_transpose.reshape((dims[0] * dims[1], dims[0] * dims[1]))
-        if xp == cp:
+        if part_transpose.device in ["gpu"]:
             sqrt = False
-            print("")
 
         # depending on a chosen method, perform corresponding calculation
         if sqrt:
-            neg = scla.sqrtm(np.matmul(part_transpose, part_transpose.conj().T))
-            neg = np.trace(neg)
-            neg = np.real(0.5 * (neg - 1))
+            tmp = part_transpose.tensordot(part_transpose.conj(), ([1], [1]))
+            neg = tmp.sqrtm()
+            neg = neg.trace(return_real_part=True, do_get=True)
+            neg = 0.5 * (neg - 1)
         else:
-            eig_vals = xp.linalg.eigvalsh(part_transpose)
-            neg = 0.5 * np.sum(abs(eig_vals) - eig_vals)
-        if xp == cp:
-            neg = neg.get()
+            absval, summe = part_transpose.get_attr("abs", "sum")
+            eig_vals = part_transpose.eigvalsh()
+            neg = summe(absval(eig_vals) - eig_vals)
+            neg = part_transpose.get_of(neg)
+            neg *= 0.5
 
         return neg
 
     def entropy(self, prob=None, local_dim=2, eps=1e-10):
         """
         This function calculates Von Neumann entropy of
         a TTO mixed state density matrix.
@@ -561,33 +557,37 @@
             warn(
                 "Concurrence can be computed only for TTO"
                 " with gauge center at the uppermost tensor."
                 f" Shifting a gauge center from {self.iso_center}"
                 " to [0,0]."
             )
             self.shift_gauge_center([0, 0])
-        xp = self._device_checks()
 
-        root_dm = xp.tensordot(self[0][0], self[0][0].conj(), axes=[[2], [2]])
+        root_dm = self[0][0].tensordot(self[0][0].conj(), [[2], [2]])
 
         root_dm = root_dm.reshape(
             (root_dm.shape[0] * root_dm.shape[1], root_dm.shape[2] * root_dm.shape[3]),
         )
 
-        if xp == cp:
-            neg = neg.get()
-        rho_sqrt = scla.sqrtm(root_dm)
+        rho_sqrt = root_dm.sqrtm()
 
-        sigma_y_mat = np.array(
-            [[0, 0, 0, -1], [0, 0, 1, 0], [0, 1, 0, 0], [-1, 0, 0, 0]]
-        )
-        rho_tilde = np.matmul(sigma_y_mat, np.matmul(np.conj(root_dm), sigma_y_mat))
+        sigma_y_mat = rho_sqrt.zeros_like(root_dm)
+        sigma_y_mat.set_matrix_entry(0, 3, -1)
+        sigma_y_mat.set_matrix_entry(1, 2, 1)
+        sigma_y_mat.set_matrix_entry(2, 1, 1)
+        sigma_y_mat.set_matrix_entry(3, 0, -1)
+
+        rho_tilde = sigma_y_mat @ root_dm.conj() @ sigma_y_mat
+        conc_mat = rho_sqrt @ rho_tilde @ rho_sqrt
+
+        conc_mat = conc_mat.sqrtm()
+
+        # Move to host
+        conc_mat = conc_mat.get().to_dense()
 
-        conc_mat = np.matmul(rho_sqrt, np.matmul(rho_tilde, rho_sqrt))
-        conc_mat = scla.sqrtm(conc_mat)
         val, _ = np.linalg.eig(conc_mat)
         val = np.sort(val)[::-1]
         conc = abs(2 * val[0] - np.sum(val))
         conc = max([0, conc])
 
         return conc
 
@@ -777,16 +777,15 @@
         # Case with given unitary
 
         # compute EoF for the specific density matrix decomposition defined
         # with unitary
         eof = func_target(init_guess, unitary=unitary)
         return eof
 
-    @staticmethod
-    def tree(matrix_in, tto, conv_params):
+    def tree(self, matrix_in, conv_params):
         """
         Transforms a given matrix into a tensor network as below:
 
         .. code-block::
 
                     |
             |       O
@@ -796,63 +795,62 @@
 
         the first index of a matrix corresponds to the lower
         leg of the input tensor
 
         Parameters
         ----------
 
-        matrix_in : ndarray
-            Matrix to be transformed.
-
-        tto : :py:class:`TTO`
+        self : :py:class:`TTO`
             Initialized TTO for which the tree method is used.
             From it, the local dimension and convergence parameters
             for SVD are extracted.
 
+        matrix_in : ndarray
+            Matrix to be transformed.
+
         conv_params : [TNConvergenceParameters]
             Input for handling convergence parameters.
 
         Returns
         -------
 
         tens_left, tens_mid, tens_right : ndarray
             Tensors of the second TN on the picture above,
             read from left to right.
             --> order of indices:
                 tens_left, tens_right - [lower, upper]
                 tens_mid - [lower left, upper, lower right]
         """
-        dim = tto.local_dim
+        dim = self.local_dim
         if len(set(list(dim))) != 1:
             raise Exception("Different local dimensions not yet supported for TTO.")
 
         dim = dim[0]
         num_sites2 = int(mt.log(matrix_in.shape[0], dim) / 2)
 
         matrix_in = matrix_in.reshape(
             (int(dim**num_sites2), int(dim**num_sites2), matrix_in.shape[1]),
         )
-        tens_left, tens_mid, _, _ = TTO.tSVD(
-            tto, matrix_in, [0], [2, 1], contract_singvals="R", conv_params=conv_params
+        tens_left, tens_mid, _, _ = matrix_in.split_svd(
+            [0], [2, 1], contract_singvals="R", conv_params=conv_params
         )
-        tens_mid, tens_right, _, _ = TTO.tSVD(
-            tto,
-            tens_mid,
+
+        tens_mid, tens_right, _, _ = tens_mid.split_svd(
             [0, 1],
             [2],
             perm_left=[0, 2, 1],
             perm_right=[1, 0],
             contract_singvals="L",
             conv_params=conv_params,
         )
 
         return tens_left, tens_mid, tens_right
 
     @classmethod
-    def dm_to_tto(cls, num_sites, dim, psi, prob, conv_params):
+    def dm_to_tto(cls, num_sites, dim, psi, prob, conv_params, tensor_backend=None):
         """
         Computes the TTO form of a given density matrix
 
         Parameters
         ----------
         num_sites : int
             Number of sites
@@ -873,67 +871,76 @@
             in particular, we are interested in:
             - the maximum bond dimension (max_bond_dimension)
             - the cut ratio (cut_ratio) after which the singular
             values in SVD are neglected, all singular values
             such that lambda/lambda_max <= eps
             are truncated
 
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
         Return
         ------
         rho_tt : :py:class:`TTO`
             TTO form of the density matrix
         """
         if dim < 2:
             raise ValueError("Local dimension must be at least 2")
-        """
-        First construct the density matrix so that it is split in two parts,
-        sqrt(pj)|psi_j> and sqrt(pj)<psi_j|
-        Take the first part and work with it, the rest will be the complex
-        conjugate
-        """
+
+        # Initialize the TTO
+        rho_tt = cls(
+            num_sites,
+            local_dim=dim,
+            conv_params=conv_params,
+            tensor_backend=tensor_backend,
+        )
+        tensor_cls = rho_tt._tensor_backend.tensor_cls
+
+        # First construct the density matrix so that it is split in two parts,
+        # sqrt(pj)|psi_j> and sqrt(pj)<psi_j|
+        # Take the first part and work with it, the rest will be the complex
+        # conjugate
+
         psi = np.sqrt(prob) * psi
         if len(psi.shape) == 1:
             psi = psi.reshape((len(psi), 1))  # =O-
 
-        """
-        Initialize the TTO
-        """
-        rho_tt = cls(num_sites, local_dim=dim, conv_params=conv_params)
-        """
-        Start growing branches layer by layer, starting from the uppermost
-        tensor towards below (check what TTO.tree function does)
-        tree2 wil be the tensor in TTO layer and tree1,tree3 are used to
-        grow lower branches
-        """
+        psi = tensor_cls.from_elem_array(psi)
+
+        # Start growing branches layer by layer, starting from the uppermost
+        # tensor towards below (check what TTO.tree function does)
+        # tree2 wil be the tensor in TTO layer and tree1,tree3 are used to
+        # grow lower branches
         mid = [deepcopy(psi)]
         for ii in range(0, rho_tt.num_layers - 1):  # iterate to get all the layers
             mid_t = deepcopy(mid)
             mid = []
             lay = []
             for tensor in mid_t:
-                tree1, tree2, tree3 = TTO.tree(tensor, rho_tt, conv_params=conv_params)
+                tree1, tree2, tree3 = rho_tt.tree(tensor, conv_params=conv_params)
                 mid.append(tree1)
                 mid.append(tree3)
                 lay.append(tree2)
             rho_tt[ii] = TTNLayer.from_tensorlist(lay, dim)
 
         lay = []
-        """
-        Reshape the lowest layer tensors to get the shape we need
-        """
+
+        # Reshape the lowest layer tensors to get the shape we need
         for tensor in mid:
             tensor = np.reshape(tensor, (dim, dim, tensor.shape[1]))
             lay.append(tensor)
         rho_tt[-1] = TTNLayer.from_tensorlist(lay)
         rho_tt.iso_center = [0, 0]
 
+        rho_tt.convert(rho_tt._tensor_backend.dtype, rho_tt._tensor_backend.device)
+
         return rho_tt
 
     @classmethod
-    def lptn_to_tto(cls, tensor_list, conv_params):
+    def lptn_to_tto(cls, tensor_list, conv_params, tensor_backend):
         """
         Transforms the density matrix from LPTN to TTO form
 
         Parameters
         ----------
         tensor_list : list
             Tensors in LPTN, LPTN.tensors
@@ -943,42 +950,49 @@
             in particular, we are interested in:
             - the maximum bond dimension (max_bond_dimension)
             - the cut ratio (cut_ratio) after which the singular
             values in SVD are neglected, all singular values
             such that lambda/lambda_max <= eps
             are truncated
 
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
+
         Return
         ------
         tto : :py:class:`TTO`
             TTO form of the input LPTN
         """
 
         num_sites = len(tensor_list)
         dim = tensor_list[0].shape[1]
 
-        tto = cls(num_sites, local_dim=dim, conv_params=conv_params)
+        tto = cls(
+            num_sites,
+            local_dim=dim,
+            conv_params=conv_params,
+            tensor_backend=tensor_backend,
+        )
 
         for ii in range(tto.num_layers - 1, 0, -1):
             work = tensor_list
             tensor_list = []
             for jj in range(0, len(work), 2):
                 # First combine and merge tensors from the tensor_list
                 # (initially LPTN tensors) into pairs
-                work2 = np.tensordot(work[jj], work[jj + 1], [[3], [0]])
-                work2 = np.transpose(work2, axes=[1, 3, 0, 2, 4, 5])
+                work2 = work[jj].tensordot(work[jj + 1], [[3], [0]])
+                work2 = work2.transpose([1, 3, 0, 2, 4, 5])
 
                 #                 ||
                 # SVD decompose  --O--  into l_mat,r_mat so that lower legs
                 #                 ||   go to l_mat and the rest goes to r_mat
 
                 # we do the SVD decomposition, truncate the
                 # singular values and contract them into r_mat
-                l_mat, r_mat, _, _ = tto.tSVD(
-                    work2,
+                l_mat, r_mat, _, _ = work2.split_svd(
                     [0, 1],
                     [2, 3, 4, 5],
                     contract_singvals="R",
                     conv_params=conv_params,
                 )
 
                 # --> l_mat will be one of the tensors in TTO layer
@@ -987,16 +1001,15 @@
                 #                                  ||
                 # Now SVD decompose r_mat matrix --O-- so that lower and side legs
                 #                                  |
                 # go to tens_down and upper legs go to tens_up
                 # tens_down is contracted with singular values, ignore tens_up because
                 # it is unitary and it cancels out with the
                 # complex conjugate from the upper part of the TN
-                tens_down, _, _, _ = tto.tSVD(
-                    r_mat,
+                tens_down, _, _, _ = r_mat.split_svd(
                     [1, 0, 4],
                     [2, 3],
                     perm_left=[0, 1, 3, 2],
                     contract_singvals="L",
                     conv_params=conv_params,
                 )
 
@@ -1006,38 +1019,38 @@
 
                 # The whole procedure will be repeated with the new
                 # lptn-like list stored in tensor_list.
 
         # For the uppermost tensor we do not need to do all of the above.
         # Contract the two remaining tensors from tensor_list and reshape
         # them to get the shape we need.
-        work2 = np.tensordot(tensor_list[0], tensor_list[1], axes=[[3], [0]])
-        work2 = np.transpose(work2, axes=[0, 1, 2, 4, 3, 5])
-        work2 = np.reshape(
-            work2, (work2.shape[1], work2.shape[2] * work2.shape[3], work2.shape[4])
+        work2 = tensor_list[0].tensordot(tensor_list[1], [[3], [0]])
+        work2 = work2.transpose([0, 1, 2, 4, 3, 5])
+        work2.reshape_update(
+            (work2.shape[1], work2.shape[2] * work2.shape[3], work2.shape[4])
         )
 
         # To truncate the probabilities, SVD the tensor so that lower and
         # side legs + singular values go to work2.
         # Ignore the other tensor because it is unitary and cancels out with the
         # complex conjugate from the upper part of the TTO.
 
         # Remark: the multiplication with 100 in tto.tSVD is because the SVD algorithm
         # otherwise has a problem with convergence. The result is later divided with
         # 100 to restore the original value.
-        work2, _, _, _ = tto.tSVD(
-            work2,
+        work2, _, _, _ = work2.split_svd(
             [0, 2],
             [1],
             contract_singvals="L",
             conv_params=conv_params,
         )
         tto[0][0] = deepcopy(work2)
         tto.iso_center = [0, 0]
 
+        tto.convert(tto._tensor_backend.dtype, tto._tensor_backend.device)
         return tto
 
     @classmethod
     def lptn_to_tto_iso(cls, tensor_list, conv_params, k_0=None, norm=False):
         """
         Transforms the density matrix from LPTN to TTO form,
         keeping the TN isometrized throughout the procedure.
@@ -1109,27 +1122,26 @@
 
             work = deepcopy(lptn_work.tensors)
             tensor_list = []
 
             for jj in range(0, len(work), 2):
                 # combine and merge tensors from the tensor_list
                 # (initially LPTN tensors) into pairs
-                work2 = np.tensordot(work[jj], work[jj + 1], [[3], [0]])
-                work2 = np.transpose(work2, axes=[1, 3, 0, 2, 4, 5])
+                work2 = work[jj].tensordot(work[jj + 1], [[3], [0]])
+                work2 = work2.transpose([1, 3, 0, 2, 4, 5])
 
                 #                 ||
                 # SVD decompose  --O--  into l_mat,r_mat so that lower legs
                 #                 ||   go to l_mat and the rest goes to r_mat
 
                 # we do the SVD decomposition, truncate the
                 # singular values and contract them into r_mat
                 # Remark: work2 matrix is divided by 100 to solve some SVD convergence issue,
                 # this is taken into account later so that the results remain the same.
-                l_mat, r_mat, _, track = tto.tSVD(
-                    work2,
+                l_mat, r_mat, _, track = work2.split_svd(
                     [0, 1],
                     [2, 3, 4, 5],
                     contract_singvals="R",
                     conv_params=conv_params,
                 )
 
                 # track the norm loss
@@ -1142,50 +1154,42 @@
                 # Now SVD decompose r_mat matrix --O-- so that lower and side legs
                 #                                  |
 
                 # go to tens_down and upper legs go to tens_up
                 # tens_down is contracted with singular values, ignore tens_up because
                 # it is unitary and it cancels out with the
                 # complex conjugate from the upper part of the TN
-                tens_down, _, _, _ = tto.tSVD(
-                    r_mat,
+                tens_down, _, _, _ = r_mat.split_svd(
                     [1, 0, 4],
                     [2, 3],
                     perm_left=[0, 1, 3, 2],
                     contract_singvals="L",
                     conv_params=conv_params,
                 )
 
                 # track the norm loss
                 norm_track = norm_track * (1 - np.sum(track**2))
 
                 # QR decompose tens_down so that the tens_down becomes unitary, and contract
                 # the R matrix with the next left tensor in order to shift the isometry center
-                shape = deepcopy(tens_down.shape)
-                tens_down = np.reshape(
-                    tens_down, (shape[0] * shape[1] * shape[2], shape[3])
-                )
-                tens_down, r_mat = nla.qr(tens_down)
-                tens_down = np.reshape(
-                    tens_down, (shape[0], shape[1], shape[2], tens_down.shape[1])
-                )
+                tens_down, r_mat = tens_down.split_qr([0, 1, 2], [3])
                 if jj != (len(work) - 2):
-                    work[jj + 2] = np.tensordot(r_mat, work[jj + 2], axes=[[1], [0]])
+                    work[jj + 2] = r_mat.tensordot(work[jj + 2], [[1], [0]])
 
                 # Now append tens_down to the new tensor_list and repeat the same
                 # procedure in next iteration over ii to get the upper layers
                 tensor_list.append(deepcopy(tens_down))
 
                 # The whole procedure will be repeated with the new
                 # lptn-like list stored in tensor_list.
 
         # For the uppermost tensor we do not need to do all of the above.
         # Contract the two remaining tensors from tensor_list and reshape
         # them to get the shape we need.
-        work2 = np.tensordot(tensor_list[0], tensor_list[1], axes=[[3], [0]])
+        work2 = tensor_list[0].tensordot(tensor_list[1], [[3], [0]])
         work2 = np.transpose(work2, axes=[0, 1, 2, 4, 3, 5])
         work2 = np.reshape(
             work2, (work2.shape[1], work2.shape[2] * work2.shape[3], work2.shape[4])
         )
 
         # To truncate the probabilities, SVD the tensor so that lower and
         # side legs + singular values go to work2.
@@ -1193,16 +1197,15 @@
         # complex conjugate from the upper part of the TTO.
 
         # Remark: the multiplication with 100 in tto.tSVD is because the SVD algorithm
         # otherwise has a problem with convergence. The result is later divided with
         # 100 to restore the original value.
         # conv_params.cut_ratio = np.sqrt(conv_params.cut_ratio)
         conv_params2 = TNConvergenceParameters(max_bond_dimension=k_0, cut_ratio=1e-8)
-        work2, _, _, track = tto.tSVD(
-            work2,
+        work2, _, _, track = work2.split_svd(
             [0, 2],
             [1],
             contract_singvals="L",
             conv_params=conv_params2,
         )
         # track the norm loss
         norm_track = norm_track * (1 - np.sum(track**2))
@@ -1234,38 +1237,48 @@
     #########################################################################
 
     #########################################################################
     ######################### Measurement methods ###########################
     #########################################################################
 
     @classmethod
-    def from_statevector(cls, statevector, device="cpu"):
+    def from_statevector(
+        cls, statevector, local_dim=2, conv_params=None, tensor_backend=None
+    ):
         """
         Initialize the TTO by decomposing a statevector into TTO form.
 
         We use the dm_to_tto function isntead of mapping the statevector to
         TTN and the TTN to TTO since in this way we avoid the problems arising
         from the different structures of the top layer.
 
         Parameters
         ----------
 
         statevector : ndarray of shape( [local_dim]*num_sites, )
             Statevector describing the interested state for initializing the TTN
 
-        device : str, optional
-            Device where the computation is done. Either "cpu" or "gpu".
+        tensor_backend : `None` or instance of :class:`TensorBackend`
+            Default for `None` is :class:`QteaTensor` with np.complex128 on CPU.
         """
         num_sites = len(statevector.shape)
-        local_dim = statevector.shape[0]
-        conv_params = None
+
+        if local_dim != statevector.shape[0]:
+            raise Exception("Mismatch local dimension (passed and one in array).")
+
         tto = cls.dm_to_tto(
-            num_sites, local_dim, statevector.reshape(-1), 1, conv_params
+            num_sites,
+            local_dim,
+            statevector.reshape(-1),
+            1,
+            conv_params,
+            tensor_backend=tensor_backend,
         )
-        tto.to_device(device)
+
+        tto.convert(tto._tensor_backend.dtype, tto._tensor_backend.device)
 
         return cls
 
     #########################################################################
     ######### Methods not well defined for TTOs inherited from TTN ##########
     #########################################################################
     def dot(self, other):
@@ -1289,19 +1302,19 @@
     def write(self, filename, cmplx=True):
         """
         Not implemented
         """
         raise NotImplementedError("write product not implemented for TTOs")
 
     @classmethod
-    def read(cls, filename, cmplx=True, order="F"):
+    def read(cls, filename, tensor_backend, cmplx=True, order="F"):
         """
         Not implemented
         """
         raise NotImplementedError("read product not implemented for TTOs")
 
     @classmethod
-    def read_v0_2_29(cls, filename, cmplx=True, order="F"):
+    def read_v0_2_29(cls, filename, tensor_backend, cmplx=True, order="F"):
         """
         Not implemented
         """
         raise NotImplementedError("read product not implemented for TTOs")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/fortran_interfaces.py` & `qtealeaves-1.1.1/qtealeaves/tooling/fortran_interfaces.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/hilbert_curvature.py` & `qtealeaves-1.1.1/qtealeaves/tooling/hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/lattice_layout.py` & `qtealeaves-1.1.1/qtealeaves/tooling/lattice_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 """
 The lattice layout helps us to support models beyond square lattices
 with - to some extent - arbitrary positions in space.
 """
 import numpy as np
 
+__all__ = ["LatticeLayout"]
+
 
 class LatticeLayout:
     """
     The LatticeLayout class stores the positions of the (num_x)x(num_y) grid
     which allows for non-square 2D lattices.
 
     **Arguments**
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/__init__.py` & `qtealeaves-1.1.1/qtealeaves/modeling/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,41 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Modeling submodule init.
+Modeling submodule qtealeaves.modeling init.
 """
 
 from . import (
     baseterm,
     localterm,
     twobodyterm1d,
     twobodyterm2d,
     twobodyterm3d,
     plaquetteterm2d,
-    quantummodel,
-    tensorproductoperator,
     blockterm2d,
     stringterm1d,
+    quantummodel,
 )
 
 # All modules have an __all__ defined
 from .baseterm import *
 from .localterm import *
 from .twobodyterm1d import *
 from .twobodyterm2d import *
 from .twobodyterm3d import *
 from .plaquetteterm2d import *
-from .quantummodel import *
-from .tensorproductoperator import *
 from .blockterm2d import *
 from .stringterm1d import *
+from .quantummodel import *
 
 __all__ = quantummodel.__all__.copy()
 __all__ += localterm.__all__.copy()
 __all__ += twobodyterm1d.__all__.copy()
 __all__ += twobodyterm2d.__all__.copy()
 __all__ += twobodyterm3d.__all__.copy()
 __all__ += plaquetteterm2d.__all__.copy()
-__all__ += tensorproductoperator.__all__.copy()
 __all__ += blockterm2d.__all__.copy()
 __all__ += stringterm1d.__all__.copy()
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/baseterm.py` & `qtealeaves-1.1.1/qtealeaves/modeling/baseterm.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,28 +9,33 @@
 # that they have been altered from the originals.
 
 """
 Abstract base class for a term in the model.
 """
 from warnings import warn
 
-from qtealeaves.parameterized import _ParameterizedClass
+from qtealeaves.tooling import _ParameterizedClass
 
 
 __all__ = ["_ModelTerm", "_ModelTerm1D"]
 
 
 class _ModelTerm(_ParameterizedClass):
     """
     Abstract base class for any term in a model.
     """
 
     strength = 1
     prefactor = 1
 
+    @property
+    def is_oqs(self):
+        """Status flag if term belongs to Hamiltonian or is Lindblad."""
+        return False
+
     @staticmethod
     def check_dim(dim):
         """
         By default, do not restrict dimensionality. Overwriting
         this methods, allows to restrict terms to 1d, 2d, or
         3d systems.
 
@@ -144,14 +149,30 @@
                 # adding offset 1
                 str_repr += "%d %d\n" % (elem[1][1] + 1, op_id_str_1)
                 str_repr += "%d %d\n" % (elem[1][0] + 1, op_id_str_0)
 
             str_repr += param_repr + " %30.15E\n" % (self.prefactor)
         return str_repr
 
+    # pylint: disable-next=unused-argument
+    def quantum_jump_weight(self, state, operators, quench, time, params):
+        """Evaluate the unnormalized weight for a jump with this Lindblad term."""
+        if self.is_oqs:
+            raise NotImplementedError("Must be overwritten for Lindblad.")
+
+        raise ValueError("Trying to evaluate quantum jump on Hamiltonian term.")
+
+    # pylint: disable-next=unused-argument
+    def quantum_jump_apply(self, state, operators, params, rand_generator):
+        """Apply jump with this Lindblad."""
+        if self.is_oqs:
+            raise NotImplementedError("Must be overwritten for Lindblad.")
+
+        raise ValueError("Trying to evaluate quantum jump on Hamiltonian term.")
+
 
 class _ModelTerm1D(_ModelTerm):
     """
     Abstract base class for any term in a 1D model.
     """
 
     @staticmethod
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/blockterm2d.py` & `qtealeaves-1.1.1/qtealeaves/modeling/blockterm2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         Default to ``None`` (all sites have the interaction)
 
 
     The order of the operators is for the shifts (0,0), (0,1), (1,0), (1,1)
     """
 
     def __init__(self, operators, strength=1, prefactor=1, has_obc=True, mask=None):
+        super().__init__()
+
         self.op_shape = operators.shape
         self.operators = operators.flatten()
         self.strength = strength
         self.prefactor = prefactor
 
         if isinstance(mask, np.ndarray):
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/localterm.py` & `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm1d.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,255 +5,190 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Local terms in a Hamiltonian or Lindblad equation.
+Two-body interactions in one-dimensional systems.
 """
-from copy import deepcopy
 import numpy as np
 
-from qtealeaves import map_selector
-from .baseterm import _ModelTerm
-from .sparsematrixoperator import SparseMatrixOperator
+from .baseterm import _ModelTerm1D
 
 
-__all__ = ["LocalTerm", "LindbladTerm", "RandomizedLocalTerm"]
+__all__ = ["TwoBodyTerm1D", "TwoBodyAllToAllTerm1D"]
 
 
-class LocalTerm(_ModelTerm):
+class TwoBodyTerm1D(_ModelTerm1D):
     """
-    Local Hamiltonian terms are versatile and probably part of any model
-    which will be implemented. For example, the external field in the
-    quantum Ising model can be represented as a local term.
+    The term defines an interaction between two sites of the Hilbert space.
+    For example, the tunneling term in the Bose-Hubbard model can be
+    represented by this term. This class represents the 1d version.
 
     **Arguments**
 
-    operator : str
-        String identifier for the operator. Before launching the simulation,
+    operators : list of two strings
+        String identifier for the operators. Before launching the simulation,
         the python API will check that the operator is defined.
 
+    shift : int
+        Defines the distance of the interaction in compliance
+        with the systems in higher dimensions. In the end,
+        we iterate over all sites and apply interactions to
+        sites (x,) and (x + shift,)
+
     strength : str, callable, numeric (optional)
         Defines the coupling strength of the local terms. It can
         be parameterized via a value in the dictionary for the
         simulation or a function.
         Default to 1.
 
     prefactor : numeric, scalar (optional)
         Scalar prefactor, e.g., in order to take into account signs etc.
         Default to 1.
 
+    add_complex_conjg : bool, optional
+        (BUG ticket #1) Aims to automatically add complex conjugated
+        terms, e.g., for the tunneling term.
+
+    has_obc : bool or list of bools, optional
+        Defines the boundary condition along each spatial dimension.
+        If scalar is given, the boundary condition along each
+        spatial dimension is assumed to be equal.
+        Default to True
+
     mask : callable or ``None``, optional
-        The true-false-mask allows to apply the local Hamiltonians
+        The true-false-mask allows to apply the Hamiltonians terms
         only to specific sites, i.e., with true values. The function
         takes the dictionary with the simulation parameters as an
-        argument.
-        Default to ``None`` (all sites have a local term)
-
-    **Attributes**
+        argument. The mask is applied to the site where the left
+        operator is acting on.
+        Default to ``None`` (all sites have the interaction)
 
-    map_type : str, optional
-        Selecting the mapping from a n-dimensional system to the
-        1d system required for the TTN simulations.
     """
 
-    def __init__(self, operator, strength=1, prefactor=1, mask=None):
-        self.operator = operator
+    def __init__(
+        self,
+        operators,
+        shift,
+        strength=1,
+        prefactor=1,
+        add_complex_conjg=False,
+        has_obc=True,
+        mask=None,
+    ):
+        super().__init__()
+
+        self.operators = operators
+        self.shift = shift
         self.strength = strength
         self.prefactor = prefactor
+        self.add_complex_conjg = add_complex_conjg
         self.mask = mask
 
-        # Will be set when adding Hamiltonian terms
-        self.map_type = None
+        if isinstance(has_obc, bool):
+            self.has_obc = [has_obc]
+        else:
+            self.has_obc = has_obc
 
-    def count(self, params):
+    def iter_shifts(self):
         """
-        Defines length as number of terms in fortran input file,
-        which by now depends the presence of a mask.
-
-        **Arguments**
-
-        params : dictionary
-            Contains the simulation parameters.
+        Return all possible shifts, which is in the case of the
+        1d systems exactly the defined shift.
         """
-        if self.mask is None:
-            return 1
-
-        return np.sum(self.mask(params))
+        yield self.shift
 
     def get_entries(self, params):
         """
-        Return the operator and the strength of this term.
+        Entries based on two coordinates; one of them is the
+        origin (0,).
 
         **Arguments**
 
         params : dictionary
             Contains the simulation parameters.
-        """
-        strength = self.eval_strength(params)
 
-        return self.operator, strength
+        **Details**
 
-    def collect_operators(self):
+        To-Do: complex-conjugate terms are wrong, i.e., they work
+        for sigma_{i}^{+} sigma_{j}^{-} or b_{i}^{dagger} b_{j}, but
+        not for terms as b_{j} sigma_{i}^{x}!
         """
-        The required operators must be provided through this
-        method; thus, we return the operator in the local term.
-        """
-        yield self.operator, None
+        for shift in self.iter_shifts():
+            coord_a = 0
+            coord_b = shift
+            coordinates = [coord_a, coord_b]
 
-    def get_fortran_str(self, ll, params, operator_map, param_map, dim):
-        """
-        Get the string representation needed to write the
-        local terms as an plocal_type for Fortran.
+            coupl_ii = {"coordinates": coordinates, "operators": self.operators}
 
-        **Arguments**
+            yield coupl_ii
 
-        ll : int
-            Number of sites along the dimensions, i.e., not the
-            total number of sites. Assuming list of sites
-            along all dimension.
+            if self.add_complex_conjg:
+                coupl_ii = {
+                    "coordinates": coordinates,
+                    "operators": self.operators[::-1],
+                }
 
-        params : dictionary
-            Contains the simulation parameters.
-
-        operator_map : OrderedDict
-            For operator string as dictionary keys, it returns the
-            corresponding integer IDs.
-
-        param_map : dict
-            This dictionary contains the mapping from the parameters
-            to integer identifiers.
-
-        dim : int
-            Dimensionality of the problem, e.g., a 2d system.
-        """
-        str_repr = ""
-        op_id_str = str(operator_map[(self.operator, None)])
-
-        has_spatial_dependency = False
-        param_repr = self.get_param_repr(param_map)
-
-        if self.mask is not None:
-            for _, idx in self.get_interactions(ll, params, dim=dim):
-                # Convert from python index to fortran index by
-                # adding offset 1
-                str_repr += "%d\n" % (idx[0] + 1)
-                str_repr += op_id_str + "\n"
-                str_repr += param_repr
-                str_repr += "%30.15E\n" % (self.prefactor)
-
-        elif has_spatial_dependency:
-            # Write for each site
-            raise NotImplementedError("To-do ...")
-        else:
-            str_repr += "-1\n"
-            str_repr += op_id_str + "\n"
-            str_repr += param_repr
-            str_repr += "%30.15E\n" % (self.prefactor)
-
-        return str_repr
+                yield coupl_ii
 
     def get_interactions(self, ll, params, **kwargs):
         """
-        Iterator returning the local terms one-by-one, e.g., to build
-        a Hamiltonian matrix. (In that sense, the "interaction" is
-        obviously misleading here.)
-
-        **Arguments**
-
-        ll : int
-            Number of sites along the dimension, i.e., not the
-            total number of sites. Assuming list of sites
-            along all dimension.
-
-        params : dictionary
-            Contains the simulation parameters.
-
-        dim : int (as keyword argument!)
-            Dimensionality of the problem, e.g., a 2d system.
+        Iterate over all interaction. The iterator yields
+        a dictionary with the operator keys and the generic
+        shift based on the origin, and a list with the
+        coordinates in the 1d system.
         """
-        if "dim" not in kwargs:
-            raise Exception("Local terms needs dim information")
-        dim = kwargs["dim"]
+        if self.mask is None:
+            local_mask = np.ones(ll, dtype=bool)
+        else:
+            local_mask = self.mask(params)
 
-        elem = {"coordinates": None, "operators": [self.operator]}
+        for elem in self.get_entries(params):
+            for ix in self.iterate_sites(ll):
+                coord_a, coord_b = elem["coordinates"]
 
-        if self.mask is None:
+                if np.sum(np.abs(np.array(coord_a))) != 0:
+                    raise Exception("Coordinate A is not the origin.")
 
-            def check_mask(*args):
-                return True
+                jx = ix + coord_b
 
-        else:
-            local_mask = self.mask(params)
-            if len(local_mask.shape) != dim:
-                raise Exception("Mask dimension does not match system dimension.")
+                if (jx >= ll[0]) and self.has_obc[0]:
+                    continue
 
-            def check_mask(*args, local_mask=local_mask):
-                if len(args) == 1:
-                    return local_mask[args[0]]
-                if len(args) == 2:
-                    return local_mask[args[0], args[1]]
-                if len(args) == 3:
-                    return local_mask[args[0], args[1], args[2]]
-
-                raise Exception("Unknown length of *args.")
-
-        if dim > 1:
-            map_to_1d = map_selector(dim, ll, self.map_type)
-
-        if dim == 1:
-            for ii in range(ll[0]):
-                if not check_mask(ii):
+                if (jx < 0) and self.has_obc[0]:
                     continue
 
-                elem_ii = deepcopy(elem)
-                elem_ii["coordinates_nd"] = (ii,)
+                if jx >= ll[0]:
+                    jx = jx % ll[0]
+                if jx < 0:
+                    jx += ll[0]
 
-                yield elem_ii, [ii]
-        elif dim == 2:
-            idx = 0
-            for ii in range(ll[0]):
-                for jj in range(ll[1]):
-                    idx += 1
-
-                    if not check_mask(ii, jj):
-                        continue
-
-                    elem_ii = deepcopy(elem)
-                    elem_ii["coordinates_nd"] = (ii, jj)
-
-                    yield elem_ii, [map_to_1d[(ii, jj)]]
-        elif dim == 3:
-            idx = 0
-            for ii in range(ll[0]):
-                for jj in range(ll[1]):
-                    for kk in range(ll[2]):
-                        idx += 1
+                if (jx >= ll[0]) or (jx < 0):
+                    raise Exception("Improve handling.")
 
-                        if not check_mask(ii, jj, kk):
-                            continue
+                if ix == jx:
+                    raise Exception("Same site ...")
 
-                        elem_ii = deepcopy(elem)
-                        elem_ii["coordinates_nd"] = (ii, jj, kk)
+                if not local_mask[ix]:
+                    continue
 
-                        yield elem_ii, [map_to_1d[(ii, jj, kk)]]
-        else:
-            raise Exception("Dimension unknown.")
+                # Still in python indices
+                coords_1d = [ix, jx]
 
-        return
+                yield elem, coords_1d
 
-    @property
-    def is_oqs(self):
-        """Status flag if term belongs to Hamiltonian or is Lindblad."""
-        return False
+    def get_fortran_str(self, ll, params, operator_map, param_map):
+        """
+        See :func:`_ModelTerm.get_fortran_str_two_body`.
+        """
+        return self.get_fortran_str_twobody(ll, params, operator_map, param_map)
 
     def get_sparse_matrix_operators(
-        self, ll, params, operator_map, param_map, **kwargs
+        self, ll, params, operator_map, param_map, sp_ops_cls, **kwargs
     ):
         """
         Construct the sparse matrix operator for this term.
 
         **Arguments**
 
         ll : int
@@ -266,164 +201,200 @@
             For operator string as dictionary keys, it returns the
             corresponding integer IDs.
 
         param_map : dict
             This dictionary contains the mapping from the parameters
             to integer identifiers.
 
+        sp_ops_cls : callable (e.g., constructor)
+            Constructor for the sparse MPO operator to be built
+            Has input bool (is_first_site), bool (is_last_site),
+            bool (do_vectors).
+
         kwargs : keyword arguments
             Keyword arguments are passed to `get_interactions`
         """
-        op_id = operator_map[(self.operator, None)]
-        param_id = self.get_param_repr(param_map)
+        if self.shift != 1:
+            raise NotImplementedError(
+                "Only nearest neighbor implemented for sparse MPO."
+            )
 
         sp_mat_ops = []
         for ii in range(np.prod(ll)):
-            sp_mat_ops.append(
-                SparseMatrixOperator(ii == 0, ii + 1 == np.prod(ll), True)
-            )
+            sp_mat_ops.append(sp_ops_cls(ii == 0, ii + 1 == np.prod(ll), True))
 
-        for _, inds in self.get_interactions(ll, params, **kwargs):
-            sp_mat_ops[inds[0]].add_local(op_id, param_id, self.prefactor, self.is_oqs)
+        op_id_0 = operator_map[(self.operators[0], "l")]
+        op_id_1 = operator_map[(self.operators[1], "r")]
 
-        return sp_mat_ops
-
-
-class LindbladTerm(LocalTerm):
-    """
-    Local Lindblad operators acting at one site are defined via this
-    term. For the arguments see See :class:`LocalTerm.check_dim`.
-
-    **Details**
-
-    The Lindblad equation is implemented as
+        param_repr = self.get_param_repr(param_map)
 
-    .. math::
+        for _, inds in self.get_interactions(ll, params, **kwargs):
+            if abs(inds[0] - inds[1]) == np.prod(ll) - 1:
+                raise Exception(
+                    "Periodic boundary conditions not implemented for spMat."
+                )
 
-        \\frac{d}{dt} \\rho = -i [H, \\rho]
-           + \\sum \\gamma (L \\rho L^{\\dagger}
-           - \\frac{1}{2} \\{ L^{\\dagger} L, \\rho \\})
+            if inds[0] == 0:
+                shape_l = (1, 3)
+            else:
+                shape_l = (2, 3)
+
+            if inds[1] + 1 == np.product(ll):
+                shape_r = (3, 1)
+            else:
+                shape_r = (3, 2)
+
+            sp_mat_l = np.zeros(shape_l, dtype=int)
+            sp_mat_r = np.zeros(shape_r, dtype=int)
+
+            prefactor_l = np.zeros(shape_l, dtype=np.complex128)
+            prefactor_r = np.zeros(shape_r, dtype=np.complex128)
+
+            params_l = np.zeros(shape_l, dtype=int)
+            params_r = np.zeros(shape_r, dtype=int)
+
+            sp_mat_l[-1, 1] = op_id_0
+            prefactor_l[-1, 1] = self.prefactor
+            params_l[-1, 1] = param_repr
+
+            sp_mat_r[1, 0] = op_id_1
+            prefactor_r[1, 0] = 1.0
+            params_r[1, 0] = -1
 
-    """
+            sp_mat_ops[inds[0]].add_term(sp_mat_l, params_l, prefactor_l)
+            sp_mat_ops[inds[1]].add_term(sp_mat_r, params_r, prefactor_r)
 
-    @property
-    def is_oqs(self):
-        """Status flag if term belongs to Hamiltonian or is Lindblad."""
-        return True
+        return sp_mat_ops
 
 
-class RandomizedLocalTerm(LocalTerm):
+class TwoBodyAllToAllTerm1D(TwoBodyTerm1D):
     """
-    Randomized local Hamiltonian terms are useful to model spinglass systems
-    where the coupling of the local term is different for each site.
+    Random all-to-all two-body interaction for a one-dimensional system,
+    e.g., as in spin glasses.
 
     **Arguments**
 
-    operator : string
+    operators : list of two strings
         String identifier for the operators. Before launching the simulation,
         the python API will check that the operator is defined.
 
-    coupling_entries : numpy ndarray of rank-1,2,3
-        The coupling for the different sites.
-        These values can only be set once and cannot
-        be time-dependent in a time-evolution. The rank depends
-        on the usage in 1d, 2d, or 3d systems.
+    coupling_matrix : numpy ndarray of rank-2
+        The coupling between the different sites in the all-to-all
+        interactions. These values can only be set once and cannot
+        be time-dependent in a time-evolution.
 
     strength : str, callable, numeric (optional)
         Defines the coupling strength of the local terms. It can
         be parameterized via a value in the dictionary for the
         simulation or a function.
         Default to 1.
 
     prefactor : numeric, scalar (optional)
         Scalar prefactor, e.g., in order to take into account signs etc.
         Default to 1.
-    """
 
-    mask = None
+    **Details**
 
-    def __init__(self, operator, coupling_entries, strength=1, prefactor=1):
-        super().__init__(operator=operator, strength=strength, prefactor=prefactor)
-        self.coupling_entries = coupling_entries
+    The term adds the following terms:
+    ``sum_{i} sum_{j>i} strength * prefactor * coupling_mat[i, j] * A_i * B_j``
+    and only the upper triangular matrix of the coupling_mat is accessed.
+    The hermiticity of the Hamiltonian is not ensured. Terms of the form
+    ``B_j A_i`` with ``j < i`` are also not added.
+    """
 
-    def count(self, params):
-        """
-        Defines length as number of terms in fortran input file,
-        which by now depends the presence of the coupling entries.
+    add_complex_conjg = False
 
-        **Arguments**
-
-        params : dictionary
-            Contains the simulation parameters.
-        """
-        ctens = self.eval_numeric_param(self.coupling_entries, params)
-        return np.sum(np.abs(ctens) != 0)
+    def __init__(self, operators, coupling_matrix, strength=1, prefactor=1):
+        super().__init__(
+            operators=operators, shift=None, strength=strength, prefactor=prefactor
+        )
+        self.coupling_matrix = coupling_matrix
 
     def get_interactions(self, ll, params, **kwargs):
-        """
-        See :class:`LocalTerm`
-        """
-        ctens = self.eval_numeric_param(self.coupling_entries, params)
+        cmat = self.eval_numeric_param(self.coupling_matrix, params)
 
-        for elem, coords_1d in super().get_interactions(ll, params, **kwargs):
-            elem["weight"] = ctens[elem["coordinates_nd"]]
+        for ii in range(ll[0]):
+            for jj in range(ii + 1, ll[0]):
+                if abs(cmat[ii, jj]) == 0.0:
+                    # Coupling will always be zero
+                    continue
 
-            if elem["weight"] == 0.0:
-                continue
+                coords_1d = [ii, jj]
 
-            yield elem, coords_1d
+                yield {"operators": self.operators, "weight": cmat[ii, jj]}, coords_1d
 
-    def get_fortran_str(self, ll, params, operator_map, param_map, dim):
+    def get_fortran_str(self, ll, params, operator_map, param_map):
         """
-        Get the string representation needed to write the
-        local terms as an plocal_type for Fortran.
+        Get the string representation needed to write
+        for Fortran. This method works for any two-body interaction.
 
         **Arguments**
 
         ll : int
-            Number of sites along one dimension, i.e., not the
-            total number of sites. Assuming equal number of sites
-            along all dimension.
+            Number of sites along one dimension in the system, e.g.,
+            number of sites for one side of the square in a 2d system.
 
         params : dictionary
             Contains the simulation parameters.
 
         operator_map : OrderedDict
             For operator string as dictionary keys, it returns the
             corresponding integer IDs.
 
         param_map : dict
             This dictionary contains the mapping from the parameters
             to integer identifiers.
 
-        dim : int
-            Dimensionality of the problem, e.g., a 2d system.
+        **Details**
+
+        We cannot use the function :func:`_ModelTerm.get_fortran_str_two_body`
+        as we have to modify the prefactor.
         """
         str_repr = ""
-        op_id_str = str(operator_map[(self.operator, None)])
-
         param_repr = self.get_param_repr(param_map)
 
-        ctens = self.eval_numeric_param(self.coupling_entries, params)
-        if isinstance(ctens, np.ndarray):
-            if len(ctens.shape) != dim:
-                raise Exception(
-                    "Coupling %d and " % (len(ctens.shape))
-                    + "dimensionality %d do not match." % (dim)
-                )
+        cmat = self.eval_numeric_param(self.coupling_matrix, params)
+        if isinstance(cmat, np.ndarray):
+            if len(cmat.shape) != 2:
+                raise Exception("Coupling must be a matrix.")
         else:
             raise Exception("Unknown type for coupling.")
 
-        for meta_info, idx in self.get_interactions(ll, params, dim=dim):
-            if abs(ctens[meta_info["coordinates_nd"]]) == 0.0:
-                # Skip entries with 0 coupling from randomization
-                continue
-
-            # Convert from python index to fortran index by
-            # adding offset 1
-            str_repr += "%d\n" % (idx[0] + 1)
-            str_repr += op_id_str + "\n"
-            str_repr += param_repr
-            prefactor = self.prefactor * ctens[meta_info["coordinates_nd"]]
-            str_repr += "%30.15E\n" % (prefactor)
+        str_repr = ""
+        counter = 0
+        for elem in self.get_interactions(ll, params):
+            if elem[1][0] == elem[1][1]:
+                raise Exception("Same site ...")
+
+            ii = elem[1][0]
+            jj = elem[1][1]
+
+            # Increment counter for non-zero term (get_interactions
+            # takes care of that)
+            counter += 1
+
+            # Ensure order is increasing (if ever enabled in get_interactions)
+            if ii < jj:
+                op_id_str_0 = operator_map[(self.operators[0], "l")]
+                op_id_str_1 = operator_map[(self.operators[1], "r")]
+
+                # Convert from python index to fortran index by
+                # adding offset 1
+                str_repr += "%d %d\n" % (ii + 1, op_id_str_0)
+                str_repr += "%d %d\n" % (jj + 1, op_id_str_1)
+            else:
+                op_id_str_0 = operator_map[(self.operators[0], "r")]
+                op_id_str_1 = operator_map[(self.operators[1], "l")]
+
+                # Convert from python index to fortran index by
+                # adding offset 1
+                str_repr += "%d %d\n" % (jj + 1, op_id_str_1)
+                str_repr += "%d %d\n" % (ii + 1, op_id_str_0)
+
+            prefactor = self.prefactor * cmat[ii, jj]
+            str_repr += param_repr + " %30.15E\n" % (prefactor)
+
+        # Insert at the beginning: number of terms and number
+        # of operators (later always 2)
+        str_repr = "%d\n%d\n" % (counter, 2) + str_repr
 
         return str_repr
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/plaquetteterm2d.py` & `qtealeaves-1.1.1/qtealeaves/modeling/plaquetteterm2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         Default to ``None`` (all sites have the interaction)
 
 
     The order of the operators is for the shifts (0,0), (0,1), (1,0), (1,1)
     """
 
     def __init__(self, operators, strength=1, prefactor=1, has_obc=True, mask=None):
+        super().__init__()
+
         self.operators = operators
         self.strength = strength
         self.prefactor = prefactor
         self.mask = mask
 
         # Will be set when adding Hamiltonian terms
         self.map_type = None
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/quantummodel.py` & `qtealeaves-1.1.1/qtealeaves/modeling/quantummodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 The organization of modeling a physical system in 1, 2, or 3 spatial dimensions.
 """
 import os
+
+# pylint: disable-next=no-name-in-module
 import os.path
 from collections import OrderedDict
 import numpy as np
 import scipy.sparse as sp
 
-from qtealeaves.parameterized import _ParameterizedClass
+from qtealeaves.tooling import _ParameterizedClass
 
 from .baseterm import _ModelTerm
 from .localterm import LocalTerm, LindbladTerm
-from .sparsematrixproductoperator import SparseMatrixProductOperator
 
 __all__ = ["QuantumModel"]
 
 
 class QuantumModel(_ParameterizedClass):
     """
     The class represents a physical model, e.g., how to build the
@@ -94,14 +95,19 @@
 
         term : instance of :class:`_ModelTerm`
             Represents the additional term in the model.
         """
         self.add_hterm(new_term)
         return self
 
+    def __iter__(self):
+        """Iterate over the terms in the model."""
+        for elem in self.hterms:
+            yield elem
+
     def collect_operators(self):
         """
         The required operators must be provided through this
         method. It relies on the same method of each
         :class:`_ModelTerm`.
         """
         op_lst = []
@@ -271,15 +277,14 @@
         local_dim = ops.get_operator("id", params).shape[0]
         ham_matrix = xp.csr_matrix((local_dim**nsites, local_dim**nsites))
 
         for elem in self.hterms:
             for subelem, coords_1d in elem.get_interactions(
                 lx_ly_lz, params, dim=self.dim
             ):
-
                 hsite_list = []
                 is_eye = [True] * nsites
                 for _ in range(nsites):
                     hsite_list.append(xp.eye(local_dim))
 
                 for ii, op_str in enumerate(subelem["operators"]):
                     op_mat = ops.get_operator(op_str, params)
@@ -327,14 +332,121 @@
                 tmp *= total_scaling
 
                 # Cannot use += when requiring type cast from real to complex
                 ham_matrix = ham_matrix + tmp
 
         return ham_matrix
 
+    def apply_ham_to_state(self, state, ops, params):
+        """
+        Apply the Hamiltonian to a state by contracting all
+        operators to it, without constructing the matrix.
+
+        **Arguments**
+
+        state : instance of :class:`StateVector` or `numpy.ndarray`
+            The input state.
+
+        ops : instance of :class:`TNOperators`
+            The operators consisting the Hamiltonian.
+
+        params : dict
+            The parameter dictionary for the simulation.
+        """
+        lx_ly_lz = self.eval_lvals(params)
+        nsites = int(np.prod(np.array(lx_ly_lz)))
+
+        local_dim = ops.get_operator("id", params).shape[0]
+
+        # get the vector from the StateVector object
+        if hasattr(state, state):
+            if isinstance(state.state, np.ndarray):
+                psi = state.state
+                original_shape = psi.shape
+            else:
+                raise Exception(
+                    f"""The object state has an attribute state.state,
+                    but it is not a numpy array but type {type(state.state)}."""
+                )
+        elif isinstance(state, np.ndarray):
+            psi = state
+            original_shape = psi.shape
+            # if not a N-legged tensor but 1D vector, reshape into N-legged.
+            if original_shape != [local_dim] * nsites:
+                if original_shape == (local_dim**nsites,):
+                    psi.reshape([local_dim] * nsites)
+                else:
+                    raise Exception(
+                        f"""The shape of the input file must be 1D: {local_dim**nsites}
+                        or N-legged tensor: {[local_dim]*nsites}, but is {original_shape}."""
+                    )
+        else:
+            raise Exception(
+                f"Input state has to be either numpy array or StateVector type, is {type(state)}."
+            )
+
+        # the array to add the H|psi> terms into
+        final_psi = np.zeros(shape=psi.shape, dtype=psi.dtype)
+        # iterate over all terms in H
+        for elem in self.hterms:
+            for subelem, coords_1d in elem.get_interactions(
+                lx_ly_lz, params, dim=self.dim
+            ):
+                # total_scaling is the prefactor of the operators in this subelem
+
+                total_scaling = elem.prefactor * elem.eval_strength(params)
+                if "weight" in subelem:
+                    total_scaling *= subelem["weight"]
+
+                # op_psi will be the state with the op applied. Initialize as the initial psi.
+                op_psi = np.copy(psi)
+                # iterate over all operators in the term
+                for ii, op_str in enumerate(subelem["operators"]):
+                    # get the operator matrix representation and multiply by its prefactor
+                    # (assumes total_scaling is scalar)
+                    op_mat = ops.get_operator(op_str, params)
+                    op_mat = op_mat * total_scaling
+                    # now set total_scaling to 1,
+                    # as only the first operator has to be multiplied by it
+                    total_scaling = 1
+
+                    # coords_1d indices are as well python and start at 0
+                    xpos = coords_1d[ii]
+
+                    # apply the op to the state
+                    # tensordot can be understood as contracting the two tensors
+                    # by the legs given in axes
+                    op_psi = np.tensordot(op_mat, op_psi, axes=(1, xpos))
+
+                    # however, this pushes the resulting leg to first place,
+                    # and it has to be permuted back.
+                    # This is achieved by transposing the result accoring to the
+                    # permutation rule.
+                    # There is space for improvement here:
+                    # Instead of transposing every time, keep track of the permutations
+                    # in a separate list and only permute once at the end.
+
+                    perm = (
+                        list(range(1, xpos + 1)) + [0] + list(range(xpos + 1, nsites))
+                    )
+                    op_psi = np.transpose(op_psi, perm)
+
+                # add the current ops into the final state
+                final_psi += op_psi
+
+        # finally reshape psi into a 1D array
+        final_psi = np.reshape(final_psi, original_shape)
+
+        if hasattr(state, state):
+            # update the state
+            setattr(state, "state", final_psi)
+            return state
+
+        return final_psi
+
     def density_matrix(
         self, ops, params, temp, return_vec=False, k_b=1, eps_p=1e-8, max_prob=None
     ):
         """
         Diagonalize a Hamiltonian and compute its density matrix at
         finite temperature.
 
@@ -437,14 +549,15 @@
 
         idx : int, optional
             The parameterization file allows to be indexed to
             support multiple files.
             Default to 0.
         """
         parameterization_file = "parameterization_%03d.dat" % (idx)
+        # pylint: disable-next=no-member
         full_file = os.path.join(folder_name_input, parameterization_file)
         str_buffer = ""
         is_real = True
 
         # Number of parameters
         str_buffer += str(len(self.coupl_params)) + "\n"
 
@@ -688,15 +801,15 @@
         coupl_str = self.get_coupl_str(elem, params, strength=strength)
 
         with open(filename, "w+") as fh:
             fh.write(coupl_str)
 
         return
 
-    def write_input(self, folder_name_input, params, operator_map, mpo_mode):
+    def write_input(self, folder_name_input, params, operator_map, mpo_mode, spo_cls):
         """
         Third generation of input file writing for parameterized
         models. The function returns the full path to the top-level
         file for the model.
 
         **Arguments**
 
@@ -715,20 +828,27 @@
             simulation.
             Choosing the MPO representation inside the simulation, where
             the value -1 enables an auto-selection.
             The other values are TPO via iTPO (0), iTPO (1), iTPO with
             update (2, for quenches), iTPO with compression (3), and sparse
             MPO (10, partially enabled), indexed sparse MPO (11, partially enabled)
             Default to -1.
+
+        spo_cls : constructor for the sparse MPO to be built for MPO mode 10, 11
         """
         parameterization_file = self.parameterization_write(folder_name_input, params)
         sparse_mpo_file = self.write_sparse_mpo(
-            folder_name_input, params, operator_map, self.coupl_params, mpo_mode
+            folder_name_input,
+            params,
+            operator_map,
+            self.coupl_params,
+            mpo_mode,
+            spo_cls,
         )
-
+        # pylint: disable-next=no-member
         full_input_file = os.path.join(folder_name_input, self.input_file)
 
         with open(full_input_file, "w+") as fh:
             fh.write(parameterization_file + "\n")
             fh.write(sparse_mpo_file + "\n")
 
             local_term = []
@@ -793,15 +913,15 @@
 
             fh.write("%d\n" % (counter))
             fh.write(tmp_str)
 
         return full_input_file
 
     def write_sparse_mpo(
-        self, folder_name_input, params, operator_map, param_map, mpo_mode
+        self, folder_name_input, params, operator_map, param_map, mpo_mode, spo_cls
     ):
         """
         Write the sparse MPO to a file for a fortran simulation.
 
         **Arguments**
 
         folder_name_input : str
@@ -822,18 +942,20 @@
             simulation.
             Choosing the MPO representation inside the simulation, where
             the value -1 enables an auto-selection.
             The other values are TPO via iTPO (0), iTPO (1), iTPO with
             update (2, for quenches), iTPO with compression (3), and sparse
             MPO (10, partially enabled), indexed sparse MPO (11, partially enabled)
             Default to -1.
+
+        spo_cls : constructor for the sparse MPO to be built for MPO mode 10, 11
         """
         if self.eval_numeric_param(mpo_mode, params) not in [10, 11]:
             return "---"
-
+        # pylint: disable-next=no-member
         sp_mpo_file = os.path.join(folder_name_input, "sp_mpo.dat")
-        spmatprodop = SparseMatrixProductOperator(params, self, operator_map, param_map)
+        spmatprodop = spo_cls(params, self, operator_map, param_map)
 
         with open(sp_mpo_file, "w+") as fh:
             spmatprodop.write(fh)
 
         return "sp_mpo.dat"
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/stringterm1d.py` & `qtealeaves-1.1.1/qtealeaves/modeling/stringterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm1d.py` & `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm2d.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,109 +5,193 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Two-body interactions in one-dimensional systems.
+Two-body interactions in a two-dimensional system.
 """
 import numpy as np
 
-from .baseterm import _ModelTerm1D
-from .sparsematrixoperator import SparseMatrixOperator
+from qtealeaves import map_selector
+from .baseterm import _ModelTerm
 
 
-__all__ = ["TwoBodyTerm1D", "TwoBodyAllToAllTerm1D"]
+__all__ = ["TwoBodyTerm2D", "TwoBodyTerm2DLatticeLayout"]
 
 
-class TwoBodyTerm1D(_ModelTerm1D):
+class TwoBodyTerm2D(_ModelTerm):
     """
     The term defines an interaction between two sites of the Hilbert space.
     For example, the tunneling term in the Bose-Hubbard model can be
-    represented by this term. This class represents the 1d version.
+    represented by this term. This class represents the 2d version.
 
     **Arguments**
 
     operators : list of two strings
         String identifier for the operators. Before launching the simulation,
         the python API will check that the operator is defined.
 
-    shift : int
-        Defines the distance of the interaction in compliance
-        with the systems in higher dimensions. In the end,
+    shift : list of two ints
+        Defines the distance of the interaction. In the end,
         we iterate over all sites and apply interactions to
-        sites (x,) and (x + shift,)
+        sites (x, y) and (x + shift[0], y + shift[1])
 
     strength : str, callable, numeric (optional)
         Defines the coupling strength of the local terms. It can
         be parameterized via a value in the dictionary for the
         simulation or a function.
         Default to 1.
 
     prefactor : numeric, scalar (optional)
         Scalar prefactor, e.g., in order to take into account signs etc.
         Default to 1.
 
+    isotropy_xyz : bool, optional
+        If False, the defined shift will only be applied as is. If true,
+        we permute the defined shift to cover all spatial directions.
+        Default to True.
+
     add_complex_conjg : bool, optional
         (BUG ticket #1) Aims to automatically add complex conjugated
         terms, e.g., for the tunneling term.
 
     has_obc : bool or list of bools, optional
         Defines the boundary condition along each spatial dimension.
         If scalar is given, the boundary condition along each
         spatial dimension is assumed to be equal.
         Default to True
+
+    mask : callable or ``None``, optional
+        The true-false-mask allows to apply the Hamiltonians terms
+        only to specific sites, i.e., with true values. The function
+        takes the dictionary with the simulation parameters as an
+        argument. The mask is applied to the site where the left
+        operator is acting on.
+        Default to ``None`` (all sites have the interaction)
+
+    **Attributes**
+
+    map_type : str, optional
+        Selecting the mapping from a n-dimensional system to the
+        1d system required for the TTN simulations.
     """
 
     def __init__(
         self,
         operators,
         shift,
         strength=1,
         prefactor=1,
+        isotropy_xyz=True,
         add_complex_conjg=False,
         has_obc=True,
+        mask=None,
     ):
+        super().__init__()
+
         self.operators = operators
         self.shift = shift
         self.strength = strength
         self.prefactor = prefactor
+        self.isotropy_xyz = isotropy_xyz
         self.add_complex_conjg = add_complex_conjg
+        self.mask = mask
+
+        # Will be set when adding Hamiltonian terms
+        self.map_type = None
 
         if isinstance(has_obc, bool):
-            self.has_obc = [has_obc]
+            self.has_obc = [has_obc] * 2
         else:
             self.has_obc = has_obc
 
+    @staticmethod
+    def check_dim(dim):
+        """
+        See :func:`_ModelTerm.check_dim`
+        """
+        if dim != 2:
+            raise Exception("Dimension does not match.")
+
+    @staticmethod
+    def iterate_sites(ll):
+        """
+        **Argument**
+
+        ll : Sequence of 2 ints
+            Number of sites along each side of the lattice.
+        """
+        for ii in range(ll[0]):
+            for jj in range(ll[1]):
+                yield ii, jj
+
+    def collect_operators(self):
+        """
+        All the required operators are returned to ensure that they are
+        written by fortran.
+        """
+        yield self.operators[0], "l"
+        yield self.operators[1], "r"
+
+        # Hilbert curvature could swap order of sites
+        yield self.operators[0], "r"
+        yield self.operators[1], "l"
+
     def iter_shifts(self):
         """
-        Return all possible shifts, which is in the case of the
-        1d systems exactly the defined shift.
+        Return all possible shifts, which depends on the isotropy
+        in the 2d case.
         """
-        yield self.shift
+        if self.isotropy_xyz:
+            n_coord = np.sum(np.abs(np.array(self.shift)) > 0)
+            if n_coord == 0:
+                raise Exception("Not implemented. Is this case useful?")
+            if n_coord == 1:
+                shifts = [
+                    [self.shift[0], self.shift[1]],
+                    [self.shift[1], self.shift[0]],
+                ]
+            elif n_coord == 2:
+                shifts = [
+                    [self.shift[0], self.shift[1]],
+                    [self.shift[0], -self.shift[1]],
+                ]
+
+                # This takes into account unequal shifts leading
+                # to four terms, e.g, (1, 2), (1, -2), (2, 1),
+                # and (2, -1)
+                if self.shift[0] != self.shift[1]:
+                    shifts.append([self.shift[1], self.shift[0]])
+                    shifts.append([self.shift[1], -self.shift[0]])
+        else:
+            shifts = [self.shift]
+
+        for elem in shifts:
+            yield elem
 
     def get_entries(self, params):
         """
-        Entries based on two coordinates; one of them is the
-        origin (0,).
+        Entries combine the information about possible shifts based
+        on the origin coordination (0, 0) and the shift with the
+        information about the operators and couplings.
 
         **Arguments**
 
         params : dictionary
             Contains the simulation parameters.
 
         **Details**
 
-        To-Do: complex-conjugate terms are wrong, i.e., they work
-        for sigma_{i}^{+} sigma_{j}^{-} or b_{i}^{dagger} b_{j}, but
-        not for terms as b_{j} sigma_{i}^{x}!
+        To-Do: adding complex conjugates for general case beyond
+        b bdagger case.
         """
         for shift in self.iter_shifts():
-            coord_a = 0
+            coord_a = [0, 0]
             coord_b = shift
             coordinates = [coord_a, coord_b]
 
             coupl_ii = {"coordinates": coordinates, "operators": self.operators}
 
             yield coupl_ii
 
@@ -117,261 +201,197 @@
                     "operators": self.operators[::-1],
                 }
 
                 yield coupl_ii
 
     def get_interactions(self, ll, params, **kwargs):
         """
-        Iterate over all interaction. The iterator yields
-        a dictionary with the operator keys and the generic
-        shift based on the origin, and a list with the
-        coordinates in the 1d system.
+        These interactions are closest to the TPO description iterating
+        over specific sites within the 1d coordinates.
+
+        **Arguments**
+
+        ll : list of ints
+            Number of sites along the dimensions, i.e., not the
+            total number of sites. Assuming list of sites
+            along all dimension.
+
+        params : dictionary
+            Contains the simulation parameters.
         """
+        map_type = self.eval_str_param(self.map_type, params)
+        map_to_1d = map_selector(2, ll, map_type)
+
+        if self.mask is None:
+            local_mask = np.ones(ll, dtype=bool)
+        else:
+            local_mask = self.mask(params)
+
         for elem in self.get_entries(params):
-            for ix in self.iterate_sites(ll):
+            for ix, iy in self.iterate_sites(ll):
                 coord_a, coord_b = elem["coordinates"]
 
                 if np.sum(np.abs(np.array(coord_a))) != 0:
                     raise Exception("Coordinate A is not the origin.")
 
-                jx = ix + coord_b
+                jx = ix + coord_b[0]
+                jy = iy + coord_b[1]
 
                 if (jx >= ll[0]) and self.has_obc[0]:
                     continue
-
                 if (jx < 0) and self.has_obc[0]:
                     continue
 
+                if (jy >= ll[1]) and self.has_obc[1]:
+                    continue
+                if (jy < 0) and self.has_obc[1]:
+                    continue
+
                 if jx >= ll[0]:
                     jx = jx % ll[0]
                 if jx < 0:
                     jx += ll[0]
 
+                if jy >= ll[1]:
+                    jy = jy % ll[1]
+                if jy < 0:
+                    jy += ll[1]
+
                 if (jx >= ll[0]) or (jx < 0):
                     raise Exception("Improve handling.")
+                if (jy >= ll[1]) or (jy < 0):
+                    raise Exception("Improve handling.")
 
-                if ix == jx:
+                if (ix == jx) and (iy == jy):
                     raise Exception("Same site ...")
 
-                # Still in python indices
-                coords_1d = [ix, jx]
+                if not local_mask[ix, iy]:
+                    continue
+
+                # Convert from python to Hilbert space index starting from 1
+                coords_1d = [map_to_1d[elem] for elem in [(ix, iy), (jx, jy)]]
 
                 yield elem, coords_1d
 
     def get_fortran_str(self, ll, params, operator_map, param_map):
         """
         See :func:`_ModelTerm.get_fortran_str_two_body`.
         """
         return self.get_fortran_str_twobody(ll, params, operator_map, param_map)
 
-    def get_sparse_matrix_operators(
-        self, ll, params, operator_map, param_map, **kwargs
-    ):
-        """
-        Construct the sparse matrix operator for this term.
-
-        **Arguments**
-
-        ll : int
-            System size.
-
-        params : dictionary
-            Contains the simulation parameters.
-
-        operator_map : OrderedDict
-            For operator string as dictionary keys, it returns the
-            corresponding integer IDs.
 
-        param_map : dict
-            This dictionary contains the mapping from the parameters
-            to integer identifiers.
-
-        kwargs : keyword arguments
-            Keyword arguments are passed to `get_interactions`
-        """
-        if self.shift != 1:
-            raise NotImplementedError(
-                "Only nearest neighbor implemented for sparse MPO."
-            )
-
-        sp_mat_ops = []
-        for ii in range(np.prod(ll)):
-            sp_mat_ops.append(
-                SparseMatrixOperator(ii == 0, ii + 1 == np.prod(ll), True)
-            )
-
-        op_id_0 = operator_map[(self.operators[0], "l")]
-        op_id_1 = operator_map[(self.operators[1], "r")]
-
-        param_repr = self.get_param_repr(param_map)
-
-        for _, inds in self.get_interactions(ll, params, **kwargs):
-            if abs(inds[0] - inds[1]) == np.prod(ll) - 1:
-                raise Exception(
-                    "Periodic boundary conditions not implemented for spMat."
-                )
-
-            if inds[0] == 0:
-                shape_l = (1, 3)
-            else:
-                shape_l = (2, 3)
-
-            if inds[1] + 1 == np.product(ll):
-                shape_r = (3, 1)
-            else:
-                shape_r = (3, 2)
-
-            sp_mat_l = np.zeros(shape_l, dtype=int)
-            sp_mat_r = np.zeros(shape_r, dtype=int)
-
-            prefactor_l = np.zeros(shape_l, dtype=np.complex128)
-            prefactor_r = np.zeros(shape_r, dtype=np.complex128)
-
-            params_l = np.zeros(shape_l, dtype=int)
-            params_r = np.zeros(shape_r, dtype=int)
-
-            sp_mat_l[-1, 1] = op_id_0
-            prefactor_l[-1, 1] = self.prefactor
-            params_l[-1, 1] = param_repr
-
-            sp_mat_r[1, 0] = op_id_1
-            prefactor_r[1, 0] = 1.0
-            params_r[1, 0] = -1
-
-            sp_mat_ops[inds[0]].add_term(sp_mat_l, params_l, prefactor_l)
-            sp_mat_ops[inds[1]].add_term(sp_mat_r, params_r, prefactor_r)
-
-        return sp_mat_ops
-
-
-class TwoBodyAllToAllTerm1D(TwoBodyTerm1D):
+class TwoBodyTerm2DLatticeLayout(TwoBodyTerm2D):
     """
-    Random all-to-all two-body interaction for a one-dimensional system,
-    e.g., as in spin glasses.
+    The term defines an interaction between two sites of the Hilbert space,
+    for an arbitrary lattice layout. For example, the tunneling term in the
+    Bose-Hubbard model can be represented by this term. This class represents
+    the 2d version.
 
     **Arguments**
 
     operators : list of two strings
         String identifier for the operators. Before launching the simulation,
         the python API will check that the operator is defined.
 
-    coupling_matrix : numpy ndarray of rank-2
-        The coupling between the different sites in the all-to-all
-        interactions. These values can only be set once and cannot
-        be time-dependent in a time-evolution.
+    distance : float
+        Defines the distance of the interaction.
+
+    layout : :class:`LatticeLayout`, str, callable
+        Instance of the :class:`LatticeLayout`. The `LatticeLayout` class stores
+        the positions of the (nx)x(ny) grid for an arbitrary lattice layout.
 
     strength : str, callable, numeric (optional)
         Defines the coupling strength of the local terms. It can
         be parameterized via a value in the dictionary for the
         simulation or a function.
         Default to 1.
 
     prefactor : numeric, scalar (optional)
         Scalar prefactor, e.g., in order to take into account signs etc.
         Default to 1.
 
-    **Details**
-
-    The term adds the following terms:
-    ``sum_{i} sum_{j>i} strength * prefactor * coupling_mat[i, j] * A_i * B_j``
-    and only the upper triangular matrix of the coupling_mat is accessed.
-    The hermiticity of the Hamiltonian is not ensured. Terms of the form
-    ``B_j A_i`` with ``j < i`` are also not added.
+    tolerance : float, optional
+        Tolerance for the distance of the interaction,
+        i.e., the absolute distance must be smaller than the tolerance
+        to consider the sites interacting.
+
+    **Attributes**
+
+    map_type : str, optional
+        Selecting the mapping from a n-dimensional system to the
+        1d system required for the TTN simulations.
     """
 
-    add_complex_conjg = False
-
-    def __init__(self, operators, coupling_matrix, strength=1, prefactor=1):
-        super().__init__(
-            operators=operators, shift=None, strength=strength, prefactor=prefactor
-        )
-        self.coupling_matrix = coupling_matrix
-
-    def get_interactions(self, ll, params, **kwargs):
-        cmat = self.eval_numeric_param(self.coupling_matrix, params)
+    def __init__(
+        self, operators, distance, layout, strength=1, prefactor=1, tolerance=1e-8
+    ):
+        super().__init__(operators, 1, strength=strength, prefactor=prefactor)
+        self.distance = distance
+        self.tolerance = tolerance
+        self.layout = layout
+
+        # Delete unused terms
+        del self.shift
+        del self.isotropy_xyz
+        del self.add_complex_conjg
+        del self.mask
+        del self.has_obc
 
-        for ii in range(ll[0]):
-            for jj in range(ii + 1, ll[0]):
-                if abs(cmat[ii, jj]) == 0.0:
-                    # Coupling will always be zero
-                    continue
+        # Will be set when adding Hamiltonian terms
+        self.map_type = None
 
-                coords_1d = [ii, jj]
+    def iter_shifts(self):
+        """
+        The function is inherited, but we overwrite it since it
+        has no meaning in this context.
+        """
+        raise Exception("This function is not available.")
 
-                yield {"operators": self.operators, "weight": cmat[ii, jj]}, coords_1d
+    def get_entries(self, params):
+        """
+        The function is inherited, but we overwrite it since it
+        has no meaning in this context.
+        """
+        raise Exception("This function is not available.")
 
-    def get_fortran_str(self, ll, params, operator_map, param_map):
+    def get_interactions(self, ll, params, **kwargs):
         """
-        Get the string representation needed to write
-        for Fortran. This method works for any two-body interaction.
+        These interactions are closest to the TPO description iterating
+        over specific sites within the 1d coordinates.
 
         **Arguments**
 
         ll : int
-            Number of sites along one dimension in the system, e.g.,
-            number of sites for one side of the square in a 2d system.
+            Number of sites along the dimensions, i.e., not the
+            total number of sites. Assuming equal number of sites
+            along all dimension.
 
         params : dictionary
             Contains the simulation parameters.
-
-        operator_map : OrderedDict
-            For operator string as dictionary keys, it returns the
-            corresponding integer IDs.
-
-        param_map : dict
-            This dictionary contains the mapping from the parameters
-            to integer identifiers.
-
-        **Details**
-
-        We cannot use the function :func:`_ModelTerm.get_fortran_str_two_body`
-        as we have to modify the prefactor.
         """
-        str_repr = ""
-        param_repr = self.get_param_repr(param_map)
+        map_to_1d = map_selector(2, ll, self.map_type)
 
-        cmat = self.eval_numeric_param(self.coupling_matrix, params)
-        if isinstance(cmat, np.ndarray):
-            if len(cmat.shape) != 2:
-                raise Exception("Coupling must be a matrix.")
-        else:
-            raise Exception("Unknown type for coupling.")
+        layout = self.eval_numeric_param(self.layout, params)
+
+        for ix, iy in self.iterate_sites(ll):
+            coord_ix, coord_iy = layout.positions[ix, iy, :]
 
-        str_repr = ""
-        counter = 0
-        for elem in self.get_interactions(ll, params):
-            if elem[1][0] == elem[1][1]:
-                raise Exception("Same site ...")
-
-            ii = elem[1][0]
-            jj = elem[1][1]
-
-            # Increment counter for non-zero term (get_interactions
-            # takes care of that)
-            counter += 1
-
-            # Ensure order is increasing (if ever enabled in get_interactions)
-            if ii < jj:
-                op_id_str_0 = operator_map[(self.operators[0], "l")]
-                op_id_str_1 = operator_map[(self.operators[1], "r")]
-
-                # Convert from python index to fortran index by
-                # adding offset 1
-                str_repr += "%d %d\n" % (ii + 1, op_id_str_0)
-                str_repr += "%d %d\n" % (jj + 1, op_id_str_1)
-            else:
-                op_id_str_0 = operator_map[(self.operators[0], "r")]
-                op_id_str_1 = operator_map[(self.operators[1], "l")]
-
-                # Convert from python index to fortran index by
-                # adding offset 1
-                str_repr += "%d %d\n" % (jj + 1, op_id_str_1)
-                str_repr += "%d %d\n" % (ii + 1, op_id_str_0)
-
-            prefactor = self.prefactor * cmat[ii, jj]
-            str_repr += param_repr + " %30.15E\n" % (prefactor)
-
-        # Insert at the beginning: number of terms and number
-        # of operators (later always 2)
-        str_repr = "%d\n%d\n" % (counter, 2) + str_repr
+            for jx, jy in self.iterate_sites(ll):
+                coord_jx, coord_jy = layout.positions[jx, jy, :]
+                dist = layout.distance((coord_ix, coord_iy), (coord_jx, coord_jy))
+
+                coords_1d_i = map_to_1d[(ix, iy)]
+                coords_1d_j = map_to_1d[(jx, jy)]
+
+                if coords_1d_i < coords_1d_j:
+                    if np.abs(dist - self.distance) <= self.tolerance:
+                        coupl_ij = {
+                            "coordinates": [(ix, iy), (jx, jy)],
+                            "operators": self.operators,
+                        }
+                        yield coupl_ij, (coords_1d_i, coords_1d_j)
 
-        return str_repr
+    def get_fortran_str(self, ll, params, operator_map, param_map):
+        """
+        See :func:`_ModelTerm.get_fortran_str_two_body`.
+        """
+        return self.get_fortran_str_twobody(ll, params, operator_map, param_map)
```

### Comparing `qtealeaves-0.5.14/qtealeaves/modeling/twobodyterm2d.py` & `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm3d.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,41 +5,47 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
-Two-body interactions in a two-dimensional system.
+Two-body interactions in a three-dimensional system.
 """
+
+# pylint: disable=too-many-locals
+# pylint: disable=too-many-branches
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
+
 import numpy as np
 
 from qtealeaves import map_selector
 from .baseterm import _ModelTerm
 
 
-__all__ = ["TwoBodyTerm2D", "TwoBodyTerm2DLatticeLayout"]
+__all__ = ["TwoBodyTerm3D"]
 
 
-class TwoBodyTerm2D(_ModelTerm):
+class TwoBodyTerm3D(_ModelTerm):
     """
     The term defines an interaction between two sites of the Hilbert space.
     For example, the tunneling term in the Bose-Hubbard model can be
     represented by this term. This class represents the 2d version.
 
     **Arguments**
 
     operators : list of two strings
         String identifier for the operators. Before launching the simulation,
         the python API will check that the operator is defined.
 
-    shift : list of two ints
+    shift : list of three ints
         Defines the distance of the interaction. In the end,
         we iterate over all sites and apply interactions to
-        sites (x, y) and (x + shift[0], y + shift[1])
+        sites (x, y, z) and (x + shift[0], y + shift[1], z + shift[2])
 
     strength : str, callable, numeric (optional)
         Defines the coupling strength of the local terms. It can
         be parameterized via a value in the dictionary for the
         simulation or a function.
         Default to 1.
 
@@ -58,22 +64,14 @@
 
     has_obc : bool or list of bools, optional
         Defines the boundary condition along each spatial dimension.
         If scalar is given, the boundary condition along each
         spatial dimension is assumed to be equal.
         Default to True
 
-    mask : callable or ``None``, optional
-        The true-false-mask allows to apply the Hamiltonians terms
-        only to specific sites, i.e., with true values. The function
-        takes the dictionary with the simulation parameters as an
-        argument. The mask is applied to the site where the left
-        operator is acting on.
-        Default to ``None`` (all sites have the interaction)
-
     **Attributes**
 
     map_type : str, optional
         Selecting the mapping from a n-dimensional system to the
         1d system required for the TTN simulations.
     """
 
@@ -82,313 +80,238 @@
         operators,
         shift,
         strength=1,
         prefactor=1,
         isotropy_xyz=True,
         add_complex_conjg=False,
         has_obc=True,
-        mask=None,
     ):
+        super().__init__()
+
         self.operators = operators
         self.shift = shift
         self.strength = strength
         self.prefactor = prefactor
         self.isotropy_xyz = isotropy_xyz
         self.add_complex_conjg = add_complex_conjg
-        self.mask = mask
 
         # Will be set when adding Hamiltonian terms
         self.map_type = None
 
         if isinstance(has_obc, bool):
-            self.has_obc = [has_obc] * 2
+            self.has_obc = [has_obc] * 3
         else:
             self.has_obc = has_obc
 
     @staticmethod
     def check_dim(dim):
         """
         See :func:`_ModelTerm.check_dim`
         """
-        if dim != 2:
+        if dim != 3:
             raise Exception("Dimension does not match.")
 
     @staticmethod
     def iterate_sites(ll):
         """
         **Argument**
 
-        ll : Sequence of 2 ints
+        ll : Sequence of 3 ints
             Number of sites along each side of the lattice.
         """
         for ii in range(ll[0]):
             for jj in range(ll[1]):
-                yield ii, jj
+                for kk in range(ll[2]):
+                    yield ii, jj, kk
 
     def collect_operators(self):
         """
         All the required operators are returned to ensure that they are
         written by fortran.
         """
         yield self.operators[0], "l"
         yield self.operators[1], "r"
 
-        # Hilbert curvature could swap order of sites
-        yield self.operators[0], "r"
+        # Have to always add ... order in sites not guaranteed and
+        # could be swapped
         yield self.operators[1], "l"
+        yield self.operators[0], "r"
+
+        if self.add_complex_conjg:
+            # Only works in the b, bdagger or sigma^{+}, sigma^{-}
+            # scenario
+
+            yield self.operators[1], "l"
+            yield self.operators[0], "r"
 
     def iter_shifts(self):
         """
         Return all possible shifts, which depends on the isotropy
-        in the 2d case.
+        in the 3d case.
         """
         if self.isotropy_xyz:
-            n_coord = np.sum(np.abs(np.array(self.shift)) > 0)
+            n_coord = np.sum(np.array(self.shift) > 0)
             if n_coord == 0:
                 raise Exception("Not implemented. Is this case useful?")
             if n_coord == 1:
                 shifts = [
-                    [self.shift[0], self.shift[1]],
-                    [self.shift[1], self.shift[0]],
+                    [self.shift[0], self.shift[1], self.shift[2]],
+                    [self.shift[1], self.shift[2], self.shift[0]],
+                    [self.shift[2], self.shift[0], self.shift[1]],
                 ]
             elif n_coord == 2:
+                if len(set(self.shift)) != 2:
+                    # Can be solved by adding the additional permutation
+                    # and then building the set
+                    raise Exception("Missing permutations.")
                 shifts = [
-                    [self.shift[0], self.shift[1]],
-                    [self.shift[0], -self.shift[1]],
+                    [self.shift[0], self.shift[1], self.shift[2]],
+                    [self.shift[0], -self.shift[1], self.shift[2]],
+                    [self.shift[1], self.shift[2], self.shift[0]],
+                    [self.shift[1], self.shift[2], -self.shift[0]],
+                    [self.shift[2], self.shift[0], self.shift[1]],
+                    [self.shift[2], -self.shift[0], self.shift[1]],
+                ]
+            elif n_coord == 3:
+                if len(set(self.shift)) != 1:
+                    # Can be solved by adding the additional permutation
+                    # and then building the set
+                    raise Exception("Maybe missing permutations.")
+                shifts = [
+                    [self.shift[0], self.shift[1], self.shift[2]],
+                    [-self.shift[0], self.shift[1], self.shift[2]],
+                    [self.shift[0], -self.shift[1], self.shift[2]],
+                    [self.shift[0], self.shift[1], -self.shift[2]],
                 ]
-
-                # This takes into account unequal shifts leading
-                # to four terms, e.g, (1, 2), (1, -2), (2, 1),
-                # and (2, -1)
-                if self.shift[0] != self.shift[1]:
-                    shifts.append([self.shift[1], self.shift[0]])
-                    shifts.append([self.shift[1], -self.shift[0]])
         else:
             shifts = [self.shift]
 
         for elem in shifts:
             yield elem
 
     def get_entries(self, params):
         """
-        Entries combine the information about possible shifts based
-        on the origin coordination (0, 0) and the shift with the
-        information about the operators and couplings.
+        Entries are defined based on two coordinates, the origin
+        chosen as (0, 0, 0) and the shift. There are no site-dependent
+        terms.
 
         **Arguments**
 
         params : dictionary
             Contains the simulation parameters.
 
         **Details**
 
-        To-Do: adding complex conjugates for general case beyond
-        b bdagger case.
-        """
+        To-Do: complex-conjugate terms are wrong, i.e., they work
+        for sigma_{i}^{+} sigma_{j}^{-} or b_{i}^{dagger} b_{j}, but
+        not for terms as b_{j} sigma_{i}^{x}!
+        """
+        if (self.has_obc[0] != self.has_obc[1]) or (self.has_obc[0] != self.has_obc[2]):
+            raise Exception(
+                "Cannot build dictionary with different " + "boundary conditions."
+            )
+
         for shift in self.iter_shifts():
-            coord_a = [0, 0]
+            coord_a = [0, 0, 0]
             coord_b = shift
             coordinates = [coord_a, coord_b]
 
-            coupl_ii = {"coordinates": coordinates, "operators": self.operators}
+            coupl_ii = {
+                "strength": self.eval_strength(params),
+                "operators": self.operators,
+                "coordinates": coordinates,
+            }
 
             yield coupl_ii
 
             if self.add_complex_conjg:
                 coupl_ii = {
+                    "strength": self.eval_strength(params),
+                    "operators": [self.operators[1], self.operators[0]],
                     "coordinates": coordinates,
-                    "operators": self.operators[::-1],
                 }
 
                 yield coupl_ii
 
     def get_interactions(self, ll, params, **kwargs):
         """
         These interactions are closest to the TPO description iterating
         over specific sites within the 1d coordinates.
 
         **Arguments**
 
-        ll : list of ints
-            Number of sites along the dimensions, i.e., not the
+        ll : int
+            Number of sites along each dimension, i.e., not the
             total number of sites. Assuming list of sites
             along all dimension.
 
         params : dictionary
             Contains the simulation parameters.
         """
-        map_to_1d = map_selector(2, ll, self.map_type)
-
-        if self.mask is None:
-            local_mask = np.ones(ll, dtype=bool)
-        else:
-            local_mask = self.mask(params)
+        map_type = self.eval_str_param(self.map_type, params)
+        map_to_1d = map_selector(3, ll, map_type)
 
         for elem in self.get_entries(params):
-            for ix, iy in self.iterate_sites(ll):
+            for ix, iy, iz in self.iterate_sites(ll):
                 coord_a, coord_b = elem["coordinates"]
 
                 if np.sum(np.abs(np.array(coord_a))) != 0:
                     raise Exception("Coordinate A is not the origin.")
 
                 jx = ix + coord_b[0]
                 jy = iy + coord_b[1]
+                jz = iz + coord_b[2]
 
                 if (jx >= ll[0]) and self.has_obc[0]:
                     continue
                 if (jx < 0) and self.has_obc[0]:
                     continue
 
                 if (jy >= ll[1]) and self.has_obc[1]:
                     continue
                 if (jy < 0) and self.has_obc[1]:
                     continue
 
+                if (jz >= ll[2]) and self.has_obc[2]:
+                    continue
+                if (jz < 0) and self.has_obc[2]:
+                    continue
+
                 if jx >= ll[0]:
                     jx = jx % ll[0]
                 if jx < 0:
                     jx += ll[0]
 
                 if jy >= ll[1]:
                     jy = jy % ll[1]
                 if jy < 0:
                     jy += ll[1]
 
+                if jz >= ll[2]:
+                    jz = jz % ll[2]
+                if jz < 0:
+                    jz += ll[2]
+
                 if (jx >= ll[0]) or (jx < 0):
                     raise Exception("Improve handling.")
                 if (jy >= ll[1]) or (jy < 0):
                     raise Exception("Improve handling.")
+                if (jz >= ll[2]) or (jz < 0):
+                    raise Exception("Improve handling.")
 
-                if (ix == jx) and (iy == jy):
+                if (ix == jx) and (iy == jy) and (iz == jz):
+                    print(ix, iy, iz)
+                    print(jx, jy, jz)
+                    print(coord_a)
+                    print(coord_b)
                     raise Exception("Same site ...")
 
-                if not local_mask[ix, iy]:
-                    continue
-
                 # Convert from python to Hilbert space index starting from 1
-                coords_1d = [map_to_1d[elem] for elem in [(ix, iy), (jx, jy)]]
+                coords_1d = [map_to_1d[elem] for elem in [(ix, iy, iz), (jx, jy, jz)]]
 
                 yield elem, coords_1d
 
     def get_fortran_str(self, ll, params, operator_map, param_map):
         """
         See :func:`_ModelTerm.get_fortran_str_two_body`.
         """
         return self.get_fortran_str_twobody(ll, params, operator_map, param_map)
-
-
-class TwoBodyTerm2DLatticeLayout(TwoBodyTerm2D):
-    """
-    The term defines an interaction between two sites of the Hilbert space,
-    for an arbitrary lattice layout. For example, the tunneling term in the
-    Bose-Hubbard model can be represented by this term. This class represents
-    the 2d version.
-
-    **Arguments**
-
-    operators : list of two strings
-        String identifier for the operators. Before launching the simulation,
-        the python API will check that the operator is defined.
-
-    distance : float
-        Defines the distance of the interaction.
-
-    layout : :class:`LatticeLayout`, str, callable
-        Instance of the :class:`LatticeLayout`. The `LatticeLayout` class stores
-        the positions of the (nx)x(ny) grid for an arbitrary lattice layout.
-
-    strength : str, callable, numeric (optional)
-        Defines the coupling strength of the local terms. It can
-        be parameterized via a value in the dictionary for the
-        simulation or a function.
-        Default to 1.
-
-    prefactor : numeric, scalar (optional)
-        Scalar prefactor, e.g., in order to take into account signs etc.
-        Default to 1.
-
-    tolerance : float, optional
-        Tolerance for the distance of the interaction,
-        i.e., the absolute distance must be smaller than the tolerance
-        to consider the sites interacting.
-
-    **Attributes**
-
-    map_type : str, optional
-        Selecting the mapping from a n-dimensional system to the
-        1d system required for the TTN simulations.
-    """
-
-    def __init__(
-        self, operators, distance, layout, strength=1, prefactor=1, tolerance=1e-8
-    ):
-        super().__init__(operators, 1, strength=strength, prefactor=prefactor)
-        self.distance = distance
-        self.tolerance = tolerance
-        self.layout = layout
-
-        # Delete unused terms
-        del self.shift
-        del self.isotropy_xyz
-        del self.add_complex_conjg
-        del self.mask
-        del self.has_obc
-
-        # Will be set when adding Hamiltonian terms
-        self.map_type = None
-
-    def iter_shifts(self):
-        """
-        The function is inherited, but we overwrite it since it
-        has no meaning in this context.
-        """
-        raise Exception("This function is not available.")
-
-    def get_entries(self, params):
-        """
-        The function is inherited, but we overwrite it since it
-        has no meaning in this context.
-        """
-        raise Exception("This function is not available.")
-
-    def get_interactions(self, ll, params, **kwargs):
-        """
-        These interactions are closest to the TPO description iterating
-        over specific sites within the 1d coordinates.
-
-        **Arguments**
-
-        ll : int
-            Number of sites along the dimensions, i.e., not the
-            total number of sites. Assuming equal number of sites
-            along all dimension.
-
-        params : dictionary
-            Contains the simulation parameters.
-        """
-        map_to_1d = map_selector(2, ll, self.map_type)
-
-        layout = self.eval_numeric_param(self.layout, params)
-
-        for ix, iy in self.iterate_sites(ll):
-            coord_ix, coord_iy = layout.positions[ix, iy, :]
-
-            for jx, jy in self.iterate_sites(ll):
-                coord_jx, coord_jy = layout.positions[jx, jy, :]
-                dist = layout.distance((coord_ix, coord_iy), (coord_jx, coord_jy))
-
-                coords_1d_i = map_to_1d[(ix, iy)]
-                coords_1d_j = map_to_1d[(jx, jy)]
-
-                if coords_1d_i < coords_1d_j:
-                    if np.abs(dist - self.distance) <= self.tolerance:
-                        coupl_ij = {
-                            "coordinates": [(ix, iy), (jx, jy)],
-                            "operators": self.operators,
-                        }
-                        yield coupl_ij, (coords_1d_i, coords_1d_j)
-
-    def get_fortran_str(self, ll, params, operator_map, param_map):
-        """
-        See :func:`_ModelTerm.get_fortran_str_two_body`.
-        """
-        return self.get_fortran_str_twobody(ll, params, operator_map, param_map)
```

### Comparing `qtealeaves-0.5.14/qtealeaves/models/__init__.py` & `qtealeaves-1.1.1/qtealeaves/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/models/bosehubbard.py` & `qtealeaves-1.1.1/qtealeaves/models/bosehubbard.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/models/quantumising.py` & `qtealeaves-1.1.1/qtealeaves/models/quantumising.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/models/xxzmodel.py` & `qtealeaves-1.1.1/qtealeaves/models/xxzmodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/__init__.py` & `qtealeaves-1.1.1/qtealeaves/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/bond_entropy.py` & `qtealeaves-1.1.1/qtealeaves/observables/bond_entropy.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,23 +140,31 @@
         ----------
         fh : filehandle
             Write the information about the measurements to this filehandle.
         is_measured : bool
             If True, the backend can measure the observable
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobsbondentropy\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
         if is_measured:
             # Number of results
-            if len(self.results_buffer) == 0:
-                fh.write("0\n")
-            else:
-                for value in self.results_buffer.values():
-                    fh.write(f"{len(self.results_buffer)}\n")
-                    fh.write(
-                        f"{len(value)}\n"
-                    )  # Number of values in the result istance
-                    for subkey, subvalue in value.items():
-                        # Index of the first tensor, index of the second tensor, value
-                        fh.write(f"{subkey[0]}, {subkey[1]}, {subvalue}")
+            buffer_str = ""
+            cntr = 0
+
+            for value in self.results_buffer.values():
+                if value is None:
+                    continue
+
+                cntr += 1
+                buffer_str += f"{len(self.results_buffer)}\n"
+
+                # Number of values in the result istance
+                buffer_str += f"{len(value)}\n"
+                for subkey, subvalue in value.items():
+                    # Index of the first tensor, index of the second tensor, value
+                    buffer_str += f"{subkey[0]}, {subkey[1]}, {subvalue}\n"
+
+            fh.write(f"{cntr}\n")
+            if cntr > 0:
+                fh.write(buffer_str)
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/correlation.py` & `qtealeaves-1.1.1/qtealeaves/observables/correlation.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 ( <A_1 B_1>   <A_1 B_2>   <A_1 B_3>   ... )
 ( <A_2 B_1>   <A_2 B_2>   <A_2 B_3>   ... )
 ( <A_3 B_1>   <A_3 B_2>   <A_3 B_3>   ... )
 (    ...         ...         ...      ... )
 """
 
 import numpy as np
+from qtealeaves.mpos import DenseMPOList, MPOSite, DenseMPO, ITPO
 from .tnobase import _TNObsBase
 
+
 __all__ = ["TNObsCorr", "TNObsCorr4"]
 
 
 class TNObsCorr(_TNObsBase):
     """
     The correlation observable measures the correlation between
     two operators. It cannot be used for fermionic operators which
@@ -44,15 +46,15 @@
 
     **Arguments**
 
     name : str
         Define a label under which we can find the observable in the
         result dictionary.
 
-    operator : list of two strings
+    operators : list of two strings
         Identifiers/strings for the operators to be measured.
     """
 
     def __init__(self, name, operators):
         super().__init__(name)
         self.operators = [operators]
 
@@ -89,14 +91,167 @@
         """
         Documentation see :func:`_TNObsBase.collect_operators`.
         """
         for elem in self.operators:
             yield (elem[0], "l")
             yield (elem[1], "r")
 
+    def _to_itpo(self, operators, tensor_backend, num_sites):
+        """
+        Return an ITPO represented the correlation observable
+
+        Parameters
+        ----------
+        operators: TNOperators
+            The operator class
+        tensor_backend: instance of `TensorBackend`
+            Tensor backend of the simulation
+        num_sites: int
+            Number of sites of the state
+
+        Returns
+        -------
+        ITPO
+            The ITPO class
+        """
+        dense_mpo_list = DenseMPOList()
+        for kk, _ in enumerate(self.name):
+            key_a = self.operators[kk][0]
+            key_b = self.operators[kk][1]
+
+            for ii in range(num_sites):
+                for jj in range(num_sites):
+                    if ii == jj:
+                        continue
+
+                    site_a = MPOSite(
+                        ii, key_a, 1.0, 1.0, operators=operators, params={}
+                    )
+                    site_b = MPOSite(
+                        jj, key_b, 1.0, 1.0, operators=operators, params={}
+                    )
+
+                    dense_mpo = DenseMPO(
+                        [site_a, site_b], tensor_backend=tensor_backend
+                    )
+                    dense_mpo_list.append(dense_mpo)
+
+        # Sites are not ordered and we have to make links match anyways
+        dense_mpo_list = dense_mpo_list.sort_sites()
+
+        itpo = ITPO(num_sites)
+        itpo.add_dense_mpo_list(dense_mpo_list)
+
+        return itpo
+
+    def to_itpo(self, operators, tensor_backend, num_sites, de_layer=None):
+        """
+        Return an ITPO represented the correlation observable.
+        In the case of the aTTN the function takes care of diagonal
+        terms of corr matrix with the disentanglers on them. These
+        diagonal terms are stored in the order of looping over ii and jj.
+
+        Parameters
+        ----------
+        operators: TNOperators
+            The operator class
+        de_layer : DELayer
+            Disentangler layer for which the iTPO layer is created
+        tensor_backend: instance of `TensorBackend`
+            Tensor backend of the simulation
+        num_sites: int
+            Number of sites of the state
+
+        Returns
+        -------
+        ITPO
+            The ITPO class
+        """
+
+        if de_layer is None:
+            return self._to_itpo(operators, tensor_backend, num_sites)
+
+        # only if aTTN
+        dense_mpo_list = DenseMPOList()
+        for kk, _ in enumerate(self.name):
+            key_a = self.operators[kk][0]
+            key_b = self.operators[kk][1]
+
+            # get all operators.ops[]
+            op_a = operators.ops[key_a]
+            op_b = operators.ops[key_b]
+            # get the matching identity
+            op_identity = op_a.eye_like(op_a.links[1])
+            op_identity.attach_dummy_link(0, is_outgoing=False)
+            op_identity.attach_dummy_link(3, is_outgoing=True)
+            key_identity = str(id(op_identity))
+            operators.ops[key_identity] = op_identity
+
+            # get the operator a x b for the diag entries
+            if op_a.ndim == 2:
+                op_ab = op_a @ op_b
+            else:
+                # Assume rank-4 (but delta charge both times to the right
+                # Assume that tensor_a and tensor_b have same link dimensions
+                op_ab = op_a.tensordot(op_b, ([2], [1]))
+                op_ab = op_ab.transpose([3, 0, 1, 4, 2, 5])
+                op_ab.fuse_links_update(4, 5)
+                op_ab.fuse_links_update(0, 1, False)
+            key_ab = str(id(op_ab))
+            operators.ops[key_ab] = op_ab
+
+            # fill the itpo with correct operators on correct sites
+            for ii in range(num_sites):
+                for jj in range(num_sites):
+                    if ii == jj and (ii in de_layer.de_sites):
+                        # Diagonal entries of correlation matrix for sites that have
+                        # a disentangler attached to it cannot longer be measured as
+                        # local terms, and thus the appropriate identity operator needs
+                        # to be added on the other site of the disentangler
+
+                        where = np.where(de_layer.de_sites == ii)
+                        # we assume max 1 disentangler per site
+                        ind = [where[0][0], where[1][0]]
+                        site_identity = de_layer.de_sites[ind[0], abs(ind[1] - 1)]
+
+                        site_a = MPOSite(
+                            ii, key_ab, 1.0, 1.0, operators=operators, params={}
+                        )
+                        site_b = MPOSite(
+                            site_identity,
+                            key_identity,
+                            1.0,
+                            1.0,
+                            operators=operators,
+                            params={},
+                        )
+                    elif ii == jj:
+                        continue
+                    else:
+                        site_a = MPOSite(
+                            ii, key_a, 1.0, 1.0, operators=operators, params={}
+                        )
+                        site_b = MPOSite(
+                            jj, key_b, 1.0, 1.0, operators=operators, params={}
+                        )
+
+                    dense_mpo = DenseMPO(
+                        [site_a, site_b], tensor_backend=tensor_backend
+                    )
+                    dense_mpo_list.append(dense_mpo)
+
+        # Sites within dense mpos are not ordered and we have to make links match anyways
+        dense_mpo_list = dense_mpo_list.sort_sites()
+
+        itpo = ITPO(num_sites)
+        itpo.add_dense_mpo_list(dense_mpo_list)
+        itpo.set_meas_status(do_measurement=True)
+
+        return itpo
+
     def read(self, fh, **kwargs):
         """
         Read the measurements of the correlation observable from fortran.
 
         **Arguments**
 
         fh : filehandle
@@ -207,15 +362,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobscorr\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 # Write column by column because this is favored
                 # by the fortran memory
@@ -387,15 +542,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobscorr4\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 # Write column by column because this is favored
                 # by the fortran memory
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/custom_correlation.py` & `qtealeaves-1.1.1/qtealeaves/observables/custom_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # that they have been altered from the originals.
 
 """
 Custom observable
 """
 
 import numpy as np
-from qtealeaves.hilbert_curvature import map_selector
+from qtealeaves.tooling import map_selector
 from .tnobase import _TNObsBase
 
 __all__ = ["TNObsCustom"]
 
 
 class TNObsCustom(_TNObsBase):
     """
@@ -270,15 +270,14 @@
             num_sites_measured = len(site_indices[ii])
             str_buffer += "%d " % num_sites_measured
         str_buffer += "\n"
 
         # iterate over measurements
         for ii in range(len(self)):
             for sites in site_indices[ii]:
-
                 # operator IDs (pad with zeros so that every list of operator IDs is
                 # of the same size - needed for storing a variable in fortran)
                 diff = self.max_term_size - term_size[ii]
                 str_buffer += "%d " % (operator_map[(self.operators[ii][0], "l")])
                 for jj in range(1, term_size[ii]):
                     str_buffer += "%d " % (operator_map[(self.operators[ii][jj], "r")])
                 for jj in range(0, diff):
@@ -314,15 +313,15 @@
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         Note: measuring TNObsCustom on python side is not yet implemented.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobscustom\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 # write is_complex = True
                 fh.write("C")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/distance2pure.py` & `qtealeaves-1.1.1/qtealeaves/observables/distance2pure.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tndistance2pure\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 real_part = np.real(self.results_buffer[name_ii])
                 imag_part = np.imag(self.results_buffer[name_ii])
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/local.py` & `qtealeaves-1.1.1/qtealeaves/observables/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,29 +154,30 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobslocal\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 result_ii = self.results_buffer[name_ii]
 
                 fh.write(" ".join(list(map(str, result_ii))) + "\n")
 
     def write_input_v1(self, folder_name, params):
         """
         Documentation see :func:`_TNObsBase.write_input_v1`.
         """
         for ii in range(len(self)):
+            # pylint: disable-next=no-member
             full_filename = os.path.join(
                 folder_name, "observable_%s.in" % (self.name[ii])
             )
 
             with open(full_filename, "w+") as fh:
                 fh.write("# Local observable?\n")
                 fh.write(".true.\n")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/probabilities.py` & `qtealeaves-1.1.1/qtealeaves/observables/probabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
       with highest probability, until the total probability measured is more then
       a threshold :math:`\mathcal{E}`. This procedure is dangerous, since it can
       take an exponentially-long time if :math:`\mathcal{E}` is too high.
     - Going down **unbiasedly** on the tree, which means drawing a ``num_sumples``
       uniformly distributed random numbers :math:`u\sim U(0,1)` and ending in the
       leaf which probability interval :math:`[p_{\mathrm{low}}, p_{\mathrm{high}}]`
       is such that :math:`u\in [p_{\mathrm{low}}, p_{\mathrm{high}}]`. This is the
-      suggested method.
+      suggested method. See http://arxiv.org/abs/2401.10330 for additional details.
 
     The result of the observable will be a dictionary where:
 
     - the keys are the measured state on a given basis
     - the values are the probabilities of measuring the key for the **even** and
       **greedy** approach, while they are the probability intervals for the
       **unbiased** approach.
@@ -70,21 +70,33 @@
     ----------
     prob_type: str, optional
         The type of probability measure. Default to 'U'. Available:
         - 'U', unbiased
         - 'G', greedy
         - 'E', even. Also implemented in Fortran backend
     num_samples: int, optional
-        Number of samples for the unbiased prob_type. Default to 100
+        Number of samples for the unbiased prob_type. Default to 100.
+        If a list is passed, the function is called multiple times with that list of
+        parameters.
     prob_threshold: float, optional
         probability treshold for `prob_type=('G', 'E')`. Default to 0.9.
+    qiskit_convention : bool, optional
+        If you should use the qiskit convention when measuring, i.e. least significant qubit
+        on the right. Default to False.
     """
 
-    def __init__(self, prob_type="U", num_samples=100, prob_threshold=0.9):
+    def __init__(
+        self,
+        prob_type="U",
+        num_samples=100,
+        prob_threshold=0.9,
+        qiskit_convention=False,
+    ):
         self.prob_type = [prob_type.upper()]
+        self.qiskit_convention = [qiskit_convention]
 
         if prob_type == "U":
             self.prob_param = [num_samples]
             name = ["unbiased_probability"]
         elif prob_type == "E":
             self.prob_param = [prob_threshold]
             name = ["even_probability"]
@@ -108,28 +120,30 @@
         """
         Documentation see :func:`_TNObsBase.__iadd__`.
         """
         if isinstance(other, TNObsProbabilities):
             self.prob_type += other.prob_type
             self.prob_param += other.prob_param
             self.name += other.name
+            self.qiskit_convention += other.qiskit_convention
         else:
             raise Exception("__iadd__ not defined for this type.")
 
         return self
 
     @classmethod
     def empty(cls):
         """
         Documentation see :func:`_TNObsBase.empty`.
         """
         obj = cls()
         obj.prob_type = []
         obj.prob_param = []
         obj.name = []
+        obj.qiskit_convention = []
 
         return obj
 
     def read(self, fh, **kwargs):
         """
         Read the measurements of the projective measurement
         observable from fortran.
@@ -184,15 +198,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobsprobabilities\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 fh.write(str(len(self.results_buffer[name_ii])) + "\n")
                 for key, value in self.results_buffer[name_ii].items():
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/projective.py` & `qtealeaves-1.1.1/qtealeaves/observables/projective.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,38 +37,44 @@
     and such is will only be an approximation of the true probability distribution,
     that in the example case would be :math:`p_{00}=p_{11}=0.5`.
 
     Parameters
     ----------
     num_shots : int
         Number of projective measurements
+    qiskit_convention : bool, optional
+        If you should use the qiskit convention when measuring, i.e. least significant qubit
+        on the right. Default to False.
     """
 
-    def __init__(self, num_shots):
+    def __init__(self, num_shots, qiskit_convention=False):
         self.num_shots = num_shots
+        self.qiskit_convention = [qiskit_convention]
         self._measures = {}
         _TNObsBase.__init__(self, "projective_measurements")
 
     def __iadd__(self, other):
         """
         Documentation see :func:`_TNObsBase.__iadd__`.
         """
         if isinstance(other, TNObsProjective):
             self.num_shots += other.num_shots
+            self.qiskit_convention += other.qiskit_convention
         else:
             raise Exception("__iadd__ not defined for this type.")
 
         return self
 
     @classmethod
     def empty(cls):
         """
         Documentation see :func:`_TNObsBase.empty`.
         """
         obj = cls(0)
+        obj.qiskit_convention = []
 
         return obj
 
     def add_trajectories(self, all_results, new):
         """
         Documentation see :func:`_TNObsBase.add_trajectories`.
         """
@@ -143,17 +149,20 @@
 
         Parameters
         ----------
         fh : filehandle
             Write the information about the measurements to this filehandle.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobsfinalmeas\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             # Number of results
-            for res in self.results_buffer.values():
-                fh.write(str(len(res)) + "\n")
-                for key, value in res.items():
-                    fh.write(f"{key} | {value} \n")
+            if len(self.results_buffer.values()) > 0:
+                for res in self.results_buffer.values():
+                    fh.write(str(len(res)) + "\n")
+                    for key, value in res.items():
+                        fh.write(f"{key} | {value} \n")
+            else:
+                fh.write("0\n")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/state2file.py` & `qtealeaves-1.1.1/qtealeaves/observables/state2file.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnstate2file\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         for name_ii in self.name:
             fh.write(self.results_buffer[name_ii] + "\n")
 
         self.results_buffer = {}
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/tensor_product.py` & `qtealeaves-1.1.1/qtealeaves/observables/tensor_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,14 @@
 
         Parameters
         ----------
         fh : filehandle
             Write the information about the measurements to this filehandle.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobstensprod\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         for name_ii in self.name:
             fh.write(f"{np.real(self.results_buffer[name_ii])}, ")
             fh.write(f"{np.imag(self.results_buffer[name_ii])} \n")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/timecorrelator.py` & `qtealeaves-1.1.1/qtealeaves/observables/timecorrelator.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         return
 
     def write_results(self, fh, is_measured, **kwargs):
         """
         Documentation see :func:`_TNObsBase.write_results`.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobstzerocorr\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 # Write column by column because this is favored
                 # by the fortran memory
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/tnobase.py` & `qtealeaves-1.1.1/qtealeaves/observables/tnobase.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Abstract base class for observables.
 """
 
-from ..parameterized import _ParameterizedClass
+from qtealeaves.tooling import _ParameterizedClass
 
 __all__ = ["_TNObsBase"]
 
 
 class _TNObsBase(_ParameterizedClass):
     """
     Abstract base class for observables.
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/tnobservables.py` & `qtealeaves-1.1.1/qtealeaves/observables/tnobservables.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import warnings
 from copy import deepcopy
 from collections import OrderedDict
 import h5py
 from qtealeaves import __version__
 
-from ..parameterized import _ParameterizedClass
+from qtealeaves.tooling import _ParameterizedClass
 from .local import TNObsLocal
 from .correlation import TNObsCorr, TNObsCorr4
 from .distance2pure import TNDistance2Pure
 from .state2file import TNState2File
 from .tensor_product import TNObsTensorProduct
 from .weighted_sum import TNObsWeightedSum
 from .projective import TNObsProjective
@@ -69,23 +69,22 @@
     Up to now, the class organizes and accepts observables of the
     type :class:`TNObsLocal`, :class:`TNObsCorr`, :class:`TNDistance2Pure`,
     :class:`TNState2File`, :class:`TNObsTensorProduct`, :class:`TNObsWeightedSum`,
     :class:`TNObsProjective`, :class:`TNObsProbabilities`, :class:`TNObsBondEntropy`,
     :class:`TNObsCustom`
     """
 
-    results_buffer = {}
-
     def __init__(
         self,
         filename_observables="observables.in",
         folder_observables="observables",
         num_trajectories=1,
         do_write_hdf5=False,
     ):
+        self.results_buffer = {}
         self.filename_observables = filename_observables
         self.folder_observables = folder_observables
         self.num_trajectories = num_trajectories
         self.do_write_hdf5 = do_write_hdf5
 
         self.obs_list = OrderedDict()
 
@@ -223,18 +222,22 @@
             Provides the mapping between the string identifiers
             for the operators to the integer index in the list
             of operators.
         """
         # We need params in the future - avoid unused argument error
         _ = len(params)
 
+        # pylint: disable-next=no-member
         full_path_file = os.path.join(folder_name, self.filename_observables)
+        # pylint: disable-next=no-member
         full_path_folder = os.path.join(folder_name, self.folder_observables)
 
+        # pylint: disable-next=no-member
         if not os.path.isdir(full_path_folder):
+            # pylint: disable-next=no-member
             os.makedirs(full_path_folder)
 
         with open(full_path_file, "w+") as fh:
             # write T or F for writing to hdf5
             eval_do_write_hdf5 = self.eval_numeric_param(
                 elem=self.do_write_hdf5, params=params
             )
@@ -294,18 +297,22 @@
 
         folder_name : str
             Name of the input folder of the simulation.
 
         params : dict
             Simulation parameters.
         """
+        # pylint: disable-next=no-member
         full_path_file = os.path.join(folder_name, self.filename_observables)
+        # pylint: disable-next=no-member
         full_path_folder = os.path.join(folder_name, self.folder_observables)
 
+        # pylint: disable-next=no-member
         if not os.path.isdir(full_path_folder):
+            # pylint: disable-next=no-member
             os.makedirs(full_path_folder)
 
         with open(full_path_file, "w+") as fh:
             for elem in self.obs_list:
                 for subfile in self.obs_list[elem].write_input_v1(
                     full_path_folder, params
                 ):
@@ -329,14 +336,15 @@
 
         Iterator returns key, value pair if available.
         """
         tmp = filename_result.split("/")
         tmp[-1] = params.get("log_file", "sim.log")
         log_file_path = "/".join(tmp)
 
+        # pylint: disable-next=no-member
         if not os.path.isfile(log_file_path):
             # Empty iterator
             return
 
         cpu_time = None
         match = "Total CPU time:"
         with open(log_file_path, "r") as log_file:
@@ -369,15 +377,14 @@
         results = {}
 
         if self.eval_numeric_param(elem=self.do_write_hdf5, params=params):
             # read from the hdf5 file
             # filename is the same as for text, but with last three chars replaced by hdf5
             hdf5_filename = filename[:-3] + "hdf5"
             with h5py.File(hdf5_filename, "r") as h5f:
-
                 # The structure of the file is:
                 # version
                 # energy
                 # time
                 # norm
                 # /TNObsLocal/0, 1, 2, ...
                 # /TNObsCorr/0/real
@@ -405,15 +412,14 @@
                             f"NOT IMPLEMENTED YET: Instance is {type(obs_object)}. "
                             + "It does not support hdf5 read/writing yet. Use do_write_hdf5=False."
                         )
 
         else:
             # reading from .dat file
             with open(filename, "r") as fh:
-
                 # First line is IO version (for future use)
                 _ = fh.readline()
                 # Separator
                 _ = fh.readline()
 
                 energy = fh.readline()
                 results["energy"] = float(energy)
@@ -452,28 +458,30 @@
         num_trajectories = self.get_num_trajectories(params=params)
 
         if num_trajectories == 1:
             # no quantum trajectories
             folder_name_output = self.eval_str_param(folder, params)
 
             # get results
+            # pylint: disable-next=no-member
             full_file_path = os.path.join(folder_name_output, filename)
             results = self.read_file(full_file_path, params)
         else:
             # read results for quantum trajectories
             results = {}
             for ii in range(num_trajectories):
                 # add trajectory id into params
                 tmp = deepcopy(params)
                 tmp["trajectory_id"] = self.get_id_trajectories(ii)
                 tmp["seed"] = self.get_seed_trajectories(tmp)
 
                 folder_name_output = self.get_folder_trajectories(folder, tmp)
 
                 # get results for each quantum trajectory
+                # pylint: disable-next=no-member
                 full_file_path = os.path.join(folder_name_output, filename)
 
                 name_ii = ("trajectory", tmp["trajectory_id"])
                 results[name_ii] = self.read_file(full_file_path, params)
                 results[name_ii]["seed"] = tmp["seed"]
 
                 # add the observables
```

### Comparing `qtealeaves-0.5.14/qtealeaves/observables/weighted_sum.py` & `qtealeaves-1.1.1/qtealeaves/observables/weighted_sum.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Observable to measure the weighted sum of tensor product observables
 """
 
+import warnings
 import numpy as np
+from qtealeaves.mpos import (
+    DenseMPOList,
+    MPOSite,
+    DenseMPO,
+    ITPO,
+)
 from .tnobase import _TNObsBase
 from .tensor_product import TNObsTensorProduct
 
 __all__ = ["TNObsWeightedSum"]
 
 
 class TNObsWeightedSum(_TNObsBase):
@@ -51,34 +58,38 @@
         Name to identify the observable
     tp_operators: :class:`TNObsTensorProduct`
         Tensor product observables. Its length, i.e. the number of tensor product
         observables contained in it, shoud be the same of the number of complex
         coefficients.
     coeffs: list of complex
         Coefficients of the weighted sum for each tp_operators
+    use_itpo: bool, optional
+        If True, measure using ITPO. Default to False. Consumed in python.
 
     """
 
-    def __init__(self, name, tp_operators, coeffs):
+    def __init__(self, name, tp_operators, coeffs, use_itpo=False):
         if np.isscalar(coeffs):
             coeffs = [coeffs]
         self.tp_operators = [tp_operators]
         self.coeffs = [coeffs]
+        self.use_itpo = use_itpo
 
         _TNObsBase.__init__(self, name)
 
     @classmethod
     def empty(cls):
         """
         Documentation see :func:`_TNObsBase.empty`.
         """
         obj = cls(None, None, None)
         obj.name = []
         obj.tp_operators = []
         obj.coeffs = []
+        obj.use_itpo = True
 
         return obj
 
     def __len__(self):
         """
         Provide appropriate length method
         """
@@ -88,39 +99,44 @@
         """
         Documentation see :func:`_TNObsBase.__iadd__`.
         """
         if isinstance(other, TNObsWeightedSum):
             self.name += other.name
             self.tp_operators += other.tp_operators
             self.coeffs += other.coeffs
+            self.use_itpo = self.use_itpo and other.use_itpo
         else:
             raise Exception("__iadd__ not defined for this type.")
 
         return self
 
-    def from_pauli_string(self, name, pauli_string):
-        """Initialize the observable from a qiskit chemistry pauli string format.
+    @classmethod
+    def from_pauli_string(cls, name, pauli_string, use_itpo=False):
+        """
+        Initialize the observable from a qiskit chemistry pauli string format.
         First, outside of the function use the WeightedPauliOperator method to_dict()
         and then give that dict as input to this function
 
         Parameters
         ----------
         name: str
             Name of the observable
         pauli_string: dict
             Dictionary of pauli strings
+        use_itpo: bool, optional
+            If True, measure using ITPO. Default to False. Consumed in python.
 
         Returns
         -------
-        None: None
+        TNObsWeightedSum
+            The weighted sum observable initialized from the pauli dictionary
         """
         assert (
             "paulis" in pauli_string.keys()
         ), "Dictionary is not in pauli string format"
-        assert name not in self.name, f"Observable {name} already initialized"
 
         addends = pauli_string["paulis"]
 
         coeffs = []
         tp_operators = TNObsTensorProduct.empty()
         # First, we look at each term in the weighted sum
         for term in addends:
@@ -128,23 +144,74 @@
             coef = term["coeff"]["real"] + 1j * term["coeff"]["imag"]
             operators = []
             sites = []
             for idx, pauli in enumerate(string):
                 if pauli != "I":
                     operators.append(pauli)
                     sites.append([idx])
-
+            if len(sites) == 0:
+                operators.append("I")
+                sites.append([0])
             tp_operators += TNObsTensorProduct(string, operators, sites)
 
             coeffs += [coef]
 
-        obs_wt = TNObsWeightedSum(name, tp_operators, coeffs)
-        self += obs_wt
+        obs_wt = cls(name, tp_operators, coeffs, use_itpo)
+
+        return obs_wt
+
+    def to_itpo(self, operators, tensor_backend, num_sites):
+        """
+        Return an ITPO represented the weighted sum observable
+
+        Parameters
+        ----------
+        operators: TNOperators
+            The operator class
+        tensor_backend: instance of `TensorBackend`
+            Tensor backend of the simulation
+        num_sites: int
+            Number of sites in the state to be measures
+
+        Returns
+        -------
+        ITPO
+            The ITPO class
+        """
+        dense_mpo_list = DenseMPOList()
+
+        # Cycle over weighted sum observables
+        for coeffs, tp_ops in zip(self.coeffs, self.tp_operators):
+            if isinstance(tp_ops, list):
+                tp_ops = tp_ops[0]
+            # Cycle over the TPO of a single weighted sum
+            for ops, sites, coef in zip(tp_ops.operators, tp_ops.sites, coeffs):
+                mpo_sites_list = []
+                # Cycle over the different operators in a single TPO
+                for op_ii, site_ii in zip(ops, sites):
+                    mpo_sites_list.append(
+                        MPOSite(
+                            site_ii[0], op_ii, 1.0, coef, operators=operators, params={}
+                        )
+                    )
+
+                    # iTPO has local weights, need to set to one after first term
+                    coef = 1.0
+                dense_mpo = DenseMPO(mpo_sites_list, tensor_backend=tensor_backend)
+                dense_mpo_list.append(dense_mpo)
+                if len(dense_mpo) > 0:
+                    warnings.warn("Adding length zero MPO to dense mpo list.")
+
+        # Sites are not ordered and we have to make links match anyways
+        dense_mpo_list = dense_mpo_list.sort_sites()
+        itpo = ITPO(num_sites)
+        itpo.add_dense_mpo_list(dense_mpo_list)
+        itpo.set_meas_status(do_measurement=True)
 
-        return None
+        return itpo
 
     def read(self, fh, **kwargs):
         """
         Read the measurements of the correlation observable from fortran.
 
         Parameters
         ----------
@@ -215,15 +282,15 @@
 
         Parameters
         ----------
         fh : filehandle
             Write the information about the measurements to this filehandle.
         """
         # Write separator first
-        fh.write("-" * 20 + "\n")
+        fh.write("-" * 20 + "tnobsweightedsum\n")
         # Assignment for the linter
         _ = fh.write("T \n") if is_measured else fh.write("F \n")
 
         if is_measured:
             for name_ii in self.name:
                 fh.write(f"{np.real(self.results_buffer[name_ii])}, ")
                 fh.write(f"{np.imag(self.results_buffer[name_ii])} \n")
```

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/__init__.py` & `qtealeaves-1.1.1/qtealeaves/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/bosonicoperators.py` & `qtealeaves-1.1.1/qtealeaves/operators/bosonicoperators.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,55 +45,55 @@
         self.ops["id"] = self.get_id
         self.ops["n"] = self.get_n
         self.ops["nint"] = self.get_nint
         self.ops["b"] = self.get_b
         self.ops["bdagger"] = self.get_bdagger
 
     @staticmethod
-    def get_id(**kwargs):
+    def get_id(params):
         """
         Define the identity operator.
         """
-        nmin = kwargs.get("fock_space_nmin", 0)
-        nmax = kwargs.get("fock_space_nmax", 3)
+        nmin = params.get("fock_space_nmin", 0)
+        nmax = params.get("fock_space_nmax", 3)
 
         return np.eye(nmax - nmin + 1)
 
     @staticmethod
-    def get_n(**kwargs):
+    def get_n(params):
         """
         Define the number operator.
         """
-        nmin = kwargs.get("fock_space_nmin", 0)
-        nmax = kwargs.get("fock_space_nmax", 3)
+        nmin = params.get("fock_space_nmin", 0)
+        nmax = params.get("fock_space_nmax", 3)
 
         return np.diag(np.arange(nmin, nmax + 1))
 
     @staticmethod
-    def get_nint(**kwargs):
+    def get_nint(params):
         """
         Define the on-site interaction operator 0.5 * n * (n - 1).
         """
-        nmin = kwargs.get("fock_space_nmin", 0)
-        nmax = kwargs.get("fock_space_nmax", 3)
+        nmin = params.get("fock_space_nmin", 0)
+        nmax = params.get("fock_space_nmax", 3)
 
         return np.diag(0.5 * np.arange(nmin, nmax + 1) * np.arange(nmin - 1, nmax))
 
     @staticmethod
-    def get_b(**kwargs):
+    def get_b(params):
         """
         Define the bosonic annihilation operator.
         """
-        nmin = kwargs.get("fock_space_nmin", 0)
-        nmax = kwargs.get("fock_space_nmax", 3)
+        nmin = params.get("fock_space_nmin", 0)
+        nmax = params.get("fock_space_nmax", 3)
 
         return np.sqrt(np.diag(np.arange(nmin, nmax + 2)))[1:, :-1]
 
     @staticmethod
-    def get_bdagger(**kwargs):
+    def get_bdagger(params):
         """
         Define the bosonic creation operator.
         """
-        nmin = kwargs.get("fock_space_nmin", 0)
-        nmax = kwargs.get("fock_space_nmax", 3)
+        nmin = params.get("fock_space_nmin", 0)
+        nmax = params.get("fock_space_nmax", 3)
 
         return np.sqrt(np.diag(np.arange(nmin, nmax + 2)))[:-1, 1:]
```

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/combinedoperators.py` & `qtealeaves-1.1.1/qtealeaves/operators/combinedoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/quditoperators.py` & `qtealeaves-1.1.1/qtealeaves/operators/quditoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/spinoperators.py` & `qtealeaves-1.1.1/qtealeaves/operators/spinoperators.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,12 +33,12 @@
         we store operators.
         Default to ``SPIN12``
     """
 
     def __init__(self, folder_operators="SPIN12"):
         super().__init__(folder_operators=folder_operators)
 
-        self.ops["id"] = np.array([[1, 0], [0, 1]])
-        self.ops["sx"] = np.array([[0, 1], [1, 0]])
-        self.ops["sz"] = np.array([[1, 0], [0, -1]])
-        self.ops["n"] = np.array([[0, 0], [0, 1]])
-        self.ops["nz"] = np.array([[1, 0], [0, 0]])
+        self.ops["id"] = np.array([[1, 0], [0, 1.0]])
+        self.ops["sx"] = np.array([[0, 1], [1, 0.0]])
+        self.ops["sz"] = np.array([[1, 0], [0, -1.0]])
+        self.ops["n"] = np.array([[0, 0], [0, 1.0]])
+        self.ops["nz"] = np.array([[1, 0], [0, 0.0]])
```

### Comparing `qtealeaves-0.5.14/qtealeaves/operators/tnoperators.py` & `qtealeaves-1.1.1/qtealeaves/operators/tnoperators.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 # that they have been altered from the originals.
 
 """
 Generic base class for operators.
 """
 
 import os
+
+# pylint: disable-next=no-name-in-module
 import os.path
 from collections import OrderedDict
 from copy import deepcopy
 import numpy as np
 
+from qtealeaves.tooling import _ParameterizedClass
 from qtealeaves import write_tensor, write_symtensor
 from qtealeaves import StrBuffer
 
 
 __all__ = ["TNOperators"]
 
 
-class TNOperators:
+class TNOperators(_ParameterizedClass):
     """
     Generic class to write operators. This class contains no pre-defined
     operators. It allows you to start from scratch if no other operator
     class fulfills your needs.
 
     **Arguments**
 
@@ -38,14 +41,32 @@
         we store operators.
     """
 
     def __init__(self, folder_operators="SPIN12"):
         self.folder_operators = folder_operators
         self.ops = OrderedDict()
 
+    def keys(self):
+        """Return the keys of the underlying dictionary."""
+        return self.ops.keys()
+
+    def __getitem__(self, key):
+        if isinstance(key, str) and isinstance(self.ops, list):
+            raise Exception("Operators are site-dependent.")
+
+        if isinstance(key, str):
+            return self.ops[key]
+
+        site_key, key = key
+
+        if isinstance(self.ops, list):
+            return self.ops[site_key][key]
+
+        return self.ops[key]
+
     def write_operator(
         self, folder_dst, operator_name, params, tensor_backend, **kwargs
     ):
         """
         Write operator to file. Format depends on the tensor backend.
 
         **Arguments**
@@ -83,14 +104,15 @@
 
         see write_operator
         """
         if hasattr(folder_dst, "write"):
             # filehandle
             full_filename = folder_dst
         else:
+            # pylint: disable-next=no-member
             full_filename = os.path.join(folder_dst, operator_name + ".dat")
 
         op_mat = self.get_operator(operator_name, params)
 
         write_tensor(op_mat, full_filename)
 
         return operator_name + ".dat"
@@ -105,14 +127,15 @@
 
         see write_operator
         """
         if hasattr(folder_dst, "write"):
             # filehandle
             dst = folder_dst
         else:
+            # pylint: disable-next=no-member
             dst = os.path.join(folder_dst, operator_name + ".dat")
 
         op_mat = self.get_operator(operator_name, params)
 
         sector = params.get("SymmetrySectors", None)
         generators = params.get("SymmetryGenerators", None)
         gen_types = params.get("SymmetryTypes", None)
@@ -171,15 +194,15 @@
             Tag/identifier of the operator.
 
         params : dict
             Simulation parameters as a dictionary; dict is passed
             to callable.
         """
         if hasattr(self.ops[operator_name], "__call__"):
-            op_mat = self.ops[operator_name](**params)
+            op_mat = self.ops[operator_name](params)
         else:
             op_mat = self.ops[operator_name]
 
         return op_mat
 
     def write_input(self, folder_name, params, tensor_backend, required_operators):
         """
@@ -199,18 +222,22 @@
             ``Tensors`` should be written to the input files.
 
         required_operators : list
             List of operators keys which is needed for AbelianSymTensors,
             where we distinguish between left, right, center, and independent
             operators.
         """
+        # pylint: disable-next=no-member
         full_path = os.path.join(folder_name, self.folder_operators)
+        # pylint: disable-next=no-member
         if not os.path.isdir(full_path):
+            # pylint: disable-next=no-member
             os.makedirs(full_path)
 
+        # pylint: disable-next=no-member
         relative_file = os.path.join(full_path, "operators.dat")
         buffer_str = StrBuffer()
 
         operator_id_mapping = {}
 
         ii = 0
         for operator_ii in self.ops.keys():
```

### Comparing `qtealeaves-0.5.14/qtealeaves/parameterized.py` & `qtealeaves-1.1.1/qtealeaves/tooling/parameterized.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 The tooling to have parameterized models and instances.
 """
+import typing
 
 __all__ = ["_ParameterizedClass"]
 
 
 class _ParameterizedClass:
     """
     Abstract base class for any other class which needs to evaluate
@@ -61,14 +62,17 @@
             the value, or directly as the numeric value.
 
         params : dict
             The parameter dictionary, which will be passed to callables.
         """
         if hasattr(elem, "__call__"):
             val = elem(params)
+        # pylint: disable-next=isinstance-second-argument-not-valid-type
+        elif not isinstance(elem, typing.Hashable):
+            val = elem
         elif elem in params:
             val = params[elem]
         else:
             val = elem
 
         return val
 
@@ -92,7 +96,35 @@
         """
         if hasattr(elem, "__call__"):
             val = elem(params)
         else:
             val = default
 
         return val
+
+    def _resolve_params_attr(self, params, attr_numeric=None, attr_str=None):
+        """
+        Resolve parameterized values (inplace-update).
+
+        **Arguments**
+
+        attr_numeric : list of strings or `None`
+            For a list of strings, `getattr` and `setattr`
+            is called for the the class to resolve potential
+            parameterization with `eval_numeric_param`
+
+        attr_str : list of strings or `None`
+            For a list of strings, `getattr` and `setattr`
+            is called for the the class to resolve potential
+            parameterization with `eval_str_param`
+        """
+        if attr_numeric is not None:
+            for elem in attr_numeric:
+                value = getattr(self, elem)
+                value = self.eval_numeric_param(value, params)
+                setattr(self, elem, value)
+
+        if attr_str is not None:
+            for elem in attr_str:
+                value = getattr(self, elem)
+                value = self.eval_str_param(value, params)
+                setattr(self, elem, value)
```

### Comparing `qtealeaves-0.5.14/qtealeaves/simulation_setup.py` & `qtealeaves-1.1.1/qtealeaves/simulation_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 The setup for a simulation with the aTTN or TTN network bringing together all
 pieces, e.g., the model, and the observables.
 """
+
 import os
+
+
 import os.path
 from pathlib import Path
 from copy import deepcopy
+import hashlib
+import json
 import shutil
 import subprocess
 import multiprocessing as mprc
 from collections import OrderedDict
 from warnings import warn
 
 # Time is not precise, but perf_counter likely does not
@@ -28,29 +33,30 @@
 from time import sleep
 
 import numpy as np
 
 import qtealeaves as qtl
 from qtealeaves import write_nml
 import qtealeaves.emulator as qtltn
-from qtealeaves.parameterized import _ParameterizedClass
+from qtealeaves.tooling import _ParameterizedClass
+from qtealeaves.mpos import SparseMatrixProductOperator as spo_cls
 
 
-__all__ = ["ATTNSimulation", "DynamicsQuench"]
+__all__ = ["QuantumGreenTeaSimulation", "ATTNSimulation", "DynamicsQuench"]
 
 
 class DisentanglerPositionException(Exception):
     """
     Class of exceptions raised when aTTN disentanglers are
     placed on the invalid position. Raised within the
     `check_disentangler_position` function.
     """
 
 
-class ATTNSimulation(_ParameterizedClass):
+class QuantumGreenTeaSimulation(_ParameterizedClass):
     """
     Simulation class containing the model, the operators, the convergence
     settings, and the observables.
 
     **Arguments**
 
     model : instance of ``RydbergModel``
@@ -73,26 +79,22 @@
         default to ``input``
 
     folder_name_output : str, or callable; optional
         Specifies the folder where the output is stored. Will be created
         if not existing. Path can contain subfolders.
         default to ``output``
 
-    version_input_processor : int, optional
-        Defines the version of the input processor. Version ``1`` refers to
-        the original input, the main improvement for version ``2`` is the
-        support namelists in fortran. Version 3 allows parameterization of
-        models, which enables dynamics in a much more convenient fashion.
-        default to 3
-
     tn_type : int, optional
         Specifies whether TTNs (1) or aTTNs (2) are used. The integer 0
         is reserved for running ED simulations within in the python
         frontend. LPTN can be called via (3) and an MPS via LPTN as (4).
-        The python backends can be used with non-symmetric TTNs (5).
+        The python backends can be used with non-symmetric TTNs (5),
+        non-symmetric MPS (6).
+        Additionally, for aTTN python backend choose (7), but only correlation
+        measurement and no groundstate search is so far implemented.
         default to 1
 
     tensor_backend : int, optional
         Choosing the underlying tensor, where the AbelianSymTensors are ``1``,
         and the Tensors are ``2``.
         default to 1
 
@@ -123,15 +125,20 @@
         Flag if log file should be created instead of writing
         the output to standard out. If False, all output will
         go to standard out.
         Default to False (no log file)
 
     store_checkpoints : bool, optional
         If True, the state will be written to a file after each
-        sweep in the ground state search.
+        sweep in the ground state search and after each time step
+        in a time evolution. Ground state searches have the option
+        to write checkpoints also after each tensor optimization,
+        which the algorithm can decide on without control by the
+        user.
+        If `True`, `delete_existing_folder` must be `False`.
         Default to True
 
     verbosity : int, optional
         Sets the output level inside the python functions. Does
         not have any effect on fortran simulations.
         Default to 1.
 
@@ -145,60 +152,72 @@
 
     The following keywords cannot be used for adapting simulations to the
     needs by the user, but have a predefined meaning. Additional predefined
     keywords may be imported, e.g., when using a specific model or a specific
     set of operators.
 
     * `continue_file` : load file at the beginning of the simulation.
+    * `use_mpo_from_continue_file` : bool (Python only). Use MPO stored
+      in continue file.
     * `seed` : seed for random number generators.
     * `magic_number` : for debugging / developing to pass something to
        fortran.
     * `SymmetrySector`
     * `SymmetryGenerators`
     * `SymmetryTypes`
     * `Quenches`
     * `ed_sparse` : bool, use in exact state emulator to
       switch between sparse and dense Hamiltonian.
+    * `sweep_order` : defines the sweep order for the statics (python only)
+    * `exclude_from_hash` : dictionary entries that will be excluded from hash.
+
+    **Details**
 
+    1) Checkpoints vs continue files: checkpointing is used to restart the same
+       simulation. Continue files can be used to set the input state across
+       simulations, but the simulation will start always at the beginning with
+       this user-provided input state.
+    2) Hashing: hashes are generated to identify that a simulation setup did
+       not change. For example, changes in a simulation which uses checkpoints
+       can be detected this way.
     """
 
     def __init__(
         self,
         model,
         operators,
         convergence,
         observables,
         folder_name_input="input",
         folder_name_output="output",
         file_name_input="TTN.in",
-        version_input_processor=3,
         tn_type=1,
         tensor_backend=1,
         mpo_mode=-1,
         disentangler=None,
         disentangler_file="disentangler.dat",
         has_log_file=False,
         store_checkpoints=True,
         verbosity=1,
         qgreentea_exe="./MainaTTN",
     ):
-        if tensor_backend != 2 and tn_type == 5:
+        if tensor_backend != 2 and tn_type in (5, 6, 7):
             raise ValueError(
                 "Only non-symmetric tensors can be used in python. Set tensor_backend=2."
             )
         self.model = model
         self.operators = operators
         self.convergence = convergence
         self.observables = observables
 
         self.file_name_input = file_name_input
         self.folder_name_input = folder_name_input
         self.folder_name_output = folder_name_output
 
-        self.version_input_processor = version_input_processor
+        self.version_input_processor = 3
         self.tn_type = tn_type
         self.tensor_backend = tensor_backend
         self.mpo_mode = mpo_mode
 
         self.disentangler = disentangler
         self.disentangler_file = disentangler_file
 
@@ -219,14 +238,32 @@
             verbosity level in the class, the ``*args`` will be
             passed to the print function.
             Default to 1
         """
         if verbosity_level <= self.verbosity:
             print(*args)
 
+    @staticmethod
+    def checkpoint_params_hash(params):
+        """Generate hash of a simulation to identify if checkpointed simulation."""
+        exclude_from_hash = params.get("exclude_from_hash", [])
+
+        if len(exclude_from_hash) == 0:
+            dict_for_hash = params
+        else:
+            dict_for_hash = {}
+            for key, value in params.items():
+                if key in exclude_from_hash:
+                    continue
+
+                dict_for_hash[key] = value
+
+        params_str = json.dumps(dict_for_hash, sort_keys=True)
+        return hashlib.sha256(params_str.encode("utf-8")).hexdigest()
+
     def get_groundstate_energy(self, params):
         """
         (DEPRECATED) Rudimentary way to extract the ground state energy via the
         convergence file.
 
         **Arguments**
 
@@ -234,24 +271,25 @@
             The parameter dictionary, which is required to obtain
             the output folder.
 
         **Details**
 
         Use ``get_static_obs`` in future.
         """
-        print("`get_groundstate_energy` is deprecated.")
+        warn("`get_groundstate_energy` is deprecated.")
 
         num_trajectories = self.observables.get_num_trajectories(params=params)
         if num_trajectories > 1:
             raise Exception(
                 "`get_groundstate_energy` not available for quantum trajectories."
             )
 
         folder_name_output = self.eval_str_param(self.folder_name_output, params)
         line = None
+        # pylint: disable-next=no-member
         with open(os.path.join(folder_name_output, "convergence.log"), "r") as fh:
             for line in fh:
                 pass
 
         if line is None:
             raise Exception("Reading ground state energy from empty file.")
 
@@ -349,15 +387,17 @@
                     try:
                         quench_results.append(
                             self.observables.read(file_name, folder_name_output, params)
                         )
 
                     except FileNotFoundError:
                         if warning_count < 3:
-                            warn(f"File {file_name} not found. Skipping.")
+                            warn(
+                                f"File {folder_name_output}/{file_name} not found. Skipping."
+                            )
                         if warning_count == 3:
                             warn("Further warnings will be suppressed.")
                         warning_count += 1
                         # If the folder is missing append None
                         # instead of the result dictionary.
                         quench_results.append(None)
 
@@ -403,14 +443,15 @@
             The parameter dictionary or dictionaries, which is required
             to obtain the output folder.
 
         delete_existing_folder : bool, optional
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
             Default to False
 
         nthreads : int, optional
             If number of threads greater is one, we launch serial
             simulations. If greater than one, multiple threads
             are started to run simulations in parallel.
             Default to 1.
@@ -434,20 +475,14 @@
             from file set by a user.
             The groundstate is found by iterative search, therefore if
             the initial condition is set by user, put `max_iter=0` in
             convergence parameters. Otherwise, set `max_iter>0`.
         #3 Perform a time evolution starting from the obtained
             initial condition.
         """
-        # if tensor network is aTTN and disentangler positions are not set,
-        # find the disentangler positions automatically
-        tn_type = self.eval_numeric_param(self.tn_type, params)
-        if (tn_type == 2) and (self.disentangler is None):
-            self.disentangler = self.autoselect_disentangler(params)
-
         # create a new list for the parameter to add different
         # entries in the case of quantum trajectories
         params_ext = self.extend_params(params=params)
 
         # Check that we don't accidentally delete the current or
         # parent directory
         if delete_existing_folder:
@@ -455,16 +490,19 @@
                 folder_name_input = self.observables.get_folder_trajectories(
                     self.folder_name_input, elem
                 )
                 folder_name_output = self.observables.get_folder_trajectories(
                     self.folder_name_output, elem
                 )
 
+                # pylint: disable-next=no-member
                 current_path = Path(os.getcwd())
+                # pylint: disable-next=no-member
                 input_path = Path(os.path.abspath(folder_name_input))
+                # pylint: disable-next=no-member
                 output_path = Path(os.path.abspath(folder_name_output))
 
                 inout_folder_danger = []
                 # True if in/out folder is the same as the current folder
                 inout_folder_danger.append(input_path == current_path)
                 inout_folder_danger.append(output_path == current_path)
                 # True if in/out folder is a parent folder of the current folder
@@ -488,14 +526,66 @@
             self.run_threaded(
                 params_ext,
                 delete_existing_folder=delete_existing_folder,
                 nthreads=nthreads,
             )
         return
 
+    def status(self, params):
+        """
+        Returns tuple of three integers containing the number of simulations
+        not started, number of simulation started but not finished, and the
+        number of finished simulations.
+
+        **Arguments**
+
+        params : dict or list of dicts
+            The parameter dictionary or dictionaries, which is required
+            to obtain the output folder.
+        """
+        # create a new list for the parameter to add different
+        # entries in the case of quantum trajectories
+        params_ext = self.extend_params(params=params)
+
+        num_unstarted = 0
+        num_interrupted = 0
+        num_finished = 0
+
+        for elem in params_ext:
+            folder_name_output = self.observables.get_folder_trajectories(
+                self.folder_name_output, elem
+            )
+
+            finished_json = os.path.join(folder_name_output, "has_finished.json")
+            if os.path.isfile(finished_json):
+                num_finished += 1
+                continue
+
+            dyn_checkpoints = os.path.join(
+                folder_name_output, "has_dyn_checkpoints.txt"
+            )
+            if os.path.isfile(dyn_checkpoints):
+                # Dynamics started, but did not finish
+                num_interrupted += 1
+                continue
+
+            stat_checkpoints = os.path.join(
+                folder_name_output, "has_stat_checkpoints.txt"
+            )
+            if os.path.isfile(stat_checkpoints):
+                # Statics started, but did not finish
+                num_interrupted += 1
+                continue
+
+            # Did not reach first checkpoint of statics, consider it as simulation
+            # which did not start yet
+            num_unstarted += 1
+
+        return num_unstarted, num_interrupted, num_finished
+
     def write_input(
         self, params, delete_existing_folder=False, do_return_params_ext=False
     ):
         """
         Write input for a simulation or multiple simulations.
 
         **Arguments**
@@ -504,14 +594,15 @@
             The parameter dictionary or dictionaries, which is required
             to obtain the output folder.
 
         delete_existing_folder : bool, optional
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
             Default to False
 
         do_return_params_ext : bool, optional
             Return additionally the full list of simulations, e.g., potentially
             extended with quantum trajectories.
             Default to False.
 
@@ -520,20 +611,14 @@
         exec_list : list of strings
             Commands to be executed to run the simulations written.
 
         params_ext : list of dicts
             Only returned as second return value if `do_return_params_ext=True`.
             Contains the full list of simulation parameter dictionaries.
         """
-        # if tensor network is aTTN and disentangler positions are not set,
-        # find the disentangler positions automatically
-        tn_type = self.eval_numeric_param(self.tn_type, params)
-        if (tn_type == 2) and (self.disentangler is None):
-            self.disentangler = self.autoselect_disentangler(params)
-
         # create a new list for the parameter to add different
         # entries in the case of quantum trajectories
         params_ext = self.extend_params(params=params)
 
         # Now we have a list
         exec_list = []
         for elem in params_ext:
@@ -564,14 +649,15 @@
             The parameter dictionary or dictionaries, which is required
             to obtain the output folder.
 
         delete_existing_folder : bool, optional
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
             Default to False
 
         submit_dir : str or `None`, optional
             If `None`, the path to the input and output folder is accesible
             from the current working directory. If a string is specified,
             the string will be used as a prefix to the input and output
             directory and they will be copied on runtime (by fortran) to the
@@ -637,17 +723,19 @@
                         self.folder_name_input, params_ext[ii]
                     )
                     output_dir = self.observables.get_folder_trajectories(
                         self.folder_name_output, params_ext[ii]
                     )
 
                     input_run_dir = input_dir
+                    # pylint: disable-next=no-member
                     input_dir = os.path.join(submit_dir, input_dir)
 
                     output_run_dir = output_dir
+                    # pylint: disable-next=no-member
                     output_dir = os.path.join(submit_dir, output_dir)
 
                 if submit_dir_approach in [1, 2]:
                     fh.write(input_dir + "\n")
                     fh.write(output_dir + "\n")
                     fh.write(input_run_dir + "\n")
                     fh.write(output_run_dir + "\n")
@@ -740,42 +828,95 @@
             The parameter dictionary, which is required to obtain
             the output folder.
 
         delete_existing_folder : bool
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
         """
         folder_name_input = self.observables.get_folder_trajectories(
             self.folder_name_input, params
         )
         folder_name_output = self.observables.get_folder_trajectories(
             self.folder_name_output, params
         )
+        sim_hash_file = os.path.join(folder_name_input, "sim_hash.json")
+        tn_type = self.eval_numeric_param(self.tn_type, params)
 
+        if self.store_checkpoints and delete_existing_folder:
+            raise ValueError("Cannot delete folders and rely on checkpoints.")
+
+        sim_hash = self.checkpoint_params_hash(params)
+
+        # There are three options:
+        #
+        # * delete_existing_folder=True, store_checkpoints=False
+        # * delete_existing_folder=False, store_checkpoints=False
+        # * delete_existing_folder=False, store_checkpoints=True
         if delete_existing_folder:
+            # Delete existing folder, checkpoints cannot be activated.
+
+            # pylint: disable-next=no-member
             if os.path.isdir(folder_name_input):
                 shutil.rmtree(folder_name_input)
 
+            # pylint: disable-next=no-member
             if os.path.isdir(folder_name_output):
                 shutil.rmtree(folder_name_output)
-        else:
+
+        elif not self.store_checkpoints:
+            # No checkpoints and not deleting existing folders
+            # pylint: disable-next=no-member
             if os.path.isdir(folder_name_input) or os.path.isdir(folder_name_output):
-                raise Exception("Enable overwritting existing folders.")
+                raise ValueError(
+                    "Folder exists, but neither checkpoints nor deleting activated."
+                )
+
+        # pylint: disable-next=no-member
+        elif os.path.isdir(folder_name_input) and os.path.isdir(folder_name_output):
+            with open(sim_hash_file, "r") as fh:
+                jdic = json.load(fh)
+                previous_sim_hash = jdic["sim_hash"]
+
+            if previous_sim_hash != sim_hash:
+                # This is not a simulation which is continued
+                raise Exception("Trying to continue simulation with different params.")
+            if tn_type in [0, 5, 6, 7]:
+                # python simulation can restart via `simulation.run`
+                return None
+
+            # Looks like a fortran simulation, need to construct
+            # nml file name
+            return self.get_full_fortran_nml(params)
+
+        # pylint: disable-next=no-member
+        if os.path.isdir(folder_name_input) or os.path.isdir(folder_name_output):
+            # raise error, this can only happen if user was interfering by hand
+            raise ValueError("Input / output folder: one exists, one does not exist.")
 
+        # pylint: disable-next=no-member
         if not os.path.isdir(folder_name_output):
+            # pylint: disable-next=no-member
             os.makedirs(folder_name_output)
+        # pylint: disable-next=no-member
         if not os.path.isdir(folder_name_input):
+            # pylint: disable-next=no-member
             os.makedirs(folder_name_input)
 
-        tn_type = self.eval_numeric_param(self.tn_type, params)
-        if tn_type == 0:
-            return None
+        # Store the simulation hash
+        sim_hash_jdic = {"sim_hash": sim_hash}
+        with open(sim_hash_file, "w+") as fh:
+            json.dump(sim_hash_jdic, fh)
 
+        if tn_type in [0, 5, 6, 7]:
+            # It is a python simulation, we do not write any input
+            return None
         if self.version_input_processor == 3:
+            # Fortran simulation with input processor 3 (only 3 valid by now)
             nml_file = self.write_input_3(params)
             return nml_file
 
         if self.version_input_processor in [1, 2]:
             raise Exception("Version of input processor not supported anymore.")
 
         raise Exception("Unknwon version of f90 input processor.")
@@ -790,40 +931,42 @@
             The parameter dictionary, which is required to obtain
             the output folder.
 
         delete_existing_folder : bool, optional
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
             Default to False
         """
         tic = tictoc()
 
         cmd_arg = self.write_input_single(params, delete_existing_folder)
 
         tn_type = self.eval_numeric_param(self.tn_type, params)
         if tn_type == 0:
             # Run ED simulation
             qtltn.run_ed_simulation(self, params)
-        elif tn_type == 5:
-            # Run pyTTN simulation
-            qtltn.ttn_simulator.run_ttn_simulation(self, params)
+        elif tn_type in (5, 6, 7):
+            # Run pyTN simulation (TTN or MPS)
+            qtltn.tn_simulation.run_tn_simulation(self, params)
 
         else:
             # All input version processor for TN simulations
             cmd = self.qgreentea_exe + " " + cmd_arg
 
             self.vprint("Will be running " + cmd)
             status = subprocess.call(cmd, shell=True)
 
             if status != 0:
                 raise Exception("Fortran error during simulation.")
 
-        toc = tictoc()
-        self.vprint("Simulation time is %2.4f." % (toc - tic))
+            # Only for fortran on purpose - python has to handle itself
+            toc = tictoc()
+            self.vprint("Simulation time is %2.4f." % (toc - tic))
 
         return
 
     def run_threaded(self, params, delete_existing_folder=False, nthreads=4):
         """
         Run simulation specified via the parameter dictionary.
 
@@ -833,14 +976,15 @@
             List of the parameter dictionaries, which is required to obtain
             the output folder.
 
         delete_existing_folder : bool, optional
             If flag is True, existing folder with potential results
             will be overwritten without warning. If False, an error
             is raised if the folders already exist.
+            If `True`, `store_checkpoints` must be `False`.
             Default to False
 
         nthreads : int, optional
             Number of threads to start multiple simulations in
             parallel.
             Default to 4.
         """
@@ -907,14 +1051,15 @@
 
         params : dict
             Dictionary with the simulation parameters.
         """
         sectors = params.get("SymmetrySectors", [0])
         nn_sym = len(sectors)
 
+        # pylint: disable-next=no-member
         full_filename = os.path.join(folder_name_input, "symmetry_sectors.dat")
         with open(full_filename, "w+") as fh:
             fh.write(str(nn_sym) + "\n")
 
             for elem in sectors:
                 fh.write(str(elem) + "\n")
 
@@ -937,14 +1082,19 @@
             Dictionary with the simulation parameters.
 
         Return
         ------
         auto_dis : np.array
             Disentangler positions.
         """
+        if self.tn_type == 7:
+            raise NotImplementedError(
+                "Automatic disentangler selection not yet implemented for"
+                " python backend aTTNs."
+            )
         # Total number of sites in the system
         ll_1d_mapped = self.model.get_number_of_sites(params)
         # The array in which the disentangler positions will be added
         auto_dis = np.array([[], []], dtype=int)
 
         # To find the positions on which we can place the disentanglers, we
         # iterate over all the pairs of sites in the system.
@@ -1197,27 +1347,29 @@
 
         params : dict
             Dictionary with the simulation parameters.
         """
         full_filename = self.eval_str_param(self.disentangler_file, params)
         disentangler_pos = self.eval_numeric_param(self.disentangler, params)
 
-        if disentangler_pos is None:
-            tn_type = self.eval_numeric_param(self.tn_type, params)
-            if tn_type == 2:
-                raise Exception(
-                    "Choosing an aTTN but defining no disentangler will not work."
-                )
-
+        tn_type = self.eval_numeric_param(self.tn_type, params)
+        if tn_type not in [2, 7]:
+            # No aTTN, return empty filename
             full_filename = ""
             return full_filename
-        else:
-            full_filename = os.path.join(folder_name_input, full_filename)
 
-        self.check_disentangler_position(params)
+        # pylint: disable-next=no-member
+        full_filename = os.path.join(folder_name_input, full_filename)
+        if disentangler_pos is None:
+            # User expects auto-selection
+            disentangler_pos = self.autoselect_disentangler(params)
+
+        if self.tn_type == 7:  # because python indexing is different!!
+            disentangler_pos = np.transpose(disentangler_pos)
+        self.check_disentangler_position(params, disentangler_pos=disentangler_pos)
 
         with open(full_filename, "w+") as fh:
             fh.write("%d\n" % (disentangler_pos.shape[1]))
 
             for ii in range(disentangler_pos.shape[1]):
                 fh.write(
                     "%d, %d\n"
@@ -1225,16 +1377,34 @@
                         disentangler_pos[0, ii] + 1,
                         disentangler_pos[1, ii] + 1,
                     )
                 )
 
             fh.write("\n")
 
+        if self.tn_type == 7:  # because python indexing is different!!
+            disentangler_pos = np.transpose(disentangler_pos)
+
         return full_filename
 
+    def get_full_fortran_nml(self, params):
+        """Return the fortran nml filename serving as entry point for simulations."""
+        folder_name_input = self.observables.get_folder_trajectories(
+            self.folder_name_input, params
+        )
+
+        file_name_input = self.eval_str_param(self.file_name_input, params)
+        if not file_name_input.endswith(".nml"):
+            file_name_input += ".nml"
+
+        # pylint: disable-next=no-member
+        full_nml = os.path.join(folder_name_input, file_name_input)
+
+        return full_nml
+
     def write_input_3(self, params):
         """
         Write all the input files for the input processor version 3. This
         version supports for example parameterization of models.
 
         **Arguments**
 
@@ -1244,28 +1414,30 @@
         folder_name_input = self.observables.get_folder_trajectories(
             self.folder_name_input, params
         )
         folder_name_output = self.observables.get_folder_trajectories(
             self.folder_name_output, params
         )
 
+        # pylint: disable-next=no-member
         if not os.path.isdir(folder_name_input):
+            # pylint: disable-next=no-member
             os.makedirs(folder_name_input)
 
         required_operators = []
         required_operators += self.model.collect_operators()
         required_operators += self.observables.collect_operators()
         required_operators = list(set(required_operators))
 
         conv_in = self.convergence.write_input(folder_name_input, params)
         operator_in, operator_map = self.operators.write_input(
             folder_name_input, params, self.tensor_backend, required_operators
         )
         model_in = self.model.write_input(
-            folder_name_input, params, operator_map, self.mpo_mode
+            folder_name_input, params, operator_map, self.mpo_mode, spo_cls
         )
         obs_in = self.observables.write(folder_name_input, params, operator_map)
 
         task_params = OrderedDict()
         task_params["input_folder"] = folder_name_input
         task_params["output_folder"] = folder_name_output
 
@@ -1300,20 +1472,29 @@
         )
 
         task_params["has_log_file"] = self.has_log_file
         # task_params['log_file'] = # THIS IS PENDING
         task_params["store_checkpoints"] = self.store_checkpoints
 
         if "Quenches" in params:
+            # assumes all quenches have the same time evolution mode
+            quench = params["Quenches"][0]
+
             task_params["time_evolution_mode"] = params["Quenches"][
                 0
             ].time_evolution_mode
-            task_params["oqs_mode"] = params["Quenches"][0].oqs_mode
+            if task_params["time_evolution_mode"] == 0:
+                # in write method, this can only be a fortran simulation with TN, never ED
+                # set to 1
+                task_params["time_evolution_mode"] = 1
+
+            task_params["time_evolution_mode"] = quench.time_evolution_mode
+            task_params["oqs_mode"] = quench.oqs_mode
         else:
-            task_params["time_evolution_mode"] = 1
+            task_params["time_evolution_mode"] = 0
             task_params["oqs_mode"] = 0
 
         task_params["mpo_mode"] = self.eval_numeric_param(self.mpo_mode, params)
         task_params["magic_number"] = params.get("magic_number", 0)
 
         seed = list(params.get("seed", [11, 13, 17, 19]))
         if len(seed) != 4:
@@ -1327,25 +1508,39 @@
 
         # Nml does not support lists (?)
         task_params["seed1"] = seed[0]
         task_params["seed2"] = seed[1]
         task_params["seed3"] = seed[2]
         task_params["seed4"] = seed[3]
 
-        file_name_input = self.eval_str_param(self.file_name_input, params)
-        if not file_name_input.endswith(".nml"):
-            file_name_input += ".nml"
-
-        full_nml = os.path.join(folder_name_input, file_name_input)
-
+        full_nml = self.get_full_fortran_nml(params)
         write_nml("TASK_VARS", task_params, full_nml)
 
         return full_nml
 
 
+class ATTNSimulation(QuantumGreenTeaSimulation):
+    """
+    For backwards compatibility.
+    """
+
+    def __init__(self, *args, **kwargs):
+        warn("Deprecated ATTNSimulation; switch to QuantumGreenTeaSimulation.")
+
+        version_input_processor = kwargs.get("version_input_processor", None)
+        if version_input_processor is not None:
+            warn("Deprecated argument input processor.")
+            del kwargs["version_input_processor"]
+
+        super().__init__(*args, **kwargs)
+
+        if version_input_processor is not None:
+            self.version_input_processor = version_input_processor
+
+
 def _run_single_thread(obj, params, delete_existing_folder):
     """
     Internal function to launch a single thread of a threaded simulation.
 
     **Arguments**
 
     obj : instance of :class:``ATTNSimulation``.
@@ -1355,14 +1550,15 @@
         The parameter dictionary, which is required to obtain
         the output folder.
 
     delete_existing_folder : bool, optional
         If flag is True, existing folder with potential results
         will be overwritten without warning. If False, an error
         is raised if the folders already exist.
+        If `True`, `store_checkpoints` must be `False`.
         Default to False
     """
     obj.run_single(params, delete_existing_folder=delete_existing_folder)
     return
 
 
 class DynamicsQuench(dict):
@@ -1374,20 +1570,28 @@
     **Arguments**
 
     dt_grid : numpy.ndarray, str, callable
         Contains the list of time steps, which can differ. Moreover,
         it can be parameterized and be a callable or string.
 
     time_evolution_mode : int, optional
-        Defines the time evolution mode and currently we have
-        a one-site TDVP (1), and the space-link expansion
-        TDVP (2).
-        Not every network type might support all time evolution
-        modes.
-        Default to 1.
+        Defines the time evolution mode.
+        0 : automatic selector
+            (Defaults to 1 for tensor networks.
+            For exact diagonalization,
+            defaults to 10 for systems smaller than 10 sites and 11 for others.)
+        1 : one-tensor TDVP
+        2 : two-tensor TDVP
+        3 : two-tensor TDVP (2nd order)
+        4 : single-tensor TDVP (2nd order)
+        5 : 9 steps of one-site and one step of two-site TDVP
+        10 : exact diagonalization with full Hamiltonian matrix generated
+        11 : exact diagonalization with Krylov
+        Not every network type might support all time evolution modes.
+        Default to 0.
 
     measurement_period : int, str, callable, optional
         Allows to define a measurement period every n time steps. It
         considers only the time steps, not the time passed. There
         is always a measurement at the end of the quench.
         Default to 1.
 
@@ -1413,15 +1617,15 @@
              - \\frac{1}{2} \\{ L^{\\dagger} L, \\rho \\})
 
     """
 
     def __init__(
         self,
         dt_grid,
-        time_evolution_mode=1,
+        time_evolution_mode=0,
         measurement_period=1,
         oqs_mode=0,
         check_superfluous=True,
     ):
         super().__init__()
         self.dt_grid = dt_grid
         self.time_evolution_mode = time_evolution_mode
```

### Comparing `qtealeaves-0.5.14/qtealeaves/version.py` & `qtealeaves-1.1.1/qtealeaves/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Version string, e.g., for installation script.
 """
-__version__ = "0.5.14"
+__version__ = "1.1.1"
```

### Comparing `qtealeaves-0.5.14/qtealeaves.egg-info/PKG-INFO` & `qtealeaves-1.1.1/qtealeaves.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 0.5.14
+Version: 1.1.1
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
 Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `qtealeaves-0.5.14/setup.py` & `qtealeaves-1.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,26 +63,34 @@
     project_urls={},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     package_dir={
         "qtealeaves": "qtealeaves",
+        "qtealeaves.tooling": "qtealeaves/tooling",
+        "qtealeaves.solvers": "qtealeaves/solvers",
+        "qtealeaves.tensors": "qtealeaves/tensors",
         "qtealeaves.emulator": "qtealeaves/emulator",
         "qtealeaves.observables": "qtealeaves/observables",
         "qtealeaves.modeling": "qtealeaves/modeling",
         "qtealeaves.models": "qtealeaves/models",
+        "qtealeaves.mpos": "qtealeaves/mpos",
         "qtealeaves.operators": "qtealeaves/operators",
         "qtealeaves.convergence_parameters": "qtealeaves/convergence_parameters",
     },
     packages=[
         "qtealeaves",
+        "qtealeaves.tooling",
+        "qtealeaves.solvers",
+        "qtealeaves.tensors",
         "qtealeaves.emulator",
         "qtealeaves.observables",
         "qtealeaves.modeling",
         "qtealeaves.models",
+        "qtealeaves.mpos",
         "qtealeaves.operators",
         "qtealeaves.convergence_parameters",
     ],
     python_requires=">=3.8",
     install_requires=install_requires,
 )
```

### Comparing `qtealeaves-0.5.14/tests/tests_formatting.py` & `qtealeaves-1.1.1/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_fortran_interface.py` & `qtealeaves-1.1.1/tests/tests_fortran_interface.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_hilbert_curvature.py` & `qtealeaves-1.1.1/tests/tests_hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_lattice_layout.py` & `qtealeaves-1.1.1/tests/tests_lattice_layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 import os.path
 import unittest
 import numpy as np
 import numpy.linalg as nla
 from shutil import rmtree
 
-from qtealeaves.lattice_layout import LatticeLayout
+from qtealeaves.tooling import LatticeLayout
 
 
 class TestLatticeLayout(unittest.TestCase):
     """
     Check if the 2D lattice layout is constructed properly.
     """
```

### Comparing `qtealeaves-0.5.14/tests/tests_linter.py` & `qtealeaves-1.1.1/tests/tests_linter.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,20 @@
     * Skip Unused argument errors when kargs
     """
 
     def setUp(self):
         """
         Provide the test setup.
         """
+        good_names = "ii,jj,kk,ll,nn,mm"
+        good_names += ",i1,i2,i3,n1,n2,n3,ix,iy,iz,jx,jy,jz"
+        good_names += ",dx,dy,dz,dt"
+        good_names += ",fh,op,xp"
         self.pylint_args = {
-            "good-names": "ii,jj,kk,nn,mm,fh,dx,dy,dz,dt,op,xp",
+            "good-names": good_names,
             "disable": "C0325,C0209,W1514,R1711,C3001",
         }
 
     def run_pylint(self, filename, local_settings={}):
         """
         Run linter test with our unit test settings for one specific
         filename.
@@ -212,22 +216,23 @@
         Linter for module ``baseterm.py``
 
         **Details**
 
         We locally ignore:
 
         * E1101: no member
+        * R0913: too many arguments.
         """
         pattern_1 = (
             "W0223(abstract-method), _ModelTerm1D] Method "
             + "'get_interactions' is abstract in class '_ModelTerm' but "
             + "is not overridden"
         )
         local_settings = {
-            "disable": "E1101",
+            "disable": "E1101,R0913",
             "good-names": "ll",
             "ignore_in_line": [pattern_1],
         }
         return local_settings
 
     def get_settings_localterm(self):
         """
@@ -324,32 +329,14 @@
         local_settings = {
             "disable": "R0902,R0912,R0913,R0914",
             "good-names": "ix,iy,jx,jy,ll,bc",
             "ignore_in_line": [pattern_1],
         }
         return local_settings
 
-    def get_settings_twobodyterm3d(self):
-        """
-        Linter for module ``twobodyterm3d.py``
-
-        **Details**
-
-        We locally ignore:
-
-        * R0902: too many instance attributes
-        * R0912: too many branches
-        * R0913: too many arguments
-        """
-        local_settings = {
-            "disable": "R0902,R0912,R0913",
-            "good-names": "ix,iy,iz,jx,jy,jz,ll,bc",
-        }
-        return local_settings
-
     def get_settings_plaquetteterm2d(self):
         """
         Linter for module ``plaquetteterm2d.py``
 
         **Details**
 
         We locally ignore:
@@ -372,19 +359,20 @@
         Linter for module ``blockterm2d.py``
 
         **Details**
 
         We locally ignore:
 
         * R0913: too many arguments
+        * R0914 : too many locals
         """
 
         pattern_1 = "Unused argument 'params'"
         local_settings = {
-            "disable": "R0913",
+            "disable": "R0913,R0914",
             "good-names": "ll,ii",
             "ignore_in_line": [pattern_1],
         }
         return local_settings
 
     def get_settings_quantummodel(self):
         """
@@ -410,19 +398,24 @@
         """
         Linter for module ``tensorproductoperator.py``
 
         **Details**
 
         We locally ignore:
 
+        * C0302: too many lines
         * R0902: too many instance attributes
+        * R0912 : too many branches
         * R0913: too many arguments
+        * R0914 : too many locals
+        * R0915 : too many statements
+        * W0212: protected access
         """
         local_settings = {
-            "disable": "R0902,R0913",
+            "disable": "C0302,R0902,R0912,R0913,R0914,R0915,W0212",
         }
         return local_settings
 
     def get_settings_rydberg_model(self):
         """
         Linter for module ``rydberg_model.py``
 
@@ -743,14 +736,18 @@
         * C0103: invalid name
         * E1121: too-many-function-args
         """
         return {
             "disable": "C0103, R0914, E1121",
         }
 
+    # --------------------------------------------------------------------------
+    #                          Settings for emulator
+    # --------------------------------------------------------------------------
+
     @staticmethod
     def get_settings_abstract_tn():
         """
         Linter settings for the abstract tensor network class.
 
         **Details**
 
@@ -762,19 +759,20 @@
         * R0912: too many branches
         * R0913: too many arguments
         * R0914: too many locals
         * R0914: too many statements
         * R0904: too many public methods
         * R1705: no-else-return
         * I1101: c-extension-no-member
+        * W0102: dangerous default value
         * W0108: unnecessary lambda
         """
         return {
-            "disable": "C0302,R0902,R0903,R0912,R0913,R0914,R0915,R1705,R0904,I1101,W0108",
-            "good-names": "tSVD,tEQR,ss,QR",
+            "disable": "C0302,R0902,R0903,R0912,R0913,R0914,R0915,R1705,R0904,I1101,W0108,W0102",
+            "good-names": "tSVD,tEQR,ss,QR,sc",
         }
 
     @staticmethod
     def get_settings_mps_simulator():
         """
         Linter settings for mps simulator.
 
@@ -786,22 +784,23 @@
         * R0904: too many public methods
         * R0912: too maby branhces
         * R0913: too many arguments
         * R0914: too many locals
         * R1720: no-else-raise
         * R1705: no-else-return
         * C0302: too-many-lines
+        * W0212: protected-access
         """
         p1 = """Variable name "addMPS" doesn't conform to snake_case naming style"""
         p2 = """Access to a protected member _cut_ratio of a client class"""
         p3 = """Access to a protected member _singvals of a client class"""
         return {
-            "disable": "R0902,R0904,R0912,R0913,R0914,R1720,R1705,C0302",
+            "disable": "R0902,R0904,R0912,R0913,R0914,R1720,R1705,C0302,W0212",
             "ignore_in_line": [p1, p2, p3],
-            "good-names": "ii, jj, kk, ss, fh, tSVD, UU, Vh, QQ, RR, op",
+            "good-names": "ii, jj, kk, ss, fh, op",
         }
 
     @staticmethod
     def get_settings_mpi_mps_simulator():
         """
         Linter settings for mpimps simulator.
 
@@ -848,39 +847,38 @@
         * R0902: too many instance attributes
         * R0904: too many public methods
         * R0912: too many branches
         * R0913: too many arguments
         * R0914: too many locals
         * R0915: too many statements
         * C0302: too-many-lines
+        * W0102 : dangerous default value
         * W0212: protected-access (needed to avoid duplicate code)
         """
         return {
-            "disable": "C0200,C0302,R0902,R0904,R0912,R0913,R0914,R0915,W0212",
-            "good-names": "ii, jj, kk,ll,i0,i1,i2,d0,d1,d2,p0,p1",
+            "disable": "C0200,C0302,R0902,R0904,R0912,R0913,R0914,R0915,W0102,W0212",
+            "good-names": "ii, jj, kk,ll,i0,i1,i2,d0,d1,d2,p0,p1,sc",
         }
 
     @staticmethod
-    def get_settings_lptn_simulator():
+    def get_settings_attn_simulator():
         """
-        Linter settings for LPTN simulator.
+        Linter settings for TTN simulator.
 
         **Details**
 
         We locally ignore:
 
-        * C0302: too-many-lines
         * R0913: too many arguments
-        * R0914: too many locals
-        * W0105: pointless string statement (raises wanring when using triple
-          quotes for multiline comments)
+        * W0102 : dangerous default value
+        -
         """
         return {
-            "disable": "C0302,R0913,R0914,W0105",
-            "good-names": "ii,jj,kk",
+            "disable": "R0913,W0102",
+            "good-names": "ii, jj, kk",
         }
 
     @staticmethod
     def get_settings_tto_simulator():
         """
         Linter settings for TTO simulator.
 
@@ -897,7 +895,148 @@
           quotes for multiline comments)
         * R0904: too many public methods
         """
         return {
             "disable": "C0302,R0912,R0913,R0914,R0915,W0105,R0904",
             "good-names": "ii,jj,kk",
         }
+
+    @staticmethod
+    def get_settings_symmetrygroups():
+        """
+        Linter settings for symmetry groups
+
+        **Details**
+
+        We locally ignore:
+
+        """
+        return {
+            "disable": "",
+            "good-names": "ii,jj,kk,n1,n2,i1,i2",
+        }
+
+    @staticmethod
+    def get_settings_abstracttensor():
+        """
+        Linter settings for abstract tensors.
+
+        **Details**
+
+        We locally ignore:
+
+        * R0904 : too many public methods
+        * R0913 : too many arguments
+        * W0102 : dangerous default value
+        """
+        return {
+            "disable": "R0904,R0913,W0102",
+            "good-names": "ii,jj,kk,sc",
+        }
+
+    @staticmethod
+    def get_settings_tensor():
+        """
+        Linter settings for tensors.
+
+        **Details**
+
+        We locally ignore:
+
+        * C0302 : too many lines
+        * R0904 : too many public methods
+        * R0913 : too many arguments
+        * R0914 : too many locals
+        * W0102 : dangereous default values
+        * W0212 : protected access
+        """
+        return {
+            "disable": "C0302,R0904,R0913,R0914,W0102,W0212",
+            "good-names": "ii,jj,kk,i1,i2,i3,j1,j2,k1,k2,d1,d2,d3,d4,r1,r2,c1,c2,sc",
+        }
+
+    @staticmethod
+    def get_settings_abeliantensor():
+        """
+        Linter settings for Abelian tensors.
+
+        **Details**
+
+        We locally ignore:
+
+        * C0302: too many lines
+        * R0904 : too many public methods
+        * R0912 : too many branches
+        * R0913 : too many arguments
+        * R0914 : too many locals
+        * R0915 : too many statements
+        * W0102 : dangereous default values
+        * W0212 : protected access
+        """
+        return {
+            "disable": "C0302,R0904,R0912,R0913,R0914,R0915,W0102,W0212",
+            "good-names": "ii,jj,kk,j1,j2,k1,k2,cs,sc",
+        }
+
+    @staticmethod
+    def get_settings_abelianlinks():
+        """
+        Linter settings for ....
+
+        **Details**
+
+        We locally ignore:
+
+        * R0914 : too many locals
+
+        """
+        return {
+            "disable": "R0914",
+            "good-names": "ii,jj,kk,k1,k2,cs",
+        }
+
+    @staticmethod
+    def get_settings_ibarrays():
+        """
+        Linter settings for ibarrays
+
+        **Details**
+
+        We locally ignore:
+
+        """
+        return {
+            "disable": "",
+            "good-names": "ii,jj,kk",
+        }
+
+    @staticmethod
+    def get_settings_couplingsectors():
+        """
+        Linter settings for ....
+
+        **Details**
+
+        We locally ignore:
+
+        * W0102 : dangerous default value
+        """
+        return {
+            "disable": "W0102",
+            "good-names": "d1,d2",
+        }
+
+    @staticmethod
+    def get_settings_irreplistings():
+        """
+        Linter settings for irrep listing
+
+        **Details**
+
+        We locally ignore:
+
+        * R0913: too many arguments
+        """
+        return {
+            "disable": "R0913",
+            "good-names": "ii,jj,kk,n2",
+        }
```

### Comparing `qtealeaves-0.5.14/tests/tests_model_terms.py` & `qtealeaves-1.1.1/tests/tests_model_terms.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_operators.py` & `qtealeaves-1.1.1/tests/tests_operators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_quantum_trajectories.py` & `qtealeaves-1.1.1/tests/tests_quantum_trajectories.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,31 +56,40 @@
             return tmp
 
         model += modeling.LocalTerm("sz", strength="r", prefactor=-1, mask=get_mask)
 
         my_obs = qtl.observables.TNObservables(num_trajectories=3)
         my_obs += qtl.observables.TNObsLocal("sz", "sz")
 
-        quench = qtl.DynamicsQuench([0.05] * 5, time_evolution_mode=2)
+        quench = qtl.DynamicsQuench([0.05] * 5, time_evolution_mode=0)
         quench["r"] = lambda tt, params: 0.5
 
-        simulation = qtl.ATTNSimulation(
+        simulation = qtl.QuantumGreenTeaSimulation(
             model,
             my_ops,
             self.conv,
             my_obs,
             tn_type=0,
-            version_input_processor=3,
             folder_name_input=self.in_folder,
             folder_name_output=self.out_folder,
             has_log_file=True,
             verbosity=False,
+            store_checkpoints=False,
         )
 
-        for elem in [{"L": 8, "J": 1.0, "g": 0.5, "r": 0.0, "Quenches": [quench]}]:
+        for elem in [
+            {
+                "L": 8,
+                "J": 1.0,
+                "g": 0.5,
+                "r": 0.0,
+                "Quenches": [quench],
+                "exclude_from_hash": ["Quenches"],
+            }
+        ]:
             simulation.run(elem, delete_existing_folder=True)
 
             ed_static = simulation.get_static_obs(elem)
             ed_dyn = simulation.get_dynamic_obs(elem)
 
             # Check that we can still access results as before
             energy = ed_static["energy"]
```

### Comparing `qtealeaves-0.5.14/tests/tests_rydberg_model.py` & `qtealeaves-1.1.1/tests/tests_rydberg_model.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-0.5.14/tests/tests_simulation_setup.py` & `qtealeaves-1.1.1/tests/tests_simulation_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,21 +91,20 @@
                 f"Invalid lattice. System dimension cannot be {dim}, only 1 or 2."
             )
 
         symmetry_sector = 0
         tensor_backend = 2 if (symmetry_sector is None) else 1
 
         # Define the simulation
-        simulation = qtl.ATTNSimulation(
+        simulation = qtl.QuantumGreenTeaSimulation(
             model,
             my_ops,
             self.conv_params,
             self.myObs,
             tn_type=2,
-            version_input_processor=3,
             tensor_backend=tensor_backend,
             disentangler=None,
             folder_name_input=self.in_folder,
             folder_name_output=self.out_folder,
             has_log_file=True,
             verbosity=0,
         )
```

