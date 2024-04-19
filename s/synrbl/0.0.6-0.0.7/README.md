# Comparing `tmp/synrbl-0.0.6.tar.gz` & `tmp/synrbl-0.0.7.tar.gz`

## Comparing `synrbl-0.0.6.tar` & `synrbl-0.0.7.tar`

### file list

```diff
@@ -1,142 +1,152 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.6/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.6/.gitattributes
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.6/lint_check.sh
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 synrbl-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.6/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 synrbl-0.0.6/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Golden/Golden.csv
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/complex.csv
--rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/patent.csv
--rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/Jaworski/typical.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Raw_data/USPTO/USPTO_50K.csv
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Rules/automated_rules.json.gz
--rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/Jaworski.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_50K.csv
--rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_diff.csv
--rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_random_class.csv
--rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/USPTO_unbalance_class.csv
--rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/golden_dataset.csv
--rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/validation_set.csv
--rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.6/Data/Validation_set/validation_set.json
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Examples/notebook.ipynb
--rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Images/Flowchart.png
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.6/Docs/Paper_fig/figures.py
--rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/Analysis_vis.ipynb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/result_evaluation.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/synrbl_pilot.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.6/Scripts/validation_set_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/test_appeal_reaction.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynChemImputer/test_peroxide_imputer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_merge.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_model.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_rules.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_structure.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_molcurator.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_process.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_check_carbon_balance.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_comparator.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_decomposer.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynProcessor/test_rmsi_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_rules.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_smiles.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_rule_constraint.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_rule_data_manager.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_imputer.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_matcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/__init__.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/test_chem_utils.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynUtils/test_functional_group_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynVis/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.6/Test/SynVis/test_reaction_visualizer.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/__main__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/confidence_prediction.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/main.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/mcs.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/postprocess.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/preprocess.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/rsmi_utils.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/rule_based.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/analysis_process.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/analysis_utils.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/eda_analysis.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/feature_analysis.py
--rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/scoring_function.dump
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynAnalysis/visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/appel_reaction.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/functional_group_checker.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynChemImputer/peroxide_imputer.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/__init__.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/cmd_benchmark.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/cmd_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynCmd/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/compound_rules.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/expand_rules.json
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules_example.json
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/model.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/rules.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/structure.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/molcurator.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/check_carbon_balance.py
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_both_side_process.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_comparator.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_decomposer.py
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynProcessor/rsmi_processing.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_rules.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_smiles.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/rule_data_manager.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/rules_manager.json.gz
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_constraint.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_imputer.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_matcher.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/chem_utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/common.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/data_utils.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/functional_group_utils.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynUtils/rsmi_utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/__init__.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/mcs_visualizer.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.6/synrbl/SynVis/reaction_visualizer.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.6/LICENSE
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 synrbl-0.0.6/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 synrbl-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.7/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.7/.gitattributes
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.7/lint.sh
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 synrbl-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.7/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 synrbl-0.0.7/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Golden/Golden.csv
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/complex.csv
+-rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/patent.csv
+-rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/typical.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/USPTO/USPTO_50K.csv
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Rules/automated_rules.json.gz
+-rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/Jaworski.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_50K.csv
+-rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_diff.csv
+-rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_random_class.csv
+-rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/golden_dataset.csv
+-rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/validation_set.csv
+-rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/validation_set.json
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Examples/notebook.ipynb
+-rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Images/Flowchart.png
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Paper_fig/figures.py
+-rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/Analysis_vis.ipynb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/result_evaluation.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/synrbl_pilot.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/validation_set_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/__init__.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/test_mcs_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_appeal_reaction.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_molecule_standardizer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_peroxide_imputer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_merge.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_model.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_rules.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_structure.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_molcurator.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_process.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_check_carbon_balance.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_comparator.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_decomposer.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_processing.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rsmi_both_side_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_rules.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_smiles.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_rule_constraint.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_rule_data_manager.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_matcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/__init__.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/test_chem_utils.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/test_functional_group_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynVis/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynVis/test_reaction_visualizer.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/__main__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/balancing.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/confidence_prediction.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/mcs_search.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/postprocess.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/preprocess.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/rsmi_utils.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/rule_based.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/analysis_process.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/analysis_utils.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/eda_analysis.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/feature_analysis.py
+-rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/scoring_function.dump
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/appel_reaction.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/compounds_template.json
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/curate_reduction.py
+-rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/functional_group_checker.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/molecule_standardizer.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/peroxide_imputer.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/reduction_template.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/reduction_templates.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/__init__.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/cmd_benchmark.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/cmd_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/compound_rules.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/expand_rules.json
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules_example.json
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/model.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/rules.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/structure.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/molcurator.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/check_carbon_balance.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_both_side_process.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_comparator.py
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_decomposer.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_processing.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_rules.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_smiles.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/rule_data_manager.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/rules_manager.json.gz
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_constraint.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_matcher.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/__init__.py
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/chem_utils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/common.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/data_utils.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/functional_group_utils.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/rsmi_utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/__init__.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/mcs_visualizer.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/reaction_visualizer.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/rxnpdf.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/rxnvis.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 synrbl-0.0.7/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 synrbl-0.0.7/PKG-INFO
```

### Comparing `synrbl-0.0.6/.github/workflows/publish-package.yml` & `synrbl-0.0.7/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/.github/workflows/test-and-lint.yml` & `synrbl-0.0.7/.github/workflows/test-and-lint.yml`

 * *Files 10% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         python -m pip install --upgrade pip
         pip install flake8 pytest
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-        ./lint_check.sh
+        ./lint.sh
     - name: Test with pytest
       run: |
         pytest
```

### Comparing `synrbl-0.0.6/Data/Raw_data/Golden/Golden.csv` & `synrbl-0.0.7/Data/Raw_data/Golden/Golden.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Raw_data/Jaworski/complex.csv` & `synrbl-0.0.7/Data/Raw_data/Jaworski/complex.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Raw_data/Jaworski/patent.csv` & `synrbl-0.0.7/Data/Raw_data/Jaworski/patent.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Raw_data/Jaworski/typical.csv` & `synrbl-0.0.7/Data/Raw_data/Jaworski/typical.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Raw_data/USPTO/USPTO_50K.csv` & `synrbl-0.0.7/Data/Raw_data/USPTO/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Rules/automated_rules.json.gz` & `synrbl-0.0.7/Data/Rules/automated_rules.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/Jaworski.csv` & `synrbl-0.0.7/Data/Validation_set/Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/USPTO_50K.csv` & `synrbl-0.0.7/Data/Validation_set/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/USPTO_diff.csv` & `synrbl-0.0.7/Data/Validation_set/USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/USPTO_random_class.csv` & `synrbl-0.0.7/Data/Validation_set/USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/USPTO_unbalance_class.csv` & `synrbl-0.0.7/Data/Validation_set/USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/golden_dataset.csv` & `synrbl-0.0.7/Data/Validation_set/golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/validation_set.csv` & `synrbl-0.0.7/Data/Validation_set/validation_set.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Data/Validation_set/validation_set.json` & `synrbl-0.0.7/Data/Validation_set/validation_set.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Docs/Examples/notebook.ipynb` & `synrbl-0.0.7/Docs/Examples/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Docs/Images/Flowchart.png` & `synrbl-0.0.7/Docs/Images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Docs/Paper_fig/figures.py` & `synrbl-0.0.7/Docs/Paper_fig/figures.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/Analysis_vis.ipynb` & `synrbl-0.0.7/Pipeline/Validation/Analysis/Analysis_vis.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv` & `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv` & `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv` & `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv` & `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv` & `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Scripts/result_evaluation.py` & `synrbl-0.0.7/Scripts/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Scripts/synrbl_pilot.py` & `synrbl-0.0.7/Scripts/synrbl_pilot.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Scripts/validation_set_interface.py` & `synrbl-0.0.7/Scripts/validation_set_interface.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynChemImputer/test_appeal_reaction.py` & `synrbl-0.0.7/Test/SynChemImputer/test_appeal_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynChemImputer/test_peroxide_imputer.py` & `synrbl-0.0.7/Test/SynChemImputer/test_peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/test_merge.py` & `synrbl-0.0.7/Test/SynMCSImputer/test_merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/test_model.py` & `synrbl-0.0.7/Test/SynMCSImputer/test_model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/test_rules.py` & `synrbl-0.0.7/Test/SynMCSImputer/test_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/test_structure.py` & `synrbl-0.0.7/Test/SynMCSImputer/test_structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/test_utils.py` & `synrbl-0.0.7/Test/SynMCSImputer/test_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py` & `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py` & `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_molcurator.py` & `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py` & `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py` & `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py`

 * *Files 22% similar despite different names*

```diff
@@ -49,27 +49,10 @@
         conditions = [[{"mcs_results": ["CCO"]}], [{"mcs_results": ["CC"]}]]
         (
             threshold_index,
             reference_results_list,
         ) = self.extractor.extract_common_mcs_index(0, 100, *conditions)
         self.assertIsNotNone(threshold_index)
 
-    def test_compare_conditions_and_get_largest(self):
-        # Test comparing conditions and getting the largest MCS
-        total_atoms_conditions = [[3], [2]]
-        conditions = [[{"mcs_results": ["CCO"]}], [{"mcs_results": ["CC"]}]]
-        results, reference_list = self.extractor.compare_conditions_and_get_largest(
-            total_atoms_conditions, *conditions
-        )
-        self.assertIsNotNone(results)
-
-    def test_extract_matching_conditions(self):
-        # Test extracting matching conditions
-        conditions = [[{"mcs_results": ["CCO"]}], [{"mcs_results": ["CC"]}]]
-        results, threshold_index = self.extractor.extract_matching_conditions(
-            0, 100, *conditions
-        )
-        self.assertIsNotNone(results)
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py` & `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_mcs_process.py` & `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     @patch(
         "synrbl.SynMCSImputer.SubStructure.mcs_graph_detector.MCSMissingGraphAnalyzer.fit"
     )
     def test_single_mcs(self, mock_fit):
         # Mocking MCSMissingGraphAnalyzer.fit to return predefined values
         mock_fit.return_value = ([], [], [], None)
 
-        result = single_mcs(self.sample_reaction_data)
+        result = single_mcs(self.sample_reaction_data, id_col="R-id")
         self.assertEqual(result["R-id"], "example_id")
         self.assertIsInstance(result["mcs_results"], list)
         self.assertIsInstance(result["sorted_reactants"], list)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `synrbl-0.0.6/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py` & `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynProcessor/test_check_carbon_balance.py` & `synrbl-0.0.7/Test/SynProcessor/test_check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynProcessor/test_rmsi_comparator.py` & `synrbl-0.0.7/Test/SynProcessor/test_rmsi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynProcessor/test_rmsi_decomposer.py` & `synrbl-0.0.7/Test/SynProcessor/test_rmsi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynProcessor/test_rmsi_processing.py` & `synrbl-0.0.7/Test/SynProcessor/test_rmsi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_rules.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_auto_extract_smiles.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_rule_constraint.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_rule_data_manager.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_imputer.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynRuleImputer/test_synthetic_rule_matcher.py` & `synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynUtils/test_chem_utils.py` & `synrbl-0.0.7/Test/SynUtils/test_chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynUtils/test_functional_group_utils.py` & `synrbl-0.0.7/Test/SynUtils/test_functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/Test/SynVis/test_reaction_visualizer.py` & `synrbl-0.0.7/Test/SynVis/test_reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/confidence_prediction.py` & `synrbl-0.0.7/synrbl/confidence_prediction.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 
 class ConfidencePredictor:
     def __init__(
         self,
         reaction_col="reaction",
         input_reaction_col="input_reaction",
         confidence_col="confidence",
+        solved_col="solved",
         solved_by_col="solved_by",
         solved_by_method="mcs-based",
+        issue_col="issue",
         mcs_col="mcs",
     ):
         self.model = joblib.load(
             importlib.resources.files(synrbl.SynAnalysis)
             .joinpath("scoring_function.dump")
             .open("rb")
         )
         self.reaction_col = reaction_col
         self.input_reaction_col = input_reaction_col
         self.confidence_col = confidence_col
+        self.solved_col = solved_col
         self.solved_by_col = solved_by_col
         self.solved_by_method = solved_by_method
+        self.issue_col = issue_col
         self.mcs_col = mcs_col
 
     def predict(self, reactions, stats=None, threshold=0):
         reactions = [
             r
             for r in reactions
             if self.solved_by_col in r.keys()
@@ -65,10 +69,18 @@
 
             confidence = np.round(self.model.predict_proba(X_pred)[:, 1], 3)
             assert len(reactions) == len(confidence)
             for r, c in zip(reactions, confidence):
                 r[self.confidence_col] = c
                 if c >= threshold:
                     conf_success += 1
+                else:
+                    assert (
+                        r[self.issue_col] == ""
+                    ), "Issue column has value for a solved reaction?"
+                    r[self.solved_col] = False
+                    r[
+                        self.issue_col
+                    ] = "Confidence is below the threshold of {:.2%}.".format(threshold)
         if stats is not None:
             stats["confident_cnt"] = conf_success
         return reactions
```

### Comparing `synrbl-0.0.6/synrbl/postprocess.py` & `synrbl-0.0.7/synrbl/postprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,29 @@
         self,
         reaction_col,
         method,
         solved_col="solved",
         solved_method_col="solved_by",
         unbalance_col="unbalance",
         carbon_balance_col="carbon_balance_check",
+        issue_col="issue",
         check_carbon_balance=True,
         n_jobs=1,
     ):
         self.reaction_col = reaction_col
         self.method = method
         self.solved_col = solved_col
         self.solved_method_col = solved_method_col
         self.unbalance_col = unbalance_col
         self.check_carbon_balance = check_carbon_balance
         self.carbon_balance_col = carbon_balance_col
+        self.issue_col = issue_col
         self.n_jobs = n_jobs
 
-    def check(self, reactions):
+    def check(self, reactions, override_unsolved=False):
         update_reactants_and_products(reactions, self.reaction_col)
         decompose = RSMIDecomposer(
             smiles=None,  # type: ignore
             data=reactions,  # type: ignore
             reactant_col="reactants",
             product_col="products",
             parallel=True,
@@ -57,9 +59,10 @@
             if (
                 b == "Balance"
                 and reaction[self.carbon_balance_col] == "balanced"
                 and not reaction[self.solved_col]
             ):
                 reaction[self.solved_col] = True
                 reaction[self.solved_method_col] = self.method
-
+            if override_unsolved and not reaction[self.solved_col]:
+                reaction[self.reaction_col] = reaction["input_reaction"]
         return reactions
```

### Comparing `synrbl-0.0.6/synrbl/preprocess.py` & `synrbl-0.0.7/synrbl/preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 
 from synrbl.SynProcessor import RSMIProcessing
 
 
-def preprocess(reactions, reaction_col, index_col, solved_col, n_jobs=1):
+def preprocess(reactions, reaction_col, index_col, solved_col, input_col, n_jobs=1):
     df = pd.DataFrame(reactions)
     df[solved_col] = False
 
     if "Unnamed: 0" in df.columns:
         df = df.drop("Unnamed: 0", axis=1)
 
     process = RSMIProcessing(
@@ -19,10 +19,10 @@
         index_col=index_col,
         drop_duplicates=False,
         save_json=False,
         save_path_name=None,  # type: ignore
         verbose=0,
     )
     reactions = process.data_splitter()
-    reactions["input_reaction"] = reactions[reaction_col]
+    reactions[input_col] = reactions[reaction_col]
 
     return reactions.to_dict("records")
```

### Comparing `synrbl-0.0.6/synrbl/rsmi_utils.py` & `synrbl-0.0.7/synrbl/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/rule_based.py` & `synrbl-0.0.7/synrbl/rule_based.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/analysis_process.py` & `synrbl-0.0.7/synrbl/SynAnalysis/analysis_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/analysis_utils.py` & `synrbl-0.0.7/synrbl/SynAnalysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/eda_analysis.py` & `synrbl-0.0.7/synrbl/SynAnalysis/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/feature_analysis.py` & `synrbl-0.0.7/synrbl/SynAnalysis/feature_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/scoring_function.dump` & `synrbl-0.0.7/synrbl/SynAnalysis/scoring_function.dump`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynAnalysis/visualizer.py` & `synrbl-0.0.7/synrbl/SynAnalysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynChemImputer/appel_reaction.py` & `synrbl-0.0.7/synrbl/SynChemImputer/appel_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynChemImputer/functional_group_checker.py` & `synrbl-0.0.7/synrbl/SynChemImputer/functional_group_checker.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynChemImputer/peroxide_imputer.py` & `synrbl-0.0.7/synrbl/SynChemImputer/peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynCmd/__init__.py` & `synrbl-0.0.7/synrbl/SynCmd/__init__.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynCmd/cmd_benchmark.py` & `synrbl-0.0.7/synrbl/SynCmd/cmd_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,151 @@
 import argparse
 import logging
 import pandas as pd
 
 from synrbl import Balancer
-from synrbl.SynUtils.chem_utils import normalize_smiles
 
 logger = logging.getLogger(__name__)
 
 
-def print_result(stats, rb_correct, mcs_correct):
+def print_result(stats, min_confidence=0):
     def _sr(v, c):
         return "{:.2%}".format(v / c) if c > 0 else "-"
 
     rxn_cnt = stats["reaction_cnt"]
+    in_blcd = stats["balanced_cnt"]
     rb_s = stats["rb_solved"]
     rb_a = stats["rb_applied"]
+    mcs_s = stats["mcs_solved"]
     mcs_a = stats["mcs_applied"]
     mcs_cth = stats["confident_cnt"]
     logger.info("{} Summary {}".format("#" * 20, "#" * 20))
-    line_fmt = "{:<15} {:>10} {:>10} {:>10}"
-    header = line_fmt.format("", "Rule-based", "MCS-based", "SynRBL")
-    logger.info(header)
-    logger.info("-" * len(header))
-    logger.info(line_fmt.format("Input", str(rb_a), str(mcs_a), str(rxn_cnt)))
-    logger.info(line_fmt.format("Solved", str(rb_s), str(mcs_cth), str(rb_s + mcs_cth)))
     logger.info(
-        line_fmt.format(
-            "Correct",
-            "{}".format(rb_correct),
-            "{}".format(mcs_correct),
-            "{}".format(rb_correct + mcs_correct),
+        "Input data contained {} balanced reactions.".format(stats["balanced_cnt"])
+    )
+    logger.info(
+        "Rule-based method solved {} out of {} reactions (success rate: {}).".format(
+            rb_s, rb_a, _sr(rb_s, rb_a)
         )
     )
     logger.info(
-        line_fmt.format(
-            "Success rate",
-            _sr(rb_s, rb_a),
-            _sr(mcs_cth, mcs_a),
-            _sr(rb_s + mcs_cth, rxn_cnt),
+        "MCS-based method solved {} out of {} reactions (success rate: {}).".format(
+            mcs_s, mcs_a, _sr(mcs_s, mcs_a)
         )
     )
+    below_th = mcs_s - mcs_cth
+    if below_th > 0:
+        logger.info(
+            "{} results where below the confidence threshold of {:.0%}.".format(
+                below_th, min_confidence
+            )
+        )
+        logger.info(
+            (
+                "MCS-based method solved {} out of {} reactions above the "
+                + "confidence threshold (success rate: {})."
+            ).format(mcs_cth, mcs_a, _sr(mcs_cth, mcs_a))
+        )
     logger.info(
-        line_fmt.format(
-            "Accuracy",
-            _sr(rb_correct, rb_s),
-            _sr(mcs_correct, mcs_cth),
-            _sr(rb_correct + mcs_correct, rb_s + mcs_cth),
+        "SynRBL solved {} out of {} reactions (success rate: {}).".format(
+            rb_s + mcs_cth, rxn_cnt - in_blcd, _sr(rb_s + mcs_cth, rxn_cnt - in_blcd)
         )
     )
 
 
-def check_columns(reactions, reaction_col, result_col):
-    if len(reactions) == 0:
-        raise ValueError("No reactions found in input.")
-    cols = reactions[0].keys()
-    if reaction_col not in cols:
-        raise KeyError("No column '{}' found in input.".format(reaction_col))
-    if result_col not in cols:
-        raise KeyError("No column '{}' found in input.".format(result_col))
+def impute(
+    src_file,
+    output_file,
+    reaction_col,
+    passthrough_cols,
+    min_confidence,
+    n_jobs=-1,
+):
+    input_reactions = pd.read_csv(src_file).to_dict("records")
 
-
-def run(args):
-    input_reactions = pd.read_csv(args.inputfile).to_dict("records")
-    check_columns(input_reactions, args.col, args.result_col)
-
-    stats = {}
     synrbl = Balancer(
-        reaction_col=args.col, confidence_threshold=args.min_confidence, n_jobs=args.p
+        reaction_col=reaction_col, confidence_threshold=min_confidence, n_jobs=n_jobs
     )
+    stats = {}
     rbl_reactions = synrbl.rebalance(input_reactions, output_dict=True, stats=stats)
 
-    rb_correct = 0
-    mcs_correct = 0
-    for i, (in_r, out_r) in enumerate(zip(input_reactions, rbl_reactions)):
-        if not out_r["solved"]:
-            continue
-        exp = in_r[args.result_col]
-        if pd.isna(exp):
-            logger.warning(
-                "Missing expected reaction ({}) in line {}.".format(args.result_col, i)
-            )
-            continue
-        exp_reaction = normalize_smiles(exp)
-        act_reaction = normalize_smiles(out_r[args.col])
-        if exp_reaction == act_reaction:
-            if out_r["solved_by"] == "rule-based":
-                rb_correct += 1
-            elif out_r["solved_by"] == "mcs-based":
-                mcs_correct += 1
-    print_result(stats, rb_correct, mcs_correct)
-
-    if args.o is not None:
-        for in_r, out_r in zip(input_reactions, rbl_reactions):
-            out_r[args.result_col] = in_r[args.result_col]
-        df = pd.DataFrame(rbl_reactions)
-        df.to_csv(args.o)
+    for in_r, out_r in zip(input_reactions, rbl_reactions):
+        for c in passthrough_cols:
+            out_r[c] = in_r[c]
+
+    df = pd.DataFrame(rbl_reactions)
+    df.to_csv(output_file)
+    print_result(stats, min_confidence)
+
+
+def run(args):
+    outputfile = args.o
+    if outputfile is None:
+        outputfile = "{}_out.csv".format(args.inputfile.split(".")[0])
+    columns = args.columns if isinstance(args.columns, list) else [args.columns]
+
+    impute(
+        args.inputfile,
+        outputfile,
+        reaction_col=args.col,
+        passthrough_cols=columns,
+        min_confidence=args.min_confidence,
+        n_jobs=args.p,
+    )
 
 
 class Range(object):
     def __init__(self, start, end):
         self.start = start
         self.end = end
 
     def __eq__(self, other):
         return self.start <= other <= self.end
 
     def __str__(self):
         return "[{}, {}]".format(self.start, self.end)
 
 
+def list_of_strings(arg):
+    return arg.split(",")
+
+
 def configure_argparser(argparser: argparse._SubParsersAction):
     test_parser = argparser.add_parser(
-        "benchmark", description="Benchmark SynRBL on your own dataset."
+        "run", description="Try to rebalance chemical reactions."
     )
 
     test_parser.add_argument(
-        "inputfile",
-        help="Path to file containing reaction SMILES and the expected result.",
-    )
-    test_parser.add_argument(
-        "-o",
-        default=None,
-        help="If set, the detailed results will be written to that file.",
+        "inputfile", help="Path to file containing reaction SMILES."
     )
+    test_parser.add_argument("-o", default=None, help="Path to output file.")
     test_parser.add_argument(
         "-p",
         default=-1,
         type=int,
         help="The number of parallel process. (Default -1 => # of processors)",
     )
     test_parser.add_argument(
         "--col",
         default="reaction",
         help="The reactions column name for in the input .csv file. "
         + "(Default: 'reaction')",
     )
     test_parser.add_argument(
-        "--result-col",
-        default="expected_reaction",
-        help="The reactions column name for in the expected output. "
-        + "(Default: 'expected_reaction')",
+        "--columns",
+        default=[],
+        type=list_of_strings,
+        help="A comma separated list of columns from the input that should "
+        + "be added to the output. (e.g.: col1,col2,col3)",
     )
     test_parser.add_argument(
         "--min-confidence",
         type=float,
         default=0,
         choices=[Range(0.0, 1.0)],
         help=(
             "Set a confidence threshold for the results "
-            + "from the MCS-based method. (Default: 0.5)"
+            + "from the MCS-based method. (Default: 0)"
         ),
     )
 
     test_parser.set_defaults(func=run)
```

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/compound_rules.json` & `synrbl-0.0.7/synrbl/SynMCSImputer/compound_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/expand_rules.json` & `synrbl-0.0.7/synrbl/SynMCSImputer/expand_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/merge.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/merge_rules.json` & `synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/model.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         )
     rules = [r.name for r in merge_result.rules]
     is_balanced = is_carbon_balanced(imputed_reaction)
     if not is_balanced:
         raise RuntimeError(
             (
                 "Failed to impute the correct structure. "
-                + "Carbon atom count in reactants and products does not match. "
+                + "Carbon atom count in reactants and products does not match."
             )
         )
     return imputed_reaction, rules
 
 
 class MCSBasedMethod:
     def __init__(
@@ -111,14 +111,16 @@
         mcs_applied = 0
         mcs_solved = 0
         block_logs = BlockLogs()
         for reaction in reactions:
             if self.mcs_data_col not in reaction.keys():
                 continue
             mcs_applied += 1
+            if reaction[self.mcs_data_col] is None:
+                continue
             try:
                 result, rules = impute_reaction(
                     reaction,
                     mcs_data_col=self.mcs_data_col,
                     reaction_col=self.reaction_col,
                     issue_col=self.issue_col,
                     carbon_balance_col=self.carbon_balance_col,
```

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/rules.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/structure.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/utils.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/molcurator.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from collections import Counter
 from rdkit import Chem
 from joblib import Parallel, delayed
-from typing import List, Dict, Tuple
+from typing import List, Dict
 
-logger = logging.getLogger("SynRBL")
+logger = logging.getLogger("synrbl")
 
 
 class ExtractMCS:
     """
     A class to extract and analyze the most common Maximum Common Substructure
     (MCS) from a list of MCS results.
     Provides functionality to determine the most common elements, the top n
@@ -40,15 +40,15 @@
                 return molecule.GetNumAtoms()
             else:
                 return 0
         except Exception:
             return 0
 
     @staticmethod
-    def calculate_total_number_atoms_mcs_parallel(condition, n_jobs=4):
+    def calculate_total_number_atoms_mcs_parallel(condition, n_jobs=4) -> list[int]:
         """
         Calculate the total number of atoms in the MCS results for each
         dictionary in a condition using parallel processing.
 
         Args:
         condition (list): A list of dictionaries, each containing
             'mcs_results', which are lists of SMILES strings.
@@ -62,15 +62,15 @@
 
         def calculate_atoms_for_dict(d):
             return sum(ExtractMCS.get_num_atoms(mcs) for mcs in d["mcs_results"])
 
         total_number_atoms = Parallel(n_jobs=n_jobs, verbose=0)(
             delayed(calculate_atoms_for_dict)(d) for d in condition
         )
-        return total_number_atoms
+        return total_number_atoms  # type: ignore
 
     def get_popular_elements_from_list(self, elements_list):
         """
         Get the most popular elements in a flat list.
 
         :param elements_list: A list containing elements.
         :return: A list of elements that appear with the highest frequency in
@@ -156,146 +156,79 @@
         threshold_index = [
             lower_threshold <= i <= upper_threshold for i in overlap_percentages
         ]
         # mcs_common = [d for d, b in zip(conditions[0], threshold_index) if b]
         return threshold_index, reference_results_list
 
     @staticmethod
-    def compare_conditions_and_get_largest(
-        total_atoms_conditions: List[List[int]], *conditions: List[List[Dict]]
-    ) -> Tuple[List[Dict], List[List[str]]]:
+    def get_largest_condition(*conditions: List[List[Dict]]) -> List[Dict]:
         """
         Compare the total number of atoms across different conditions and find
         the condition with the largest MCS for each index.
         In case of a tie, compares the total number of atoms in the first
         SMILES/SMARTS for those conditions.
 
         Args:
         - total_atoms_conditions (list): A list of lists, where each sublist
-            contains the total number of atoms for each MCS result in a condition.
+            contains the total number of atoms for each MCS result in
+            a condition.
 
         Returns:
-        - Tuple:
-            - A list of dictionaries, each representing the condition with the
-                largest MCS for a given index.
-            - A reference list of the biggest MCS for each index across the
-                conditions.
+            list[dict]: A list of conditions. Each row contains the condition
+                with the largest maximum-common-substructure or None if no
+                suitable result was found.
         """
-        results = []
-        reference_list = []
+
+        total_atoms_conditions = [
+            ExtractMCS.calculate_total_number_atoms_mcs_parallel(condition, n_jobs=4)
+            for condition in conditions
+        ]
+
+        result = []
         min_length = min(len(total) for total in total_atoms_conditions)
 
         for idx in range(min_length):
             tied_conditions = []
             max_atoms = 0
-            max_condition = -1
+            max_condition_idx = -1
+            max_condition = None
 
             # First pass: Find conditions with the largest total atom counts
             for condition_idx, total in enumerate(total_atoms_conditions):
                 if idx < len(total):
                     if total[idx] > max_atoms:
                         max_atoms = total[idx]
                         tied_conditions = [(condition_idx, total[idx])]
                     elif total[idx] == max_atoms:
                         tied_conditions.append((condition_idx, total[idx]))
 
             # Second pass: In case of a tie, compare the first SMILES/SMARTS
             if len(tied_conditions) > 1:
                 max_first_smarts_atoms = 0
-                winning_condition = -1
+                winning_condition_idx = -1
                 for condition_idx, _ in tied_conditions:
                     first_smarts = (
                         conditions[condition_idx][idx]["mcs_results"][0]
                         if conditions[condition_idx][idx]["mcs_results"]
                         else ""
                     )
                     first_smarts_atoms = ExtractMCS.get_num_atoms(first_smarts)
                     if first_smarts_atoms > max_first_smarts_atoms:
                         max_first_smarts_atoms = first_smarts_atoms
-                        winning_condition = condition_idx
+                        winning_condition_idx = condition_idx
 
                 # Finalize the winning condition
-                if winning_condition != -1:
-                    max_condition = winning_condition
-                    max_mcs = conditions[max_condition][idx]["mcs_results"]
+                if winning_condition_idx != -1:
+                    max_condition_idx = winning_condition_idx
+                    max_condition = conditions[max_condition_idx][idx]
             else:
-                max_condition = tied_conditions[0][0] if tied_conditions else -1
-                max_mcs = (
-                    conditions[max_condition][idx]["mcs_results"]
-                    if max_condition != -1
-                    else []
+                max_condition_idx = tied_conditions[0][0] if tied_conditions else -1
+                max_condition = (
+                    conditions[max_condition_idx][idx]
+                    if max_condition_idx != -1
+                    else None
                 )
 
-            if max_condition != -1:
-                result_entry = {
-                    "name": f"Condition {max_condition + 1}",
-                    "biggest_mcs": max_mcs,
-                }
-                results.append(result_entry)
-                reference_list.append(max_mcs)
-
-        return results, reference_list
-
-    def extract_matching_conditions(
-        self,
-        lower_threshold,
-        upper_threshold,
-        *conditions,
-        extraction_method="ensemble",
-        using_threshold=False,
-    ):
-        """
-        Extract and return the first matching condition for each index that
-        meets the threshold.
-
-        :param threshold_index: A list of boolean values indicating whether
-            each condition meets the threshold.
-        :param conditions: A list of conditions, each a list of dictionaries
-            containing 'mcs_results'.
-        :param reference_results_list: A list of reference results to match
-            against the conditions.
-        :return: A list of dictionaries representing the matching condition
-            for each index that meets the threshold.
-        """
-
-        threshold_index = (
-            []
-        )  # Initialize threshold_index to an empty list or a suitable default value
-
-        if extraction_method == "ensemble":
-            threshold_index, reference_results_list = self.extract_common_mcs_index(
-                lower_threshold, upper_threshold, *conditions
-            )
-        elif extraction_method == "largest_mcs":
-            total_atoms_conditions = [
-                ExtractMCS.calculate_total_number_atoms_mcs_parallel(
-                    condition, n_jobs=4
-                )
-                for condition in conditions
-            ]
-            _, reference_results_list = ExtractMCS.compare_conditions_and_get_largest(
-                total_atoms_conditions, *conditions
-            )
-            if using_threshold:
-                threshold_index, _ = self.extract_common_mcs_index(
-                    lower_threshold, upper_threshold, *conditions
-                )
-            else:
-                threshold_index = [True] * len(
-                    conditions[0]
-                )  # Make sure to set threshold_index in this branch
-
-        results = []
-        for key, value in enumerate(threshold_index):
-            if value:
-                try:
-                    for condition in conditions:
-                        if sorted(reference_results_list[key]) == sorted(
-                            condition[key]["mcs_results"]
-                        ):
-                            results.append(condition[key])
-                            break
-
-                except Exception as e:
-                    logger.error(f"Error processing condition at index {key}: {e}")
-                    continue
-        return results, threshold_index
+            if max_condition is not None:
+                result.append(max_condition)
+
+        return result
```

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,14 +212,17 @@
         elif method == "MCES":
             params = rdRascalMCES.RascalOptions()
             params.singleLargestFrag = False
             params.returnEmptyMCES = True
             params.timeout = Timeout
             params.similarityThreshold = similarityThreshold
 
+        else:
+            raise ValueError("Method '{}' is not implemented.".format(method))
+
         if reaction_dict["carbon_balance_check"] in ["products", "balanced"]:
             # Calculate the MCS for each reactant with the product
             reactant_smiles, product_smiles = MCSMissingGraphAnalyzer.get_smiles(
                 reaction_dict
             )
             reactant_mol_list = [
                 MCSMissingGraphAnalyzer.convert_smiles_to_molecule(smiles)
@@ -265,7 +268,13 @@
                 params,
                 method=method,
                 sort=sort,
                 remove_substructure=remove_substructure,
             )
 
             return mcs_list, sorted_parents, product_mol_list, reactant_mol
+        else:
+            raise RuntimeError(
+                "Invalid carbon_balance_check value: '{}'".format(
+                    reaction_dict["carbon_balance_check"]
+                )
+            )
```

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/mcs_process.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_process.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import datetime
 import time
-import copy
 import logging
 
+import rdkit.Chem.rdmolfiles as rdmolfiles
+
 from synrbl.SynMCSImputer.SubStructure.mcs_graph_detector import MCSMissingGraphAnalyzer
-from rdkit import Chem
 from joblib import Parallel, delayed
 
 from rdkit.rdBase import BlockLogs
 
-logger = logging.getLogger("SynRBL")
+logger = logging.getLogger("synrbl")
 
 
 def single_mcs(
     data_dict,
+    id_col="id",
+    issue_col="issue",
     RingMatchesRingOnly=True,
     CompleteRingsOnly=True,
     Timeout=60,
     sort="MCES",
     method="MCES",
     similarityThreshold=0.5,
     remove_substructure=True,
@@ -30,55 +32,66 @@
     - data_dict: Dict containing reaction data.
     - params: Optional parameters for MCS analysis.
 
     Returns:
     - dict: A dictionary containing MCS results and any sorted reactants encountered.
     """
     block_logs = BlockLogs()
-    mcs_results_dict = copy.deepcopy(data_dict)
-    mcs_results_dict["mcs_results"] = []
-    mcs_results_dict["sorted_reactants"] = []
-    mcs_results_dict["issue"] = []
+    mcs_data = {
+        id_col: data_dict[id_col],
+        "mcs_results": [],
+        "sorted_reactants": [],
+        issue_col: "",
+    }
 
     try:
         analyzer = MCSMissingGraphAnalyzer()
         mcs_list, sorted_reactants, reactant_mol_list, _ = analyzer.fit(
             data_dict,
             RingMatchesRingOnly=RingMatchesRingOnly,
             CompleteRingsOnly=CompleteRingsOnly,
             sort=sort,
             method=method,
             remove_substructure=remove_substructure,
             Timeout=Timeout,
             similarityThreshold=similarityThreshold,
             ignore_bond_order=ignore_bond_order,
         )
-        mcs_list_smiles = [Chem.MolToSmarts(mol) for mol in mcs_list]
-        sorted_reactants_smiles = [Chem.MolToSmiles(mol) for mol in sorted_reactants]
-        mcs_results_dict["mcs_results"] = mcs_list_smiles
-        mcs_results_dict["sorted_reactants"] = sorted_reactants_smiles
 
         if len(reactant_mol_list) != len(sorted_reactants):
-            mcs_results_dict["issue"] = "MCS_Uncertainty"
+            mcs_data["issue"] = "Uncertian MCS."
+        else:
+            mcs_data["mcs_results"] = [rdmolfiles.MolToSmarts(mol) for mol in mcs_list]
+            mcs_data["sorted_reactants"] = [
+                rdmolfiles.MolToSmiles(mol) for mol in sorted_reactants
+            ]
+    except Exception as e:
+        mcs_data[issue_col] = "MCS identification failed. {}".format(str(e))
 
-    except Exception:
-        mcs_results_dict["issue"] = "Single MCS identification failed."
     del block_logs
-    return mcs_results_dict
+    return mcs_data
 
 
-def ensemble_mcs(data, conditions, n_jobs=-1, Timeout=60):
+def ensemble_mcs(
+    data, conditions, id_col="id", issue_col="issue", n_jobs=-1, Timeout=60
+):
     condition_results = []
     start_time = time.time()
     last_tsmp = start_time
     for i, condition in enumerate(conditions):
         all_results = []  # Accumulate results for each condition
 
         p_generator = Parallel(n_jobs=n_jobs, verbose=0, return_as="generator")(
-            delayed(single_mcs)(data_dict, **condition, Timeout=Timeout)
+            delayed(single_mcs)(
+                data_dict,
+                id_col=id_col,
+                issue_col=issue_col,
+                **condition,
+                Timeout=Timeout,
+            )
             for data_dict in data
         )
         for result in p_generator:
             all_results.append(result)  # Combine batch results
             prg = (i * len(data) + len(all_results)) / (len(conditions) * len(data))
             t = time.time()
             if t - last_tsmp > 10:
```

### Comparing `synrbl-0.0.6/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py` & `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynProcessor/check_carbon_balance.py` & `synrbl-0.0.7/synrbl/SynProcessor/check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynProcessor/rsmi_both_side_process.py` & `synrbl-0.0.7/synrbl/SynProcessor/rsmi_both_side_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,18 +119,19 @@
         # Process reactions in parallel for efficiency
         diff_dict = Parallel(n_jobs=n_jobs, verbose=0)(
             delayed(self.enforce_product_side)(react, prod)
             for react, prod in zip(react_dict_both, product_dict_both)
         )
 
         # Post-process to determine the new balance status
-        results = [self.reverse_values_if_negative_except_Q(item) for item in diff_dict]
         diff_dict_both, unbalance_both = [], []
-        if len(results) == 2:
-            diff_dict_both, unbalance_both = zip(*results)
+        for item in diff_dict:
+            d, u = self.reverse_values_if_negative_except_Q(item)
+            diff_dict_both.append(d)
+            unbalance_both.append(u)
 
         # Update diff_formula and unbalance lists
         for index, diff_new, unbalance_new in zip(
             both_index, diff_dict_both, unbalance_both
         ):
             self.diff_formula[index] = diff_new
             self.unbalance[index] = unbalance_new
```

### Comparing `synrbl-0.0.6/synrbl/SynProcessor/rsmi_comparator.py` & `synrbl-0.0.7/synrbl/SynProcessor/rsmi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynProcessor/rsmi_decomposer.py` & `synrbl-0.0.7/synrbl/SynProcessor/rsmi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynProcessor/rsmi_processing.py` & `synrbl-0.0.7/synrbl/SynProcessor/rsmi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_rules.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/auto_extract_smiles.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/rule_data_manager.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/rules_manager.json.gz` & `synrbl-0.0.7/synrbl/SynRuleImputer/rules_manager.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_constraint.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_imputer.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynRuleImputer/synthetic_rule_matcher.py` & `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynUtils/chem_utils.py` & `synrbl-0.0.7/synrbl/SynVis/reaction_visualizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,259 +1,261 @@
 import io
-import re
-import tempfile
 import matplotlib.pyplot as plt
 
-from typing import List, Dict
-from typing import Union
 from rdkit import Chem
+from rdkit.Chem import AllChem
+from rdkit.Chem.Draw import rdMolDraw2D
 from PIL import Image
-from reportlab.pdfgen import canvas
-from reportlab.lib.pagesizes import landscape, letter
-from synrbl.SynVis.reaction_visualizer import ReactionVisualizer
+from typing import Dict, Tuple, Optional
 
 
-class CheckCarbonBalance:
+class ReactionVisualizer:
+    """
+    Plot and optionally compare two chemical reactions for visualization using
+    data from a given source.
+
+    This method allows the visualization of chemical reactions represented as
+    strings. It can plot a single reaction or compare two reactions
+    side-by-side, depending on the 'compare' parameter. The reactions are
+    visualized using RDKit and plotted using Matplotlib.
+
+    Parameters
+    ----------
+    data : dict
+        A dictionary containing the reaction data.
+    old_reaction_col : str
+        The key in 'data' for the old reaction string.
+    new_reaction_col : str
+        The key in 'data' for the new reaction string.
+    compare : bool, optional
+        If True, both the old and new reactions are plotted side by side for
+        comparison. Default is False.
+    orientation : str, optional
+        The layout orientation of the plots, either 'vertical' or 'horizontal'.
+        Default is 'vertical'.
+    savefig : bool, optional
+        If True, the figure is saved to the specified pathname. Default is False.
+    pathname : str, optional
+        The pathname where the figure will be saved, if 'savefig' is True.
+    dpi : int, optional
+        The resolution of the figure in dots per inch. Default is 300.
+
+    Examples
+    --------
+    # Example usage of the plot_reactions method
+    visualizer = ReactionVisualizer()
+    reaction_data = {
+        "old_reaction": "C1=CC=CC=C1.CCO>>C1=CC=CC=C1OCCO",
+        "new_reaction": "C1=CC=CC=C1>>CCO",
+    }
+    visualizer.plot_reactions(
+        reaction_data,
+        "old_reaction",
+        "new_reaction",
+        compare=True,
+        orientation="horizontal",
+    )
+
+    # To save the plot as an image
+    visualizer.plot_reactions(
+        reaction_data,
+        "old_reaction",
+        "new_reaction",
+        compare=True,
+        savefig=True,
+        pathname="reaction_comparison.png",
+    )
+    """
+
     def __init__(
-        self, reactions_data: List[Dict[str, str]], rsmi_col="reactions", symbol=">>"
-    ):
+        self,
+        compare: bool = True,
+        orientation: str = "vertical",
+        figsize: Tuple[int, int] = (10, 5),
+        label_position: str = "below",
+        dpi: int = 300,
+        bond_line_width: float = 6,
+        atom_label_font_size: int = 50,
+        padding: float = 0.001,
+    ) -> None:
         """
-        Initialize the CheckCarbonBalance class with reaction data.
+        Initialize the ReactionVisualizer.
 
         Parameters:
-        reactions_data (List[Dict[str, str]]): A list of dictionaries, each
-            containing reaction information.
+        - compare (bool): Whether to compare old and new reactions side by
+            side. Default is True.
+        - orientation (str): Orientation of comparison ('vertical' or
+            'horizontal'). Default is 'vertical'.
+        - figsize (Tuple[int, int]): Figure size (width, height) in inches.
+            Default is (10, 5).
+        - label_position (str): Position of labels ('above' or 'below') the
+            reaction images. Default is 'below'.
+        - dpi (int): Dots per inch for image resolution. Default is 300.
+        - bond_line_width (float): Width of bond lines in the reaction image.
+            Default is 6.
+        - atom_label_font_size (int): Font size for atom labels in the reaction
+            image. Default is 50.
+        - padding (float): Padding around the drawing in the reaction image.
+            Default is 0.001.
         """
-        self.reactions_data = reactions_data
-        self.rsmi_col = rsmi_col
-        self.symbol = symbol
+        self.compare = compare
+        self.orientation = orientation
+        self.figsize = figsize
+        self.label_position = label_position
+        self.dpi = dpi
+        self.bond_line_width = bond_line_width
+        self.atom_label_font_size = atom_label_font_size
+        self.padding = padding
 
     @staticmethod
-    def count_carbon_atoms(smiles: str) -> int:
+    def draw_molecule_with_atom_numbers(mol):
         """
-        Count the number of carbon atoms in a molecule represented by a SMILES
-        string.
+        Draw a molecule with atom numbers annotated.
 
-        Parameters:
-        smiles (str): A SMILES string.
-
-        Returns:
-        int: The number of carbon atoms in the molecule. Returns 0 if the
-            SMILES string is invalid.
+        Parameters
+        ----------
+        mol : RDKit Molecule object
+            The molecule to be drawn with atom numbers.
+
+        Returns
+        -------
+        mol : RDKit Molecule object
+            The molecule with atom numbers.
         """
-        mol = Chem.MolFromSmiles(smiles)
-        return (
-            sum(1 for atom in mol.GetAtoms() if atom.GetSymbol() == "C") if mol else 0
-        )
-
-    def check_carbon_balance(self) -> None:
+        mol_with_atom_numbers = Chem.Mol(mol)
+        for atom in mol_with_atom_numbers.GetAtoms():
+            atom.SetProp("atomLabel", str(atom.GetIdx()))
+        return mol_with_atom_numbers
+
+    def visualize_reaction(
+        self, reaction_str: str, show_atom_numbers: bool = False
+    ) -> Image:
         """
-        Check and update the carbon balance status for each reaction in the
-        reactions data.
+        Visualize a single chemical reaction and return the image.
 
-        The method updates each reaction dictionary in the reactions data with
-        a new key 'carbon_balance_check'. This key will have the value
-        'products' if the number of carbon atoms in the products is greater
-        than or equal to the reactants, and 'reactants' otherwise.
+        Parameters
+        ----------
+        reaction_str : str
+            A string representation of the reaction (e.g., 'C1=CC=CC=C1>>CCO').
+
+        Returns
+        -------
+        PIL.Image.Image
+            An image of the chemical reaction.
         """
-        for reaction in self.reactions_data:
-            try:
-                reactants_smiles, products_smiles = reaction[self.rsmi_col].split(
-                    self.symbol
-                )
-                reactants_carbon = sum(
-                    self.count_carbon_atoms(smiles)
-                    for smiles in reactants_smiles.split(".")
-                )
-                products_carbon = sum(
-                    self.count_carbon_atoms(smiles)
-                    for smiles in products_smiles.split(".")
-                )
-
-                if reactants_carbon >= products_carbon:
-                    reaction["carbon_balance_check"] = "products"
-                else:
-                    reaction["carbon_balance_check"] = "reactants"
-            except KeyError as e:
-                print(f"Key error: {e}")
-            except ValueError as e:
-                print(f"Value error: {e}")
-
-    def is_carbon_balance(self) -> None:
+        # Parse reactants and products from the reaction string
+        reactants_str, products_str = reaction_str.split(">>")
+        reactants = [Chem.MolFromSmiles(smiles) for smiles in reactants_str.split(".")]
+        products = [Chem.MolFromSmiles(smiles) for smiles in products_str.split(".")]
+
+        if show_atom_numbers:
+            reactants = [self.draw_molecule_with_atom_numbers(mol) for mol in reactants]
+            products = [self.draw_molecule_with_atom_numbers(mol) for mol in products]
+
+        rxn = AllChem.ChemicalReaction()
+        for reactant in reactants:
+            rxn.AddReactantTemplate(reactant)
+        for product in products:
+            rxn.AddProductTemplate(product)
+
+        # Set up RDKit drawer with customizable parameters
+        drawer = rdMolDraw2D.MolDraw2DCairo(2000, 600)  # Adjust canvas size as needed
+        opts = drawer.drawOptions()
+        opts.bondLineWidth = self.bond_line_width  # Increase bond line width
+        opts.atomLabelFontSize = (
+            self.atom_label_font_size
+        )  # Increase font size for atom labels
+        opts.padding = self.padding  # Adjust padding around the drawing
+
+        drawer.DrawReaction(rxn)
+        drawer.FinishDrawing()
+        return Image.open(io.BytesIO(drawer.GetDrawingText()))
+
+    def plot_reactions(
+        self,
+        data: Dict[str, str],
+        old_reaction_col: str,
+        new_reaction_col: str,
+        compare: bool = False,
+        orientation: str = "vertical",
+        savefig: bool = False,
+        pathname: Optional[str] = None,
+        dpi: int = 300,
+        show_atom_numbers: bool = False,
+    ) -> None:
         """
-        Check and update the carbon balance status for each reaction in the
-        reactions data.
+        Plot one or two chemical reactions for visualization.
 
-        The method updates each reaction dictionary in the reactions data with
-        a new key 'carbon_balance_check'. This key will have the value
-        'products' if the number of carbon atoms in the products is greater
-        than or equal to the reactants, and 'reactants' otherwise.
+        Parameters
+        ----------
+        data : Dict[str, str]
+            A dictionary containing the data with keys as column names and
+            values as reaction strings.
+        old_reaction_col : str
+            The column name containing the string representation of the old reaction.
+        new_reaction_col : str
+            The column name containing the string representation of the new reaction.
+        compare : bool, optional
+            If True, both the old and new reactions are plotted. Default is False.
+        orientation : str, optional
+            The layout orientation of the plots ('vertical' or 'horizontal').
+            Default is 'vertical'.
+        savefig : bool, optional
+            If True, saves the figure to the specified pathname. Default is False.
+        pathname : str, optional
+            Pathname to save the figure, if savefig is True.
+        dpi : int, optional
+            Resolution of the figure in dots per inch. Default is 300.
         """
-        for reaction in self.reactions_data:
-            try:
-                reactants_smiles, products_smiles = reaction[self.rsmi_col].split(
-                    self.symbol
-                )
-                reactants_carbon = sum(
-                    self.count_carbon_atoms(smiles)
-                    for smiles in reactants_smiles.split(".")
-                )
-                products_carbon = sum(
-                    self.count_carbon_atoms(smiles)
-                    for smiles in products_smiles.split(".")
-                )
-                reaction["is_carbon_balance"] = reactants_carbon == products_carbon
-
-            except KeyError as e:
-                print(f"Key error: {e}")
-            except ValueError as e:
-                print(f"Value error: {e}")
-
-
-def calculate_net_charge(sublist: list[dict[str, Union[str, int]]]) -> int:
-    """
-    Calculate the net charge from a list of molecules represented as SMILES
-    strings.
-
-    Args:
-        sublist: A list of dictionaries, each with a 'smiles' string and a
-            'Ratio' integer.
-
-    Returns:
-        The net charge of the sublist as an integer.
-    """
-    total_charge = 0
-    for item in sublist:
-        if "smiles" in item and "Ratio" in item:
-            mol = Chem.MolFromSmiles(item["smiles"])
-            if mol:
-                charge = (
-                    sum(abs(atom.GetFormalCharge()) for atom in mol.GetAtoms())
-                    * item["Ratio"]
-                )
-                total_charge += charge
-    return total_charge
-
-
-def save_reactions_to_pdf(
-    data: List[Dict[str, str]],
-    old_reaction_col: str,
-    new_reaction_col: str,
-    pdf_filename: str,
-    compare: bool = False,
-    orientation: str = "vertical",
-    show_atom_numbers: bool = False,
-):
-    """
-    Save a list of reaction visualizations to a PDF file.
-
-    Parameters
-    ----------
-    data : List[Dict[str, str]]
-        A list of dictionaries containing reaction data.
-    old_reaction_col : str
-        The column name containing the string representation of the old reaction.
-    new_reaction_col : str
-        The column name containing the string representation of the new reaction.
-    pdf_filename : str
-        The filename of the PDF to be saved.
-    compare : bool, optional
-        If True, both the old and new reactions are plotted. Default is False.
-    orientation : str, optional
-        The layout orientation of the plots ('vertical' or 'horizontal').
-        Default is 'vertical'.
-    show_atom_numbers : bool, optional
-        Whether to show atom numbers in the reaction visualizations.
-        Default is False.
-    scale_factor : float, optional
-        Factor to scale the reaction image size in the PDF. Default is 1.0.
-    title_font_size : int, optional
-        Font size for the title. Default is 14.
-
-    Notes
-    -----
-    The method plots each reaction using the plot_reactions method and saves
-    it to a PDF file. Each reaction is plotted on a separate page. The method
-    also handles scaling of the reaction image and includes a customizable
-    title for each reaction page in the PDF.
-    """
-    c = canvas.Canvas(pdf_filename, pagesize=landscape(letter))
-    page_width, page_height = landscape(letter)
-
-    for reaction_data in data:
-        # Create a figure using plot_reactions method
-        fig = ReactionVisualizer(figsize=(10, 5)).plot_reactions(
-            reaction_data,
-            old_reaction_col,
-            new_reaction_col,
-            compare,
-            orientation,
-            show_atom_numbers,
+        # Get the old and new reaction strings from the data
+        old_reaction_str = data[old_reaction_col]
+        new_reaction_str = data[new_reaction_col]
+
+        # Create reaction images
+        new_reaction_image = self.visualize_reaction(
+            new_reaction_str, show_atom_numbers
+        )
+        old_reaction_image = (
+            self.visualize_reaction(old_reaction_str, show_atom_numbers)
+            if compare
+            else None
         )
 
-        # Save figure to a temporary buffer
-        buf = io.BytesIO()
-        plt.savefig(buf, format="png")
-        plt.close(fig)
-        buf.seek(0)
-        img = Image.open(buf)
-
-        # Save the image to a temporary file
-        with tempfile.NamedTemporaryFile(suffix=".png") as img_temp:
-            img.save(img_temp, format="PNG")
-            img_temp.flush()
-
-            # Image dimensions
-            img_width, img_height = img.size
-            scale_factor = min(
-                (page_width - 100) / img_width, (page_height - 100) / img_height
+        # Set up plot layout
+        if compare:
+            nrows, ncols = (2, 1) if orientation == "vertical" else (1, 2)
+            fig, axs = plt.subplots(nrows, ncols, figsize=self.figsize, dpi=dpi)
+            ax_new = axs[1] if orientation == "vertical" else axs[0]
+            ax_old = axs[0] if orientation == "vertical" else axs[1]
+        else:
+            fig, ax = plt.subplots(figsize=self.figsize, dpi=dpi)
+
+        # Plotting logic
+        if compare:
+            ax_old.imshow(old_reaction_image)
+            ax_old.axis("off")
+            ax_new.imshow(new_reaction_image)
+            ax_new.axis("off")
+        else:
+            ax.imshow(new_reaction_image)
+            ax.axis("off")
+
+        # Setting titles
+        label_y_position = -0.1 if self.label_position == "below" else 1.1
+        if compare:
+            ax_old.set_title(
+                "Old Reaction", position=(0.5, label_y_position), weight="bold"
             )
-            scaled_width, scaled_height = (
-                img_width * scale_factor,
-                img_height * scale_factor,
+            ax_new.set_title(
+                "New Reaction", position=(0.5, label_y_position), weight="bold"
             )
-
-            # Calculate coordinates to center the image
-            x = (page_width - scaled_width) / 2
-            y = (page_height - scaled_height) / 2
-
-            # Draw the centered image
-            c.drawImage(
-                img_temp.name,
-                x,
-                y,
-                width=scaled_width,
-                height=scaled_height,
-                mask="auto",
+        else:
+            ax.set_title(
+                "New Reaction", position=(0.5, label_y_position), weight="bold"
             )
-            c.showPage()
-
-    c.save()
-    print(f"Saved reactions to {pdf_filename}")
 
+        # Saving the figure
+        if savefig and pathname:
+            fig.savefig(pathname, dpi=dpi)
 
-def remove_atom_mapping(smiles: str) -> str:
-    pattern = re.compile(r":\d+")
-    smiles = pattern.sub("", smiles)
-    pattern = re.compile(r"\[(?P<atom>(B|C|N|O|P|S|F|Cl|Br|I){1,2})(?:H\d?)?\]")
-    smiles = pattern.sub(r"\g<atom>", smiles)
-    return smiles
-
-
-def normalize_smiles(smiles: str) -> str:
-    smiles = smiles.replace("@", "")
-    if ">>" in smiles:
-        return ">>".join([normalize_smiles(t) for t in smiles.split(">>")])
-    elif "." in smiles:
-        token = sorted(
-            smiles.split("."),
-            key=lambda x: (sum(1 for c in x if c.isupper()), sum(ord(c) for c in x)),
-            reverse=True,
-        )
-        token = [normalize_smiles(t) for t in token]
-        token.sort(
-            key=lambda x: (sum(1 for c in x if c.isupper()), sum(ord(c) for c in x)),
-            reverse=True,
-        )
-        return ".".join(token)
-    else:
-        return Chem.CanonSmiles(remove_atom_mapping(smiles))
+        # plt.tight_layout()
+        return fig
```

### Comparing `synrbl-0.0.6/synrbl/SynUtils/data_utils.py` & `synrbl-0.0.7/synrbl/SynUtils/data_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynUtils/functional_group_utils.py` & `synrbl-0.0.7/synrbl/SynUtils/functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynUtils/rsmi_utils.py` & `synrbl-0.0.7/synrbl/SynUtils/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/synrbl/SynVis/mcs_visualizer.py` & `synrbl-0.0.7/synrbl/SynVis/mcs_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/.gitignore` & `synrbl-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/LICENSE` & `synrbl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.6/README.md` & `synrbl-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,43 @@
+Metadata-Version: 2.3
+Name: synrbl
+Version: 0.0.7
+Summary: Synthesis Rebalancing Framework for Computational Chemistry
+Project-URL: homepage, https://github.com/TieuLongPhan/SynRBL
+Project-URL: source, https://github.com/TieuLongPhan/SynRBL
+Project-URL: issues, https://github.com/TieuLongPhan/SynRBL/issues
+Author-email: Tieu Long Phan <long.tieu_phan@uni-leipzig.de>, Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Requires-Dist: imbalanced-learn>=0.12.0
+Requires-Dist: joblib>=1.3.2
+Requires-Dist: rdkit>=2023.9.4
+Requires-Dist: reportlab>=4.1.0
+Requires-Dist: scikit-learn>=1.4.1.post1
+Requires-Dist: seaborn>=0.13.2
+Requires-Dist: xgboost>=2.0.3
+Description-Content-Type: text/markdown
+
 # SynRBL: Synthesis Rebalancing Framework
 
 SynRBL is a toolkit tailored for computational chemistry, aimed at correcting imbalances in chemical reactions. It employs a dual strategy: a rule-based method for adjusting non-carbon elements and an mcs-based (maximum common substructure) technique for carbon element adjustments.
 
 ![screenshot](./Docs/Images/Flowchart.png)
 
 
 ## Table of Contents
-- [Repository Structure](#repository-structure)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
 - [Acknowledgments](#acknowledgments)
 
-## Repository Structure
-
-SynRBL is organized into several key components, each dedicated to a specific aspect of chemical data processing:
-
-### Main Components
-
-- `SynRBL/`: Main package directory
-  - `SynProcessor/`: Data processing module
-  - `SynRuleImputer/`: Rule-based imputation module
-  - `SynMCSImputer/`: MCS-based imputation module
-  - `SynChemImputer/`: MCS-based imputation module
-  - `SynVis/`: Data visualization module
-
-### Test Suite
-
-- `tests/`: Test scripts and related files
-  - `SynProcessor/`: Tests for SynExtract module
-  - `SynRuleImputer/`: Tests for SynRuleImpute module
-  - `SynMCSImputer/`: Tests for MCS-based imputation module
-  - `SynChemImputer/`: Tests for MCS-based imputation module
-  - `SynVis/`: Tests for SynVis module
-
-### Additional Resources
-
-- `License`: License document
-- `README.md`: Overview and documentation
-- `setup.py`: Installation
-- `.gitignore`: Configuration for ignoring certain files and directories
 
 ## Installation
 
 To install and set up the SynRBL framework, follow these steps. Please ensure you have Python 3.11 or later installed on your system.
 
 ### Prerequisites
 
@@ -73,38 +66,42 @@
   Or Conda
 
   ```bash
   conda create --name synrbl-env python=3.11
   conda activate synrbl-env
   ```
 
-3. **Cloning and Installing SynRBL:**
+3. **Install with pip:**
   Clone the SynRBL repository from GitHub and install it:
 
   ```bash
-  git clone https://github.com/TieuLongPhan/SynRBL.git
-  cd SynRBL
-  pip install .
+  pip install synrbl
   ```
 
 4. **Verify Installation:**
   After installation, you can verify that SynRBL is correctly installed by running a simple test or checking the package version.
 
   ```python
   python -c "import synrbl; print(synrbl.__version__)"
   ```
 
 ## Usage
-
+1. **Jupyter Notebook:**
   ```python
   from synrbl import Balancer
   ```
+2. **Command line**
+  ```bash
+  python -m synrbl run --help
+  ```
 
-
-TODO
+3. **Reproduce the experiment**
+  ```bash
+  python -m synrbl run -o validation_results.csv -p 4 ./Data/Validation_set/validation_set.csv
+  ```
 
 ## Contributing
 - [Tieu-Long Phan](https://tieulongphan.github.io/)
 - [Klaus Weinbauer](https://github.com/klausweinbauer)
 
 ## License
```

### Comparing `synrbl-0.0.6/pyproject.toml` & `synrbl-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synrbl"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
 	{name="Tieu Long Phan", email="long.tieu_phan@uni-leipzig.de"}, 
 	{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}
 	]
 description = "Synthesis Rebalancing Framework for Computational Chemistry"
 readme = "README.md"
 requires-python = ">=3.11"
```

