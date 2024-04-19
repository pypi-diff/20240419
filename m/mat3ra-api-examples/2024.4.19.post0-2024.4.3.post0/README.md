# Comparing `tmp/mat3ra_api_examples-2024.4.19.post0.tar.gz` & `tmp/mat3ra-api-examples-2024.4.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_api_examples-2024.4.19.post0.tar", last modified: Fri Apr 19 05:11:26 2024, max compression
+gzip compressed data, was "mat3ra-api-examples-2024.4.3.post0.tar", last modified: Wed Apr  3 18:31:48 2024, max compression
```

## Comparing `mat3ra_api_examples-2024.4.19.post0.tar` & `mat3ra-api-examples-2024.4.3.post0.tar`

### file list

```diff
@@ -1,139 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.599039 mat3ra_api_examples-2024.4.19.post0/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.575039 mat3ra_api_examples-2024.4.19.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.579038 mat3ra_api_examples-2024.4.19.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.github/workflows/check_links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.github/workflows/zip_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.lycheeignore
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-04-19 05:11:26.599039 mat3ra_api_examples-2024.4.19.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/README.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.579038 mat3ra_api_examples-2024.4.19.post0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/assets/Si.pz-vbc.UPF
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/assets/bash_workflow_template.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/assets/mp-978534.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/examples/job/
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/create_and_submit_job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/create_and_submit_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/get-file-from-job.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/get-file-from-job.py
--rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/ml-train-model-predict-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/ml-train-model-predict-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/run-simulations-and-extract-properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/job/run-simulations-and-extract-properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/examples/material/
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/create_material.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/create_material.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/get_materials_by_formula.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/get_materials_by_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/upload_materials_from_file_poscar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/material/upload_materials_from_file_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/examples/system/
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/system/get_authentication_params.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/system/get_authentication_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/examples/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/workflow/get_workflows.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/workflow/get_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/workflow/qe_scf_calculation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/examples/workflow/qe_scf_calculation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.575039 mat3ra_api_examples-2024.4.19.post0/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/extra/css/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/extra/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.583039 mat3ra_api_examples-2024.4.19.post0/images/
--rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/images/reusable-kernel.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 05:11:26.000000 mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.587039 mat3ra_api_examples-2024.4.19.post0/other/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.587039 mat3ra_api_examples-2024.4.19.post0/other/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/bitter-sweet.csv
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/bittersweet_xgboost.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/deepchem_smiles_vocab.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/gamma_alumina_digne_et_al.poscar
--rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/assets/sci_adv_dean_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.587039 mat3ra_api_examples-2024.4.19.post0/other/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.587039 mat3ra_api_examples-2024.4.19.post0/other/experiments/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/uploads/Gr.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/experiments/uploads/Ni.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/jarvis/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/job/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/job/Smiles_Generation_Markov_Chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/neural_network_train.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/machine_learning/neural_network_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/import_materials_from_files.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/uploads/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materials_designer/uploads/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.591039 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/api_interoperability_showcase.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/api_interoperability_showcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/import_materials_from_materialsproject.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/materialsproject/import_materials_from_materialsproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/1_layer_on_substrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/2_strain_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/3_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/4_custom_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/python_transformations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/other/webinar/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/adsorption-study.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/adsorption-study.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/generate-al2o3-slab-structures.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/generate-al2o3-slab-structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/predict_with_machine_learning.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/predict_with_machine_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/scripts/change-branch-in-urls.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/scripts/env.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/scripts/render-notebooks.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 05:11:26.599039 mat3ra_api_examples-2024.4.19.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/jupyterlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 05:11:26.595039 mat3ra_api_examples-2024.4.19.post0/utils/web/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/web/renderjson.css
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/utils/web/renderjson.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-19 05:10:51.000000 mat3ra_api_examples-2024.4.19.post0/wheel_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.118079 mat3ra-api-examples-2024.4.3.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/check_links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.lycheeignore
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/Si.pz-vbc.UPF
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/assets/mp-978534.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.126079 mat3ra-api-examples-2024.4.3.post0/examples/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15961 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21116 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21904 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/material/
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/examples/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.122079 mat3ra-api-examples-2024.4.3.post0/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/extra/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/extra/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   413869 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 18:31:48.000000 mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.130079 mat3ra-api-examples-2024.4.3.post0/other/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   638208 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/bittersweet_xgboost.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/deepchem_smiles_vocab.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12157 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)    25385 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24590 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24750 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/jarvis/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16800 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30016 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12408 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.134079 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materials_designer/uploads/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10185 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/other/webinar/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/env.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2267 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:48.142079 mat3ra-api-examples-2024.4.3.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:48.138079 mat3ra-api-examples-2024.4.3.post0/utils/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 18:30:40.000000 mat3ra-api-examples-2024.4.3.post0/wheel_server.py
```

### Comparing `mat3ra_api_examples-2024.4.19.post0/.gitattributes` & `mat3ra-api-examples-2024.4.3.post0/.gitattributes`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/.github/workflows/cicd.yml` & `mat3ra-api-examples-2024.4.3.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/.github/workflows/zip_release.yml` & `mat3ra-api-examples-2024.4.3.post0/.github/workflows/zip_release.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/.gitignore` & `mat3ra-api-examples-2024.4.3.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/PKG-INFO` & `mat3ra-api-examples-2024.4.3.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.19.post0
+Version: 2024.4.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
```

### Comparing `mat3ra_api_examples-2024.4.19.post0/README.md` & `mat3ra-api-examples-2024.4.3.post0/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/config.yml` & `mat3ra-api-examples-2024.4.3.post0/config.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/assets/bash_workflow_template.json` & `mat3ra-api-examples-2024.4.3.post0/examples/assets/bash_workflow_template.json`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/config.py` & `mat3ra-api-examples-2024.4.3.post0/examples/config.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/create_and_submit_job.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/create_and_submit_job.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/create_and_submit_job.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/get-file-from-job.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/get-file-from-job.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/get-file-from-job.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/ml-train-model-predict-properties.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/ml-train-model-predict-properties.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/ml-train-model-predict-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/run-simulations-and-extract-properties.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/job/run-simulations-and-extract-properties.py` & `mat3ra-api-examples-2024.4.3.post0/examples/job/run-simulations-and-extract-properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/create_material.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/create_material.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/create_material.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/get_materials_by_formula.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/get_materials_by_formula.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/get_materials_by_formula.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/upload_materials_from_file_poscar.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/material/upload_materials_from_file_poscar.py` & `mat3ra-api-examples-2024.4.3.post0/examples/material/upload_materials_from_file_poscar.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/system/get_authentication_params.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/system/get_authentication_params.py` & `mat3ra-api-examples-2024.4.3.post0/examples/system/get_authentication_params.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/workflow/get_workflows.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/workflow/get_workflows.py` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/get_workflows.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/workflow/qe_scf_calculation.ipynb` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/examples/workflow/qe_scf_calculation.py` & `mat3ra-api-examples-2024.4.3.post0/examples/workflow/qe_scf_calculation.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/images/reusable-kernel.png` & `mat3ra-api-examples-2024.4.3.post0/images/reusable-kernel.png`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/PKG-INFO` & `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-api-examples
-Version: 2024.4.19.post0
+Version: 2024.4.3.post0
 Summary: Mat3ra API Examples
 Project-URL: homepage, https://exabyte-io.github.io/api-examples
 Project-URL: documentation, https://exabyte-io.github.io/api-examples
 Project-URL: repository, https://github.com/Exabyte-io/api-examples
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ase>=3.21.1
```

### Comparing `mat3ra_api_examples-2024.4.19.post0/mat3ra_api_examples.egg-info/SOURCES.txt` & `mat3ra-api-examples-2024.4.3.post0/mat3ra_api_examples.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitattributes
 .gitignore
 .lycheeignore
 .pre-commit-config.yaml
-README.ipynb
 README.md
 config.yml
 mkdocs.yml
 pyproject.toml
 wheel_server.py
 .github/workflows/check_links.yml
 .github/workflows/cicd.yml
```

### Comparing `mat3ra_api_examples-2024.4.19.post0/mkdocs.yml` & `mat3ra-api-examples-2024.4.3.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/assets/README.md` & `mat3ra-api-examples-2024.4.3.post0/other/assets/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/assets/bitter-sweet.csv` & `mat3ra-api-examples-2024.4.3.post0/other/assets/bitter-sweet.csv`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/assets/gamma_alumina_digne_et_al.poscar` & `mat3ra-api-examples-2024.4.3.post0/other/assets/gamma_alumina_digne_et_al.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/assets/sci_adv_dean_data.csv` & `mat3ra-api-examples-2024.4.3.post0/other/assets/sci_adv_dean_data.csv`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_min_energy_by_miller_indices.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_alignn.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/create_interface_with_relaxation_matgl_m3gnet.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/uploads/Gr.json` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Gr.json`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/experiments/uploads/Ni.json` & `mat3ra-api-examples-2024.4.3.post0/other/experiments/uploads/Ni.json`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/jarvis/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/jarvis/run_job_using_material_from_jarvis_db.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/job/Smiles_Generation_Markov_Chain.py` & `mat3ra-api-examples-2024.4.3.post0/other/job/Smiles_Generation_Markov_Chain.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Classification_of_Bitterness_XGBoost.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/Prediction_of_Perovskite_Unit_Cell_Volume.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/machine_learning/neural_network_train.py` & `mat3ra-api-examples-2024.4.3.post0/other/machine_learning/neural_network_train.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/Introduction.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_min_strain_zsl.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/create_interface_with_relaxation_ase_emt.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_material_from_jarvis_db_entry.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/import_materials_from_files.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/import_materials_from_files.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/pymatgen_coherent_interface_builder.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materials_designer/src/utils.py` & `mat3ra-api-examples-2024.4.3.post0/other/materials_designer/src/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materialsproject/api_interoperability_showcase.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materialsproject/api_interoperability_showcase.py` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/api_interoperability_showcase.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materialsproject/import_materials_from_materialsproject.ipynb` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.ipynb`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/materialsproject/import_materials_from_materialsproject.py` & `mat3ra-api-examples-2024.4.3.post0/other/materialsproject/import_materials_from_materialsproject.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/python_transformations/1_layer_on_substrate.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/1_layer_on_substrate.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/python_transformations/2_strain_matching.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/2_strain_matching.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/python_transformations/3_imports.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/3_imports.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/python_transformations/4_custom_transformation.py` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/4_custom_transformation.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/python_transformations/README.md` & `mat3ra-api-examples-2024.4.3.post0/other/python_transformations/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/webinar/adsorption-study.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/adsorption-study.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/webinar/generate-al2o3-slab-structures.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/generate-al2o3-slab-structures.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/webinar/predict_with_machine_learning.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/predict_with_machine_learning.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/other/webinar/wulff-construction-surface-energy-study-cu.py` & `mat3ra-api-examples-2024.4.3.post0/other/webinar/wulff-construction-surface-energy-study-cu.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/pyproject.toml` & `mat3ra-api-examples-2024.4.3.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/scripts/change-branch-in-urls.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/change-branch-in-urls.sh`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/scripts/env.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/env.sh`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/scripts/render-notebooks.sh` & `mat3ra-api-examples-2024.4.3.post0/scripts/render-notebooks.sh`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/generic.py` & `mat3ra-api-examples-2024.4.3.post0/utils/generic.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/jupyterlite.py` & `mat3ra-api-examples-2024.4.3.post0/utils/jupyterlite.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/material.py` & `mat3ra-api-examples-2024.4.3.post0/utils/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/notebook.py` & `mat3ra-api-examples-2024.4.3.post0/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/settings.py` & `mat3ra-api-examples-2024.4.3.post0/utils/settings.py`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/utils/web/renderjson.js` & `mat3ra-api-examples-2024.4.3.post0/utils/web/renderjson.js`

 * *Files identical despite different names*

### Comparing `mat3ra_api_examples-2024.4.19.post0/wheel_server.py` & `mat3ra-api-examples-2024.4.3.post0/wheel_server.py`

 * *Files identical despite different names*
