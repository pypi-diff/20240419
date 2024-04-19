# Comparing `tmp/sctreeshap-0.7.6.1.tar.gz` & `tmp/sctreeshap-0.7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sctreeshap-0.7.6.1.tar", last modified: Tue Feb  1 13:19:31 2022, max compression
+gzip compressed data, was "sctreeshap-0.7.6.2.tar", last modified: Fri Apr 19 08:44:34 2024, max compression
```

## Comparing `sctreeshap-0.7.6.1.tar` & `sctreeshap-0.7.6.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2022-02-01 13:19:31.435986 sctreeshap-0.7.6.1/
--rw-rw-rw-   0        0        0     1087 2022-02-01 13:06:44.000000 sctreeshap-0.7.6.1/LICENSE
--rw-rw-rw-   0        0        0    10237 2022-02-01 13:19:31.435986 sctreeshap-0.7.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     9703 2022-02-01 13:19:20.000000 sctreeshap-0.7.6.1/README.md
-drwxrwxrwx   0        0        0        0 2022-02-01 13:19:31.433987 sctreeshap-0.7.6.1/sctreeshap.egg-info/
--rw-rw-rw-   0        0        0    10237 2022-02-01 13:19:31.000000 sctreeshap-0.7.6.1/sctreeshap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2022-02-01 13:19:31.000000 sctreeshap-0.7.6.1/sctreeshap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-01 13:19:31.000000 sctreeshap-0.7.6.1/sctreeshap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      231 2022-02-01 13:19:31.000000 sctreeshap-0.7.6.1/sctreeshap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-02-01 13:19:31.000000 sctreeshap-0.7.6.1/sctreeshap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0   129407 2022-02-01 13:17:04.000000 sctreeshap-0.7.6.1/sctreeshap.py
--rw-rw-rw-   0        0        0       42 2022-02-01 13:19:31.435986 sctreeshap-0.7.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1294 2022-02-01 13:17:09.000000 sctreeshap-0.7.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:44:34.165408 sctreeshap-0.7.6.2/
+-rw-rw-rw-   0        0        0     1087 2024-04-19 08:17:45.000000 sctreeshap-0.7.6.2/LICENSE
+-rw-rw-rw-   0        0        0    11082 2024-04-19 08:44:34.154409 sctreeshap-0.7.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10129 2024-04-19 08:43:28.000000 sctreeshap-0.7.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 08:44:34.147410 sctreeshap-0.7.6.2/sctreeshap.egg-info/
+-rw-rw-rw-   0        0        0    11082 2024-04-19 08:44:33.000000 sctreeshap-0.7.6.2/sctreeshap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-19 08:44:33.000000 sctreeshap-0.7.6.2/sctreeshap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:44:33.000000 sctreeshap-0.7.6.2/sctreeshap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2024-04-19 08:44:33.000000 sctreeshap-0.7.6.2/sctreeshap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 08:44:33.000000 sctreeshap-0.7.6.2/sctreeshap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0   129457 2024-04-19 08:35:34.000000 sctreeshap-0.7.6.2/sctreeshap.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:44:34.165408 sctreeshap-0.7.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1257 2024-04-19 08:14:36.000000 sctreeshap-0.7.6.2/setup.py
```

### Comparing `sctreeshap-0.7.6.1/LICENSE` & `sctreeshap-0.7.6.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Haoxuan Xie
+Copyright (c) 2024 Haoxuan Xie
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sctreeshap-0.7.6.1/PKG-INFO` & `sctreeshap-0.7.6.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,32 @@
-Metadata-Version: 2.1
-Name: sctreeshap
-Version: 0.7.6.1
-Summary: sctreeshap: a cluster tree data structure, and for shap analysis
-Home-page: https://github.com/ForwardStar/sctreeshap
-Author: Haoxuan Xie
-Author-email: haoxuanxie@link.cuhk.edu.cn
-License: LICENSE
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sctreeshap
 
-When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree.
+When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree. Following cluster tree represents [Allen Human Brain Atlas](https://human.brain-map.org/):
 
 ![clustertree.png](https://i.loli.net/2021/07/19/2bBatvnr45WczpK.png)
 
-We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. sctreeshap constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
+We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. This package ``sctreeshap`` constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
 
 Github repo:
 
 https://github.com/ForwardStar/sctreeshap
 
-# v0.7.6 && v0.7.6.1 Update
+# v0.7.6 && v0.7.6.1 && v0.7.6.2 Update
+
+Resolve dependency error:
+- Replace ``pathlib`` with ``pathlib2`` since ``pathlib`` has no longer been supported in Python 3.10;
+- Remove deprecated sklearn dependency.
 
-Resolve dependency error: replace pathlib with pathlib2 since pathlib has no longer been supported in Python 3.10.
+Bug fixes: fix function ``geneFiltering`` error for the deprecated ``pandas.DataFrame.iteritems()`` function.
 
 # v0.7.5 Update
 
 - Custom model supported.
 
-In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using 'geneFiltering()' before setting output as 'probability'.
+In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using ``geneFiltering()`` before setting output as ``probability``.
 
 A sample code is as follows:
 
 ```python
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
@@ -62,15 +50,15 @@
     "model_output" : 'probability', # set output mode as 'probability'
     "bar_plot" : True,
     "beeswarm" : True,
     "decision_plot" : True
 })
 ```
 
-While in v0.7.5, we supported custom models in 'explainBinary()' and 'explainMulti()'. Currently, there is a new parameter 'model' in the two function. You can set model='XGBClassifier', model='RandomForestClassifier' or model='DecisionTreeClassifier'. However, in the most cases the default XGBClassifier has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
+While in v0.7.5, we supported custom models in ``explainBinary()`` and ``explainMulti()``. Currently, there is a new parameter ``model`` in the two function. You can set ``model='XGBClassifier'``, ``model='RandomForestClassifier'`` or ``model='DecisionTreeClassifier'``. However, in the most cases the default ``XGBClassifier`` has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
 
 # Documentations
 
 ## Installing sctreeshap
 
 Directly install by pip:
 
@@ -84,15 +72,15 @@
 conda create -n sctreeshap python=3.8
 conda activate sctreeshap
 pip install sctreeshap
 ```
 
 ## Example
 
-An example dataset, human brain MTG cell type, can be analyzed as default:
+An example dataset, [human brain MTG cell type](https://www.nature.com/articles/s41586-019-1506-7), can be analyzed as default:
 
 ```python
 # Run in Jupyter Notebook
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
 sample_dataset = sample.loadDefault()
@@ -214,32 +202,32 @@
 After reading in data, you can select a branch in the cluster tree. Cells with clusters not under the branch will be filtered:
 
 ```python
 # Select non-neuron branch: n70
 data = Sample.selectBranch(data, 'n70')
 ```
 
-You can also filter low-expressed genes, housekeeping genes and general genes by:
+You can also filter low-expressed genes, [housekeeping genes](https://housekeeping.unicamp.br/) and general genes by:
 
 ```python
 prefix = ["MT", "RPS", "RPL", "HSP", "HLA"]
 housekeeping = Sample.loadHousekeeping('human')
 data = Sample.geneFiltering(data, min_partial=0.3, gene_set=housekeeping, gene_prefix=prefix, use_PCA=False)
 print(data)
 ```
 
-Then genes expressed in <30% cells will be filtered. Genes in gene_set or with prefix in gene_prefix will also be filtered.
+Then genes expressed in <30% cells will be filtered. Genes in ``gene_set`` or with prefix in ``gene_prefix`` will also be filtered.
 
 You can merge clusters under a branch if needed:
 
 ```python
 data = Sample.mergeBranch(data, 'n73')
 ```
 
-This relabels cells with cluster ['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP'] as 'n73'.
+This relabels cells with cluster ``['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP']`` as ``n73``.
 
 ## Displaying Shap Figures
 
 Note: this part is recommended to run in jupyter notebook.
 
 After reading in the data and filtering, you can build multi-classification model and generate shap figures:
 
@@ -274,15 +262,15 @@
         "decision_plot": False
     }
 )
 ```
 
 ## Get Shap Values and Marker Genes
 
-After running explainBinary() or explainMulti(), you can run:
+After running ``explainBinary()`` or ``explainMulti()``, you can run:
 
 ```python
 shap_values = Sample.getShapValues()
 marker_genes = Sample.getTopGenes()
 ```
 
 to get shapley values and marker genes (with top absolute mean shap values).
@@ -298,9 +286,7 @@
 and query the details of a function by:
 
 ```python
 function_name = 'readData' # Can be whatever the function in the class
 print(Sample.help(function_name))
 ```
 
-
-
```

### Comparing `sctreeshap-0.7.6.1/README.md` & `sctreeshap-0.7.6.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,61 @@
+Metadata-Version: 2.1
+Name: sctreeshap
+Version: 0.7.6.2
+Summary: sctreeshap: a cluster tree data structure, and for shap analysis
+Home-page: https://github.com/ForwardStar/sctreeshap
+Author: Haoxuan Xie
+Author-email: haoxuanxie@link.cuhk.edu.cn
+License: LICENSE
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: shap>=0.39.0
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: anndata>=0.7.6
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: pandas>=1.2.4
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: imblearn>=0.0
+Requires-Dist: imbalanced-learn>=0.8.0
+Requires-Dist: xgboost>=1.4.2
+Requires-Dist: loompy>=3.0.6
+Requires-Dist: tqdm>=4.61.2
+Requires-Dist: requests>=2.26.0
+Requires-Dist: pathlib2>=2.0
+Requires-Dist: pip>=21.1.3
+
 # sctreeshap
 
-When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree.
+When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree. Following cluster tree represents [Allen Human Brain Atlas](https://human.brain-map.org/):
 
 ![clustertree.png](https://i.loli.net/2021/07/19/2bBatvnr45WczpK.png)
 
-We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. sctreeshap constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
+We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. This package ``sctreeshap`` constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
 
 Github repo:
 
 https://github.com/ForwardStar/sctreeshap
 
-# v0.7.6 && v0.7.6.1 Update
+# v0.7.6 && v0.7.6.1 && v0.7.6.2 Update
+
+Resolve dependency error:
+- Replace ``pathlib`` with ``pathlib2`` since ``pathlib`` has no longer been supported in Python 3.10;
+- Remove deprecated sklearn dependency.
 
-Resolve dependency error: replace pathlib with pathlib2 since pathlib has no longer been supported in Python 3.10.
+Bug fixes: fix function ``geneFiltering`` error for the deprecated ``pandas.DataFrame.iteritems()`` function.
 
 # v0.7.5 Update
 
 - Custom model supported.
 
-In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using 'geneFiltering()' before setting output as 'probability'.
+In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using ``geneFiltering()`` before setting output as ``probability``.
 
 A sample code is as follows:
 
 ```python
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
@@ -46,15 +79,15 @@
     "model_output" : 'probability', # set output mode as 'probability'
     "bar_plot" : True,
     "beeswarm" : True,
     "decision_plot" : True
 })
 ```
 
-While in v0.7.5, we supported custom models in 'explainBinary()' and 'explainMulti()'. Currently, there is a new parameter 'model' in the two function. You can set model='XGBClassifier', model='RandomForestClassifier' or model='DecisionTreeClassifier'. However, in the most cases the default XGBClassifier has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
+While in v0.7.5, we supported custom models in ``explainBinary()`` and ``explainMulti()``. Currently, there is a new parameter ``model`` in the two function. You can set ``model='XGBClassifier'``, ``model='RandomForestClassifier'`` or ``model='DecisionTreeClassifier'``. However, in the most cases the default ``XGBClassifier`` has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
 
 # Documentations
 
 ## Installing sctreeshap
 
 Directly install by pip:
 
@@ -68,15 +101,15 @@
 conda create -n sctreeshap python=3.8
 conda activate sctreeshap
 pip install sctreeshap
 ```
 
 ## Example
 
-An example dataset, human brain MTG cell type, can be analyzed as default:
+An example dataset, [human brain MTG cell type](https://www.nature.com/articles/s41586-019-1506-7), can be analyzed as default:
 
 ```python
 # Run in Jupyter Notebook
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
 sample_dataset = sample.loadDefault()
@@ -198,32 +231,32 @@
 After reading in data, you can select a branch in the cluster tree. Cells with clusters not under the branch will be filtered:
 
 ```python
 # Select non-neuron branch: n70
 data = Sample.selectBranch(data, 'n70')
 ```
 
-You can also filter low-expressed genes, housekeeping genes and general genes by:
+You can also filter low-expressed genes, [housekeeping genes](https://housekeeping.unicamp.br/) and general genes by:
 
 ```python
 prefix = ["MT", "RPS", "RPL", "HSP", "HLA"]
 housekeeping = Sample.loadHousekeeping('human')
 data = Sample.geneFiltering(data, min_partial=0.3, gene_set=housekeeping, gene_prefix=prefix, use_PCA=False)
 print(data)
 ```
 
-Then genes expressed in <30% cells will be filtered. Genes in gene_set or with prefix in gene_prefix will also be filtered.
+Then genes expressed in <30% cells will be filtered. Genes in ``gene_set`` or with prefix in ``gene_prefix`` will also be filtered.
 
 You can merge clusters under a branch if needed:
 
 ```python
 data = Sample.mergeBranch(data, 'n73')
 ```
 
-This relabels cells with cluster ['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP'] as 'n73'.
+This relabels cells with cluster ``['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP']`` as ``n73``.
 
 ## Displaying Shap Figures
 
 Note: this part is recommended to run in jupyter notebook.
 
 After reading in the data and filtering, you can build multi-classification model and generate shap figures:
 
@@ -258,15 +291,15 @@
         "decision_plot": False
     }
 )
 ```
 
 ## Get Shap Values and Marker Genes
 
-After running explainBinary() or explainMulti(), you can run:
+After running ``explainBinary()`` or ``explainMulti()``, you can run:
 
 ```python
 shap_values = Sample.getShapValues()
 marker_genes = Sample.getTopGenes()
 ```
 
 to get shapley values and marker genes (with top absolute mean shap values).
```

### Comparing `sctreeshap-0.7.6.1/sctreeshap.egg-info/PKG-INFO` & `sctreeshap-0.7.6.2/sctreeshap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 Metadata-Version: 2.1
 Name: sctreeshap
-Version: 0.7.6.1
+Version: 0.7.6.2
 Summary: sctreeshap: a cluster tree data structure, and for shap analysis
 Home-page: https://github.com/ForwardStar/sctreeshap
 Author: Haoxuan Xie
 Author-email: haoxuanxie@link.cuhk.edu.cn
 License: LICENSE
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: shap>=0.39.0
+Requires-Dist: matplotlib>=3.4.2
+Requires-Dist: anndata>=0.7.6
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: pandas>=1.2.4
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: imblearn>=0.0
+Requires-Dist: imbalanced-learn>=0.8.0
+Requires-Dist: xgboost>=1.4.2
+Requires-Dist: loompy>=3.0.6
+Requires-Dist: tqdm>=4.61.2
+Requires-Dist: requests>=2.26.0
+Requires-Dist: pathlib2>=2.0
+Requires-Dist: pip>=21.1.3
 
 # sctreeshap
 
-When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree.
+When doing single-cell RNA sequencing work, we firstly do clustering by community detection. Then we match the clusters to major cell types, which forms a cluster tree. Following cluster tree represents [Allen Human Brain Atlas](https://human.brain-map.org/):
 
 ![clustertree.png](https://i.loli.net/2021/07/19/2bBatvnr45WczpK.png)
 
-We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. sctreeshap constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
+We usually need to select a branch for analysis, which helps us investigate on gene differential expressions on cell subtypes. This package ``sctreeshap`` constructs a data structure, which helps us quickly filter data whose clusters are under a specific branch (or in a specific cluster set). Moreover, it can run shap automatically to indicate marker genes.
 
 Github repo:
 
 https://github.com/ForwardStar/sctreeshap
 
-# v0.7.6 && v0.7.6.1 Update
+# v0.7.6 && v0.7.6.1 && v0.7.6.2 Update
 
-Resolve dependency error: replace pathlib with pathlib2 since pathlib has no longer been supported in Python 3.10.
+Resolve dependency error:
+- Replace ``pathlib`` with ``pathlib2`` since ``pathlib`` has no longer been supported in Python 3.10;
+- Remove deprecated sklearn dependency.
+
+Bug fixes: fix function ``geneFiltering`` error for the deprecated ``pandas.DataFrame.iteritems()`` function.
 
 # v0.7.5 Update
 
 - Custom model supported.
 
-In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using 'geneFiltering()' before setting output as 'probability'.
+In v0.7.0--v0.7.4, we mainly worked for supporting probability output for shap values. This is not stable and could not deal with a large feature set. Therefore, try using ``geneFiltering()`` before setting output as ``probability``.
 
 A sample code is as follows:
 
 ```python
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
@@ -62,15 +79,15 @@
     "model_output" : 'probability', # set output mode as 'probability'
     "bar_plot" : True,
     "beeswarm" : True,
     "decision_plot" : True
 })
 ```
 
-While in v0.7.5, we supported custom models in 'explainBinary()' and 'explainMulti()'. Currently, there is a new parameter 'model' in the two function. You can set model='XGBClassifier', model='RandomForestClassifier' or model='DecisionTreeClassifier'. However, in the most cases the default XGBClassifier has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
+While in v0.7.5, we supported custom models in ``explainBinary()`` and ``explainMulti()``. Currently, there is a new parameter ``model`` in the two function. You can set ``model='XGBClassifier'``, ``model='RandomForestClassifier'`` or ``model='DecisionTreeClassifier'``. However, in the most cases the default ``XGBClassifier`` has the best accuracy. You can also set the model as one you defined, like some neuron networks, which may even outperform xgboost models. We do not ensure that shap explainer supports your custom model.
 
 # Documentations
 
 ## Installing sctreeshap
 
 Directly install by pip:
 
@@ -84,15 +101,15 @@
 conda create -n sctreeshap python=3.8
 conda activate sctreeshap
 pip install sctreeshap
 ```
 
 ## Example
 
-An example dataset, human brain MTG cell type, can be analyzed as default:
+An example dataset, [human brain MTG cell type](https://www.nature.com/articles/s41586-019-1506-7), can be analyzed as default:
 
 ```python
 # Run in Jupyter Notebook
 from sctreeshap import sctreeshap
 
 sample = sctreeshap()
 sample_dataset = sample.loadDefault()
@@ -214,32 +231,32 @@
 After reading in data, you can select a branch in the cluster tree. Cells with clusters not under the branch will be filtered:
 
 ```python
 # Select non-neuron branch: n70
 data = Sample.selectBranch(data, 'n70')
 ```
 
-You can also filter low-expressed genes, housekeeping genes and general genes by:
+You can also filter low-expressed genes, [housekeeping genes](https://housekeeping.unicamp.br/) and general genes by:
 
 ```python
 prefix = ["MT", "RPS", "RPL", "HSP", "HLA"]
 housekeeping = Sample.loadHousekeeping('human')
 data = Sample.geneFiltering(data, min_partial=0.3, gene_set=housekeeping, gene_prefix=prefix, use_PCA=False)
 print(data)
 ```
 
-Then genes expressed in <30% cells will be filtered. Genes in gene_set or with prefix in gene_prefix will also be filtered.
+Then genes expressed in <30% cells will be filtered. Genes in ``gene_set`` or with prefix in ``gene_prefix`` will also be filtered.
 
 You can merge clusters under a branch if needed:
 
 ```python
 data = Sample.mergeBranch(data, 'n73')
 ```
 
-This relabels cells with cluster ['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP'] as 'n73'.
+This relabels cells with cluster ``['OPC L1-6 PDGFRA', 'Astro L1-6 FGFR3 SLC14A1', 'Astro L1-2 FGFR3 GFAP']`` as ``n73``.
 
 ## Displaying Shap Figures
 
 Note: this part is recommended to run in jupyter notebook.
 
 After reading in the data and filtering, you can build multi-classification model and generate shap figures:
 
@@ -274,15 +291,15 @@
         "decision_plot": False
     }
 )
 ```
 
 ## Get Shap Values and Marker Genes
 
-After running explainBinary() or explainMulti(), you can run:
+After running ``explainBinary()`` or ``explainMulti()``, you can run:
 
 ```python
 shap_values = Sample.getShapValues()
 marker_genes = Sample.getTopGenes()
 ```
 
 to get shapley values and marker genes (with top absolute mean shap values).
@@ -298,9 +315,7 @@
 and query the details of a function by:
 
 ```python
 function_name = 'readData' # Can be whatever the function in the class
 print(Sample.help(function_name))
 ```
 
-
-
```

### Comparing `sctreeshap-0.7.6.1/sctreeshap.py` & `sctreeshap-0.7.6.2/sctreeshap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __name__ = 'sctreeshap'
-__version__ = "0.7.6.1"
+__version__ = "0.7.6.2"
 headers = {'User-Agent':'Mozilla/5.0 (Windows; U; Windows NT 6.1; en-US; rv:1.9.1.6) Gecko/20091201 Firefox/3.5.6'}
 
 import time
 import threading
 import numpy as np
 import anndata as ad
 import pandas as pd
@@ -818,30 +818,30 @@
             files = "Housekeeping_GenesHuman.csv"
             if not os.path.exists(data_directory) or not os.path.isfile(os.path.join(data_directory, files)):
                 from pathlib import Path
                 print("First time loading. Downloading " + files + "...")
                 if not os.path.exists(data_directory):
                     os.mkdir(data_directory)
                 path = Path(os.path.join(data_directory, files))
-                url = "https://housekeeping.unicamp.br/Housekeeping_GenesHuman.csv"
+                url = "https://raw.githubusercontent.com/ForwardStar/sctreeshap/main/Housekeeping_GenesHuman.csv"
                 download(url, path)
             file = open(os.path.join(data_directory, files), "r", encoding='utf-8')
             for lines in file.readlines()[1:]:
                 lines = lines.split(';')
                 hkg.append(lines[1])
         elif category == 'mouse':
             import os
             files = "Housekeeping_GenesMouse.csv"
             if not os.path.exists(data_directory) or not os.path.isfile(os.path.join(data_directory, files)):
                 from pathlib import Path
                 print("First time loading. Downloading " + files + "...")
                 if not os.path.exists(data_directory):
                     os.mkdir(data_directory)
                 path = Path(os.path.join(data_directory, files))
-                url = "https://housekeeping.unicamp.br/Housekeeping_GenesMouse.csv"
+                url = "https://raw.githubusercontent.com/ForwardStar/sctreeshap/main/Housekeeping_GenesMouse.csv"
                 download(url, path)
             file = open(os.path.join(data_directory, files), "r", encoding='utf-8')
             for lines in file.readlines()[1:]:
                 lines = lines.split(';')
                 hkg.append(lines[1])
         else:
             raise ValueError("in method 'sctreeshap.sctreeshap.loadHousekeeping()' (in file '" + __file__ + "'), parameter 'category' receives an unrecognized value: '" + category + "', expected 'human' or 'mouse'.")
@@ -873,15 +873,15 @@
                         return True
                 return False
             target = [item for item in data.columns.values if check(item)]
             data = data.drop(target, axis=1)
         if isinstance(min_partial, float):
             target = []
             cluster = data.columns.values[-1]
-            for idx, columns in data.iteritems():
+            for idx, _ in data.items():
                 if idx != cluster:
                     expression = data[idx].to_numpy()
                     expression = expression[expression > 0]
                     if len(expression) / len(data) < min_partial:
                         target.append(idx)
             data = data.drop(target, axis=1)
         if isAnnData:
```

### Comparing `sctreeshap-0.7.6.1/setup.py` & `sctreeshap-0.7.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="sctreeshap",
-  version="0.7.6.1",
+  version="0.7.6.2",
   author="Haoxuan Xie",
   author_email="haoxuanxie@link.cuhk.edu.cn",
   url="https://github.com/ForwardStar/sctreeshap",
   py_modules=["sctreeshap"],
   description="sctreeshap: a cluster tree data structure, and for shap analysis",
   long_description=long_description,
   long_description_content_type="text/markdown",
@@ -20,15 +20,14 @@
   "Operating System :: OS Independent",
   ],
   install_requires=['shap>=0.39.0',
                     'matplotlib>=3.4.2',
                     'anndata>=0.7.6',
                     'numpy>=1.19.5',
                     'pandas>=1.2.4',
-                    'sklearn>=0.0',
                     'scikit-learn>=0.24.2',
                     'imblearn>=0.0',
                     'imbalanced-learn>=0.8.0',
                     'xgboost>=1.4.2',
                     'loompy>=3.0.6',
                     'tqdm>=4.61.2',
                     'requests>=2.26.0',
```

