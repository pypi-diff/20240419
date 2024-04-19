# Comparing `tmp/contrastive-ne-0.3.4.tar.gz` & `tmp/contrastive_ne-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contrastive-ne-0.3.4.tar", last modified: Wed Jan 10 16:34:31 2024, max compression
+gzip compressed data, was "contrastive_ne-0.3.5.tar", last modified: Fri Apr 19 13:16:02 2024, max compression
```

## Comparing `contrastive-ne-0.3.4.tar` & `contrastive_ne-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive-ne-0.3.4/LICENSE
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-01-10 16:02:34.000000 contrastive-ne-0.3.4/VERSION
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      842 2023-12-07 09:42:08.000000 contrastive-ne-0.3.4/pyproject.toml
--rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive-ne-0.3.4/readme.md
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/setup.cfg
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/src/
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/src/cne/
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive-ne-0.3.4/src/cne/__init__.py
--rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14269 2024-01-10 10:44:36.000000 contrastive-ne-0.3.4/src/cne/_cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6003 2023-11-09 16:15:45.000000 contrastive-ne-0.3.4/src/cne/callbacks.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29066 2024-01-10 15:38:01.000000 contrastive-ne-0.3.4/src/cne/cne.py
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive-ne-0.3.4/src/cne/old_loss_implementation.py
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/
--rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-01-10 16:34:31.000000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/PKG-INFO
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-01-10 16:34:31.000000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/SOURCES.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-01-10 16:34:31.000000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/dependency_links.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-01-10 16:34:31.000000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/requires.txt
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-01-10 16:34:31.000000 contrastive-ne-0.3.4/src/contrastive_ne.egg-info/top_level.txt
-drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-01-10 16:34:31.601000 contrastive-ne-0.3.4/tests/
--rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-01-10 16:14:33.000000 contrastive-ne-0.3.4/tests/test.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)     1228 2022-06-03 14:04:54.000000 contrastive_ne-0.3.5/LICENSE
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        6 2024-04-19 13:11:35.000000 contrastive_ne-0.3.5/VERSION
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      842 2023-12-07 09:42:08.000000 contrastive_ne-0.3.5/pyproject.toml
+-rwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)    12894 2024-01-10 09:58:06.000000 contrastive_ne-0.3.5/readme.md
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       38 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/setup.cfg
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/cne/
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)      112 2023-11-09 09:56:09.000000 contrastive_ne-0.3.5/src/cne/__init__.py
+-rwxr-xr-x   0 sdamrich  (1000) sdamrich  (1000)    14263 2024-02-28 14:17:24.000000 contrastive_ne-0.3.5/src/cne/_cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     6076 2024-04-10 08:53:32.000000 contrastive_ne-0.3.5/src/cne/callbacks.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)    29379 2024-04-19 13:03:09.000000 contrastive_ne-0.3.5/src/cne/cne.py
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)     8899 2023-02-08 10:47:49.000000 contrastive_ne-0.3.5/src/cne/old_loss_implementation.py
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/
+-rw-r--r--   0 sdamrich  (1000) sdamrich  (1000)    13540 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/PKG-INFO
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      370 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        1 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)       88 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/requires.txt
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)        4 2024-04-19 13:16:02.000000 contrastive_ne-0.3.5/src/contrastive_ne.egg-info/top_level.txt
+drwxrwxr-x   0 sdamrich  (1000) sdamrich  (1000)        0 2024-04-19 13:16:02.536645 contrastive_ne-0.3.5/tests/
+-rw-rw-r--   0 sdamrich  (1000) sdamrich  (1000)      654 2024-01-10 16:14:33.000000 contrastive_ne-0.3.5/tests/test.py
```

### Comparing `contrastive-ne-0.3.4/LICENSE` & `contrastive_ne-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `contrastive-ne-0.3.4/PKG-INFO` & `contrastive_ne-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.4
+Version: 0.3.5
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `contrastive-ne-0.3.4/pyproject.toml` & `contrastive_ne-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contrastive-ne-0.3.4/readme.md` & `contrastive_ne-0.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `contrastive-ne-0.3.4/src/cne/_cne.py` & `contrastive_ne-0.3.5/src/cne/_cne.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                     neighs_, _ = self.annoy.get_nns_by_item(i, self.k + 1, include_distances=True)
                     neighs = neighs_[1:]
                     adj[i, neighs] = 1
                     adj[neighs, i] = 1  # symmetrize on the fly
 
                 self.neighbor_mat = adj.tocsr()
             elif graph == "pykeops":
-                print("Computing approximate kNN graph with pykeops")
+                print("Computing exact kNN graph with pykeops")
                 from pykeops.torch import LazyTensor
                 import scipy.sparse
 
                 # set up pykeops LazyTensors
                 x_cuda = torch.tensor(X).to("cuda").contiguous()
                 x_i = LazyTensor(x_cuda[:, None])
                 x_j = LazyTensor(x_cuda[None])
```

### Comparing `contrastive-ne-0.3.4/src/cne/callbacks.py` & `contrastive_ne-0.3.5/src/cne/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         if n is not None:
             self.ds = torch.utils.data.TensorDataset(torch.arange(n))
             self.dl = torch.utils.data.DataLoader(self.ds,
                                                   batch_size=256,
                                                   shuffle=False)
 
-    def __call__(self, epoch, model, negative_samples, loss_mode, log_Z=None, noise_in_estimator=None):
+    def __call__(self, epoch, model, negative_samples, loss_mode, log_Z=None, neg_spec=None):
         # read out the embeddings from the model if anything shall be logged
         if isinstance(model, torch.nn.modules.sparse.Embedding):
             # non-parametric case, just get all embeddings from embedding layer
             embd = model.weight.detach().cpu().numpy()
         else:
             # parametric case, model is Embedding layer + FCNetwork
             # Just feed indices from self.dl
@@ -95,17 +95,19 @@
                                                   m=negative_samples,
                                                   Z=Z_prime,
                                                   a=1.0,
                                                   b=1.0,
                                                   noise_log_arg=True,
                                                   eps=1e-4))
             elif loss_mode == "neg":
-                # turn noise_in_estimator back into Z via
-                # Z * m * p_n = 1 <--> Z = 1 / (m * p_n)
-                Z = (negative_samples / len(embd)**2)**-1
+                # turn neg_spec back into Z via
+                # Z * m * p_n = neg_spec <--> Z = neg_spec / (m * p_n)
+                if neg_spec is None:
+                    neg_spec = 1.0
+                Z = neg_spec / (negative_samples / len(embd)**2)
                 self.losses.append(NCE_loss_keops(high_sim=self.graph,
                                                   embedding=embd,
                                                   m=negative_samples,
                                                   Z=Z,
                                                   a=1.0,
                                                   b=1.0,
                                                   noise_log_arg=True,
```

### Comparing `contrastive-ne-0.3.4/src/cne/cne.py` & `contrastive_ne-0.3.5/src/cne/cne.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         :param lr_min_factor: float Minimal value to which learning rate is annealed
         :param momentum: float Momentum of SGD
         :param temperature: float Temperature used in Cosine similarity
         :param noise_in_estimator: float Value used in negative sampling's fraction q / (q+ noise_in_estimator), redundant with Z_bar. Deprecated, use neg_spec instead.
         :param neg_spec: float Value used in negative sampling's fraction q / (q+ neg_spec). Controls the point on the negative sampling spectrum. Redundant with Z_bar, which has priority.
         :param ince_spec: float The repulsive term in the InfoNCE loss is multiplied by the inverse of ince_spec. Controls the InfoNCE spectrum. Redundant with s, which has priority.
         :param Z_bar: float Fixed normalization constant in negative sampling. Controls the negative sampling spectrum. Redundant with s, which has priority.
-        :param s: float Slider parameter for the spectrum of neighbor embeddings. If s=1, the embedding will be similar to a UMAP embedding. If s=0, the embedding will be similar to a t-SNE embedding. Logarithmic inter-/ extrapolation. Works for the loss modes "infonce", "infonce_alt" and "neg".
+        :param s: float Spectrum parameter for the spectrum of neighbor embeddings. If s=1, the embedding will be similar to a UMAP embedding (independent of the number of negative samples, unlike in the ICLR paper). If s=0, the embedding will be similar to a t-SNE embedding. Logarithmic inter-/ extrapolation. Works for the loss modes "infonce", "infonce_alt" and "neg".
         :param eps: float Iterpolates between UMAP's implicit similarity (eps = 0) and the Cauchy kernels (eps = 1.0)
         :param clamp_high: float Upper value at which arguments to logarithms are clamped. Default "auto" chooses values based on the metric. For metric="euclidean" it is 1.0, for metric="cosine" it is inf.
         :param clamp_low: float Lower value at which arguments to logarithms are clamped. Default "auto" chooses values based on the metric. For metric="euclidean" it is 1e-4, for metric="cosine" it is -inf.
         :param Z: float Initial value for the learned normalization parameter of NCE
         :param loss_mode: str Specifies which loss to use. Must be one of "umap", "neg", "nce", "infonce", "infonce_alt". "neg_sample" is deprecated and defaults to "neg"
         :param metric: str Specifies which metric to use for computing distances. Must be "cosine" or "euclidean".
         :param optimizer: str Specifies which optimizer to use. Must be "sgd" or "adam"
@@ -216,15 +216,17 @@
             early_exaggeration = False
         else:
             self.log_Z = None
 
         if self.loss_mode == "neg":
             n_specified_params = (noise_in_estimator is not None) + (Z_bar is not None) + (s is not None) + (neg_spec is not None)
             if n_specified_params == 0:
-                s = 1.0  # default for neg is umap
+                # This will produce UMAP like embds for 5 negative samples and shift along the spectrum as the number
+                # of negative samples changes, like in the ICLR paper.
+                neg_spec = 1.0
 
             if n_specified_params > 1:
                 print(
                     "Warning: More than one of 'noise_in_estimator', 'neg_spec', 'Z_bar' and "
                     "'s' were specified. 's' will supersede 'Z_bar', which supersedes 'neg_spec', which supersedes 'noise_in_estimator'."
                 )
 
@@ -284,15 +286,15 @@
 
         assert n is not None or X is not None, "Either n or X must be passed to process_spec_param"
         if self.loss_mode == "neg":
             # if not explicitly passed, use dataset length, only works if DataLoader is over data points, not over similar pairs
             n = len(X) if n is None else n
             if s is not None:
                 # overwrite self.Z_bar
-                Z_umap = n ** 2 / self.negative_samples
+                Z_umap = n ** 2 / 5  # UMAP uses 5 negative samples by default
                 Z_tsne = 100 * n
                 # s = 0 --> z_tsne, s = 1 --> z_umap; using logs for numerical stability
                 Z_bar = Z_tsne * np.exp(s * (np.log(Z_umap) - np.log(Z_tsne)))
 
             if Z_bar is not None:
                 # assume uniform noise distribution over n**2 many edges
                 neg_spec = self.negative_samples * Z_bar / n ** 2
@@ -386,14 +388,15 @@
         ):
             self.callback(
                 -1,
                 self.model,
                 self.negative_samples,
                 self.loss_mode,
                 self.log_Z,
+                self.neg_spec
             )
 
         batch_losses = []
 
         # logging memory usage
         mem_dict = {
             "active_bytes.all.peak": [],
@@ -459,15 +462,15 @@
             if (
                 self.save_freq is not None
                 and self.save_freq > 0
                 and epoch % self.save_freq == 0
                 and callable(self.callback)
             ):
                 self.callback(
-                    epoch, self.model, self.negative_samples, self.loss_mode, self.log_Z
+                    epoch, self.model, self.negative_samples, self.loss_mode, self.log_Z, self.neg_spec
                 )
             # print epoch progress
             if self.print_freq_epoch is not None and epoch % self.print_freq_epoch == 0:
                 print(f"Finished epoch {epoch}/{self.n_epochs}, loss {sum(bl)/ len(bl):.3f}", file=sys.stderr)
 
         self.losses = batch_losses
         self.mem_dict = mem_dict
```

### Comparing `contrastive-ne-0.3.4/src/cne/old_loss_implementation.py` & `contrastive_ne-0.3.5/src/cne/old_loss_implementation.py`

 * *Files identical despite different names*

### Comparing `contrastive-ne-0.3.4/src/contrastive_ne.egg-info/PKG-INFO` & `contrastive_ne-0.3.5/src/contrastive_ne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contrastive-ne
-Version: 0.3.4
+Version: 0.3.5
 Summary: Contrastive Neighbor Embeddings
 Author-email: Sebastian Damrich <sebastian.damrich@uni-tuebingen.de>, Niklas Böhm <jan-niklas.boehm@uni-tuebingen.de>
 License: MIT
 Project-URL: homepage, https://github.com/berenslab/contrastive-ne
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `contrastive-ne-0.3.4/tests/test.py` & `contrastive_ne-0.3.5/tests/test.py`

 * *Files identical despite different names*

