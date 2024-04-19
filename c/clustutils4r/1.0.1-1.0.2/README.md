# Comparing `tmp/clustutils4r-1.0.1.tar.gz` & `tmp/clustutils4r-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-1.0.1.tar", last modified: Fri Apr 12 05:40:18 2024, max compression
+gzip compressed data, was "clustutils4r-1.0.2.tar", last modified: Fri Apr 19 05:04:08 2024, max compression
```

## Comparing `clustutils4r-1.0.1.tar` & `clustutils4r-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-1.0.1/LICENSE
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     3328 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     2696 2024-04-12 05:38:56.000000 clustutils4r-1.0.1/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2024-04-12 05:39:52.000000 clustutils4r-1.0.1/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:29:24.000000 clustutils4r-1.0.1/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-1.0.1/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25864 2024-04-12 04:58:42.000000 clustutils4r-1.0.1/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:40:18.204480 clustutils4r-1.0.1/src/clustutils4r.egg-info/
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     3328 2024-04-12 05:40:18.000000 clustutils4r-1.0.1/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      266 2024-04-12 05:40:18.000000 clustutils4r-1.0.1/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-12 05:40:18.000000 clustutils4r-1.0.1/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2024-04-12 05:40:18.000000 clustutils4r-1.0.1/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:04:08.605111 clustutils4r-1.0.2/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-1.0.2/LICENSE
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     3328 2024-04-19 05:04:08.601112 clustutils4r-1.0.2/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     2696 2024-04-12 05:38:56.000000 clustutils4r-1.0.2/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2024-04-19 05:03:46.000000 clustutils4r-1.0.2/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-19 05:04:08.605111 clustutils4r-1.0.2/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:29:24.000000 clustutils4r-1.0.2/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:04:08.601112 clustutils4r-1.0.2/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:04:08.601112 clustutils4r-1.0.2/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-1.0.2/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    24988 2024-04-19 04:53:07.000000 clustutils4r-1.0.2/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-19 05:04:08.601112 clustutils4r-1.0.2/src/clustutils4r.egg-info/
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     3328 2024-04-19 05:04:08.000000 clustutils4r-1.0.2/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      266 2024-04-19 05:04:08.000000 clustutils4r-1.0.2/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-19 05:04:08.000000 clustutils4r-1.0.2/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2024-04-19 05:04:08.000000 clustutils4r-1.0.2/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-1.0.1/LICENSE` & `clustutils4r-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-1.0.1/PKG-INFO` & `clustutils4r-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clustutils4r-1.0.1/README.md` & `clustutils4r-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clustutils4r-1.0.1/pyproject.toml` & `clustutils4r-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-1.0.1/setup.py` & `clustutils4r-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `clustutils4r-1.0.1/src/clustutils4r/eval_clustering.py` & `clustutils4r-1.0.2/src/clustutils4r/eval_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 ## Features Clustering
 from sklearn.cluster import KMeans, SpectralClustering, \
     AgglomerativeClustering, \
     AffinityPropagation, MeanShift, \
     DBSCAN, HDBSCAN, \
     OPTICS, Birch
+
 from sklearn.metrics import silhouette_samples, silhouette_score
 from sklearn.metrics import calinski_harabasz_score, davies_bouldin_score
 
 from sklearn.metrics import rand_score, adjusted_rand_score
 from sklearn.metrics import mutual_info_score, adjusted_mutual_info_score, normalized_mutual_info_score
 from sklearn.metrics import homogeneity_completeness_v_measure
 from sklearn.metrics import fowlkes_mallows_score
@@ -271,15 +272,15 @@
 
 def plot_grid_search_metrics(hparam_search_results, metric="Calinski-Harabasz", show=False, save=False, save_dir=None):
     hparams = [col for col in hparam_search_results.columns if col.startswith("param_")]
     metrics = [col for col in hparam_search_results.columns if col.startswith("mean_test_")]
 
     dimslist4parcoordplot = []
     for hparam_name in hparams:
-        if hparam_search_results[hparam_name].dtype in ["object", "categorical"]: 
+        if hparam_search_results[hparam_name].dtype in ["object", "categorical", "bool"]: 
             le = LabelEncoder()
             encoded_hparam = le.fit_transform(hparam_search_results[hparam_name])
             dimslist4parcoordplot.append(
                 dict(   
                         ticktext=le.classes_, tickvals=le.transform(le.classes_),
                         label=hparam_name.split("param_")[-1], 
                         values=encoded_hparam
@@ -307,31 +308,29 @@
                     showscale = True,
                 ),
             dimensions = dimslist4parcoordplot
         )
     )
     # fig.update_layout(width=1500, height=500)
     if save:
+        fig.update_layout(width=2000, height=500)
         fig.write_html(save_dir+"/parcoord_plot.html")
         fig.write_image(save_dir+"/parcoord_plot.png")
     if show:
         fig.show()
 
 def cluster_feats(X=None, gt_labels=[],
-                n_clusters_range = range(3,21),
-                clustering_algorithms=["KMeans", "AgglomerativeClustering", "HDBSCAN", "MeanShift"], 
-                num_runs=1, best_model_metric="Calinski-Harabasz",
-                make_silhoutte_plots=False, embed_data_in_2d = False,
-                show=False, save=False, save_dir=None):
-    '''
-    Cluster fixed-length segments of time as represented by a set of statistical features derived from time-segments data of all channels using partition clustering approach.
-    In partition clustering approach, the user must provide the number of clusters as a parameter and the dataset gets partitioned into those many clusters.
-    '''
-    # if len(gt_labels)!=0:
-    #     print("Ground truth labels provided. Computing ground truth-based clustering metrics along with non-ground truth based metrics.") 
+                    n_clusters_range = range(3,21),
+                    clustering_algorithms=["KMeans", "AgglomerativeClustering", "HDBSCAN", "MeanShift"], 
+                    num_runs=1, best_model_metric="Calinski-Harabasz",
+                    make_silhoutte_plots=False, embed_data_in_2d = False,
+                    show=False, save=False, save_dir=None):
+
+    if len(gt_labels)!=0:
+        print("Ground truth labels provided. Computing ground truth-based clustering metrics along with non-ground truth based metrics.") 
     
     # print("[Implementation: pyclustertend] Hopkins Statistic (0=clustered, 0.5=randomly distributed) : {}".format(hopkins_statistic(X).round(3)))
     # print("[Implementation: mine] Hopkins Statistic (1=clustered, 0.5=random, 0=uniforrm) : {}".format(hopkins_statistic_v2(X).round(3)))
    
     if len(gt_labels)!=0:
         print("Ground truth labels provided. Computing ground truth-based clustering metrics along with non-ground truth based metrics.")
         def scorer(estimator, X, y):
@@ -524,26 +523,15 @@
         with open(os.path.join(save_dir, 'best_model_info.json'), 'w') as f:
             json.dump(best_model_info, f, default=str)
         ## Save the best overall model using joblib
         joblib.dump(best_estimator_overall, os.path.join(save_dir, f'best_model.joblib'))
 
     return best_estimator_overall, grid_search_results
 
-def eval_clustering(X=None, gt_labels=[], 
-                    num_runs=1, 
-                    best_model_metric="Calinski-Harabasz",
-                    make_silhoutte_plots=False, embed_data_in_2d=False,
-                    show=False, save=False, save_dir=None):
-    
-    return cluster_feats(
-                            X=X, gt_labels=gt_labels,
-                            num_runs=num_runs, best_model_metric=best_model_metric,
-                            make_silhoutte_plots=make_silhoutte_plots, embed_data_in_2d=embed_data_in_2d,
-                            show=show, save=save, save_dir=save_dir
-                        )
+eval_clustering = cluster_feats
     
 if __name__ == "__main__":
     ## For testing purposes
     
     rng = np.random.RandomState(0)
     n_samples=1000
```

### Comparing `clustutils4r-1.0.1/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-1.0.2/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

