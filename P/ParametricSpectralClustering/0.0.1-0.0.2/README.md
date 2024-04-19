# Comparing `tmp/ParametricSpectralClustering-0.0.1.tar.gz` & `tmp/ParametricSpectralClustering-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ParametricSpectralClustering-0.0.1.tar", last modified: Tue Mar 26 10:05:23 2024, max compression
+gzip compressed data, was "dist/ParametricSpectralClustering-0.0.2.tar", last modified: Fri Apr 19 11:26:39 2024, max compression
```

## Comparing `ParametricSpectralClustering-0.0.1.tar` & `ParametricSpectralClustering-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,38 @@
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.024268 ParametricSpectralClustering-0.0.1/
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.016661 ParametricSpectralClustering-0.0.1/Experiments/
--rw-r--r--   0 ivychang   (501) staff       (20)    16372 2024-01-24 14:41:46.000000 ParametricSpectralClustering-0.0.1/Experiments/psc_tmp.py
--rw-r--r--   0 ivychang   (501) staff       (20)     6536 2024-02-08 08:15:30.000000 ParametricSpectralClustering-0.0.1/Experiments/test1.py
--rw-r--r--   0 ivychang   (501) staff       (20)      208 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.1/Experiments/tmp.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.013633 ParametricSpectralClustering-0.0.1/JSS_Experiments/
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.016921 ParametricSpectralClustering-0.0.1/JSS_Experiments/Firewall_table3/
--rw-r--r--   0 ivychang   (501) staff       (20)    14281 2024-02-04 08:47:37.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Firewall_table3/fixed_n_wo_sampling_ratio.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.017213 ParametricSpectralClustering-0.0.1/JSS_Experiments/Firewall_table4/
--rw-r--r--   0 ivychang   (501) staff       (20)     7428 2024-02-04 08:09:40.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Firewall_table4/fixed_n_with_sampling_ratio.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.017471 ParametricSpectralClustering-0.0.1/JSS_Experiments/NIDS_table7/
--rw-r--r--   0 ivychang   (501) staff       (20)     7486 2024-02-24 13:19:35.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/NIDS_table7/main.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.019307 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/
--rw-r--r--   0 ivychang   (501) staff       (20)     9549 2024-02-27 16:37:41.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/Figure_1.py
--rw-r--r--   0 ivychang   (501) staff       (20)     2792 2024-02-24 15:54:33.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/compare.py
--rw-r--r--   0 ivychang   (501) staff       (20)      111 2024-03-12 10:11:45.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/compare_txt.py
--rw-r--r--   0 ivychang   (501) staff       (20)    10431 2024-03-12 10:09:02.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/figure1.py
--rw-r--r--   0 ivychang   (501) staff       (20)     6588 2024-02-08 08:49:22.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/figure2.py
--rw-r--r--   0 ivychang   (501) staff       (20)    16846 2024-02-27 16:52:34.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/psc.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.019698 ParametricSpectralClustering-0.0.1/JSS_Experiments/table_5/
--rw-r--r--   0 ivychang   (501) staff       (20)     6210 2024-02-04 07:36:05.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/table_5/firewall_n_eq_m.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.019966 ParametricSpectralClustering-0.0.1/JSS_Experiments/table_6/
--rw-r--r--   0 ivychang   (501) staff       (20)     9400 2024-02-04 08:34:21.000000 ParametricSpectralClustering-0.0.1/JSS_Experiments/table_6/main.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1066 2023-08-21 09:34:30.000000 ParametricSpectralClustering-0.0.1/LICENSE.txt
--rw-r--r--   0 ivychang   (501) staff       (20)       44 2023-08-21 09:45:35.000000 ParametricSpectralClustering-0.0.1/MANIFEST.in
--rw-r--r--   0 ivychang   (501) staff       (20)     3474 2024-03-26 10:05:23.024080 ParametricSpectralClustering-0.0.1/PKG-INFO
--rw-r--r--   0 ivychang   (501) staff       (20)    18780 2023-08-28 08:07:46.000000 ParametricSpectralClustering-0.0.1/PSC_lib.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.020647 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering/
--rw-r--r--   0 ivychang   (501) staff       (20)       47 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering/__init__.py
--rw-r--r--   0 ivychang   (501) staff       (20)    15151 2024-03-26 10:00:23.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering/psc.py
--rw-r--r--   0 ivychang   (501) staff       (20)    16472 2024-01-24 14:41:16.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering/psc_tmp.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.022145 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/
--rw-r--r--   0 ivychang   (501) staff       (20)     3474 2024-03-26 10:05:22.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/PKG-INFO
--rw-r--r--   0 ivychang   (501) staff       (20)     1256 2024-03-26 10:05:22.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/SOURCES.txt
--rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-03-26 10:05:22.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/dependency_links.txt
--rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-01-30 05:57:05.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/not-zip-safe
--rw-r--r--   0 ivychang   (501) staff       (20)       38 2024-03-26 10:05:22.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/requires.txt
--rw-r--r--   0 ivychang   (501) staff       (20)       29 2024-03-26 10:05:22.000000 ParametricSpectralClustering-0.0.1/ParametricSpectralClustering.egg-info/top_level.txt
--rw-r--r--   0 ivychang   (501) staff       (20)     2639 2024-03-26 10:01:16.000000 ParametricSpectralClustering-0.0.1/README.md
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.022642 ParametricSpectralClustering-0.0.1/bin/
--rw-r--r--   0 ivychang   (501) staff       (20)     2566 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.1/bin/clustering.py
--rw-r--r--   0 ivychang   (501) staff       (20)     3276 2024-02-11 14:01:58.000000 ParametricSpectralClustering-0.0.1/bin/run.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1641 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.1/bin/train_psc.py
--rw-r--r--   0 ivychang   (501) staff       (20)      872 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.1/fix_seed_psc.py
--rw-r--r--   0 ivychang   (501) staff       (20)       38 2024-03-26 10:05:23.024325 ParametricSpectralClustering-0.0.1/setup.cfg
--rw-r--r--   0 ivychang   (501) staff       (20)     1259 2024-03-26 10:05:05.000000 ParametricSpectralClustering-0.0.1/setup.py
--rw-r--r--   0 ivychang   (501) staff       (20)      760 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.1/test.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-03-26 10:05:23.023711 ParametricSpectralClustering-0.0.1/tests/
--rw-r--r--   0 ivychang   (501) staff       (20)        0 2023-08-22 05:19:40.000000 ParametricSpectralClustering-0.0.1/tests/__init__.py
--rw-r--r--   0 ivychang   (501) staff       (20)      948 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.1/tests/test_Accuracy.py
--rw-r--r--   0 ivychang   (501) staff       (20)      716 2024-01-07 05:49:34.000000 ParametricSpectralClustering-0.0.1/tests/test_Four_layer_FNN.py
--rw-r--r--   0 ivychang   (501) staff       (20)     2864 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.1/tests/test_PSC.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1435 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.1/tests/test_error_handling.py
--rw-r--r--   0 ivychang   (501) staff       (20)      539 2023-09-03 07:44:54.000000 ParametricSpectralClustering-0.0.1/unittest_example.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.451058 ParametricSpectralClustering-0.0.2/
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446065 ParametricSpectralClustering-0.0.2/JSS_Experiments/
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446372 ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/
+-rw-r--r--   0 ivychang   (501) staff       (20)    14281 2024-04-03 04:53:46.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/main.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446716 ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/
+-rw-r--r--   0 ivychang   (501) staff       (20)     7449 2024-04-03 04:53:22.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/main.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.447334 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/
+-rw-r--r--   0 ivychang   (501) staff       (20)    10399 2024-04-19 11:08:05.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure1.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     6588 2024-02-08 08:49:22.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure2.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     2000 2024-04-19 11:23:25.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/run.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.447584 ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/
+-rw-r--r--   0 ivychang   (501) staff       (20)     9400 2024-04-03 04:54:58.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/main.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1066 2023-08-21 09:34:30.000000 ParametricSpectralClustering-0.0.2/LICENSE.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)       44 2023-08-21 09:45:35.000000 ParametricSpectralClustering-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivychang   (501) staff       (20)     4376 2024-04-19 11:26:39.450887 ParametricSpectralClustering-0.0.2/PKG-INFO
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.448151 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/
+-rw-r--r--   0 ivychang   (501) staff       (20)       47 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/__init__.py
+-rw-r--r--   0 ivychang   (501) staff       (20)    15151 2024-03-26 10:00:23.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/psc.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.449102 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/
+-rw-r--r--   0 ivychang   (501) staff       (20)     4376 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/PKG-INFO
+-rw-r--r--   0 ivychang   (501) staff       (20)      813 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/SOURCES.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/dependency_links.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-01-30 05:57:05.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/not-zip-safe
+-rw-r--r--   0 ivychang   (501) staff       (20)      113 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/requires.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)       29 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/top_level.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)     3591 2024-04-19 11:14:38.000000 ParametricSpectralClustering-0.0.2/README.md
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.449492 ParametricSpectralClustering-0.0.2/bin/
+-rw-r--r--   0 ivychang   (501) staff       (20)     2566 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/bin/clustering.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     3276 2024-02-11 14:01:58.000000 ParametricSpectralClustering-0.0.2/bin/run.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1641 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/bin/train_psc.py
+-rw-r--r--   0 ivychang   (501) staff       (20)       38 2024-04-19 11:26:39.451114 ParametricSpectralClustering-0.0.2/setup.cfg
+-rw-r--r--   0 ivychang   (501) staff       (20)     1348 2024-04-19 11:25:51.000000 ParametricSpectralClustering-0.0.2/setup.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.450489 ParametricSpectralClustering-0.0.2/tests/
+-rw-r--r--   0 ivychang   (501) staff       (20)        0 2023-08-22 05:19:40.000000 ParametricSpectralClustering-0.0.2/tests/__init__.py
+-rw-r--r--   0 ivychang   (501) staff       (20)      948 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_Accuracy.py
+-rw-r--r--   0 ivychang   (501) staff       (20)      716 2024-01-07 05:49:34.000000 ParametricSpectralClustering-0.0.2/tests/test_Four_layer_FNN.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     2864 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_PSC.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1435 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_error_handling.py
```

### Comparing `ParametricSpectralClustering-0.0.1/Experiments/psc_tmp.py` & `ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/psc.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,84 +184,87 @@
             The adjusted rand index.
         ami : float
             The adjusted mutual information.
         """
         clusterAcc = self.cluster_acc()
         ari = self.ARI()
         ami = self.AMI()
-
-        print(f"Clustering Accuracy: {clusterAcc}")
-        print(f"Adjusted rand index: {ari}")
-        print(f"Adjusted mutual information: {ami}")
         return clusterAcc, ari, ami
 
 
 class PSC:
     """Parametric Spectral Clustering.
 
     Parameters
     ----------
     n_neighbor : int, default=8
         Number of neighbors to use when constructing the adjacency matrix using k-nearest neighbors.
-    sigma : float, default=1
-        The sigma value for the Gaussian kernel.
-    k : int, default=10
+    n_clusters : int, default=10
         Number of clusters.
     model : torch.nn.Module
         The model used to learn the embedding.
     criterion : torch.nn.modules.loss, default=nn.MSELoss()
         The loss function used to train the model.
     epochs : int, default=50
         Number of epochs to train the model.
-    clustering_method : sklearn.cluster, default=None
-        The clustering method used to cluster the embedding.
-    spliting_rate : float, default=0.3
+    sampling_ratio : float, default=0.3
         The spliting rate of the testing data.
     batch_size_data : int, default=50
         The batch size of the training data.
     batch_size_dataloader : int, default=20
         The batch size of the dataloader.
+    clustering_method : sklearn.cluster, default=None
+        The clustering method used to cluster the embedding.
+    n_components : int, default=0
+        The number of embedding dimensions.
+    random_state : int, default=None
+        The random state.
 
     Attributes
     ----------
     n_neighbor : int
         Number of neighbors to use when constructing the adjacency matrix using k-nearest neighbors.
     n_clusters : int
         Number of clusters.
     model : torch.nn.Module
         The model used to learn the embedding.
     criterion : torch.nn.modules.loss
         The loss function used to train the model.
-    sampling_rat : float
+    sampling_ratio : float
         The spliting rate of the testing data.
     optimizer : torch.optim
         The optimizer used to train the model.
-    epochs : int
-        Number of epochs to train the model.
     clustering : str
         The clustering method used to cluster the embedding.
+    n_components : int
+        The number of embedding dimensions.
+    random_state : int
+        The random state.
+    epochs : int
+        Number of epochs to train the model.
     model_fitted : bool
         Whether the model has been fitted.
-    dataloader : torch.utils.data.DataLoader
-        The dataloader used to train the model.
     batch_size_data : int
         The batch size of the training data.
     batch_size_dataloader : int
         The batch size of the dataloader.
+    dataloader : torch.utils.data.DataLoader
+        The dataloader used to train the model.
+
 
     Examples
     --------
     >>> from ParametricSpectralClustering import PSC, Four_layer_FNN
     >>> from sklearn.datasets import load_digits
     >>> from sklearn.cluster import KMeans
     >>> digits = load_digits()
     >>> X = digits.data/16
     >>> cluster_method = KMeans(n_clusters=10, init="k-means++", n_init=1, max_iter=100, algorithm='elkan')
     >>> model = Four_layer_FNN(64, 128, 256, 64, 10)
-    >>> psc = PSC(model=model, clustering_method=cluster_method, n_neighbor=10, sampling_rat=0, batch_size_data=1797)
+    >>> psc = PSC(model=model, clustering_method=cluster_method, n_neighbor=10, sampling_ratio=0, batch_size_data=1797)
     >>> psc.fit(X)
     >>> psc.save_model("model")
     >>> cluster_idx = psc.predict(X)
 
     >>> from ParametricSpectralClustering import PSC, Four_layer_FNN
     >>> from sklearn.datasets import load_digits
     >>> from sklearn.cluster import KMeans
@@ -291,35 +294,36 @@
         self.n_neighbor = n_neighbor
         self.n_clusters = n_clusters
         self.model = model
         self.criterion = criterion
         self.sampling_ratio = sampling_ratio
         self.optimizer = torch.optim.Adam(model.parameters(), lr=0.001)
 
+        if random_state is None:
+            self.random_state = random.randint(1, 100)
+        else:
+            self.random_state = random_state
+
         if clustering_method is None:
-            self.clustering_method = KMeans(
+            self.clustering = KMeans(
                 n_clusters=self.n_clusters,
                 init="k-means++",
                 n_init=1,
                 max_iter=100,
                 algorithm="elkan",
+                random_state=self.random_state,
             )
         else:
-            self.clustering_method = clustering_method
+            self.clustering = clustering_method
 
         if n_components == 0:
-            self.n_components = self.clustering_method.n_clusters
+            self.n_components = self.n_clusters
         else:
             self.n_components = n_components
 
-        if random_state is None:
-            self.random_state = random.randint(1, 100)
-        else:
-            self.random_state = random_state
-
         self.epochs = epochs
         self.model_fitted = False
 
         self.batch_size_data = batch_size_data
         self.batch_size_dataloader = batch_size_dataloader
 
     def __loss_calculation(self):
@@ -341,22 +345,23 @@
             X, n_neighbors=self.n_neighbor, include_self=False
         )
         affinity_matrix_ = 0.5 * (connectivity + connectivity.T)
         embedding = spectral_embedding(
             affinity_matrix_,
             n_components=self.n_components,
             eigen_solver="arpack",
-            random_state=1,  # do we have to set random_state?
+            random_state=1,
             eigen_tol="auto",
             drop_first=False,
         )
         u = torch.from_numpy(embedding).type(torch.FloatTensor)
         dataset = torch.utils.data.TensorDataset(x, u)
+        # not sure whether shuffle = True will affect the result
         dataloader = torch.utils.data.DataLoader(
-            dataset, batch_size=self.batch_size_dataloader, shuffle=True
+            dataset, batch_size=self.batch_size_dataloader, shuffle=False
         )
         self.dataloader = dataloader
         total_loss = 0
         for _ in range(self.epochs):
             loss = self.__loss_calculation()
             total_loss += loss
         return total_loss / self.epochs
@@ -364,33 +369,32 @@
     def __check_file_exist(self, file_name) -> bool:
         for entry in os.listdir("./"):
             if entry == file_name:
                 return True
         return False
 
     def __check_clustering_method(self) -> None:
-        if self.clustering_method is None:
+        if self.clustering is None:
             raise ValueError("No clustering method assigned.")
 
     def __check_model(self) -> None:
         if self.model is None:
             raise ValueError("No model assigned.")
 
-    def training_psc_model(self, X):
-        """Train the model and return the embedding.
+    def fit(self, X):
+        """Train a model to convert input features into spectral embeddings.
 
         Parameters
         ----------
         X : array-like of shape
             Training data.
 
         Returns
         -------
-        U : array-like of shape
-            The embedding of the training data.
+        No return value
         """
 
         self.__check_clustering_method()
         self.__check_model()
 
         x = torch.from_numpy(X).type(torch.FloatTensor)
 
@@ -403,83 +407,53 @@
             X_train, x_train = X, x
 
         else:
             X_train, _, x_train, _ = train_test_split(
                 X,
                 x,
                 test_size=self.sampling_ratio,
-                random_state=random.randint(1, 100),
+                random_state=self.random_state,
             )
 
         batch_size = self.batch_size_data
         total_loss = 0
         i = 1
         # Train the model in mini-batches
         for start_idx in range(0, len(X_train), batch_size):
             end_idx = start_idx + batch_size
             X_batch = X_train[start_idx:end_idx]
             x_batch = x_train[start_idx:end_idx]
             loss = self.__train_model(X_batch, x_batch)
             total_loss += loss
             if i % 20 == 0:
-                print(f"Loss in {i-20} to {i}: {total_loss/20}")
                 total_loss = 0
             i += 1
 
-        emb = self.model(x).detach().numpy()
-
-        return emb
-
-    def fit(self, X):
-        """Fit the model according to the given training data.
-
-        Parameters
-        ----------
-        X : array-like of shape (n_samples, n_features)
-            Training data.
-
-        Returns
-        -------
-        self : object
-            Returns the instance itself.
-        """
-        emb = self.training_psc_model(X)
-
-        if hasattr(self.clustering_method, "fit") is False:
-            raise AttributeError(
-                f"'{type(self.clustering_method)}' object has no attribute 'fit'"
-            )
-
-        self.clustering_method.fit(emb)
-
-        return self
-
     def fit_predict(self, X):
-        """Fit the model according to the given training data and predict the closest cluster each sample in X belongs to.
+        """Fit the model and predict the closest cluster each sample in X belongs to.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             Training data.
 
         Returns
         -------
         cluster_index : array-like of shape (n_samples,)
             Index of the cluster each sample belongs to.
         """
-        emb = self.training_psc_model(X)
+        self.fit(X)
 
-        if hasattr(self.clustering_method, "fit_predict") is False:
+        if hasattr(self.clustering, "fit_predict") is False:
             raise AttributeError(
-                f"'{type(self.clustering_method)}' object has no attribute 'fit_predict'"
+                f"'{type(self.clustering)}' object has no attribute 'fit_predict'"
             )
 
-        return self.clustering_method.fit_predict(emb)
+        return self.predict(X)
 
-    # predict the closest cluster
     def predict(self, X):
         """Predict the closest cluster each sample in X belongs to.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             New data.
@@ -487,45 +461,33 @@
         Returns
         -------
         cluster_index : array-like of shape (n_samples,)
             Index of the cluster each sample belongs to.
         """
 
         x = torch.from_numpy(X).type(torch.FloatTensor)
+
+        # turn input data points into low-dim embedding
         emb = self.model(x).detach().numpy()
-        if hasattr(self.clustering_method, "predict") is False:
+
+        if hasattr(self.clustering, "fit_predict") is False:
             raise AttributeError(
-                f"'{type(self.clustering_method)}' object has no attribute 'predict'"
+                f"'{type(self.clustering)}' object has no attribute 'predict'"
             )
 
-        if self.model_fitted is False:
-            return self.clustering_method.fit_predict(emb)
-
-        return self.clustering_method.predict(emb)
-
-    def set_model(self, self_defined_model) -> None:
-        """Set the model to a self-defined model.
-
-        Parameters
-        ----------
-        self_defined_model : torch.nn.Module
-            The self-defined model.
-        """
-
-        self.model = self_defined_model
+        return self.clustering.fit_predict(emb)
 
     def save_model(self, path: str) -> None:
         """Save the model to a file.
 
         Parameters
         ----------
         path : str
             The path of the file.
         """
-        torch.save(self.model.state_dict(), path)
 
         with open(path, "wb") as f:
             pickle.dump(self.model, f)
 
     def load_model(self, path: str) -> None:
         """Load the model from a file.
```

### Comparing `ParametricSpectralClustering-0.0.1/Experiments/test1.py` & `ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure2.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         x = self.relu(x)
         x = self.fc5(x)
         x = self.output_layer(x)
         return x
 
 
 n_samples = 10000
-seed = 30
+seed = 72
 noisy_circles = datasets.make_circles(
     n_samples=n_samples, factor=0.5, noise=0.05, random_state=seed
 )
 noisy_moons = datasets.make_moons(n_samples=n_samples, noise=0.05, random_state=seed)
 blobs = datasets.make_blobs(n_samples=n_samples, random_state=seed)
 rng = np.random.RandomState(seed)
 no_structure = rng.rand(n_samples, 2), None
@@ -223,12 +223,16 @@
         colors = np.append(colors, ["#000000"])
         plt.scatter(X[:, 0], X[:, 1], s=10, color=colors[y_pred])
 
         plt.xlim(-2.5, 2.5)
         plt.ylim(-2.5, 2.5)
         plt.xticks(())
         plt.yticks(())
+
         plot_num += 1
 
 
-plt.savefig("Experiments/figure2_KMedian.pdf", format="pdf")
+plt.savefig(
+    "JSS_Experiments/Synthesis_dataset/Figure2_custom_clustering_KMedian.pdf",
+    format="pdf",
+)
 plt.show()
```

### Comparing `ParametricSpectralClustering-0.0.1/JSS_Experiments/Firewall_table3/fixed_n_wo_sampling_ratio.py` & `ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 df = pd.read_csv("JSS_Experiments/datasets/firewall.csv")
 action = {"allow": 1, "deny": 2, "drop": 3, "reset-both": 4}
 df["Action"] = df["Action"].map(action)
 y_tmp = df["Action"].values
 x_tmp = df.drop(["Action"], axis=1).values
 
 
-f = open("JSS_Experiments/Firewall_table3/log.txt", "a+")
+f = open("JSS_Experiments/Firewall_table4/log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
 
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
     y = y_tmp
@@ -73,15 +73,15 @@
 psc_acc_1_60000 = []
 psc_acc_15001_60000 = []
 psc_time_1_15000 = []
 psc_time_1_30000 = []
 psc_time_1_45000 = []
 psc_time_1_60000 = []
 
-result = pd.read_csv("JSS_Experiments/Firewall_table3/result.csv")
+result = pd.read_csv("JSS_Experiments/Firewall_table4/result.csv")
 
 for _ in range(10):
     if "sc" in methods:
         spectral_clustering = SpectralClustering(
             n_clusters=4,
             eigen_solver="arpack",
             affinity="nearest_neighbors",
@@ -427,8 +427,8 @@
     )
     result.at[4, "Accuracy.3"] = (
         str(psc_acc_1_60000_mean) + "±" + str(psc_acc_1_60000_std)
     )
 
 
 f.close()
-result.to_csv("JSS_Experiments/Firewall_table3/result.csv", index=False)
+result.to_csv("JSS_Experiments/Firewall_table4/result.csv", index=False)
```

### Comparing `ParametricSpectralClustering-0.0.1/JSS_Experiments/NIDS_table7/main.py` & `ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from ParametricSpectralClustering import PSC, Accuracy
 import time
 import datetime
 import argparse
 import warnings
 import numpy as np
 
-# python NIDS/exp.py --methods kmeans --size -1 --rate 0.9
-
 warnings.filterwarnings("ignore")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-datasize", "--size", type=int, help="data size used for training")
 parser.add_argument("-methods", "--methods", nargs="+", help="which method to test")
 parser.add_argument("-sampling_ratio", "--ratio", type=float, help="sampling ratio")
 args = parser.parse_args()
@@ -65,15 +63,15 @@
 }
 df["Attack"] = df["Attack"].map(Class)
 print(df.drop(["Attack", "IPV4_SRC_ADDR", "IPV4_DST_ADDR", "Dataset"], axis=1).info())
 
 y_tmp = df["Attack"].values
 x_tmp = df.drop(["Attack", "IPV4_SRC_ADDR", "IPV4_DST_ADDR", "Dataset"], axis=1).values
 
-f = open("JSS_Experiments/NIDS_table7/log.txt", "a+")
+f = open("JSS_Experiments/NIDS_table5/log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
     y = y_tmp
 else:
@@ -86,15 +84,15 @@
 methods = args.methods
 
 total_acc = []
 total_time = []
 total_ari = []
 total_ami = []
 
-result = pd.read_csv("JSS_Experiments/NIDS_table7/result.csv", index_col=0)
+result = pd.read_csv("JSS_Experiments/NIDS_table5/result.csv", index_col=0)
 
 for i in range(10):
     # --------Spectral Clustering--------
     if "sc" in methods:
         spectral_clustering = SpectralClustering(
             n_clusters=10,
             eigen_solver="arpack",
@@ -162,15 +160,15 @@
         # measure time spent
         start_time = round(time.time() * 1000)
         psc.fit(x)
         psc_index = psc.predict(x)
         end_time = round(time.time() * 1000)
 
         # save model
-        psc.save_model("NIDS/psc_model" + str(i + 1) + ".pkl")
+        psc.save_model("JSS_Experiments/NIDS_table5/psc_model" + str(i + 1) + ".pkl")
 
         # calculate acc, ari, ami
         acc = Accuracy(y_true=y, y_pred=psc_index)
         psc_accRate, psc_ari, psc_ami = acc.acc_report()
         total_acc.append(psc_accRate)
         total_ari.append(psc_ari)
         total_ami.append(psc_ami)
@@ -217,8 +215,8 @@
 if "sc" in methods:
     result.at[str(args), "SC"] = str(time_mean) + "±" + str(time_std)
     result.at[str(args), "SC.1"] = str(acc_mean) + "±" + str(acc_std)
     result.at[str(args), "SC.2"] = str(ari_mean) + "±" + str(ari_std)
     result.at[str(args), "SC.3"] = str(ami_mean) + "±" + str(ami_std)
 
 f.close()
-df.to_csv("JSS_Experiments/NIDS_table7/result.csv")
+df.to_csv("JSS_Experiments/NIDS_table5/result.csv")
```

### Comparing `ParametricSpectralClustering-0.0.1/JSS_Experiments/Synthesis_dataset/Figure_1.py` & `ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,340 +1,365 @@
-import time
-import warnings
-import torch
-import numpy as np
-import matplotlib.pyplot as plt
-import torch.nn as nn
-import random
-import argparse
-from sklearn import cluster, datasets, mixture
-from sklearn.neighbors import kneighbors_graph
-from sklearn.preprocessing import StandardScaler
-from itertools import cycle, islice
-
-# from ParametricSpectralClustering.psc import PSC
-from psc import PSC
-
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "-dataset",
-    "--dataset",
-    type=str,
-    help="the dataset used in this single experiment",
-)
-args = parser.parse_args()
-
-r = 72
-rng = np.random.RandomState(r)
-torch.manual_seed(0)
-random.seed(int(r))
-np.random.seed(0)
-
-# ============
-# Generate datasets. We choose the size big enough to see the scalability
-# of the algorithms, but not too big to avoid too long running times
-# ============
-n_samples = 10000
-noisy_circles = datasets.make_circles(
-    n_samples=n_samples, factor=0.5, noise=0.05, random_state=rng
-)
-x, y = noisy_circles
-noisy_moons = datasets.make_moons(n_samples=n_samples, noise=0.05, random_state=rng)
-blobs = datasets.make_blobs(n_samples=n_samples, random_state=8)
-no_structure = np.random.rand(n_samples, 2), None
-
-# Anisotropicly distributed data
-random_state = 170
-X, y = datasets.make_blobs(n_samples=n_samples, random_state=random_state)
-transformation = [[0.6, -0.6], [-0.4, 0.8]]
-X_aniso = np.dot(X, transformation)
-aniso = (X_aniso, y)
-
-# blobs with varied variances
-varied = datasets.make_blobs(
-    n_samples=n_samples, cluster_std=[1.0, 2.5, 0.5], random_state=random_state
-)
-
-# ============
-# Set up cluster parameters
-# ============
-plt.figure(figsize=(7.5, 3))
-plt.subplots_adjust(
-    left=0.02, right=0.98, bottom=0.001, top=0.96, wspace=0.05, hspace=0.01
-)
-
-plot_num = 1
-
-default_base = {
-    "quantile": 0.3,
-    "eps": 0.3,
-    "damping": 0.9,
-    "preference": -200,
-    "n_neighbors": 10,
-    "n_clusters": 3,
-    "min_samples": 20,
-    "xi": 0.05,
-    "min_cluster_size": 0.1,
-}
-
-datasets = [
-    (
-        "noisy_circles",
-        noisy_circles,
-        {
-            "damping": 0.77,
-            "preference": -240,
-            "quantile": 0.2,
-            "n_clusters": 2,
-            "min_samples": 20,
-            "xi": 0.25,
-        },
-    ),
-    (
-        "noisy_moons",
-        noisy_moons,
-        {"damping": 0.75, "preference": -220, "n_clusters": 2},
-    ),
-    (
-        "varied",
-        varied,
-        {
-            "eps": 0.18,
-            "n_neighbors": 2,
-            "min_samples": 5,
-            "xi": 0.035,
-            "min_cluster_size": 0.2,
-        },
-    ),
-    (
-        "aniso",
-        aniso,
-        {
-            "eps": 0.15,
-            "n_neighbors": 2,
-            "min_samples": 20,
-            "xi": 0.1,
-            "min_cluster_size": 0.2,
-        },
-    ),
-    ("blobs", blobs, {}),
-    ("no_structure", no_structure, {}),
-]
-
-if args.dataset == "noisy_circles":
-    datasets = [datasets[0]]
-    fig_num = 1
-elif args.dataset == "noisy_moons":
-    datasets = [datasets[1]]
-    fig_num = 2
-elif args.dataset == "varied":
-    datasets = [datasets[2]]
-    fig_num = 3
-elif args.dataset == "aniso":
-    datasets = [datasets[3]]
-    fig_num = 4
-elif args.dataset == "blobs":
-    datasets = [datasets[4]]
-    fig_num = 5
-elif args.dataset == "no_structure":
-    datasets = [datasets[5]]
-    fig_num = 6
-
-
-# for noisy_circles, noisy_moons, blobs, no_structure
-class Net1(nn.Module):
-    def __init__(self, out_put):
-        super(Net1, self).__init__()
-        # Define the layers
-        self.fc1 = nn.Linear(2, 32)
-        self.fc2 = nn.Linear(32, 64)
-        self.fc3 = nn.Linear(64, 128)
-        self.fc4 = nn.Linear(128, 64)
-        self.fc5 = nn.Linear(64, 32)
-        self.output_layer = nn.Linear(32, out_put)
-
-        self.relu = nn.ReLU()
-
-    def forward(self, x):
-        x = self.fc1(x)
-        x = self.fc2(x)
-        x = self.relu(x)
-        x = self.fc3(x)
-        x = self.fc4(x)
-        x = self.relu(x)
-        x = self.fc5(x)
-        x = self.output_layer(x)
-        return x
-
-
-# for varied
-class Net2(nn.Module):
-    def __init__(self, out_put):
-        super(Net2, self).__init__()
-        # Define the layers
-        self.fc1 = nn.Linear(2, 16)
-        self.fc2 = nn.Linear(16, 32)
-        self.fc3 = nn.Linear(32, 16)
-        self.fc4 = nn.Linear(16, 8)
-        self.output_layer = nn.Linear(8, out_put)
-        self.relu = nn.ReLU()
-
-    def forward(self, x):
-        x = self.fc1(x)
-        x = self.fc2(x)
-        x = self.fc3(x)
-        x = self.fc4(x)
-        x = self.output_layer(x)
-        return x
-
-
-# for aniso
-class Net3(nn.Module):
-    def __init__(self, out_put):
-        super(Net3, self).__init__()
-        # Define the layers
-        self.fc1 = nn.Linear(2, 32)
-        self.fc2 = nn.Linear(32, 64)
-        self.fc3 = nn.Linear(64, 32)
-        self.fc4 = nn.Linear(32, 16)
-        self.output_layer = nn.Linear(16, out_put)
-        self.relu = nn.ReLU()
-
-    def forward(self, x):
-        x = self.fc1(x)
-        x = self.fc2(x)
-        x = self.fc3(x)
-        x = self.fc4(x)
-        x = self.output_layer(x)
-        return x
-
-
-for i_dataset, (name, dataset, algo_params) in enumerate(datasets):
-    # update parameters with dataset-specific values
-    params = default_base.copy()
-    params.update(algo_params)
-
-    X, y = dataset
-
-    # normalize dataset for easier parameter selection
-    X = StandardScaler().fit_transform(X)
-
-    # estimate bandwidth for mean shift
-    bandwidth = cluster.estimate_bandwidth(X, quantile=params["quantile"])
-
-    # connectivity matrix for structured Ward
-    connectivity = kneighbors_graph(
-        X, n_neighbors=params["n_neighbors"], include_self=False
-    )
-    # make connectivity symmetric
-    connectivity = 0.5 * (connectivity + connectivity.T)
-
-    # ============
-    # Create cluster objects
-    # ============
-    KMeans = cluster.KMeans(
-        n_clusters=params["n_clusters"],
-        init="random",
-        n_init="auto",
-        algorithm="elkan",
-        random_state=rng,
-    )
-    spectral = cluster.SpectralClustering(
-        n_clusters=params["n_clusters"],
-        eigen_solver="arpack",
-        affinity="nearest_neighbors",
-        random_state=rng,
-    )
-    torch.manual_seed(0)
-    model_1 = Net1(params["n_clusters"])
-    torch.manual_seed(0)
-    model_2 = Net2(params["n_clusters"])
-    torch.manual_seed(0)
-    model_3 = Net3(params["n_clusters"])
-    kmeans_psc = cluster.KMeans(
-        n_clusters=params["n_clusters"], random_state=rng, n_init=10, verbose=False
-    )
-
-    l = ["noisy_circles", "noisy_moons", "blobs", "no_structure"]
-    if name in l:
-        model = model_1
-    elif name == "varied":
-        model = model_2
-    elif name == "aniso":
-        model = model_3
-
-    psc = PSC(
-        model=model,
-        clustering_method=kmeans_psc,
-        sampling_ratio=0,
-        n_components=params["n_clusters"],
-        n_neighbor=params["n_neighbors"],
-        batch_size_data=10000,
-        random_state=rng,
-    )
-
-    clustering_algorithms = (
-        ("KMeans", KMeans),
-        ("SpectralClustering", spectral),
-        ("PSC", psc),
-    )
-
-    for algo_name, algorithm in clustering_algorithms:
-        t0 = time.time()
-
-        # catch warnings related to kneighbors_graph
-        with warnings.catch_warnings():
-            warnings.filterwarnings(
-                "ignore",
-                message="the number of connected components of the "
-                + "connectivity matrix is [0-9]{1,2}"
-                + " > 1. Completing it to avoid stopping the tree early.",
-                category=UserWarning,
-            )
-            warnings.filterwarnings(
-                "ignore",
-                message="Graph is not fully connected, spectral embedding"
-                + " may not work as expected.",
-                category=UserWarning,
-            )
-            algorithm.fit(X)
-
-        t1 = time.time()
-        if hasattr(algorithm, "labels_"):
-            y_pred = algorithm.labels_.astype(np.int32)
-        else:
-            y_pred = algorithm.predict(X)
-
-        plt.subplot(len(datasets), len(clustering_algorithms), plot_num)
-        if i_dataset == 0:
-            plt.title(algo_name, size=10)
-
-        colors = np.array(
-            list(
-                islice(
-                    cycle(
-                        [
-                            "#377eb8",
-                            "#ff7f00",
-                            "#4daf4a",
-                            "#f781bf",
-                            "#a65628",
-                            "#984ea3",
-                            "#999999",
-                            "#e41a1c",
-                            "#dede00",
-                        ]
-                    ),
-                    int(max(y_pred) + 1),
-                )
-            )
-        )
-        colors = np.append(colors, ["#000000"])
-        plt.scatter(X[:, 0], X[:, 1], s=10, color=colors[y_pred])
-
-        plt.xlim(-2.5, 2.5)
-        plt.ylim(-2.5, 2.5)
-        plt.xticks(())
-        plt.yticks(())
-        plot_num += 1
-# fig_name = "C:\\git\\PSC_library\\JSS_Experiments\\Synthesis_dataset\\Figure1--" + str(fig_num) + ".pdf"
-# plt.savefig(fig_name, format="pdf", bbox_inches="tight", dpi=50)
+import time
+import warnings
+import torch
+import numpy as np
+import matplotlib.pyplot as plt
+import torch.nn as nn
+import random
+import argparse
+from sklearn import cluster, datasets, mixture
+from sklearn.neighbors import kneighbors_graph
+from sklearn.preprocessing import StandardScaler
+from itertools import cycle, islice
+
+from ParametricSpectralClustering.psc import PSC
+
+parser = argparse.ArgumentParser()
+parser.add_argument(
+    "-dataset",
+    "--dataset",
+    type=str,
+    help="the dataset used in this single experiment",
+)
+args = parser.parse_args()
+
+r = 72
+rng = np.random.RandomState(r)
+torch.manual_seed(0)
+random.seed(int(r))
+np.random.seed(0)
+
+# ============
+# Generate datasets. We choose the size big enough to see the scalability
+# of the algorithms, but not too big to avoid too long running times
+# ============
+n_samples = 10000
+noisy_circles = datasets.make_circles(
+    n_samples=n_samples, factor=0.5, noise=0.05, random_state=rng
+)
+x, y = noisy_circles
+noisy_moons = datasets.make_moons(n_samples=n_samples, noise=0.05, random_state=rng)
+blobs = datasets.make_blobs(n_samples=n_samples, random_state=8)
+no_structure = np.random.rand(n_samples, 2), None
+
+# Anisotropicly distributed data
+random_state = 170
+X, y = datasets.make_blobs(n_samples=n_samples, random_state=random_state)
+transformation = [[0.6, -0.6], [-0.4, 0.8]]
+X_aniso = np.dot(X, transformation)
+aniso = (X_aniso, y)
+
+# blobs with varied variances
+varied = datasets.make_blobs(
+    n_samples=n_samples, cluster_std=[1.0, 2.5, 0.5], random_state=random_state
+)
+
+# ============
+# Set up cluster parameters
+# ============
+plt.figure(figsize=(7.5, 3))
+plt.subplots_adjust(
+    left=0.02, right=0.98, bottom=0.001, top=0.96, wspace=0.05, hspace=0.01
+)
+
+plot_num = 1
+
+default_base = {
+    "quantile": 0.3,
+    "eps": 0.3,
+    "damping": 0.9,
+    "preference": -200,
+    "n_neighbors": 10,
+    "n_clusters": 3,
+    "min_samples": 20,
+    "xi": 0.05,
+    "min_cluster_size": 0.1,
+}
+
+datasets = [
+    (
+        "noisy_circles",
+        noisy_circles,
+        {
+            "damping": 0.77,
+            "preference": -240,
+            "quantile": 0.2,
+            "n_clusters": 2,
+            "min_samples": 20,
+            "xi": 0.25,
+        },
+    ),
+    (
+        "noisy_moons",
+        noisy_moons,
+        {"damping": 0.75, "preference": -220, "n_clusters": 2},
+    ),
+    (
+        "varied",
+        varied,
+        {
+            "eps": 0.18,
+            "n_neighbors": 2,
+            "min_samples": 5,
+            "xi": 0.035,
+            "min_cluster_size": 0.2,
+        },
+    ),
+    (
+        "aniso",
+        aniso,
+        {
+            "eps": 0.15,
+            "n_neighbors": 2,
+            "min_samples": 20,
+            "xi": 0.1,
+            "min_cluster_size": 0.2,
+        },
+    ),
+    ("blobs", blobs, {}),
+    ("no_structure", no_structure, {}),
+]
+
+if args.dataset == "noisy_circles":
+    datasets = [datasets[0]]
+    fig_num = 1
+elif args.dataset == "noisy_moons":
+    datasets = [datasets[1]]
+    fig_num = 2
+elif args.dataset == "varied":
+    datasets = [datasets[2]]
+    fig_num = 3
+elif args.dataset == "aniso":
+    datasets = [datasets[3]]
+    fig_num = 4
+elif args.dataset == "blobs":
+    datasets = [datasets[4]]
+    fig_num = 5
+elif args.dataset == "no_structure":
+    datasets = [datasets[5]]
+    fig_num = 6
+
+
+# for noisy_circles, noisy_moons, blobs, no_structure
+class Net1(nn.Module):
+    def __init__(self, out_put):
+        super(Net1, self).__init__()
+        # Define the layers
+        self.fc1 = nn.Linear(2, 32)
+        self.fc2 = nn.Linear(32, 64)
+        self.fc3 = nn.Linear(64, 128)
+        self.fc4 = nn.Linear(128, 64)
+        self.fc5 = nn.Linear(64, 32)
+        self.output_layer = nn.Linear(32, out_put)
+
+        self.relu = nn.ReLU()
+
+    def forward(self, x):
+        x = self.fc1(x)
+        x = self.fc2(x)
+        x = self.relu(x)
+        x = self.fc3(x)
+        x = self.fc4(x)
+        x = self.relu(x)
+        x = self.fc5(x)
+        x = self.output_layer(x)
+        return x
+
+
+# for varied
+class Net2(nn.Module):
+    def __init__(self, out_put):
+        super(Net2, self).__init__()
+        # Define the layers
+        self.fc1 = nn.Linear(2, 16)
+        self.fc2 = nn.Linear(16, 32)
+        self.fc3 = nn.Linear(32, 16)
+        self.fc4 = nn.Linear(16, 8)
+        self.output_layer = nn.Linear(8, out_put)
+        self.relu = nn.ReLU()
+
+    def forward(self, x):
+        x = self.fc1(x)
+        x = self.fc2(x)
+        x = self.fc3(x)
+        x = self.fc4(x)
+        x = self.output_layer(x)
+        return x
+
+
+# for aniso
+class Net3(nn.Module):
+    def __init__(self, out_put):
+        super(Net3, self).__init__()
+        # Define the layers
+        self.fc1 = nn.Linear(2, 32)
+        self.fc2 = nn.Linear(32, 64)
+        self.fc3 = nn.Linear(64, 32)
+        self.fc4 = nn.Linear(32, 16)
+        self.output_layer = nn.Linear(16, out_put)
+        self.relu = nn.ReLU()
+
+    def forward(self, x):
+        x = self.fc1(x)
+        x = self.fc2(x)
+        x = self.fc3(x)
+        x = self.fc4(x)
+        x = self.output_layer(x)
+        return x
+
+
+for i_dataset, (name, dataset, algo_params) in enumerate(datasets):
+    # update parameters with dataset-specific values
+    # print(name)
+    params = default_base.copy()
+    params.update(algo_params)
+
+    X, y = dataset
+
+    # normalize dataset for easier parameter selection
+    X = StandardScaler().fit_transform(X)
+
+    # estimate bandwidth for mean shift
+    bandwidth = cluster.estimate_bandwidth(X, quantile=params["quantile"])
+
+    # connectivity matrix for structured Ward
+    connectivity = kneighbors_graph(
+        X, n_neighbors=params["n_neighbors"], include_self=False
+    )
+    # make connectivity symmetric
+    connectivity = 0.5 * (connectivity + connectivity.T)
+
+    # ============
+    # Create cluster objects
+    # ============
+    KMeans = cluster.KMeans(
+        n_clusters=params["n_clusters"],
+        init="random",
+        n_init="auto",
+        algorithm="elkan",
+        random_state=rng,
+    )
+    spectral = cluster.SpectralClustering(
+        n_clusters=params["n_clusters"],
+        eigen_solver="arpack",
+        affinity="nearest_neighbors",
+        random_state=rng,
+    )
+    torch.manual_seed(0)
+    model_1 = Net1(params["n_clusters"])
+    torch.manual_seed(0)
+    model_2 = Net2(params["n_clusters"])
+    torch.manual_seed(0)
+    model_3 = Net3(params["n_clusters"])
+    kmeans_psc = cluster.KMeans(
+        n_clusters=params["n_clusters"], random_state=rng, n_init=10, verbose=False
+    )
+
+    l = ["noisy_circles", "noisy_moons", "blobs", "no_structure"]
+    if name in l:
+        model = model_1
+        # print("1")
+    elif name == "varied":
+        model = model_2
+        # print("2")
+    elif name == "aniso":
+        model = model_3
+        # print("3")
+
+    # for name, param in model.named_parameters():
+    #     print(f"Parameter name: {name}, Shape: {param.shape}")
+    #     print(f"Parameter values:\n{param.data}\n")
+
+    psc = PSC(
+        model=model,
+        clustering_method=kmeans_psc,
+        sampling_ratio=0,
+        n_components=params["n_clusters"],
+        n_neighbor=params["n_neighbors"],
+        batch_size_data=10000,
+        random_state=rng,
+    )
+
+    clustering_algorithms = (
+        # ("KMeans", KMeans),
+        # ("SpectralClustering", spectral),
+        ("PSC", psc),
+    )
+
+    for algo_name, algorithm in clustering_algorithms:
+        t0 = time.time()
+
+        # catch warnings related to kneighbors_graph
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                message="the number of connected components of the "
+                + "connectivity matrix is [0-9]{1,2}"
+                + " > 1. Completing it to avoid stopping the tree early.",
+                category=UserWarning,
+            )
+            warnings.filterwarnings(
+                "ignore",
+                message="Graph is not fully connected, spectral embedding"
+                + " may not work as expected.",
+                category=UserWarning,
+            )
+            algorithm.fit(X)
+            # if algo_name == "PSC":
+            #     for name, param in algorithm.model.named_parameters():
+            #         print(f"Parameter name: {name}, Shape: {param.shape}")
+            #         print(f"Parameter values:\n{param.data}\n")
+
+        t1 = time.time()
+        if hasattr(algorithm, "labels_"):
+            y_pred = algorithm.labels_.astype(np.int32)
+        else:
+            y_pred = algorithm.predict(X)
+
+        if args.dataset == "noisy_circles":
+            np.savetxt("y_pred_noisy_circles.txt", y_pred, fmt="%d", delimiter=",")
+        elif args.dataset == "noisy_moons":
+            np.savetxt("y_pred_noisy_moons.txt", y_pred, fmt="%d", delimiter=",")
+        elif args.dataset == "varied":
+            np.savetxt("y_pred_varied2.txt", y_pred, fmt="%d", delimiter=",")
+        elif args.dataset == "aniso":
+            np.savetxt("y_pred_aniso.txt", y_pred, fmt="%d", delimiter=",")
+        elif args.dataset == "blobs":
+            np.savetxt("y_pred_blobs.txt", y_pred, fmt="%d", delimiter=",")
+        elif args.dataset == "no_structure":
+            np.savetxt("y_pred_no_structure.txt", y_pred, fmt="%d", delimiter=",")
+
+        plt.subplot(len(datasets), len(clustering_algorithms), plot_num)
+        if i_dataset == 0:
+            plt.title(algo_name, size=10)
+
+        colors = np.array(
+            list(
+                islice(
+                    cycle(
+                        [
+                            "#377eb8",
+                            "#ff7f00",
+                            "#4daf4a",
+                            "#f781bf",
+                            "#a65628",
+                            "#984ea3",
+                            "#999999",
+                            "#e41a1c",
+                            "#dede00",
+                        ]
+                    ),
+                    int(max(y_pred) + 1),
+                )
+            )
+        )
+        colors = np.append(colors, ["#000000"])
+        plt.scatter(X[:, 0], X[:, 1], s=10, color=colors[y_pred])
+
+        plt.xlim(-2.5, 2.5)
+        plt.ylim(-2.5, 2.5)
+        plt.xticks(())
+        plt.yticks(())
+        plot_num += 1
+fig_name = "JSS_Experiments/Synthesis_dataset/Figure1-" + str(fig_num) + ".pdf"
+plt.savefig(fig_name, format="pdf", bbox_inches="tight")
+# f.close()
```

### Comparing `ParametricSpectralClustering-0.0.1/JSS_Experiments/table_5/firewall_n_eq_m.py` & `ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 import time
 import datetime
 import argparse
 import warnings
 import sklearn
 from sklearn.cluster import SpectralClustering, KMeans
 from ParametricSpectralClustering import PSC, Accuracy
+from scipy.io import arff
 
 warnings.filterwarnings("ignore")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-datasize", "--size", type=int, help="data size used for training")
 parser.add_argument(
     "-methods",
     "--methods",
     nargs="+",
     help="select clustering method (psc, sc, kmeans)",
 )
+parser.add_argument(
+    "-dataset",
+    "--dataset",
+    type=str,
+    help="choose Letter dataset or Pendigits dataset in this experiment",
+)
+
 args = parser.parse_args()
 
 
 class Net(nn.Module):
     def __init__(self) -> None:
         super(Net, self).__init__()
 
@@ -33,23 +41,66 @@
             nn.Linear(32, 4),
         )
 
     def forward(self, x):
         return self.model(x)
 
 
-df = pd.read_csv("JSS_Experiments/datasets/firewall.csv")
-action = {"allow": 1, "deny": 2, "drop": 3, "reset-both": 4}
-df["Action"] = df["Action"].map(action)
-y_tmp = df["Action"].values
-x_tmp = df.drop(["Action"], axis=1).values
+dataset = args.dataset
+
+if "Pendigits" in dataset:
+    pendigits = pd.read_csv("JSS_Experiments/datasets/Pendigits.csv")
+    y_tmp = pendigits["class"].values
+    x_tmp = pendigits.drop(columns=["id", "class"]).values
+
+elif "Letter" in dataset:
+    letter_arff = arff.loadarff("JSS_Experiments/datasets/dataset_6_letter.arff")
+    letter = pd.DataFrame(letter_arff[0])
+    letter["class"] = letter["class"].astype(str)
+
+    Class = {
+        "A": 1,
+        "B": 2,
+        "C": 3,
+        "D": 4,
+        "E": 5,
+        "F": 6,
+        "G": 7,
+        "H": 8,
+        "I": 9,
+        "J": 10,
+        "K": 11,
+        "L": 12,
+        "M": 13,
+        "N": 14,
+        "O": 15,
+        "P": 16,
+        "Q": 17,
+        "R": 18,
+        "S": 19,
+        "T": 20,
+        "U": 21,
+        "V": 22,
+        "W": 23,
+        "X": 24,
+        "Y": 25,
+        "Z": 26,
+    }
+
+    letter["class"] = letter["class"].map(Class)
+    y_tmp = letter["class"].values
+    x_data_tmp = letter.drop(["class"], axis=1).values
+
+    scaler = sklearn.preprocessing.StandardScaler().fit(x_data_tmp)
+    x_tmp = scaler.transform(x_data_tmp)
 
-f = open("JSS_Experiments/table5/log.txt", "a+")
+f = open("JSS_Experiments/table_3/log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
+f.write("dataset: " + str(args.dataset) + "\n")
 
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
     y = y_tmp
 
 else:
@@ -57,23 +108,27 @@
     x_data = x_tmp[: args.size]
     y = y_tmp[: args.size]
 
 scaler = sklearn.preprocessing.StandardScaler().fit(x_data)
 x = scaler.transform(x_data)
 methods = args.methods
 
+kmeans_total_acc = []
+kmeans_total_ari = []
+kmeans_total_ami = []
+
 sc_total_acc = []
 sc_total_ari = []
 sc_total_ami = []
 
 psc_total_acc = []
 psc_total_ari = []
 psc_total_ami = []
 
-result = pd.read_csv("JSS_Experiments/table_5/result.csv", index_col=0)
+result = pd.read_csv("JSS_Experiments/table_3/result.csv", index_col=[0, 1])
 
 for _ in range(10):
     if "sc" in methods:
         spectral_clustering = SpectralClustering(
             n_clusters=4,
             eigen_solver="arpack",
             affinity="nearest_neighbors",
@@ -91,22 +146,20 @@
 
         # write result into ratio_log.txt
         f.write("---SpectralClustering---\n")
         f.write("acc rate: " + str(sc_accRate) + "\n")
         f.write("ari: " + str(sc_ari) + "\n")
         f.write("ami: " + str(sc_ami) + "\n")
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
-
         sc_total_acc.append(sc_accRate)
-        sc_total_ari.append(sc_ari)
         sc_total_ami.append(sc_ami)
+        sc_total_ari.append(sc_ari)
 
     if "psc" in methods:
         kmeans = KMeans(n_clusters=4, init="random", n_init="auto", algorithm="elkan")
-
         psc = PSC(
             model=Net(),
             clustering_method=kmeans,
             sampling_ratio=0,
             n_components=4,
             n_neighbor=4,
             batch_size_data=args.size,
@@ -114,72 +167,113 @@
 
         # measure total time spent
         start_time = round(time.time() * 1000)
         psc.fit(x)
         psc_index = psc.predict(x)
         end_time = round(time.time() * 1000)
 
-        # calculate acc, ari, ami
+        # calculate acc[1:m]
         acc = Accuracy(y_true=y, y_pred=psc_index)
         psc_accRate, psc_ari, psc_ami = acc.acc_report()
-
-        # write result into log.txt
         f.write("----------PSC-----------\n")
         f.write("acc rate: " + str(psc_accRate) + "\n")
         f.write("ari: " + str(psc_ari) + "\n")
         f.write("ami: " + str(psc_ami) + "\n")
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
 
         psc_total_acc.append(psc_accRate)
         psc_total_ari.append(psc_ari)
         psc_total_ami.append(psc_ami)
 
+    if "kmeans" in methods:
+        kmeans = KMeans(n_clusters=4, init="random", n_init="auto", algorithm="elkan")
+
+        start_time = round(time.time() * 1000)
+        kmeans_index = kmeans.fit_predict(x)
+        end_time = round(time.time() * 1000)
+
+        acc = Accuracy(y_true=y, y_pred=kmeans_index)
+        kmeans_accRate, kmeans_ari, kmeans_ami = acc.acc_report()
+
+        f.write("----------KMeans-----------\n")
+        f.write("acc rate: " + str(kmeans_accRate) + "\n")
+        f.write("ari: " + str(kmeans_ari) + "\n")
+        f.write("ami: " + str(kmeans_ami) + "\n")
+        f.write("time spent: " + str(end_time - start_time) + "\n\n")
+
+        kmeans_total_acc.append(kmeans_accRate)
+        kmeans_total_ari.append(kmeans_ari)
+        kmeans_total_ami.append(kmeans_ami)
 
-# calculate mean±std
 if "sc" in methods:
     ari_mean, ari_std = np.mean(sc_total_ari), np.std(sc_total_ari)
     ami_mean, ami_std = np.mean(sc_total_ami), np.std(sc_total_ami)
     acc_mean, acc_std = np.mean(sc_total_acc), np.std(sc_total_acc)
     # write result into log.txt
     f.write("==============report==============\n")
     f.write("|data size: " + str(args.size) + "|\n")
-    f.write("|method: " + str(args.methods) + "|\n")
+    f.write("|method: Spectral Clustering|\n")
     f.write("|acc: " + str(acc_mean) + "±" + str(acc_std) + "|\n")
     f.write("|ari: " + str(ari_mean) + "±" + str(ari_std) + "|\n")
     f.write("|ami: " + str(ami_mean) + "±" + str(ami_std) + "|\n")
     f.write("=====================================\n\n")
     # print result
     print("=========report=========")
     print("acc:", acc_mean, "±", acc_std)
     print("ari:", ari_mean, "±", ari_std)
     print("ami:", ami_mean, "±", ami_std)
     print("===========================\n\n\n")
     # write result into result.csv
-    result.at[str(args), "SC"] = str(acc_mean) + "±" + str(acc_std)
-    result.at[str(args), "SC.1"] = str(ari_mean) + "±" + str(ari_std)
-    result.at[str(args), "SC.2"] = str(ami_mean) + "±" + str(ami_std)
+    result.at[("SC", "ClusterAcc"), args.dataset] = str(acc_mean) + "±" + str(acc_std)
+    result.at[("SC", "ARI"), args.dataset] = str(ari_mean) + "±" + str(ari_std)
+    result.at[("SC", "AMI"), args.dataset] = str(ami_mean) + "±" + str(ami_std)
 
 if "psc" in methods:
     ari_mean, ari_std = np.mean(psc_total_ari), np.std(psc_total_ari)
     ami_mean, ami_std = np.mean(psc_total_ami), np.std(psc_total_ami)
     acc_mean, acc_std = np.mean(psc_total_acc), np.std(psc_total_acc)
-    # write result inot log.txt
+    # write result into log.txt
+    f.write("==============report==============\n")
+    f.write("|data size: " + str(args.size) + "|\n")
+    f.write("|method: PSC|\n")
+    f.write("|acc: " + str(acc_mean) + "±" + str(acc_std) + "|\n")
+    f.write("|ari: " + str(ari_mean) + "±" + str(ari_std) + "|\n")
+    f.write("|ami: " + str(ami_mean) + "±" + str(ami_std) + "|\n")
+    f.write("=====================================\n\n")
+    # print result
+    print("=========report=========")
+    print("acc:", acc_mean, "±", acc_std)
+    print("ari:", ari_mean, "±", ari_std)
+    print("ami:", ami_mean, "±", ami_std)
+    print("===========================\n\n\n")
+    # write result into result.csv
+    result.at[("PSC", "ClusterAcc"), args.dataset] = str(acc_mean) + "±" + str(acc_std)
+    result.at[("PSC", "ARI"), args.dataset] = str(ari_mean) + "±" + str(ari_std)
+    result.at[("PSC", "AMI"), args.dataset] = str(ami_mean) + "±" + str(ami_std)
+
+if "kmeans" in methods:
+    ari_mean, ari_std = np.mean(kmeans_total_ari), np.std(kmeans_total_ari)
+    ami_mean, ami_std = np.mean(kmeans_total_ami), np.std(kmeans_total_ami)
+    acc_mean, acc_std = np.mean(kmeans_total_acc), np.std(kmeans_total_acc)
+    # write result into log.txt
     f.write("==============report==============\n")
     f.write("|data size: " + str(args.size) + "|\n")
-    f.write("|method: " + str(args.methods) + "|\n")
+    f.write("|method: KMeans|\n")
     f.write("|acc: " + str(acc_mean) + "±" + str(acc_std) + "|\n")
     f.write("|ari: " + str(ari_mean) + "±" + str(ari_std) + "|\n")
     f.write("|ami: " + str(ami_mean) + "±" + str(ami_std) + "|\n")
     f.write("=====================================\n\n")
     # print result
     print("=========report=========")
     print("acc:", acc_mean, "±", acc_std)
     print("ari:", ari_mean, "±", ari_std)
     print("ami:", ami_mean, "±", ami_std)
     print("===========================\n\n\n")
     # write result into result.csv
-    result.at[str(args), "PSC"] = str(acc_mean) + "±" + str(acc_std)
-    result.at[str(args), "PSC.1"] = str(ari_mean) + "±" + str(ari_std)
-    result.at[str(args), "PSC.2"] = str(ami_mean) + "±" + str(ami_std)
+    result.at[("KMeans", "ClusterAcc"), args.dataset] = (
+        str(acc_mean) + "±" + str(acc_std)
+    )
+    result.at[("KMeans", "ARI"), args.dataset] = str(ari_mean) + "±" + str(ari_std)
+    result.at[("KMeans", "AMI"), args.dataset] = str(ami_mean) + "±" + str(ami_std)
 
 f.close()
-result.to_csv("JSS_Experiments/table_5/result.csv")
+result.to_csv("JSS_Experiments/table_3/result.csv")
```

### Comparing `ParametricSpectralClustering-0.0.1/LICENSE.txt` & `ParametricSpectralClustering-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/PKG-INFO` & `ParametricSpectralClustering-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,48 @@
-Metadata-Version: 2.1
-Name: ParametricSpectralClustering
-Version: 0.0.1
-Summary: A library for users to use parametric spectral clustering
-Home-page: 
-Author: Ivy Chang, Hsin Ju Tai
-Author-email: ivy900403@gmail.com, luludai020127@gmail.com
-License: MIT
-Keywords: Spectral Clustering,Incremental Clustering,Online Clustering,Non-linear clustering
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <!-- Parametric Spectral Clustering -->
+
 # Parametric Spectral Clustering
 
 This repository provides a PyTorch implementation of the **Parametric Spectral Clustering** (PSC) algorithm, which offers a favorable alternative to the traditional spectral clustering algorithm. PSC addresses issues related to computational efficiency, memory usage, and the absence of online learning capabilities. It serves as a versatile framework suitable for applying spectral clustering to large datasets.
 
 <!-- PREREQUISITES -->
+
 # Installation
+
 ## Dependencies
+
 Parametric Spectral Clustering requires:
 
-* Python (>= 3.8)
-* NumPy (>= 1.24.3)
-* SciPy (>= 1.10.3)
-* PyTorch (>= 1.12.1)
-* scikit-learn (>= 1.3.2)
-* Pandas (>= 2.0.3)
+-   Python (>= 3.8)
+-   NumPy (>= 1.26.4)
+-   SciPy (>= 1.13.0)
+-   PyTorch (>= 2.2.2)
+-   scikit-learn (>= 1.4.2)
+-   Pandas (>= 2.2.2)
 
 ---
 
 <!-- INSTALLATION -->
+
 ## User installation
 
 Use setup.py:
+
 ```sh
 python setup.py install
 ```
 
 Use pip:
+
 ```sh
-pip install -i [url] ParametricSpectralClustering==0.0.14
+pip install ParametricSpectralClustering
 ```
 
 <!-- SAMPLE USAGE -->
+
 ## Sample Usage
 
 Using UCI ML hand-written digits datasets as an example.
 
 ```sh
 >>> from ParametricSpectralClustering import PSC, Four_layer_FNN
 >>> from sklearn.datasets import load_digits
@@ -64,48 +54,68 @@
 >>> psc = PSC(model=model, clustering_method=cluster_method, n_neighbor=10, sampling_ratio=0, batch_size_data=1797)
 >>> psc.fit(X)
 >>> psc.save_model("model")
 >>> cluster_idx = psc.predict(X)
 ```
 
 <!-- COMMEND LINE TOOL -->
+
 ## Command line tool
+
 After installation, you may run the following scripts directly.
 
 ```sh
-python bin\run.py [data] [rate] [n_cluster] [model_path] [cluster_result_format]
+python bin/run.py [data] [rate] [n_cluster] [model_path] [cluster_result_format]
 ```
 
-The ``[data]`` can accept .txt, .csv, and .npy format of data.
+The `[data]` can accept .txt, .csv, and .npy format of data.
+
+The `[rate]` should be in float, between 0.0 and 1.0. It represent the proportion of the input data reserved for training the mapping function from the original feature space to the spectral embedding.
+
+The `[n_cluster]` is the number of clusters the user intends to partition. This number needs to be lower than the total data points available within the dataset.
+
+The `[model_path]` is the path to save the trained model.
+
+The `[cluster_result_format]` can be either .txt or .csv. It represent the format of the cluster result.
 
-The ``[rate]`` should be in float, between 0.0 and 1.0. It represent the proportion of the input data reserved for training the mapping function from the original feature space to the spectral embedding.
+<!-- EXPERIMENT-->
 
-The ``[n_cluster]`` is the number of clusters the user intends to partition. This number needs to be lower than the total data points available within the dataset.
+# Experiment
 
-The ``[model_path]`` is the path to save the trained model.
+The 'JSS_Experiments' directory contains the code for the experiments detailed in the paper "PSC: a Python Package for Parametric Spectral Clustering." This includes scripts for experiments on the Firewall, NIDS, and Synthesis datasets.
 
-The ``[cluster_result_format]`` can be either .txt or .csv. It represent the format of the cluster result.
+Prior to executing these scripts, ensure that the necessary datasets have been downloaded and placed in the appropriate location. The datasets can be obtained from the following sources:
+
+-   NIDS Dataset: https://www.kaggle.com/datasets/aryashah2k/nfuqnidsv2-network-intrusion-detection-dataset
+
+Please place the downloaded datasets in the ‘JSS_Experiments/datasets’ directory. Ensure the datasets are correctly located before running the scripts.
+
+```sh
+cd JSS_Experiments
+bash run.sh
+```
+
+<!-- Test -->
+
+# Test
+
+To run the test, use the following command:
+
+```sh
+pytest tests
+```
 
 <!-- LICENSE -->
-## License
+
+# License
 
 Distributed under the MIT License. See `LICENSE.txt` for more information.
 
 <!-- CONTACT -->
-## Contact
-|Author|Ivy Chang|Hsin Ju Tai|
-|---|---|---|
-|E-mail|ivy900403@gmail.com|hsinjutai@gmail.com|
-
-Project Link: [TBA](https://github.com/your_username/repo_name)
-
 
-Change Log
-==========
+# Contact
 
-0.0.10 (2023/08/21)
--------------------
-- First release
+| Author | Ivy Chang           | Hsin Ju Tai         |
+| ------ | ------------------- | ------------------- |
+| E-mail | ivy900403@gmail.com | hsinjutai@gmail.com |
 
-0.0.13 (2023/08/21)
--------------------
-- Fix pickle
+Project Link: [Parametric Spectral Clsutering](https://github.com/IvyChang04/PSC_library)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ParametricSpectralClustering-0.0.1/bin/clustering.py` & `ParametricSpectralClustering-0.0.2/bin/clustering.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/bin/run.py` & `ParametricSpectralClustering-0.0.2/bin/run.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/bin/train_psc.py` & `ParametricSpectralClustering-0.0.2/bin/train_psc.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/setup.py` & `ParametricSpectralClustering-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,21 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: OS Independent",
 ]
 
 requirements = [
-    "torch",
-    "numpy",
-    "scikit-learn",
-    "scipy",
-    "pandas",
+    "scipy>=1.13.0",
+    "torch>=2.2.2",
+    "torchaudio>=2.2.2",
+    "torchvision>=0.17.2",
+    "scikit-learn>=1.4.2",
+    "pandas>=2.2.2",
+    "numpy==1.26.4",
 ]
 
 scripts = [
     "bin/clustering.py",
     "bin/train_psc.py",
     "bin/run.py",
 ]
@@ -27,15 +29,15 @@
     "Incremental Clustering",
     "Online Clustering",
     "Non-linear clustering",
 ]
 
 setup(
     name="ParametricSpectralClustering",
-    version="0.0.1",
+    version="0.0.2",
     description="A library for users to use parametric spectral clustering",
     long_description=open("README.md").read() + "\n\n" + open("CHANGELOG.txt").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests*"]),
     classifiers=classifiers,
     keywords=keywords,
     url="",
```

### Comparing `ParametricSpectralClustering-0.0.1/tests/test_Accuracy.py` & `ParametricSpectralClustering-0.0.2/tests/test_Accuracy.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/tests/test_Four_layer_FNN.py` & `ParametricSpectralClustering-0.0.2/tests/test_Four_layer_FNN.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/tests/test_PSC.py` & `ParametricSpectralClustering-0.0.2/tests/test_PSC.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.1/tests/test_error_handling.py` & `ParametricSpectralClustering-0.0.2/tests/test_error_handling.py`

 * *Files identical despite different names*

