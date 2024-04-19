# Comparing `tmp/flowMC-0.3.1.tar.gz` & `tmp/flowmc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.3.1.tar", last modified: Thu Apr 11 20:08:33 2024, max compression
+gzip compressed data, was "flowmc-0.3.2.tar", last modified: Fri Apr 19 21:33:15 2024, max compression
```

## Comparing `flowMC-0.3.1.tar` & `flowmc-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-11 20:08:29.000000 flowMC-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-11 20:08:33.527804 flowMC-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-11 20:08:29.000000 flowMC-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 20:08:29.000000 flowMC-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 20:08:33.527804 flowMC-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/rqSpline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/HMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/MALA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/flowHMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/global_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/importance_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/EvolutionaryOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-19 21:33:11.000000 flowmc-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 21:33:15.737426 flowmc-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-19 21:33:11.000000 flowmc-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-19 21:33:11.000000 flowmc-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 21:33:15.737426 flowmc-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.729426 flowmc-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/nfmodel/rqSpline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.733426 flowmc-0.3.2/src/flowMC/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/proposal/flowHMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/global_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/importance_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/strategy/optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-19 21:33:11.000000 flowmc-0.3.2/src/flowMC/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:33:15.737426 flowmc-0.3.2/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 21:33:15.000000 flowmc-0.3.2/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowMC-0.3.1/LICENSE` & `flowmc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/PKG-INFO` & `flowmc-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.1
+Version: 0.3.2
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.1 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.2 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowMC-0.3.1/README.md` & `flowmc-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/setup.cfg` & `flowmc-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flowMC
-version = 0.3.1
+version = 0.3.2
 author = Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/flowMC
 description = Normalizing flow exhanced sampler in jax
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
```

### Comparing `flowMC-0.3.1/src/flowMC/Sampler.py` & `flowmc-0.3.2/src/flowMC/Sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         self.likelihood_vec = self.local_sampler.logpdf_vmap
 
         self.optim = optax.chain(
             optax.clip(1.0), optax.adam(self.learning_rate, self.momentum)
         )
         self.optim_state = self.optim.init(eqx.filter(self.nf_model, eqx.is_array))
 
-        self.strategies = [
+        default_strategies = [
             GlobalTuning(
                 n_dim=self.n_dim,
                 n_chains=self.n_chains,
                 n_local_steps=self.n_local_steps,
                 n_global_steps=self.n_global_steps,
                 n_loop=self.n_loop_training,
                 output_thinning=self.output_thinning,
@@ -157,15 +157,23 @@
                 verbose=self.verbose,
             ),
         ]
 
         if kwargs.get("strategies") is not None:
             kwargs_strategies = kwargs.get("strategies")
             assert isinstance(kwargs_strategies, list)
-            self.strategies = kwargs_strategies
+            self.strategies = []
+            for strategy in kwargs_strategies:
+                if isinstance(strategy, str):
+                    if strategy.lower() == "default":
+                        self.strategies += default_strategies
+                else:
+                    self.strategies.append(strategy)
+        else:
+            self.strategies = default_strategies 
 
         self.summary = {}
 
     def sample(self, initial_position: Float[Array, "n_chains n_dim"], data: dict):
         """
         Sample from the posterior using the local sampler.
```

### Comparing `flowMC-0.3.1/src/flowMC/nfmodel/base.py` & `flowmc-0.3.2/src/flowMC/nfmodel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         loss_values = jnp.zeros(num_epochs)
         if verbose:
             pbar = trange(num_epochs, desc="Training NF", miniters=int(num_epochs / 10))
         else:
             pbar = range(num_epochs)
 
         best_model = model = self
+        best_state = state
         best_loss = 1e9
         for epoch in pbar:
             # Use a separate PRNG key to permute image data during shuffling
             rng, input_rng = jax.random.split(rng)
             # Run an optimization step over a training batch
             value, model, state = model.train_epoch(
                 input_rng, optim, state, data, batch_size
```

### Comparing `flowMC-0.3.1/src/flowMC/nfmodel/common.py` & `flowmc-0.3.2/src/flowMC/nfmodel/common.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/nfmodel/realNVP.py` & `flowmc-0.3.2/src/flowMC/nfmodel/realNVP.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/nfmodel/rqSpline.py` & `flowmc-0.3.2/src/flowMC/nfmodel/rqSpline.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/Gaussian_random_walk.py` & `flowmc-0.3.2/src/flowMC/proposal/Gaussian_random_walk.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/HMC.py` & `flowmc-0.3.2/src/flowMC/proposal/HMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/MALA.py` & `flowmc-0.3.2/src/flowMC/proposal/MALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/NF_proposal.py` & `flowmc-0.3.2/src/flowMC/proposal/NF_proposal.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/base.py` & `flowmc-0.3.2/src/flowMC/proposal/base.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/proposal/flowHMC.py` & `flowmc-0.3.2/src/flowMC/proposal/flowHMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/strategy/base.py` & `flowmc-0.3.2/src/flowMC/strategy/base.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/strategy/global_tuning.py` & `flowmc-0.3.2/src/flowMC/strategy/global_tuning.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/utils/EvolutionaryOptimizer.py` & `flowmc-0.3.2/src/flowMC/utils/EvolutionaryOptimizer.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/utils/PythonFunctionWrap.py` & `flowmc-0.3.2/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC/utils/postprocessing.py` & `flowmc-0.3.2/src/flowMC/utils/postprocessing.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.1/src/flowMC.egg-info/PKG-INFO` & `flowmc-0.3.2/src/flowMC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.1
+Version: 0.3.2
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.1 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.2 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowMC-0.3.1/src/flowMC.egg-info/SOURCES.txt` & `flowmc-0.3.2/src/flowMC.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 src/flowMC/proposal/__init__.py
 src/flowMC/proposal/base.py
 src/flowMC/proposal/flowHMC.py
 src/flowMC/strategy/__init__.py
 src/flowMC/strategy/base.py
 src/flowMC/strategy/global_tuning.py
 src/flowMC/strategy/importance_sampling.py
+src/flowMC/strategy/optimization.py
 src/flowMC/utils/EvolutionaryOptimizer.py
 src/flowMC/utils/PythonFunctionWrap.py
 src/flowMC/utils/__init__.py
 src/flowMC/utils/postprocessing.py
```

