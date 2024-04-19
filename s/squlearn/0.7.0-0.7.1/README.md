# Comparing `tmp/squlearn-0.7.0.tar.gz` & `tmp/squlearn-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squlearn-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "squlearn-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `squlearn-0.7.0.tar` & `squlearn-0.7.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     5514 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2187 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      487 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      532 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/workflows/doc_checks.yml
--rw-r--r--   0        0        0      564 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/workflows/format.yml
--rw-r--r--   0        0        0      679 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1717 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      630 2024-04-18 15:18:51.055120 squlearn-0.7.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0     3314 2024-04-18 15:18:51.055120 squlearn-0.7.0/.gitignore
--rw-r--r--   0        0        0     1452 2024-04-18 15:18:51.055120 squlearn-0.7.0/CITATION.cff
--rw-r--r--   0        0        0    11421 2024-04-18 15:18:51.055120 squlearn-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     3424 2024-04-18 15:18:51.055120 squlearn-0.7.0/README.md
--rw-r--r--   0        0        0      632 2024-04-18 15:18:51.055120 squlearn-0.7.0/docs/Makefile
--rw-r--r--   0        0        0      278 2024-04-18 15:18:51.055120 squlearn-0.7.0/docs/README.md
--rw-r--r--   0        0        0     4126 2024-04-18 15:18:51.055120 squlearn-0.7.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0     2249 2024-04-18 15:18:51.055120 squlearn-0.7.0/docs/_static/favicon.png
--rw-r--r--   0        0        0    12664 2024-04-18 15:18:51.055120 squlearn-0.7.0/docs/_static/logo.png
--rw-r--r--   0        0        0    44296 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_static/qnn/qnn.svg
--rw-r--r--   0        0        0    36032 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_static/schematic.png
--rw-r--r--   0        0        0   121611 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_static/util/executor.png
--rw-r--r--   0        0        0      161 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_templates/class.rst
--rw-r--r--   0        0        0      486 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_templates/class_with_call.rst
--rw-r--r--   0        0        0      165 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/_templates/function.rst
--rw-r--r--   0        0        0     3542 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/conf.py
--rw-r--r--   0        0        0      146 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/examples/example_kernel_digit_classification.nblink
--rw-r--r--   0        0        0       67 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/examples/example_kernel_grid_search.nblink
--rw-r--r--   0        0        0      142 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/examples/example_qnn_backend_mitigation.nblink
--rw-r--r--   0        0        0      148 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/examples/example_quantum_bayesian_optimization.nblink
--rw-r--r--   0        0        0      223 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/examples/examples_index.rst
--rw-r--r--   0        0        0      524 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/index.rst
--rw-r--r--   0        0        0      940 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/install/install.rst
--rw-r--r--   0        0        0     1018 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/make.bat
--rw-r--r--   0        0        0     5764 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/modules/classes.rst
--rw-r--r--   0        0        0       60 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/qiskit_settings.conf
--rw-r--r--   0        0        0      144 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/requirements.txt
--rw-r--r--   0        0        0      461 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0    10216 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/encoding_circuits.rst
--rw-r--r--   0        0        0    13519 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/executor.rst
--rw-r--r--   0        0        0    15401 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/kernel_methods.rst
--rw-r--r--   0        0        0     6098 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/observables.rst
--rw-r--r--   0        0        0    18179 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/quantum_neural_networks.rst
--rw-r--r--   0        0        0      165 2024-04-18 15:18:51.059120 squlearn-0.7.0/docs/user_guide/user_guide_index.rst
--rw-r--r--   0        0        0    96711 2024-04-18 15:18:51.059120 squlearn-0.7.0/examples/encoding_circuits/layered_encoding_circuit.ipynb
--rw-r--r--   0        0        0    23998 2024-04-18 15:18:51.059120 squlearn-0.7.0/examples/encoding_circuits/pruning_example.ipynb
--rw-r--r--   0        0        0   552422 2024-04-18 15:18:51.063120 squlearn-0.7.0/examples/encoding_circuits/various_encoding_circuit.ipynb
--rw-r--r--   0        0        0     9791 2024-04-18 15:18:51.063120 squlearn-0.7.0/examples/executor/example_executor_qiskit.ipynb
--rw-r--r--   0        0        0     7553 2024-04-18 15:18:51.063120 squlearn-0.7.0/examples/integration/mlflow.ipynb
--rw-r--r--   0        0        0    40419 2024-04-18 15:18:51.063120 squlearn-0.7.0/examples/kernel/example_fidelity_kernel.ipynb
--rw-r--r--   0        0        0   392223 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/kernel/example_projected_kernel.ipynb
--rw-r--r--   0        0        0    57347 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/kernel/example_regularization_mitigation.ipynb
--rw-r--r--   0        0        0   132621 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/kernel/qgpc_workflow.ipynb
--rw-r--r--   0        0        0    64202 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/kernel/qgpr_optimization_workflow.ipynb
--rw-r--r--   0        0        0    64741 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/kernel/qgpr_workflow.ipynb
--rw-r--r--   0        0        0    96580 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/qnn/classification_example.ipynb
--rw-r--r--   0        0        0    75008 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/qnn/example_adam.ipynb
--rw-r--r--   0        0        0    76093 2024-04-18 15:18:51.067120 squlearn-0.7.0/examples/qnn/example_minibatch.ipynb
--rw-r--r--   0        0        0   400751 2024-04-18 15:18:51.071120 squlearn-0.7.0/examples/qnn/example_qcnn_encoding_circuit.ipynb
--rw-r--r--   0        0        0   220203 2024-04-18 15:18:51.071120 squlearn-0.7.0/examples/qnn/regression_example.ipynb
--rw-r--r--   0        0        0   194050 2024-04-18 15:18:51.071120 squlearn-0.7.0/examples/qnn/regression_with_variance.ipynb
--rw-r--r--   0        0        0   147762 2024-04-18 15:18:51.075120 squlearn-0.7.0/examples/tutorials/images/encoding_circuit.png
--rw-r--r--   0        0        0    30308 2024-04-18 15:18:51.075120 squlearn-0.7.0/examples/tutorials/images/pipeline.png
--rw-r--r--   0        0        0    97978 2024-04-18 15:18:51.075120 squlearn-0.7.0/examples/tutorials/images/projected_quantum_kernel.png
--rw-r--r--   0        0        0   157564 2024-04-18 15:18:51.075120 squlearn-0.7.0/examples/tutorials/images/quantum_bo.png
--rw-r--r--   0        0        0   503838 2024-04-18 15:18:51.079120 squlearn-0.7.0/examples/tutorials/kernel_digit_classification.ipynb
--rw-r--r--   0        0        0   244971 2024-04-18 15:18:51.079120 squlearn-0.7.0/examples/tutorials/kernel_grid_search.ipynb
--rw-r--r--   0        0        0    90619 2024-04-18 15:18:51.079120 squlearn-0.7.0/examples/tutorials/kernel_regression.ipynb
--rw-r--r--   0        0        0   253985 2024-04-18 15:18:51.079120 squlearn-0.7.0/examples/tutorials/qnn_backend_mitigation.ipynb
--rw-r--r--   0        0        0   745771 2024-04-18 15:18:51.087120 squlearn-0.7.0/examples/tutorials/quantum_bayesian_optimization.ipynb
--rw-r--r--   0        0        0     2034 2024-04-18 15:18:51.087120 squlearn-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      336 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/__init__.py
--rw-r--r--   0        0        0     9625 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
--rw-r--r--   0        0        0     6454 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
--rw-r--r--   0        0        0     7139 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
--rw-r--r--   0        0        0    10302 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
--rw-r--r--   0        0        0     6419 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
--rw-r--r--   0        0        0     5685 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
--rw-r--r--   0        0        0     3808 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
--rw-r--r--   0        0        0    31845 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
--rw-r--r--   0        0        0     8823 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
--rw-r--r--   0        0        0     4555 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
--rw-r--r--   0        0        0    12664 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/encoding_circuit_base.py
--rw-r--r--   0        0        0    13217 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
--rw-r--r--   0        0        0   125558 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/layered_encoding_circuit.py
--rw-r--r--   0        0        0    12914 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
--rw-r--r--   0        0        0     7106 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
--rw-r--r--   0        0        0      315 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/__init__.py
--rw-r--r--   0        0        0      161 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/__init__.py
--rw-r--r--   0        0        0    13444 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/fidelity_kernel.py
--rw-r--r--   0        0        0    12641 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
--rw-r--r--   0        0        0    15109 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/kernel_matrix_base.py
--rw-r--r--   0        0        0     1237 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/kernel_util.py
--rw-r--r--   0        0        0    28126 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py
--rw-r--r--   0        0        0     2626 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/matrix/regularization.py
--rw-r--r--   0        0        0      168 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/__init__.py
--rw-r--r--   0        0        0     5636 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/qgpc.py
--rw-r--r--   0        0        0    12897 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/qgpr.py
--rw-r--r--   0        0        0     9115 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/qkrr.py
--rw-r--r--   0        0        0     5972 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/qsvc.py
--rw-r--r--   0        0        0     5940 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/ml/qsvr.py
--rw-r--r--   0        0        0      190 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/__init__.py
--rw-r--r--   0        0        0      646 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_loss_base.py
--rw-r--r--   0        0        0     1323 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_optimization_base.py
--rw-r--r--   0        0        0     3675 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_optimizer.py
--rw-r--r--   0        0        0     2811 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/negative_log_likelihood.py
--rw-r--r--   0        0        0     2648 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/kernel/optimization/target_alignment.py
--rw-r--r--   0        0        0      579 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/__init__.py
--rw-r--r--   0        0        0    18957 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_base.py
--rw-r--r--   0        0        0    13837 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_derivatives.py
--rw-r--r--   0        0        0        0 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/__init__.py
--rw-r--r--   0        0        0     4154 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/custom_observable.py
--rw-r--r--   0        0        0     6619 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
--rw-r--r--   0        0        0     3331 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/single_pauli.py
--rw-r--r--   0        0        0     3449 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/single_probability.py
--rw-r--r--   0        0        0     4602 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/summed_paulis.py
--rw-r--r--   0        0        0     4433 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/observables/observable_implemented/summed_probabilities.py
--rw-r--r--   0        0        0      350 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/optimizers/__init__.py
--rw-r--r--   0        0        0     7904 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/optimizers/adam.py
--rw-r--r--   0        0        0     4606 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/optimizers/approximated_gradients.py
--rw-r--r--   0        0        0     2822 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/optimizers/optimizer_base.py
--rw-r--r--   0        0        0     6830 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/optimizers/optimizers_wrapper.py
--rw-r--r--   0        0        0      486 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/qnn/__init__.py
--rw-r--r--   0        0        0     8625 2024-04-18 15:18:51.087120 squlearn-0.7.0/src/squlearn/qnn/barren_plateau_analysis.py
--rw-r--r--   0        0        0    12397 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/base_qnn.py
--rw-r--r--   0        0        0    28576 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/loss.py
--rw-r--r--   0        0        0     1650 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn.py
--rw-r--r--   0        0        0     4928 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_base.py
--rw-r--r--   0        0        0    38214 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_pennylane.py
--rw-r--r--   0        0        0    44856 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_qiskit.py
--rw-r--r--   0        0        0    10052 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/qnnc.py
--rw-r--r--   0        0        0     9069 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/qnnr.py
--rw-r--r--   0        0        0    19726 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/qnn/training.py
--rw-r--r--   0        0        0       92 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/__init__.py
--rw-r--r--   0        0        0     3841 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/data_preprocessing.py
--rw-r--r--   0        0        0    73387 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/executor.py
--rw-r--r--   0        0        0      548 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/optree/__init__.py
--rw-r--r--   0        0        0    32033 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/optree/optree.py
--rw-r--r--   0        0        0    17472 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/optree/optree_derivative.py
--rw-r--r--   0        0        0    69561 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/optree/optree_evaluate.py
--rw-r--r--   0        0        0      166 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/pennylane/__init__.py
--rw-r--r--   0        0        0    24901 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/pennylane/pennylane_circuit.py
--rw-r--r--   0        0        0     1905 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/pennylane/pennylane_gates.py
--rw-r--r--   0        0        0     7776 2024-04-18 15:18:51.091120 squlearn-0.7.0/src/squlearn/util/qfi.py
--rw-r--r--   0        0        0     9207 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/encoding_circuit/test_layered_encoding_circuit.py
--rw-r--r--   0        0        0     6832 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/kernel/ml/test_qgpc.py
--rw-r--r--   0        0        0     7604 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/kernel/ml/test_qgpr.py
--rw-r--r--   0        0        0     6249 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/kernel/ml/test_qkrr.py
--rw-r--r--   0        0        0     6812 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/kernel/ml/test_qsvc.py
--rw-r--r--   0        0        0     6811 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/kernel/ml/test_qsvr.py
--rw-r--r--   0        0        0     4953 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/qnn/test_base_qnn.py
--rw-r--r--   0        0        0     7013 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/qnn/test_qnnc.py
--rw-r--r--   0        0        0     7055 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/qnn/test_qnnr.py
--rw-r--r--   0        0        0     6768 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/qnn/test_training.py
--rw-r--r--   0        0        0     5527 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/util/optree/test_optree_derivative.py
--rw-r--r--   0        0        0     9928 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/util/optree/test_optree_evaluate.py
--rw-r--r--   0        0        0     7337 2024-04-18 15:18:51.091120 squlearn-0.7.0/tests/util/test_executor.py
--rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 squlearn-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5514 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2187 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      487 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      532 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/doc_checks.yml
+-rw-r--r--   0        0        0      564 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/format.yml
+-rw-r--r--   0        0        0      679 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1717 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      630 2024-04-19 13:32:49.108146 squlearn-0.7.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0     3314 2024-04-19 13:32:49.108146 squlearn-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1452 2024-04-19 13:32:49.108146 squlearn-0.7.1/CITATION.cff
+-rw-r--r--   0        0        0    11421 2024-04-19 13:32:49.108146 squlearn-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     3424 2024-04-19 13:32:49.108146 squlearn-0.7.1/README.md
+-rw-r--r--   0        0        0      632 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0      278 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/README.md
+-rw-r--r--   0        0        0     4126 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     2249 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/favicon.png
+-rw-r--r--   0        0        0    12664 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/logo.png
+-rw-r--r--   0        0        0    44296 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/qnn/qnn.svg
+-rw-r--r--   0        0        0    36032 2024-04-19 13:32:49.108146 squlearn-0.7.1/docs/_static/schematic.png
+-rw-r--r--   0        0        0   121611 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_static/util/executor.png
+-rw-r--r--   0        0        0      161 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/class.rst
+-rw-r--r--   0        0        0      486 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/class_with_call.rst
+-rw-r--r--   0        0        0      165 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/_templates/function.rst
+-rw-r--r--   0        0        0     3542 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0      146 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_kernel_digit_classification.nblink
+-rw-r--r--   0        0        0       67 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_kernel_grid_search.nblink
+-rw-r--r--   0        0        0      142 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_qnn_backend_mitigation.nblink
+-rw-r--r--   0        0        0      148 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/example_quantum_bayesian_optimization.nblink
+-rw-r--r--   0        0        0      223 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/examples/examples_index.rst
+-rw-r--r--   0        0        0      524 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0      940 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/install/install.rst
+-rw-r--r--   0        0        0     1018 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0     5764 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/modules/classes.rst
+-rw-r--r--   0        0        0       60 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/qiskit_settings.conf
+-rw-r--r--   0        0        0      144 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/requirements.txt
+-rw-r--r--   0        0        0      461 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0    10216 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/encoding_circuits.rst
+-rw-r--r--   0        0        0    13519 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/executor.rst
+-rw-r--r--   0        0        0    15401 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/kernel_methods.rst
+-rw-r--r--   0        0        0     6098 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/observables.rst
+-rw-r--r--   0        0        0    18179 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/quantum_neural_networks.rst
+-rw-r--r--   0        0        0      165 2024-04-19 13:32:49.112146 squlearn-0.7.1/docs/user_guide/user_guide_index.rst
+-rw-r--r--   0        0        0    96711 2024-04-19 13:32:49.112146 squlearn-0.7.1/examples/encoding_circuits/layered_encoding_circuit.ipynb
+-rw-r--r--   0        0        0    23998 2024-04-19 13:32:49.112146 squlearn-0.7.1/examples/encoding_circuits/pruning_example.ipynb
+-rw-r--r--   0        0        0   552422 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/encoding_circuits/various_encoding_circuit.ipynb
+-rw-r--r--   0        0        0     9791 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/executor/example_executor_qiskit.ipynb
+-rw-r--r--   0        0        0     7553 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/integration/mlflow.ipynb
+-rw-r--r--   0        0        0    40419 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_fidelity_kernel.ipynb
+-rw-r--r--   0        0        0   392223 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_projected_kernel.ipynb
+-rw-r--r--   0        0        0    57347 2024-04-19 13:32:49.116146 squlearn-0.7.1/examples/kernel/example_regularization_mitigation.ipynb
+-rw-r--r--   0        0        0   132621 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpc_workflow.ipynb
+-rw-r--r--   0        0        0    64202 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpr_optimization_workflow.ipynb
+-rw-r--r--   0        0        0    64741 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/kernel/qgpr_workflow.ipynb
+-rw-r--r--   0        0        0    96580 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/classification_example.ipynb
+-rw-r--r--   0        0        0    75008 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/example_adam.ipynb
+-rw-r--r--   0        0        0    76093 2024-04-19 13:32:49.120146 squlearn-0.7.1/examples/qnn/example_minibatch.ipynb
+-rw-r--r--   0        0        0   400751 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/example_qcnn_encoding_circuit.ipynb
+-rw-r--r--   0        0        0   220203 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/regression_example.ipynb
+-rw-r--r--   0        0        0   194050 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/qnn/regression_with_variance.ipynb
+-rw-r--r--   0        0        0   147762 2024-04-19 13:32:49.124146 squlearn-0.7.1/examples/tutorials/images/encoding_circuit.png
+-rw-r--r--   0        0        0    30308 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/pipeline.png
+-rw-r--r--   0        0        0    97978 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/projected_quantum_kernel.png
+-rw-r--r--   0        0        0   157564 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/images/quantum_bo.png
+-rw-r--r--   0        0        0   503838 2024-04-19 13:32:49.128146 squlearn-0.7.1/examples/tutorials/kernel_digit_classification.ipynb
+-rw-r--r--   0        0        0   244971 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/kernel_grid_search.ipynb
+-rw-r--r--   0        0        0    90619 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/kernel_regression.ipynb
+-rw-r--r--   0        0        0   253985 2024-04-19 13:32:49.132146 squlearn-0.7.1/examples/tutorials/qnn_backend_mitigation.ipynb
+-rw-r--r--   0        0        0   745771 2024-04-19 13:32:49.136146 squlearn-0.7.1/examples/tutorials/quantum_bayesian_optimization.ipynb
+-rw-r--r--   0        0        0     2034 2024-04-19 13:32:49.136146 squlearn-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/__init__.py
+-rw-r--r--   0        0        0     9625 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py
+-rw-r--r--   0        0        0     6454 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py
+-rw-r--r--   0        0        0     7139 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py
+-rw-r--r--   0        0        0    10302 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py
+-rw-r--r--   0        0        0     6419 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py
+-rw-r--r--   0        0        0     5685 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py
+-rw-r--r--   0        0        0     3808 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py
+-rw-r--r--   0        0        0    31845 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py
+-rw-r--r--   0        0        0     8823 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py
+-rw-r--r--   0        0        0     4555 2024-04-19 13:32:49.136146 squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py
+-rw-r--r--   0        0        0    12664 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_base.py
+-rw-r--r--   0        0        0    13217 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py
+-rw-r--r--   0        0        0   125558 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/layered_encoding_circuit.py
+-rw-r--r--   0        0        0    12914 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/pruned_encoding_circuit.py
+-rw-r--r--   0        0        0     7106 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py
+-rw-r--r--   0        0        0      315 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/__init__.py
+-rw-r--r--   0        0        0      161 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/__init__.py
+-rw-r--r--   0        0        0    13444 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel.py
+-rw-r--r--   0        0        0    12641 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py
+-rw-r--r--   0        0        0    15109 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_matrix_base.py
+-rw-r--r--   0        0        0     1237 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_util.py
+-rw-r--r--   0        0        0    28126 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/projected_quantum_kernel.py
+-rw-r--r--   0        0        0     2626 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/matrix/regularization.py
+-rw-r--r--   0        0        0      168 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/__init__.py
+-rw-r--r--   0        0        0     5636 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qgpc.py
+-rw-r--r--   0        0        0    12897 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qgpr.py
+-rw-r--r--   0        0        0     9115 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qkrr.py
+-rw-r--r--   0        0        0     5972 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qsvc.py
+-rw-r--r--   0        0        0     5940 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/ml/qsvr.py
+-rw-r--r--   0        0        0      190 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/__init__.py
+-rw-r--r--   0        0        0      646 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_loss_base.py
+-rw-r--r--   0        0        0     1323 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimization_base.py
+-rw-r--r--   0        0        0     3675 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimizer.py
+-rw-r--r--   0        0        0     2811 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/negative_log_likelihood.py
+-rw-r--r--   0        0        0     2648 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/kernel/optimization/target_alignment.py
+-rw-r--r--   0        0        0      579 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/__init__.py
+-rw-r--r--   0        0        0    18957 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_base.py
+-rw-r--r--   0        0        0    13837 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_derivatives.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/__init__.py
+-rw-r--r--   0        0        0     4154 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/custom_observable.py
+-rw-r--r--   0        0        0     6619 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/ising_hamiltonian.py
+-rw-r--r--   0        0        0     3331 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_pauli.py
+-rw-r--r--   0        0        0     3449 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_probability.py
+-rw-r--r--   0        0        0     4602 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_paulis.py
+-rw-r--r--   0        0        0     4433 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_probabilities.py
+-rw-r--r--   0        0        0      350 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/__init__.py
+-rw-r--r--   0        0        0     7904 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/adam.py
+-rw-r--r--   0        0        0     4606 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/approximated_gradients.py
+-rw-r--r--   0        0        0     2822 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/optimizer_base.py
+-rw-r--r--   0        0        0     6830 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/optimizers/optimizers_wrapper.py
+-rw-r--r--   0        0        0      486 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/__init__.py
+-rw-r--r--   0        0        0     8625 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/barren_plateau_analysis.py
+-rw-r--r--   0        0        0    12397 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/base_qnn.py
+-rw-r--r--   0        0        0    28576 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/loss.py
+-rw-r--r--   0        0        0     1650 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn.py
+-rw-r--r--   0        0        0     4928 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_base.py
+-rw-r--r--   0        0        0    38214 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_pennylane.py
+-rw-r--r--   0        0        0    44856 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_qiskit.py
+-rw-r--r--   0        0        0    10052 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/qnnc.py
+-rw-r--r--   0        0        0     9069 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/qnnr.py
+-rw-r--r--   0        0        0    19726 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/qnn/training.py
+-rw-r--r--   0        0        0       92 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/util/__init__.py
+-rw-r--r--   0        0        0     3841 2024-04-19 13:32:49.140146 squlearn-0.7.1/src/squlearn/util/data_preprocessing.py
+-rw-r--r--   0        0        0    73387 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/executor.py
+-rw-r--r--   0        0        0      548 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/__init__.py
+-rw-r--r--   0        0        0    32033 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree.py
+-rw-r--r--   0        0        0    17472 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree_derivative.py
+-rw-r--r--   0        0        0    69544 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/optree/optree_evaluate.py
+-rw-r--r--   0        0        0      166 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/__init__.py
+-rw-r--r--   0        0        0    24901 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_circuit.py
+-rw-r--r--   0        0        0     1905 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_gates.py
+-rw-r--r--   0        0        0     7776 2024-04-19 13:32:49.144146 squlearn-0.7.1/src/squlearn/util/qfi.py
+-rw-r--r--   0        0        0     9207 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/encoding_circuit/test_layered_encoding_circuit.py
+-rw-r--r--   0        0        0     6832 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qgpc.py
+-rw-r--r--   0        0        0     7604 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qgpr.py
+-rw-r--r--   0        0        0     6249 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qkrr.py
+-rw-r--r--   0        0        0     6812 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qsvc.py
+-rw-r--r--   0        0        0     6811 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/kernel/ml/test_qsvr.py
+-rw-r--r--   0        0        0     4953 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_base_qnn.py
+-rw-r--r--   0        0        0     7013 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_qnnc.py
+-rw-r--r--   0        0        0     7055 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_qnnr.py
+-rw-r--r--   0        0        0     6768 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/qnn/test_training.py
+-rw-r--r--   0        0        0     5527 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/optree/test_optree_derivative.py
+-rw-r--r--   0        0        0     9928 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/optree/test_optree_evaluate.py
+-rw-r--r--   0        0        0     7337 2024-04-19 13:32:49.144146 squlearn-0.7.1/tests/util/test_executor.py
+-rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 squlearn-0.7.1/PKG-INFO
```

### Comparing `squlearn-0.7.0/.github/CODE_OF_CONDUCT.md` & `squlearn-0.7.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/CONTRIBUTING.md` & `squlearn-0.7.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `squlearn-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/workflows/doc_checks.yml` & `squlearn-0.7.1/.github/workflows/doc_checks.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/workflows/format.yml` & `squlearn-0.7.1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/workflows/publish.yml` & `squlearn-0.7.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/workflows/publish_docs.yml` & `squlearn-0.7.1/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.github/workflows/tests.yaml` & `squlearn-0.7.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/.gitignore` & `squlearn-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/CITATION.cff` & `squlearn-0.7.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/LICENSE.txt` & `squlearn-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/README.md` & `squlearn-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/Makefile` & `squlearn-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/css/custom.css` & `squlearn-0.7.1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/favicon.png` & `squlearn-0.7.1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/logo.png` & `squlearn-0.7.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/qnn/qnn.svg` & `squlearn-0.7.1/docs/_static/qnn/qnn.svg`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/schematic.png` & `squlearn-0.7.1/docs/_static/schematic.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/_static/util/executor.png` & `squlearn-0.7.1/docs/_static/util/executor.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/conf.py` & `squlearn-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/index.rst` & `squlearn-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/install/install.rst` & `squlearn-0.7.1/docs/install/install.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/make.bat` & `squlearn-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/modules/classes.rst` & `squlearn-0.7.1/docs/modules/classes.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/user_guide/encoding_circuits.rst` & `squlearn-0.7.1/docs/user_guide/encoding_circuits.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/user_guide/executor.rst` & `squlearn-0.7.1/docs/user_guide/executor.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/user_guide/kernel_methods.rst` & `squlearn-0.7.1/docs/user_guide/kernel_methods.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/user_guide/observables.rst` & `squlearn-0.7.1/docs/user_guide/observables.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/docs/user_guide/quantum_neural_networks.rst` & `squlearn-0.7.1/docs/user_guide/quantum_neural_networks.rst`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/encoding_circuits/layered_encoding_circuit.ipynb` & `squlearn-0.7.1/examples/encoding_circuits/layered_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/encoding_circuits/pruning_example.ipynb` & `squlearn-0.7.1/examples/encoding_circuits/pruning_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/encoding_circuits/various_encoding_circuit.ipynb` & `squlearn-0.7.1/examples/encoding_circuits/various_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/executor/example_executor_qiskit.ipynb` & `squlearn-0.7.1/examples/executor/example_executor_qiskit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/integration/mlflow.ipynb` & `squlearn-0.7.1/examples/integration/mlflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/example_fidelity_kernel.ipynb` & `squlearn-0.7.1/examples/kernel/example_fidelity_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/example_projected_kernel.ipynb` & `squlearn-0.7.1/examples/kernel/example_projected_kernel.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/example_regularization_mitigation.ipynb` & `squlearn-0.7.1/examples/kernel/example_regularization_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/qgpc_workflow.ipynb` & `squlearn-0.7.1/examples/kernel/qgpc_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/qgpr_optimization_workflow.ipynb` & `squlearn-0.7.1/examples/kernel/qgpr_optimization_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/kernel/qgpr_workflow.ipynb` & `squlearn-0.7.1/examples/kernel/qgpr_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/classification_example.ipynb` & `squlearn-0.7.1/examples/qnn/classification_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/example_adam.ipynb` & `squlearn-0.7.1/examples/qnn/example_adam.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/example_minibatch.ipynb` & `squlearn-0.7.1/examples/qnn/example_minibatch.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/example_qcnn_encoding_circuit.ipynb` & `squlearn-0.7.1/examples/qnn/example_qcnn_encoding_circuit.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/regression_example.ipynb` & `squlearn-0.7.1/examples/qnn/regression_example.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/qnn/regression_with_variance.ipynb` & `squlearn-0.7.1/examples/qnn/regression_with_variance.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/images/encoding_circuit.png` & `squlearn-0.7.1/examples/tutorials/images/encoding_circuit.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/images/pipeline.png` & `squlearn-0.7.1/examples/tutorials/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/images/projected_quantum_kernel.png` & `squlearn-0.7.1/examples/tutorials/images/projected_quantum_kernel.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/images/quantum_bo.png` & `squlearn-0.7.1/examples/tutorials/images/quantum_bo.png`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/kernel_digit_classification.ipynb` & `squlearn-0.7.1/examples/tutorials/kernel_digit_classification.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/kernel_grid_search.ipynb` & `squlearn-0.7.1/examples/tutorials/kernel_grid_search.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/kernel_regression.ipynb` & `squlearn-0.7.1/examples/tutorials/kernel_regression.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/qnn_backend_mitigation.ipynb` & `squlearn-0.7.1/examples/tutorials/qnn_backend_mitigation.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/examples/tutorials/quantum_bayesian_optimization.ipynb` & `squlearn-0.7.1/examples/tutorials/quantum_bayesian_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/pyproject.toml` & `squlearn-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/__init__.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_pqc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_rx.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/chebyshev_tower.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/highdim_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/hubregtsen_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/multi_control_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/param_z_feature_map.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qcnn_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/qiskit_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/circuit_library/yz_cx_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/encoding_circuit_base.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/encoding_circuit_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/layered_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/pruned_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/pruned_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py` & `squlearn-0.7.1/src/squlearn/encoding_circuit/transpiled_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/fidelity_kernel.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/fidelity_kernel_pennylane.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/kernel_matrix_base.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_matrix_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/kernel_util.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/kernel_util.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/projected_quantum_kernel.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/matrix/regularization.py` & `squlearn-0.7.1/src/squlearn/kernel/matrix/regularization.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/ml/qgpc.py` & `squlearn-0.7.1/src/squlearn/kernel/ml/qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/ml/qgpr.py` & `squlearn-0.7.1/src/squlearn/kernel/ml/qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/ml/qkrr.py` & `squlearn-0.7.1/src/squlearn/kernel/ml/qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/ml/qsvc.py` & `squlearn-0.7.1/src/squlearn/kernel/ml/qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/ml/qsvr.py` & `squlearn-0.7.1/src/squlearn/kernel/ml/qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_loss_base.py` & `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_loss_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_optimization_base.py` & `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimization_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/optimization/kernel_optimizer.py` & `squlearn-0.7.1/src/squlearn/kernel/optimization/kernel_optimizer.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/optimization/negative_log_likelihood.py` & `squlearn-0.7.1/src/squlearn/kernel/optimization/negative_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/kernel/optimization/target_alignment.py` & `squlearn-0.7.1/src/squlearn/kernel/optimization/target_alignment.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/__init__.py` & `squlearn-0.7.1/src/squlearn/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_base.py` & `squlearn-0.7.1/src/squlearn/observables/observable_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_derivatives.py` & `squlearn-0.7.1/src/squlearn/observables/observable_derivatives.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/custom_observable.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/custom_observable.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/ising_hamiltonian.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/single_pauli.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_pauli.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/single_probability.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/single_probability.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/summed_paulis.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_paulis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/observables/observable_implemented/summed_probabilities.py` & `squlearn-0.7.1/src/squlearn/observables/observable_implemented/summed_probabilities.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/optimizers/adam.py` & `squlearn-0.7.1/src/squlearn/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/optimizers/approximated_gradients.py` & `squlearn-0.7.1/src/squlearn/optimizers/approximated_gradients.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/optimizers/optimizer_base.py` & `squlearn-0.7.1/src/squlearn/optimizers/optimizer_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/optimizers/optimizers_wrapper.py` & `squlearn-0.7.1/src/squlearn/optimizers/optimizers_wrapper.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/barren_plateau_analysis.py` & `squlearn-0.7.1/src/squlearn/qnn/barren_plateau_analysis.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/base_qnn.py` & `squlearn-0.7.1/src/squlearn/qnn/base_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/loss.py` & `squlearn-0.7.1/src/squlearn/qnn/loss.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn.py` & `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_base.py` & `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_base.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_pennylane.py` & `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_pennylane.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/lowlevel_qnn_qiskit.py` & `squlearn-0.7.1/src/squlearn/qnn/lowlevel_qnn_qiskit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/qnnc.py` & `squlearn-0.7.1/src/squlearn/qnn/qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/qnnr.py` & `squlearn-0.7.1/src/squlearn/qnn/qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/qnn/training.py` & `squlearn-0.7.1/src/squlearn/qnn/training.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/data_preprocessing.py` & `squlearn-0.7.1/src/squlearn/util/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/executor.py` & `squlearn-0.7.1/src/squlearn/util/executor.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/optree/__init__.py` & `squlearn-0.7.1/src/squlearn/util/optree/__init__.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/optree/optree.py` & `squlearn-0.7.1/src/squlearn/util/optree/optree.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/optree/optree_derivative.py` & `squlearn-0.7.1/src/squlearn/util/optree/optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/optree/optree_evaluate.py` & `squlearn-0.7.1/src/squlearn/util/optree/optree_evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,15 +751,14 @@
 
     # Create a list of PauliList objects from the observable
     op_pauli_list = [PauliList(obs.paulis) for obs in operator]
 
     # Check if only the Z and I Paulis are used in the observable
     # Too late for a basis change
     for p in op_pauli_list:
-        print(p)
         if p.x.any():
             raise ValueError(
                 "Observable only with Z and I Paulis are supported, "
                 + "run transform_to_zbasis first"
             )
 
     # If no measurement is present, create one where every circuit is connected to all
```

### Comparing `squlearn-0.7.0/src/squlearn/util/pennylane/pennylane_circuit.py` & `squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/pennylane/pennylane_gates.py` & `squlearn-0.7.1/src/squlearn/util/pennylane/pennylane_gates.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/src/squlearn/util/qfi.py` & `squlearn-0.7.1/src/squlearn/util/qfi.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/encoding_circuit/test_layered_encoding_circuit.py` & `squlearn-0.7.1/tests/encoding_circuit/test_layered_encoding_circuit.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/kernel/ml/test_qgpc.py` & `squlearn-0.7.1/tests/kernel/ml/test_qgpc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/kernel/ml/test_qgpr.py` & `squlearn-0.7.1/tests/kernel/ml/test_qgpr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/kernel/ml/test_qkrr.py` & `squlearn-0.7.1/tests/kernel/ml/test_qkrr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/kernel/ml/test_qsvc.py` & `squlearn-0.7.1/tests/kernel/ml/test_qsvc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/kernel/ml/test_qsvr.py` & `squlearn-0.7.1/tests/kernel/ml/test_qsvr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/qnn/test_base_qnn.py` & `squlearn-0.7.1/tests/qnn/test_base_qnn.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/qnn/test_qnnc.py` & `squlearn-0.7.1/tests/qnn/test_qnnc.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/qnn/test_qnnr.py` & `squlearn-0.7.1/tests/qnn/test_qnnr.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/qnn/test_training.py` & `squlearn-0.7.1/tests/qnn/test_training.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/util/optree/test_optree_derivative.py` & `squlearn-0.7.1/tests/util/optree/test_optree_derivative.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/util/optree/test_optree_evaluate.py` & `squlearn-0.7.1/tests/util/optree/test_optree_evaluate.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/tests/util/test_executor.py` & `squlearn-0.7.1/tests/util/test_executor.py`

 * *Files identical despite different names*

### Comparing `squlearn-0.7.0/PKG-INFO` & `squlearn-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squlearn
-Version: 0.7.0
+Version: 0.7.1
 Summary: A library for quantum machine learning following the scikit-learnstandard.
 Keywords: quantum,machine learning,qml
 Author-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Frederic Rapp <frederic.rapp@ipa.fraunhofer.de>, Marco Roth <marco.roth@ipa.fraunhofer.de>, Jan Schnabel <jan.schnabel@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
 Maintainer-email: David Kreplin <david.kreplin@ipa.fraunhofer.de>, Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
```

