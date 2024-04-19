# Comparing `tmp/sae_lens-0.5.0.tar.gz` & `tmp/sae_lens-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.5.0.tar", max compression
+gzip compressed data, was "sae_lens-0.5.1.tar", max compression
```

## Comparing `sae_lens-0.5.0.tar` & `sae_lens-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2024-04-17 16:45:34.877116 sae_lens-0.5.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-04-17 16:45:34.877116 sae_lens-0.5.0/README.md
--rw-r--r--   0        0        0     1705 2024-04-17 16:45:35.857121 sae_lens-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-17 16:45:35.853121 sae_lens-0.5.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      595 2024-04-17 16:45:34.885116 sae_lens-0.5.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    19373 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     5562 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16799 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2861 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     9222 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1527 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     7855 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    13743 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    17382 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-17 16:45:34.889116 sae_lens-0.5.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     3923 1970-01-01 00:00:00.000000 sae_lens-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-19 11:04:19.539424 sae_lens-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2553 2024-04-19 11:04:19.539424 sae_lens-0.5.1/README.md
+-rw-r--r--   0        0        0     1775 2024-04-19 11:04:20.771440 sae_lens-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-19 11:04:20.771440 sae_lens-0.5.1/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      992 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    17944 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     5562 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    16793 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     9804 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8052 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    14328 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    19031 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     4888 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-19 11:04:19.551424 sae_lens-0.5.1/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 sae_lens-0.5.1/PKG-INFO
```

### Comparing `sae_lens-0.5.0/LICENSE` & `sae_lens-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/README.md` & `sae_lens-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/pyproject.toml` & `sae_lens-0.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.5.0"
+version = "0.5.1"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,41 +16,44 @@
 nbformat = "^5.9.2"
 ipykernel = "^6.29.2"
 matplotlib = "^3.8.3"
 matplotlib-inline = "^0.1.6"
 datasets = "^2.17.1"
 babe = "^0.0.7"
 nltk = "^3.8.1"
-sae-vis = "0.2.6"
+sae-vis = "^0.2.15"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.15"
 mkdocs-autorefs = "^1.0.1"
 mkdocs-section-index = "^0.3.8"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
 safetensors = "^0.4.2"
+typer = "^0.12.3"
 mamba-lens = { version = "^0.0.4", optional = true }
+pyzmq = "26.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 flake8 = "^7.0.0"
-isort = "^5.13.2"
+isort = "5.13.2"
 pyright = "^1.1.351"
 mamba-lens = "^0.0.4"
 
 [tool.poetry.extras]
 mamba = ["mamba-lens"]
 
 
 [tool.isort]
 profile = "black"
+src_paths = ["sae_lens", "tests"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportMissingTypeStubs = "none"
 reportUnknownMemberType = "none"
 reportUnknownArgumentType = "none"
 reportUnknownVariableType = "none"
```

### Comparing `sae_lens-0.5.0/sae_lens/__init__.py` & `sae_lens-0.5.1/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.5.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.5.1/sae_lens/analysis/dashboard_runner.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 import time
 import uuid
 
 import pandas as pd
 import plotly
 import plotly.express as px
 import torch
+import wandb
 from sae_vis.data_config_classes import (
     ActsHistogramConfig,
     Column,
     FeatureTablesConfig,
     SaeVisConfig,
     SaeVisLayoutConfig,
     SequencesConfig,
 )
 from sae_vis.data_fetching_fns import get_feature_data
 from torch.nn.functional import cosine_similarity
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
-import wandb
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 
 class DashboardRunner:
 
     model: HookedTransformer | None = None
```

### Comparing `sae_lens-0.5.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.5.1/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.5.1/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 import os
 from typing import Any, Dict, List, Optional, Union, cast
 
 # set TOKENIZERS_PARALLELISM to false to avoid warnings
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 import json
-import time
 
 import numpy as np
 import torch
 from matplotlib import colors
 from sae_vis.data_config_classes import (
     ActsHistogramConfig,
     Column,
     FeatureTablesConfig,
+    LogitsHistogramConfig,
+    LogitsTableConfig,
     SaeVisConfig,
     SaeVisLayoutConfig,
     SequencesConfig,
 )
-from sae_vis.data_fetching_fns import get_feature_data
+from sae_vis.data_storing_fns import SaeVisData
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
+from sae_lens.toolkit.pretrained_saes import load_sparsity
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
+from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 OUT_OF_RANGE_TOKEN = "<|outofrange|>"
 
 BG_COLOR_MAP = colors.LinearSegmentedColormap.from_list(
     "bg_color_map", ["white", "darkorange"]
 )
 
+DEFAULT_SPARSITY_THRESHOLD = -5
+
+HTML_ANOMALIES = {
+    "âĢĶ": "—",
+    "âĢĵ": "–",
+    "âĢľ": "“",
+    "âĢĿ": "”",
+    "âĢĺ": "‘",
+    "âĢĻ": "’",
+    "âĢĭ": " ",  # todo: this is actually zero width space
+    "Ġ": " ",
+    "Ċ": "\n",
+    "ĉ": "\t",
+}
+
 
 class NpEncoder(json.JSONEncoder):
     def default(self, o: Any):
         if isinstance(o, np.integer):
             return int(o)
         if isinstance(o, np.floating):
             return float(o)
         if isinstance(o, np.ndarray):
             return o.tolist()
         return super(NpEncoder, self).default(o)
 
 
 class NeuronpediaRunner:
 
-    model: HookedTransformer | None = None
-
     def __init__(
         self,
+        sae_id: str,
         sae_path: str,
-        feature_sparsity_path: Optional[str] = None,
-        neuronpedia_parent_folder: str = "./neuronpedia_outputs",
-        init_session: bool = True,
+        outputs_dir: str,
+        sparsity_threshold: int = DEFAULT_SPARSITY_THRESHOLD,
         # token pars
         n_batches_to_sample_from: int = 2**12,
         n_prompts_to_select: int = 4096 * 6,
-        # sampling pars
-        n_features_at_a_time: int = 1024,
-        buffer_tokens_left: int = 8,
-        buffer_tokens_right: int = 8,
-        # start and end batch
+        # batching
+        n_features_at_a_time: int = 128,
         start_batch_inclusive: int = 0,
         end_batch_inclusive: Optional[int] = None,
     ):
-        self.sae_path = sae_path
-        if init_session:
-            self.init_sae_session()
 
-        self.feature_sparsity_path = feature_sparsity_path
+        self.device = "cpu"
+        if torch.backends.mps.is_available():
+            self.device = "mps"
+        elif torch.cuda.is_available():
+            self.device = "cuda"
+
+        self.sae_path = sae_path
+        self.sparse_autoencoder = SparseAutoencoder.load_from_pretrained(
+            self.sae_path, device=self.device
+        )
+        loader = LMSparseAutoencoderSessionloader(self.sparse_autoencoder.cfg)
+        self.model, _, self.activation_store = loader.load_sae_training_group_session()
+        self.model_id = self.sparse_autoencoder.cfg.model_name
+        self.layer = self.sparse_autoencoder.cfg.hook_point_layer
+        self.sae_id = sae_id
+        self.sparsity_threshold = sparsity_threshold
         self.n_features_at_a_time = n_features_at_a_time
-        self.buffer_tokens_left = buffer_tokens_left
-        self.buffer_tokens_right = buffer_tokens_right
         self.n_batches_to_sample_from = n_batches_to_sample_from
         self.n_prompts_to_select = n_prompts_to_select
         self.start_batch = start_batch_inclusive
         self.end_batch = end_batch_inclusive
 
-        # Deal with file structure
-        if not os.path.exists(neuronpedia_parent_folder):
-            os.makedirs(neuronpedia_parent_folder)
-        self.neuronpedia_folder = (
-            f"{neuronpedia_parent_folder}/{self.get_folder_name()}"
-        )
-        if not os.path.exists(self.neuronpedia_folder):
-            os.makedirs(self.neuronpedia_folder)
-
-    def get_folder_name(self):
-        model = self.sparse_autoencoder.cfg.model_name
-        hook_point = self.sparse_autoencoder.cfg.hook_point
-        d_sae = self.sparse_autoencoder.cfg.d_sae
-        dashboard_folder_name = f"{model}_{hook_point}_{d_sae}"
-
-        return dashboard_folder_name
-
-    def init_sae_session(self):
-        (
-            model,
-            sae_group,
-            self.activation_store,
-        ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
-        # only HookedTransformer works with this runner
-        assert isinstance(model, HookedTransformer)
-        self.model = model
-        # TODO: handle multiple autoencoders
-        self.sparse_autoencoder = next(iter(sae_group))[1]
+        if not os.path.exists(outputs_dir):
+            os.makedirs(outputs_dir)
+        self.outputs_dir = outputs_dir
 
     def get_tokens(
-        self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
+        self,
+        n_batches_to_sample_from: int = 2**12,
+        n_prompts_to_select: int = 4096 * 6,
     ):
         all_tokens_list = []
         pbar = tqdm(range(n_batches_to_sample_from))
         for _ in pbar:
             batch_tokens = self.activation_store.get_batch_tokens()
             batch_tokens = batch_tokens[torch.randperm(batch_tokens.shape[0])][
                 : batch_tokens.shape[0]
@@ -120,15 +120,17 @@
         all_tokens = all_tokens[torch.randperm(all_tokens.shape[0])]
         return all_tokens[:n_prompts_to_select]
 
     def round_list(self, to_round: list[float]):
         return list(np.round(to_round, 3))
 
     def to_str_tokens_safe(
-        self, vocab_dict: Dict[int, str], tokens: Union[int, List[int], torch.Tensor]
+        self,
+        vocab_dict: Dict[int, str],
+        tokens: Union[int, List[int], torch.Tensor],
     ):
         """
         does to_str_tokens, except handles out of range
         """
         assert self.model is not None
         vocab_max_index = self.model.cfg.d_vocab - 1
         # Deal with the int case separately
@@ -147,81 +149,82 @@
             for t in tokens.flatten().tolist()
         ]
 
         # Reshape
         return np.reshape(str_tokens, tokens.shape).tolist()
 
     def run(self):
-        """
-        Generate the Neuronpedia outputs.
-        """
-
-        if self.model is None:
-            self.init_sae_session()
-
         self.n_features = self.sparse_autoencoder.cfg.d_sae
         assert self.n_features is not None
 
         # if we have feature sparsity, then use it to only generate outputs for non-dead features
         self.target_feature_indexes: list[int] = []
-        if self.feature_sparsity_path:
-            loaded = torch.load(
-                self.feature_sparsity_path, map_location=self.sparse_autoencoder.device
-            )
-            self.target_feature_indexes = (
-                (loaded > -5).nonzero(as_tuple=True)[0].tolist()
-            )
-        else:
-            self.target_feature_indexes = list(range(self.n_features))
-            print("No feat sparsity path specified - doing all indexes.")
+        sparsity = load_sparsity(self.sae_path)
+        # convert sparsity to logged sparsity if it's not
+        # TODO: standardize the sparsity file format
+        if len(sparsity) > 0 and sparsity[0] >= 0:
+            sparsity = torch.log10(sparsity + 1e-10)
+        sparsity = sparsity.to(self.device)
+        self.target_feature_indexes = (
+            (sparsity > self.sparsity_threshold).nonzero(as_tuple=True)[0].tolist()
+        )
 
         # divide into batches
         feature_idx = torch.tensor(self.target_feature_indexes)
         n_subarrays = np.ceil(len(feature_idx) / self.n_features_at_a_time).astype(int)
         feature_idx = np.array_split(feature_idx, n_subarrays)
         feature_idx = [x.tolist() for x in feature_idx]
 
-        print(f"==== Starting at batch: {self.start_batch}")
-        if self.end_batch is not None:
-            print(f"==== Ending at batch: {self.end_batch}")
+        # print(f"==== Starting Batch: {self.start_batch}")
+        # if self.end_batch is not None and self.end_batch != self.start_batch:
+        #     print(f"==== Ending at Batch: {self.end_batch}")
 
         if self.start_batch > len(feature_idx) + 1:
             print(
                 f"Start batch {self.start_batch} is greater than number of batches + 1 {len(feature_idx)}, exiting"
             )
             exit()
 
         # write dead into file so we can create them as dead in Neuronpedia
         skipped_indexes = set(range(self.n_features)) - set(self.target_feature_indexes)
-        skipped_indexes_json = json.dumps({"skipped_indexes": list(skipped_indexes)})
-        with open(f"{self.neuronpedia_folder}/skipped_indexes.json", "w") as f:
+        skipped_indexes_json = json.dumps(
+            {
+                "model_id": self.model_id,
+                "layer": str(self.layer),
+                "sae_id": self.sae_id,
+                "skipped_indexes": list(skipped_indexes),
+            }
+        )
+        with open(f"{self.outputs_dir}/skipped_indexes.json", "w") as f:
             f.write(skipped_indexes_json)
 
-        print(f"Total features to run: {len(self.target_feature_indexes)}")
-        print(f"Total skipped: {len(skipped_indexes)}")
-        print(f"Total batches: {len(feature_idx)}")
-
-        print(f"Hook Point Layer: {self.sparse_autoencoder.cfg.hook_point_layer}")
-        print(f"Hook Point: {self.sparse_autoencoder.cfg.hook_point}")
-        print(f"Writing files to: {self.neuronpedia_folder}")
-
-        # get tokens:
-        start = time.time()
-        tokens = self.get_tokens(
-            self.n_batches_to_sample_from, self.n_prompts_to_select
-        )
-        end = time.time()
-        print(f"Time to get tokens: {end - start}")
+        tokens_file = f"{self.outputs_dir}/tokens_{self.n_batches_to_sample_from}_{self.n_prompts_to_select}.pt"
+        if os.path.isfile(tokens_file):
+            print("Tokens exist, loading them.")
+            tokens = torch.load(tokens_file)
+        else:
+            print("Tokens don't exist, making them.")
+            tokens = self.get_tokens(
+                self.n_batches_to_sample_from, self.n_prompts_to_select
+            )
+            torch.save(
+                tokens,
+                tokens_file,
+            )
+
+        vocab_dict = self.model.tokenizer.vocab
+        new_vocab_dict = {}
+        # Replace substrings in the keys of vocab_dict using HTML_ANOMALIES
+        for k, v in vocab_dict.items():
+            modified_key = k
+            for anomaly in HTML_ANOMALIES:
+                modified_key = modified_key.replace(anomaly, HTML_ANOMALIES[anomaly])
+            new_vocab_dict[v] = modified_key
+        vocab_dict = new_vocab_dict
 
-        assert self.model is not None
-        vocab_dict = cast(Any, self.model.tokenizer).vocab
-        vocab_dict = {
-            v: k.replace("Ġ", " ").replace("\n", "\\n").replace("Ċ", "\n")
-            for k, v in vocab_dict.items()
-        }
         # pad with blank tokens to the actual vocab size
         for i in range(len(vocab_dict), self.model.cfg.d_vocab):
             vocab_dict[i] = OUT_OF_RANGE_TOKEN
 
         with torch.no_grad():
             feature_batch_count = 0
             for features_to_process in tqdm(feature_idx):
@@ -230,52 +233,45 @@
                 if feature_batch_count < self.start_batch:
                     # print(f"Skipping batch - it's after start_batch: {feature_batch_count}")
                     continue
                 if self.end_batch is not None and feature_batch_count > self.end_batch:
                     # print(f"Skipping batch - it's after end_batch: {feature_batch_count}")
                     continue
 
-                print(f"Doing batch: {feature_batch_count}")
+                print(f"========== Running Batch #{feature_batch_count} ==========")
 
                 layout = SaeVisLayoutConfig(
                     columns=[
                         Column(
                             SequencesConfig(
                                 stack_mode="stack-all",
-                                buffer=(
-                                    self.buffer_tokens_left,
-                                    self.buffer_tokens_right,
-                                ),
-                                compute_buffer=False,
-                                n_quantiles=10,
+                                buffer=None,  # type: ignore
+                                compute_buffer=True,
+                                n_quantiles=5,
                                 top_acts_group_size=20,
                                 quantile_group_size=5,
                             ),
-                            width=650,
-                        ),
-                        Column(
                             ActsHistogramConfig(),
-                            FeatureTablesConfig(n_rows=5),
-                            width=500,
-                        ),
-                    ],
-                    height=1000,
+                            LogitsHistogramConfig(),
+                            LogitsTableConfig(),
+                            FeatureTablesConfig(n_rows=3),
+                        )
+                    ]
                 )
                 feature_vis_params = SaeVisConfig(
                     hook_point=self.sparse_autoencoder.cfg.hook_point,
-                    minibatch_size_features=256,
+                    minibatch_size_features=128,
                     minibatch_size_tokens=64,
                     features=features_to_process,
-                    verbose=False,
+                    verbose=True,
                     feature_centric_layout=layout,
                 )
-
-                feature_data = get_feature_data(
+                feature_data = SaeVisData.create(
                     encoder=self.sparse_autoencoder,  # type: ignore
-                    model=self.model,
+                    model=cast(HookedTransformer, self.model),
                     tokens=tokens,
                     cfg=feature_vis_params,
                 )
 
                 features_outputs = []
                 for _, feat_index in enumerate(feature_data.feature_data_dict.keys()):
                     feature = feature_data.feature_data_dict[feat_index]
@@ -284,105 +280,78 @@
                     feature_output["featureIndex"] = feat_index
 
                     top10_logits = self.round_list(feature.logits_table_data.top_logits)
                     bottom10_logits = self.round_list(
                         feature.logits_table_data.bottom_logits
                     )
 
-                    # TODO: don't precompute/store these. should do it on the frontend
-                    max_value = max(
-                        np.absolute(bottom10_logits).max(),
-                        np.absolute(top10_logits).max(),
-                    )
-                    neg_bg_values = self.round_list(
-                        np.absolute(bottom10_logits) / max_value
-                    )
-                    pos_bg_values = self.round_list(
-                        np.absolute(top10_logits) / max_value
-                    )
-                    feature_output["neg_bg_values"] = neg_bg_values
-                    feature_output["pos_bg_values"] = pos_bg_values
-
                     if feature.feature_tables_data:
                         feature_output["neuron_alignment_indices"] = (
                             feature.feature_tables_data.neuron_alignment_indices
                         )
                         feature_output["neuron_alignment_values"] = self.round_list(
                             feature.feature_tables_data.neuron_alignment_values
                         )
                         feature_output["neuron_alignment_l1"] = self.round_list(
                             feature.feature_tables_data.neuron_alignment_l1
                         )
                         feature_output["correlated_neurons_indices"] = (
                             feature.feature_tables_data.correlated_neurons_indices
                         )
-                        # TODO: this value doesn't exist in the new output type, commenting out for now
-                        # there is a cossim value though - is that what's needed?
-                        # feature_output["correlated_neurons_l1"] = self.round_list(
-                        #     feature.feature_tables_data.correlated_neurons_l1
-                        # )
+                        feature_output["correlated_neurons_l1"] = self.round_list(
+                            feature.feature_tables_data.correlated_neurons_cossim
+                        )
                         feature_output["correlated_neurons_pearson"] = self.round_list(
                             feature.feature_tables_data.correlated_neurons_pearson
                         )
-                        # feature_output["correlated_features_indices"] = (
-                        #     feature.feature_tables_data.correlated_features_indices
-                        # )
-                        # feature_output["correlated_features_l1"] = self.round_list(
-                        #     feature.feature_tables_data.correlated_features_l1
-                        # )
-                        # feature_output["correlated_features_pearson"] = self.round_list(
-                        #     feature.feature_tables_data.correlated_features_pearson
-                        # )
+                        feature_output["correlated_features_indices"] = (
+                            feature.feature_tables_data.correlated_features_indices
+                        )
+                        feature_output["correlated_features_l1"] = self.round_list(
+                            feature.feature_tables_data.correlated_features_cossim
+                        )
+                        feature_output["correlated_features_pearson"] = self.round_list(
+                            feature.feature_tables_data.correlated_features_pearson
+                        )
 
                     feature_output["neg_str"] = self.to_str_tokens_safe(
                         vocab_dict, feature.logits_table_data.bottom_token_ids
                     )
                     feature_output["neg_values"] = bottom10_logits
                     feature_output["pos_str"] = self.to_str_tokens_safe(
                         vocab_dict, feature.logits_table_data.top_token_ids
                     )
                     feature_output["pos_values"] = top10_logits
 
-                    # TODO: don't know what this should be in the new version
-                    # feature_output["frac_nonzero"] = (
-                    #     feature.middle_plots_data.frac_nonzero
-                    # )
+                    feature_output["frac_nonzero"] = (
+                        float(
+                            feature.acts_histogram_data.title.split(" = ")[1].split(
+                                "%"
+                            )[0]
+                        )
+                        / 100
+                        if feature.acts_histogram_data.title is not None
+                        else 0
+                    )
 
                     freq_hist_data = feature.acts_histogram_data
                     freq_bar_values = self.round_list(freq_hist_data.bar_values)
                     feature_output["freq_hist_data_bar_values"] = freq_bar_values
-                    feature_output["freq_hist_data_tick_vals"] = self.round_list(
-                        freq_hist_data.tick_vals
-                    )
-
-                    # TODO: don't precompute/store these. should do it on the frontend
-                    freq_bar_values_clipped = [
-                        (0.4 * max(freq_bar_values) + 0.6 * v) / max(freq_bar_values)
-                        for v in freq_bar_values
-                    ]
-                    freq_bar_colors = [
-                        colors.rgb2hex(BG_COLOR_MAP(v)) for v in freq_bar_values_clipped
-                    ]
                     feature_output["freq_hist_data_bar_heights"] = self.round_list(
                         freq_hist_data.bar_heights
                     )
-                    feature_output["freq_bar_colors"] = freq_bar_colors
 
                     logits_hist_data = feature.logits_histogram_data
                     feature_output["logits_hist_data_bar_heights"] = self.round_list(
                         logits_hist_data.bar_heights
                     )
                     feature_output["logits_hist_data_bar_values"] = self.round_list(
                         logits_hist_data.bar_values
                     )
-                    feature_output["logits_hist_data_tick_vals"] = self.round_list(
-                        logits_hist_data.tick_vals
-                    )
 
-                    # TODO: check this
                     feature_output["num_tokens_for_dashboard"] = (
                         self.n_prompts_to_select
                     )
 
                     activations = []
                     sdbs = feature.sequence_data
                     for sgd in sdbs.seq_group_data:
@@ -437,15 +406,24 @@
                                 )
 
                                 activations.append(activation)
                     feature_output["activations"] = activations
 
                     features_outputs.append(feature_output)
 
-                json_object = json.dumps(features_outputs, cls=NpEncoder)
+                to_write = {
+                    "model_id": self.model_id,
+                    "layer": str(self.layer),
+                    "sae_id": self.sae_id,
+                    "features": features_outputs,
+                    "n_batches_to_sample_from": self.n_batches_to_sample_from,
+                    "n_prompts_to_select": self.n_prompts_to_select,
+                }
+                json_object = json.dumps(to_write, cls=NpEncoder)
 
                 with open(
-                    f"{self.neuronpedia_folder}/batch-{feature_batch_count}.json", "w"
+                    f"{self.outputs_dir}/batch-{feature_batch_count}.json",
+                    "w",
                 ) as f:
                     f.write(json_object)
 
         return
```

### Comparing `sae_lens-0.5.0/sae_lens/analysis/tsea.py` & `sae_lens-0.5.1/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.5.1/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/activations_store.py` & `sae_lens-0.5.1/sae_lens/training/activations_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             dataset=dataset or cfg.dataset_path,
             hook_point=cfg.hook_point,
             hook_point_layers=listify(cfg.hook_point_layer),
             hook_point_head_index=cfg.hook_point_head_index,
             context_size=cfg.context_size,
             d_in=cfg.d_in,
             n_batches_in_buffer=cfg.n_batches_in_buffer,
-            total_training_tokens=cfg.total_training_tokens,
+            total_training_tokens=cfg.training_tokens,
             store_batch_size=cfg.store_batch_size,
             train_batch_size=cfg.train_batch_size,
             prepend_bos=cfg.prepend_bos,
             device=cfg.device,
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
             model_kwargs=cfg.model_kwargs,
```

### Comparing `sae_lens-0.5.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.5.1/sae_lens/training/cache_activations_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         if len(os.listdir(activations_store.cached_activations_path)) > 0:
             raise Exception(
                 f"Activations directory ({activations_store.cached_activations_path}) is not empty. Please delete it or specify a different path. Exiting the script to prevent accidental deletion of files."
             )
     else:
         os.makedirs(activations_store.cached_activations_path)
 
-    print(f"Started caching {cfg.total_training_tokens} activations")
+    print(f"Started caching {cfg.training_tokens} activations")
     tokens_per_buffer = (
         cfg.store_batch_size * cfg.context_size * cfg.n_batches_in_buffer
     )
-    n_buffers = math.ceil(cfg.total_training_tokens / tokens_per_buffer)
+    n_buffers = math.ceil(cfg.training_tokens / tokens_per_buffer)
     # for i in tqdm(range(n_buffers), desc="Caching activations"):
     for i in range(n_buffers):
         buffer = activations_store.get_buffer(cfg.n_batches_in_buffer)
         torch.save(buffer, f"{activations_store.cached_activations_path}/{i}.pt")
         del buffer
 
         if i % cfg.shuffle_every_n_buffers == 0 and i > 0:
```

### Comparing `sae_lens-0.5.0/sae_lens/training/config.py` & `sae_lens-0.5.1/sae_lens/training/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass, field
 from typing import Any, Optional, cast
 
 import torch
-
 import wandb
 
 DTYPE_MAP = {
     "torch.float32": torch.float32,
     "torch.float64": torch.float64,
     "torch.float16": torch.float16,
     "torch.bfloat16": torch.bfloat16,
@@ -41,41 +40,53 @@
     expansion_factor: int | list[int] = 4
     from_pretrained_path: Optional[str] = None
     apply_b_dec_to_input: bool = True
     decoder_orthogonal_init: bool = False
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
-    total_training_tokens: int = 2_000_000
+    training_tokens: int = 2_000_000
+    finetuning_tokens: int = 0
     store_batch_size: int = 32
     train_batch_size: int = 4096
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"  # type: ignore #
     prepend_bos: bool = True
 
     # Training Parameters
+
+    ## Batch size
+    train_batch_size: int = 4096
+
+    ## Adam
     adam_beta1: float | list[float] = 0
     adam_beta2: float | list[float] = 0.999
+
+    ## Loss Function
     mse_loss_normalization: Optional[str] = None
     l1_coefficient: float | list[float] = 1e-3
     lp_norm: float | list[float] = 1
+
+    ## Learning Rate Schedule
     lr: float | list[float] = 3e-4
     lr_scheduler_name: str | list[str] = (
         "constant"  # constant, cosineannealing, cosineannealingwarmrestarts
     )
     lr_warm_up_steps: int | list[int] = 500
     lr_end: float | list[float] | None = (
         None  # only used for cosine annealing, default is lr / 10
     )
     lr_decay_steps: int | list[int] = 0
     n_restart_cycles: int | list[int] = 1  # used only for cosineannealingwarmrestarts
-    train_batch_size: int = 4096
+
+    ## FineTuning
+    finetuning_method: Optional[str] = None  # scale, decoder or unrotated_decoder
 
     # Resampling protocol args
     use_ghost_grads: bool | list[bool] = (
         False  # want to change this to true on some timeline.
     )
     feature_sampling_window: int = 2000
     dead_feature_window: int = 1000  # unless this window is larger feature sampling,
@@ -107,15 +118,15 @@
         if not isinstance(self.expansion_factor, list):
             self.d_sae = self.d_in * self.expansion_factor
         self.tokens_per_buffer = (
             self.train_batch_size * self.context_size * self.n_batches_in_buffer
         )
 
         if self.run_name is None:
-            self.run_name = f"{self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.total_training_tokens:3.3e}"
+            self.run_name = f"{self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
 
         if self.b_dec_init_method not in ["geometric_median", "mean", "zeros"]:
             raise ValueError(
                 f"b_dec_init_method must be geometric_median, mean, or zeros. Got {self.b_dec_init_method}"
             )
         if self.b_dec_init_method == "zeros":
             print(
@@ -125,14 +136,20 @@
         if isinstance(self.dtype, str) and self.dtype not in DTYPE_MAP:
             raise ValueError(
                 f"dtype must be one of {list(DTYPE_MAP.keys())}. Got {self.dtype}"
             )
         elif isinstance(self.dtype, str):
             self.dtype: torch.dtype = DTYPE_MAP[self.dtype]
 
+        # if we use decoder fine tuning, we can't be applying b_dec to the input
+        if (self.finetuning_method == "decoder") and (self.apply_b_dec_to_input):
+            raise ValueError(
+                "If we are fine tuning the decoder, we can't be applying b_dec to the input.\nSet apply_b_dec_to_input to False."
+            )
+
         self.device: str | torch.device = torch.device(self.device)
 
         if self.lr_end is None:
             if isinstance(self.lr, list):
                 self.lr_end = [lr / 10 for lr in self.lr]
             else:
                 self.lr_end = self.lr / 10
@@ -140,27 +157,29 @@
         unique_id = cast(
             Any, wandb
         ).util.generate_id()  # not sure why this type is erroring
         self.checkpoint_path = f"{self.checkpoint_path}/{unique_id}"
 
         if self.verbose:
             print(
-                f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.total_training_tokens:3.3e}"
+                f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
             )
             # Print out some useful info:
             n_tokens_per_buffer = (
                 self.store_batch_size * self.context_size * self.n_batches_in_buffer
             )
             print(f"n_tokens_per_buffer (millions): {n_tokens_per_buffer / 10 **6}")
             n_contexts_per_buffer = self.store_batch_size * self.n_batches_in_buffer
             print(
                 f"Lower bound: n_contexts_per_buffer (millions): {n_contexts_per_buffer / 10 **6}"
             )
 
-            total_training_steps = self.total_training_tokens // self.train_batch_size
+            total_training_steps = (
+                self.training_tokens + self.finetuning_tokens
+            ) // self.train_batch_size
             print(f"Total training steps: {total_training_steps}")
 
             total_wandb_updates = total_training_steps // self.wandb_log_frequency
             print(f"Total wandb updates: {total_wandb_updates}")
 
             # how many times will we sample dead neurons?
             # assert self.dead_feature_window <= self.feature_sampling_window, "dead_feature_window must be smaller than feature_sampling_window"
@@ -205,15 +224,15 @@
     )
 
     # SAE Parameters
     d_in: int = 512
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
-    total_training_tokens: int = 2_000_000
+    training_tokens: int = 2_000_000
     store_batch_size: int = 32
     train_batch_size: int = 4096
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"
```

### Comparing `sae_lens-0.5.0/sae_lens/training/evals.py` & `sae_lens-0.5.1/sae_lens/training/evals.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 from typing import Any, Mapping, cast
 
 import pandas as pd
 import torch
+import wandb
 from transformer_lens.hook_points import HookedRootModule
 
-import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 @torch.no_grad()
 def run_evals(
     sparse_autoencoder: SparseAutoencoder,
```

### Comparing `sae_lens-0.5.0/sae_lens/training/geometric_median.py` & `sae_lens-0.5.1/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/lm_runner.py` & `sae_lens-0.5.1/sae_lens/training/lm_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, cast
 
 import wandb
+
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.session_loader import LMSparseAutoencoderSessionloader
 
 # from sae_lens.training.activation_store import ActivationStore
 from sae_lens.training.train_sae_on_language_model import train_sae_on_language_model
```

### Comparing `sae_lens-0.5.0/sae_lens/training/load_model.py` & `sae_lens-0.5.1/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/optim.py` & `sae_lens-0.5.1/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/sae_group.py` & `sae_lens-0.5.1/sae_lens/training/sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
         # handle loading old autoencoders where before SAEGroup existed, where we just save a dict
         if isinstance(group, dict):
             cfg = group["cfg"]
             # need to add this field to old configs
             if not hasattr(cfg, "model_kwargs"):
                 cfg.model_kwargs = {}
             sparse_autoencoder = SparseAutoencoder(cfg=cfg)
+            # add dummy scaling factor to the state dict
+            group["state_dict"]["scaling_factor"] = torch.ones(
+                cfg.d_sae, dtype=cfg.dtype, device=cfg.device
+            )
             sparse_autoencoder.load_state_dict(group["state_dict"])
             group = cls(cfg)
             for key in group.autoencoders:
                 group.autoencoders[key] = sparse_autoencoder
 
         if not isinstance(group, cls):
             raise ValueError("The loaded object is not a valid SAEGroup")
```

### Comparing `sae_lens-0.5.0/sae_lens/training/session_loader.py` & `sae_lens-0.5.1/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.5.1/sae_lens/training/sparse_autoencoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,19 @@
             # Anthropic normalize this to have unit columns
             self.set_decoder_norm_to_unit_norm()
 
         self.b_dec = nn.Parameter(
             torch.zeros(self.d_in, dtype=self.dtype, device=self.device)
         )
 
+        # scaling factor for fine-tuning (not to be used in initial training)
+        self.scaling_factor = nn.Parameter(
+            torch.ones(self.d_sae, dtype=self.dtype, device=self.device)
+        )
+
         self.hook_sae_in = HookPoint()
         self.hook_hidden_pre = HookPoint()
         self.hook_hidden_post = HookPoint()
         self.hook_sae_out = HookPoint()
 
         self.setup()  # Required for `HookedRootModule`s
 
@@ -120,15 +125,16 @@
             )
             + self.b_enc
         )
         feature_acts = self.hook_hidden_post(torch.nn.functional.relu(hidden_pre))
 
         sae_out = self.hook_sae_out(
             einops.einsum(
-                feature_acts,
+                feature_acts
+                * self.scaling_factor,  # need to make sure this handled when loading old models.
                 self.W_dec,
                 "... d_sae, d_sae d_in -> ... d_in",
             )
             + self.b_dec
         )
 
         # add config for whether l2 is normalized:
@@ -326,14 +332,22 @@
         config = LanguageModelSAERunnerConfig(**config)
         sae = SparseAutoencoder(config)
 
         tensors = {}
         with safe_open(weight_path, framework="pt", device=device) as f:  # type: ignore
             for k in f.keys():
                 tensors[k] = f.get_tensor(k)
+
+        # old saves may not have scaling factors.
+        if "scaling_factor" not in tensors:
+            assert isinstance(config.d_sae, int)
+            tensors["scaling_factor"] = torch.ones(
+                config.d_sae, dtype=config.dtype, device=config.device
+            )
+
         sae.load_state_dict(tensors)
 
         return sae
 
     def get_name(self):
         sae_name = f"sparse_autoencoder_{self.cfg.model_name}_{self.cfg.hook_point}_{self.cfg.d_sae}"
         return sae_name
```

### Comparing `sae_lens-0.5.0/sae_lens/training/toy_model_runner.py` & `sae_lens-0.5.1/sae_lens/training/toy_model_runner.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, cast
 
 import einops
 import torch
-
 import wandb
+
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 from sae_lens.training.toy_models import Config as ToyConfig
 from sae_lens.training.toy_models import Model as ToyModel
 from sae_lens.training.train_sae_on_toy_model import train_toy_sae
 
 
 @dataclass
```

### Comparing `sae_lens-0.5.0/sae_lens/training/toy_models.py` & `sae_lens-0.5.1/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.5.1/sae_lens/training/train_sae_on_language_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import os
 from dataclasses import dataclass
 from typing import Any, cast
 
 import torch
+import wandb
 from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
 from transformer_lens.hook_points import HookedRootModule
 
-import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
+# used to map between parameters which are updated during finetuning and the config str.
+FINETUNING_PARAMETERS = {
+    "scale": ["scaling_factor"],
+    "decoder": ["scaling_factor", "W_dec", "b_dec"],
+    "unrotated_decoder": ["scaling_factor", "b_dec"],
+}
+
 
 def _log_feature_sparsity(
     feature_sparsity: torch.Tensor, eps: float = 1e-10
 ) -> torch.Tensor:
     return torch.log10(feature_sparsity + eps).detach().cpu()
 
 
@@ -31,23 +38,39 @@
     """
 
     act_freq_scores: torch.Tensor
     n_forward_passes_since_fired: torch.Tensor
     n_frac_active_tokens: int
     optimizer: Optimizer
     scheduler: LRScheduler
+    finetuning: bool = False
 
     @property
     def feature_sparsity(self) -> torch.Tensor:
         return self.act_freq_scores / self.n_frac_active_tokens
 
     @property
     def log_feature_sparsity(self) -> torch.Tensor:
         return _log_feature_sparsity(self.feature_sparsity)
 
+    def begin_finetuning(self, sae: SparseAutoencoder):
+
+        # finetuning method should be set in the config
+        # if not, then we don't finetune
+        if not isinstance(sae.cfg.finetuning_method, str):
+            return
+
+        for name, param in sae.named_parameters():
+            if name in FINETUNING_PARAMETERS[sae.cfg.finetuning_method]:
+                param.requires_grad = True
+            else:
+                param.requires_grad = False
+
+        self.finetuning = True
+
 
 @dataclass
 class TrainSAEGroupOutput:
     sae_group: SparseAutoencoderDictionary
     checkpoint_paths: list[str]
     log_feature_sparsities: dict[str, torch.Tensor]
 
@@ -84,18 +107,21 @@
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ) -> TrainSAEGroupOutput:
-    total_training_tokens = sae_group.cfg.total_training_tokens
+    total_training_tokens = (
+        sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
+    )
     total_training_steps = total_training_tokens // batch_size
     n_training_steps = 0
     n_training_tokens = 0
+    started_fine_tuning = False
 
     checkpoint_thresholds = []
     if n_checkpoints > 0:
         checkpoint_thresholds = list(
             range(0, total_training_tokens, total_training_tokens // n_checkpoints)
         )[1:]
 
@@ -176,14 +202,24 @@
 
         n_training_steps += 1
         pbar.set_description(
             f"{n_training_steps}| MSE Loss {torch.stack(mse_losses).mean().item():.3f} | L1 {torch.stack(l1_losses).mean().item():.3f}"
         )
         pbar.update(batch_size)
 
+        ### If n_training_tokens > sae_group.cfg.training_tokens, then we should switch to fine-tuning (if we haven't already)
+        if (not started_fine_tuning) and (
+            n_training_tokens > sae_group.cfg.training_tokens
+        ):
+            started_fine_tuning = True
+            for name, sparse_autoencoder in sae_group.autoencoders.items():
+                ctx = train_contexts[name]
+                # this should turn grads on for the scaling factor and other parameters.
+                ctx.begin_finetuning(sae_group.autoencoders[name])
+
     # save final sae group to checkpoints folder
     final_checkpoint = _save_checkpoint(
         sae_group,
         train_contexts=train_contexts,
         checkpoint_name="final",
         wandb_aliases=["final_model"],
     )
@@ -244,14 +280,20 @@
     )
     n_forward_passes_since_fired = torch.zeros(
         cast(int, sae.cfg.d_sae),
         device=sae.cfg.device,
     )
     n_frac_active_tokens = 0
 
+    # we don't train the scaling factor (initially)
+    # set requires grad to false for the scaling factor
+    for name, param in sae.named_parameters():
+        if "scaling_factor" in name:
+            param.requires_grad = False
+
     optimizer = Adam(
         sae.parameters(),
         lr=sae.cfg.lr,
         betas=(
             sae.cfg.adam_beta1,  # type: ignore
             sae.cfg.adam_beta2,  # type: ignore
         ),
```

### Comparing `sae_lens-0.5.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.5.1/sae_lens/training/train_sae_on_toy_model.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, cast
 
 import torch
+import wandb
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-import wandb
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 def train_toy_sae(
     sparse_autoencoder: SparseAutoencoder,
     activation_store: torch.Tensor,  # TODO: this type seems strange / wrong
     batch_size: int = 1024,
```

### Comparing `sae_lens-0.5.0/sae_lens/training/utils.py` & `sae_lens-0.5.1/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.5.0/PKG-INFO` & `sae_lens-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.5.0
+Version: 0.5.1
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -22,18 +22,20 @@
 Requires-Dist: mkdocs-section-index (>=0.3.8,<0.4.0)
 Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
 Requires-Dist: mkdocstrings-python (>=1.9.0,<2.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
-Requires-Dist: sae-vis (==0.2.6)
+Requires-Dist: pyzmq (==26.0.0)
+Requires-Dist: sae-vis (>=0.2.15,<0.3.0)
 Requires-Dist: safetensors (>=0.4.2,<0.5.0)
 Requires-Dist: transformer-lens (>=1.14.0,<2.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
 <img width="1308" alt="Screenshot 2024-03-21 at 3 08 28 pm" src="https://github.com/jbloomAus/mats_sae_training/assets/69127271/209012ec-a779-4036-b4be-7b7739ea87f6">
 
 # SAE Lens 
 [![PyPI](https://img.shields.io/pypi/v/sae-lens?color=blue)](https://pypi.org/project/sae-lens/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

