# Comparing `tmp/taker-0.9.8.tar.gz` & `tmp/taker-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taker-0.9.8.tar", max compression
+gzip compressed data, was "taker-0.9.9.tar", max compression
```

## Comparing `taker-0.9.8.tar` & `taker-0.9.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     3298 2024-01-16 11:16:40.603818 taker-0.9.8/README.md
--rw-r--r--   0        0        0     1283 2024-01-16 11:16:40.605158 taker-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       24 2024-01-16 11:16:40.605370 taker-0.9.8/src/taker/__init__.py
--rw-r--r--   0        0        0    31066 2024-01-16 11:16:40.605500 taker-0.9.8/src/taker/activations.py
--rw-r--r--   0        0        0     2190 2024-01-16 11:16:40.605623 taker-0.9.8/src/taker/data/imagenet_birds.json
--rw-r--r--   0        0        0     6385 2024-01-16 11:16:40.605696 taker-0.9.8/src/taker/data/llama_most_common_tokens.json
--rw-r--r--   0        0        0    20345 2024-01-16 11:16:40.605809 taker-0.9.8/src/taker/data_classes.py
--rw-r--r--   0        0        0     5719 2024-01-16 11:16:40.605909 taker-0.9.8/src/taker/detoxify.py
--rw-r--r--   0        0        0    43190 2024-01-16 11:16:40.606089 taker-0.9.8/src/taker/eval.py
--rw-r--r--   0        0        0     2068 2024-01-16 11:16:40.606171 taker-0.9.8/src/taker/mia.py
--rw-r--r--   0        0        0    47170 2024-01-16 11:16:40.606348 taker-0.9.8/src/taker/model.py
--rw-r--r--   0        0        0    37528 2024-01-16 11:16:40.606597 taker-0.9.8/src/taker/model_maps.py
--rw-r--r--   0        0        0     1023 2024-01-16 11:16:40.607520 taker-0.9.8/src/taker/model_repos.py
--rw-r--r--   0        0        0    16625 2024-01-16 11:16:40.607658 taker-0.9.8/src/taker/nn.py
--rw-r--r--   0        0        0     2668 2024-01-16 11:16:40.607748 taker-0.9.8/src/taker/parser.py
--rw-r--r--   0        0        0    17827 2024-01-16 11:16:40.607865 taker-0.9.8/src/taker/prune.py
--rw-r--r--   0        0        0     6001 2024-01-16 11:16:40.607966 taker-0.9.8/src/taker/scoring.py
--rw-r--r--   0        0        0    14296 2024-01-16 11:16:40.608066 taker-0.9.8/src/taker/texts.py
--rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 taker-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     3298 2024-01-12 16:32:32.588594 taker-0.9.9/README.md
+-rw-r--r--   0        0        0     1283 2024-02-02 15:48:57.990759 taker-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/__init__.py
+-rw-r--r--   0        0        0    31066 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/activations.py
+-rw-r--r--   0        0        0     2190 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/data/imagenet_birds.json
+-rw-r--r--   0        0        0     6385 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/data/llama_most_common_tokens.json
+-rw-r--r--   0        0        0    20413 2024-01-19 10:31:54.457977 taker-0.9.9/src/taker/data_classes.py
+-rw-r--r--   0        0        0     5719 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/detoxify.py
+-rw-r--r--   0        0        0    43207 2024-01-23 17:20:03.543449 taker-0.9.9/src/taker/eval.py
+-rw-r--r--   0        0        0     2068 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/mia.py
+-rw-r--r--   0        0        0    49103 2024-02-02 13:45:00.611485 taker-0.9.9/src/taker/model.py
+-rw-r--r--   0        0        0    40479 2024-02-02 13:57:58.972571 taker-0.9.9/src/taker/model_maps.py
+-rw-r--r--   0        0        0     1023 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/model_repos.py
+-rw-r--r--   0        0        0    16746 2024-02-02 12:57:26.562194 taker-0.9.9/src/taker/nn.py
+-rw-r--r--   0        0        0     2668 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/parser.py
+-rw-r--r--   0        0        0    17827 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/prune.py
+-rw-r--r--   0        0        0     6001 2024-01-12 16:08:36.301278 taker-0.9.9/src/taker/scoring.py
+-rw-r--r--   0        0        0    14842 2024-01-24 13:37:57.631556 taker-0.9.9/src/taker/texts.py
+-rw-r--r--   0        0        0     1951 2024-01-23 16:29:31.218097 taker-0.9.9/src/taker/vit_processor.py
+-rw-r--r--   0        0        0     4931 1970-01-01 00:00:00.000000 taker-0.9.9/PKG-INFO
```

### Comparing `taker-0.9.8/README.md` & `taker-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/pyproject.toml` & `taker-0.9.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taker"
-version = "0.9.8"
+version = "0.9.9"
 description = "Tools for Transformer Activations Knowledge ExtRaction"
 authors = ["Nicky Pochinkov"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -18,16 +18,16 @@
 numpy = "^1.23"
 numexpr = "^2.7.0"
 torch = "^2.0.1"
 tensorboardx = "^2.5.1"
 tensorboard = "^2.11.2"
 dict-deep = "^4.1.2"
 pandas = "^1.5.3"
-transformers = "^4.30.0"
-tokenizers = "^0.13.3"
+transformers = "^4.33.0"
+tokenizers = "^0.15.1"
 sentencepiece = "^0.1.99"
 bitsandbytes = "^0.40.2"
 scipy = "^1.11.1"
 datasets = "^2.9.0"
 evaluate = "^0.4.0"
 zstandard = "^0.19.0"
 welford-torch = "^0.2.1"
```

### Comparing `taker-0.9.8/src/taker/activations.py` & `taker-0.9.9/src/taker/activations.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/data/imagenet_birds.json` & `taker-0.9.9/src/taker/data/imagenet_birds.json`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/data/llama_most_common_tokens.json` & `taker-0.9.9/src/taker/data/llama_most_common_tokens.json`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/data_classes.py` & `taker-0.9.9/src/taker/data_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 @dataclass
 class EvalConfig:
     dataset_name: str
     dataset_repo: str = None
     dataset_subset: str = None
     dataset_type: str = "prediction" # ["prediction", "generation", "mmlu"]
     dataset_text_key: str = "text"
+    dataset_text_label_key: str = "label" # for text classification
     dataset_filter: Optional[Callable] = None
     dataset_has_test_split: bool = True
     dataset_split: str = None # "test", "train"
     streaming: bool = True # Do not download the whole dataset by default
     sample_size: int = 1e5
     skip_token_strings: Optional[List[str]] = None
     skip_token_ids: Tensor = None
```

### Comparing `taker-0.9.8/src/taker/detoxify.py` & `taker-0.9.9/src/taker/detoxify.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/eval.py` & `taker-0.9.9/src/taker/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 from torch import Tensor
 from datasets import load_dataset, get_dataset_config_names, Dataset
 from welford_torch import Welford
 from tqdm import tqdm
 from .data_classes import EvalConfig, EvalOutput, EvalAllOutput, RawAccuracyData
 from .model import Model
-from .texts import infer_dataset_config, prepare_dataset
+from .texts import infer_dataset_config, prepare_dataset, prepare
 
 ######################################################################################
 # Code that handles loop of: text -> outputs + expected inputs
 ######################################################################################
 
 def get_skip_ids(model, eval_config: EvalConfig):
     # Get the set of token ids to skip when evaluating performance
@@ -331,14 +331,15 @@
             eval_config: EvalConfig,
         ):
 
         dataset = prepare_dataset(eval_config)
 
         for data in dataset:
             # predict next token from text
+            print(data)
             img   = data[eval_config.dataset_image_key]
             label = data[eval_config.dataset_image_label_key]
             with torch.no_grad():
                 try:
                     inputs = model.processor(img, return_tensors="pt")
                 except ValueError:
                     print("Skipping image due to error.")
@@ -363,15 +364,15 @@
 ######################################################################################
 
 class LossTracker:
     def __init__(self):
         self.loss = Welford()
         self.log_loss = Welford()
         self.perplexity = Welford()
-    
+
     def add(self, losses):
         self.loss.add(losses.mean())
         self.log_loss.add(torch.log(losses).mean())
         self.perplexity.add(torch.exp(losses).mean())
 
     def add_all(self, losses):
         self.loss.add_all(losses)
@@ -477,14 +478,15 @@
         c = eval_config
 
         # Initialize variables
         total_acc_data = RawAccuracyData()
         loss_tracker = LossTracker()
 
         # Loop over the dataset
+        print(c.sample_size)
         pbar = tqdm(total=c.sample_size)
         for _item  in generator:
             (logits, expected_ids, _other_data) = _item
 
             # If start index != 0, skip the first tokens
             if c.start_index != 0:
                 logits       = logits[..., c.start_index:]
@@ -539,21 +541,21 @@
         frac_toxic = np.sum(toxicity_arr > 0.8)/eval_config.generated_text_num_samples
         mean_toxicity = np.mean(toxicity_arr)
 
         return EvalOutput(misc={
             "frac_toxic": frac_toxic,
             "mean_toxicity": mean_toxicity,
         })
-    
+
     def evaluate_mia(self,
             model: Model,
             eval_config: EvalConfig
             ):
         from .mia import get_membership_attack_prob
-        
+
         retain_config = infer_dataset_config(eval_config.mia_retain) # eg: cifar100 no mushrooms train
         retain_config.dataset_split = eval_config.mia_retain_split or retain_config.dataset_split
         retain_config.is_train_mode = True
         forget_config = infer_dataset_config(eval_config.mia_forget) # eg: cifar100 mushrooms train
         forget_config.dataset_split = eval_config.mia_forget_split or forget_config.dataset_split
         forget_config.is_train_mode = True
         test_config   = infer_dataset_config(eval_config.mia_test) # eg: cifar100 all test
@@ -591,15 +593,15 @@
         evaluator = Evaluator().evaluate_dataset
         return generator, evaluator
 
     if eval_config.dataset_type == "image-classification":
         generator = ImageGenerators.get_image_classification_generator
         evaluator = Evaluator().evaluate_dataset
         return generator, evaluator
-    
+
     if eval_config.dataset_type == "image-membership-inference-attack":
         generator = ImageGenerators.return_model_as_generator
         evaluator = Evaluator().evaluate_mia
         return generator, evaluator
 
     evaluator = Evaluator().evaluate_dataset
     if eval_config.masked_model:
@@ -936,15 +938,15 @@
         token_count += step_size
         buffer_tokens = buffer_tokens[step_size:]
 
 def evaluate_wikitext(opt: Model,
         sample_size: int = 1024,
         topk: int = 10,
     ):
-    _dataset, _label, skip_eval = prepare('wiki', test=1)
+    _dataset, _label, skip_eval = prepare('wiki')
     wiki_id_generator = sliding_window_dataset(opt.tokenizer, _dataset,
         buffer_size=1024, step_size=512)
         #, max_tokens=sample_size)
 
     def wiki_generator():
         for ids in wiki_id_generator:
             ids = torch.tensor([ids], device=opt.device)
@@ -1094,21 +1096,21 @@
     # Use custom generator for some datasets (eg: MMLU)
     if dataset_name[:4] == "mmlu":
         config = dataset_name[5:]
         generator, n = get_mmlu_generator(opt, config, n_shot=n_shot,
                                           masked=masked, verbose=verbose)
         return generator, None, n
 
-    dataset, label, skip_eval = prepare( dataset_name, test=dataset_tokens_to_skip )
+    dataset, label, skip_eval = prepare(dataset_name)
 
     if masked:
         generator = masked_generator(opt, dataset, label)
         return generator, skip_eval, sample_size
 
-    generator = opt.default_generator(dataset, label)
+    generator = Generators.get_next_token_generator(dataset, label)
     return generator, skip_eval, sample_size
 
 def evaluate( opt: Model,
         dataset_name: str,
         sample_size: int = 1e5,
         topk: int = 10,
         dataset_tokens_to_skip: int = 0,
```

### Comparing `taker-0.9.8/src/taker/mia.py` & `taker-0.9.9/src/taker/mia.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/model.py` & `taker-0.9.9/src/taker/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Defines the 'Model' class which wraps the Meta OPT model,
+""" Defines the 'Model' class which wraps Transformer models,
 with additional methods for inspecting the activations of the model.
 """
 
 # import types for typed python
 from typing import Optional, List, Tuple, Callable
 import warnings
 import time
@@ -45,19 +45,19 @@
 
     s = str(number)
     k = n_digits - len(s)
     k = k if k > 0 else 0
     return "0"*k + s
 
 class Model():
-    """ Wrapper Class for Meta OPT model that allows me to do interpretability
+    """ Wrapper Class for Transformer models that allows me to do interpretability
     work on it's activations and modify it's parameters as needed. """
 
     def __init__( self,
-            model_repo: str  = "facebook/opt-125m",
+            model_repo: str  = "nickypro/tinyllama-15m",
             limit: int = None,
             model_device: str = None,
             output_device: str = None,
             use_accelerator: bool = True,
             dtype: Optional[str] = None,
             torch_dtype: Optional[torch.dtype] = None,
             svd_attn: bool = False,
@@ -74,31 +74,35 @@
         """
 
         # Initialize model differently depending on accelerator use
         self.use_accelerator = use_accelerator and torch.cuda.device_count() > 1
         self.dtype = dtype
         self.svd_attn = svd_attn
 
-        # Handle dtype
-        if dtype is None and torch_dtype is None:
-            dtype = "fp16"
-        self.dtype_map = DtypeMap(dtype, torch_dtype)
-        self.dtype = self.dtype_map._dtype
-        self.dtype_args = self.dtype_map._dtype_args
-
+        # Handle multi-gpu stuff
         if self.use_accelerator:
             self.accelerator = Accelerator()
             self.device = self.accelerator.device
             self.output_device = output_device if output_device else 'cuda:1'
 
         else:
             self.device = 'cuda' if torch.cuda.is_available() else 'cpu'
             self.device = model_device if model_device else self.device
             self.output_device = output_device if output_device else self.device
 
+        # Handle dtype
+        if dtype is None and torch_dtype is None:
+            dtype = "fp16"
+        if self.device == "cpu":
+            dtype = "fp32"
+        self.dtype_map = DtypeMap(dtype, torch_dtype)
+        self.dtype = self.dtype_map._dtype
+        self.dtype_args = self.dtype_map._dtype_args
+
+
         # Define the model repo
         self.model_size: str = None
         self.model_repo: str = None
         self.tokenizer_repo: str = None
         self.set_repo(model_repo, tokenizer_repo)
 
         # Add masking parameters
@@ -145,16 +149,15 @@
         self.cfg = convert_hf_model_config(self.model_repo)
         self.cfg.is_low_precision = self.dtype_map.is_low_precision
 
         # Import model components (Default: Causal Language Models)
         if self.cfg.model_modality == "vision":
             from transformers import AutoImageProcessor, AutoModelForImageClassification
             self.tokenizer = None,
-            self.processor = AutoImageProcessor.from_pretrained(
-                self.model_repo, device_map=device_map, **self.dtype_args)
+            self.init_image_processor(device_map)
             self.predictor = AutoModelForImageClassification.from_pretrained(
                 self.model_repo, device_map=device_map, **self.dtype_args)
         elif self.cfg.model_modality == "language":
             self.tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_repo, legacy=False)
             self.processor = None
             self.predictor = AutoModelForCausalLM.from_pretrained(
                 self.model_repo, device_map=device_map, **self.dtype_args)
@@ -186,14 +189,38 @@
             return self
         if self.svd_attn:
             self.svd_attention_layers()
         else:
             self.register_inverse_out_proj()
         return self
 
+    def init_image_processor(self, device_map):
+        """ Initialize processor from raw pixel values to normalised tensors"""
+        try:
+            from transformers import AutoImageProcessor
+            self.processor = AutoImageProcessor.from_pretrained(
+                self.model_repo, device_map=device_map, **self.dtype_args)
+
+        except:
+            from .vit_processor import SsdVitProcessor
+            self.processor = SsdVitProcessor()
+
+
+    def init_vit(self):
+        from transformers import ViTModel, ViTForImageClassification, AutoConfig
+
+        vit_base_repo = "google/vit-base-patch16-224"
+        vit_cifar_repo = "Ahmed9275/Vit-Cifar100"
+        cfg = AutoConfig.from_pretained("Ahmed9275/Vit-Cifar100")
+        model = ViTForImageClassification(cfg)
+        vit = ViTModel.from_pretrained(vit_base_repo)
+        model.vit = vit
+
+        return model.to(self.device)
+
     def show_details( self, verbose=True ):
         if verbose:
             print( " - n_layers :", self.cfg.n_layers )
             print( " - d_model  :", self.cfg.d_model  )
             print( " - n_heads  :", self.cfg.n_heads  )
             print( " - d_head   :", self.cfg.d_head   )
         else:
@@ -233,26 +260,26 @@
                 return
             self.activations[component][name] = detached(_input)
         return hook
 
     def register_activations( self ):
         # Configure what to hook
         self.attn_pre_out_mode = "hook" if "attn.out_proj" in self.layers[0] else "calc"
-        self.mlp_pre_out_mode  = "hook" if "fc2" in self.layers[0] else "calc"
+        self.mlp_pre_out_mode  = "hook" if "mlp.out_proj" in self.layers[0] else "calc"
 
         # register the forward hook to attention outputs
         for layer_index, layer in enumerate(self.layers):
             # Build normal attention hook
             attn = layer["attn"]
             name = pad_zeros( layer_index ) + "-attention"
             attn.register_forward_hook(self.build_output_hook("attn", name))
 
             # Listen to inputs for FF_out
             if self.mlp_pre_out_mode == "hook":
-                fc2 = layer["fc2"]
+                fc2 = layer["mlp.out_proj"]
                 name = pad_zeros( layer_index ) + "-mlp-pre-out"
                 fc2.register_forward_pre_hook(self.build_input_hook("mlp_pre_out", name))
 
             # Optionally, build pre_out hook if possible
             if self.attn_pre_out_mode == "hook":
                 attn_o = layer["attn.out_proj"]
                 name = pad_zeros( layer_index ) + "-attention-out"
@@ -290,15 +317,15 @@
     def register_masks(self):
         """Register the masks for each layer in the model."""
         if self.mask_fn == "delete":
             return
 
         for layer_index, layer in enumerate(self.layers):
             # Listen to inputs for FF_out
-            fc2 = layer["fc2"]
+            fc2 = layer["mlp.out_proj"]
             self.register_input_mask(fc2, "mlp_pre_out", layer_index)
 
             # Optionally, build pre_out hook if possible
             attn_o = layer["attn.out_proj"]
             self.register_input_mask(attn_o, "attn_pre_out", layer_index)
 
         self.masks["mlp_pre_out"]  = NeuronFunctionList(self.masks["mlp_pre_out"])
@@ -308,26 +335,26 @@
             module: torch.nn.Module,
             component: str,
             layer_index: int
             ):
         if component not in self.post_biases:
             self.post_biases[component] = [None for _ in range(self.cfg.n_layers)]
         if self.post_biases[component][layer_index] is not None:
-            print(f"WARNING: {component} {layer_index} already has a mask!")
+            print(f"WARNING: {component} {layer_index} already has a post bias!")
 
         shape = (self.cfg.d_model,)
         if component == "attn_v":
             shape = (self.cfg.n_heads, self.cfg.d_head)
         if component == "mlp_in":
             shape = (self.cfg.d_mlp,)
 
         post_bias = NeuronPostBias(shape)
         dtype, device = self.dtype, module.weight.device
-        mask = post_bias.to(dtype=dtype, device=device)
-        self.post_biases[component][layer_index] = mask
+        post_bias = post_bias.to(dtype=dtype, device=device)
+        self.post_biases[component][layer_index] = post_bias
 
         # Register the post-hook for biasing
         def post_hook_bias(_module, _input, _output):
             if not self.post_biases_enabled:
                 return _output
             return post_bias(_output)
 
@@ -338,33 +365,53 @@
 
         do_attn_vo_biases = \
             "attn.v_proj" in self.layers[0] and \
             self.layers[0]["attn.v_proj"] is not None
 
         if do_attn_vo_biases:
             for layer_index, layer in enumerate(self.layers):
-                attn_v = layer["attn.v_proj"]
-                self.register_output_bias(attn_v, "attn_v", layer_index)
+                # TODO: fix when cfg.n_key_value_heads != cfg.n_heads
+                # attn_v = layer["attn.v_proj"]
+                # self.register_output_bias(attn_v, "attn_v", layer_index)
                 attn_o = layer["attn.out_proj"]
                 self.register_output_bias(attn_o, "attn_o", layer_index)
 
-            self.post_biases["attn_v"] = NeuronFunctionList(self.post_biases["attn_v"])
+            # self.post_biases["attn_v"] = NeuronFunctionList(self.post_biases["attn_v"])
             self.post_biases["attn_o"] = NeuronFunctionList(self.post_biases["attn_o"])
 
+        if "mlp.out_proj" in self.layers[0]:
+            for layer_index, layer in enumerate(self.layers):
+                mlp_out = layer["mlp.out_proj"]
+                self.register_output_bias(mlp_out, "mlp_out", layer_index)
+
+            self.post_biases["mlp_out"] = NeuronFunctionList(self.post_biases["mlp_out"])
+
+
     def list_masks(self, mask_labels=None):
         if isinstance(mask_labels, str):
-            mask_labels = []
+            mask_labels = [mask_labels]
         if mask_labels is None:
             mask_labels = self.masks.keys()
         masks_list = []
         for label in mask_labels:
             for mask in self.masks[label]:
                 masks_list.append(mask)
         return masks_list
 
+    def list_post_biases(self, post_bias_labels=None):
+        if isinstance(post_bias_labels, str):
+            post_bias_labels = [post_bias_labels]
+        if post_bias_labels is None:
+            post_bias_labels = self.post_biases.keys()
+        post_biases_list = []
+        for label in post_bias_labels:
+            for post_bias in self.post_biases[label]:
+                post_biases_list.append(post_bias)
+        return post_biases_list
+
     def register_inverse_out_proj( self ):
         # Make it possible to get the output right before out_proj
         for layer in self.layers:
             #print(layer["attn.W_O"].shape)
             inv_out_proj = InverseLinear(
                 original_weights=layer["attn.W_O"],
                 original_biases=layer["attn.b_O"],
@@ -500,19 +547,22 @@
             # 0     1      2    3      4        -3     -2   -1
             inpt = residual_stream[0]
             attention_out = residual_stream[1:-2:2] - residual_stream[0:-3:2]
             ff_out = residual_stream[2:-1:2] - residual_stream[1:-2:2]
             output = residual_stream[-1]
             return inpt, attention_out, ff_out, output
 
-        if inputs_embeds is None and input_ids is None and text is None:
-            raise ValueError( "must provide data: inputs_embeds | input_ids | text" )
+        if text is not None and input_ids is None:
+            input_ids = self.get_ids(text, limit=limit)
+
+        if input_ids is not None and inputs_embeds is None:
+            inputs_embeds = self.get_inputs_embeds( input_ids=input_ids, limit=limit )
 
-        if text or (not input_ids is None):
-            inputs_embeds = self.get_inputs_embeds( text, input_ids, limit )
+        if inputs_embeds is None:
+            raise ValueError( "must provide data: inputs_embeds | input_ids | text" )
 
         # run the model
         outputs = self.model( inputs_embeds=inputs_embeds,
                               output_hidden_states=True, **kwargs )
 
         # get the hidden states
         hidden_states = self.out_stack( outputs.hidden_states ).squeeze().detach()
@@ -932,15 +982,15 @@
     def calculate_ff_keys_layer( self,
             ff_in: Tensor,
             layer: int,
             use_activation_function: bool = True,
         ):
         u = self.layers[ layer ]
         _x = u["ln2"]( ff_in )
-        x_in = u["fc1"]( _x )
+        x_in = u["mlp.in_proj"]( _x )
         if not use_activation_function:
             return x_in
 
         act_fn = u["activation_fn"]
         if self.cfg.gated_mlp:
             x_gated = u["fc3"]( _x )
             return act_fn(x_gated) * x_in
@@ -958,17 +1008,17 @@
                     use_activation_function=use_activation_function )
             )
         return self.out_stack( out )
 
     def calculate_ff_out_layer( self, ff_in: Tensor, layer: int):
         u = self.layers[ layer ]
         x = u["ln2"]( ff_in )
-        x = u["fc1"]( x )
+        x = u["mlp.in_proj"]( x )
         x = u["activation_fn"]( x )
-        x = u["fc2"]( x )
+        x = u["mlp.out_proj"]( x )
         return x
 
     def calculate_ff_out( self, ff_in: Tensor, add_residual: bool = False ):
         out = []
         for layer_index, ff_in_layer in enumerate(ff_in):
             ff_out = self.calculate_ff_out_layer( ff_in_layer, layer_index )
             if add_residual:
```

### Comparing `taker-0.9.8/src/taker/model_maps.py` & `taker-0.9.9/src/taker/model_maps.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     n_ctx: int
     eps: float
     d_vocab: int
     act_fn: str
     normalization_type: str
     architecture: str
     tokenizer_name: str
+    n_key_value_heads: int = None
     is_low_precision: bool = False
     use_attn_scale: bool = None
     use_local_attn: bool = None
     scale_attn_by_inverse_layer_idx: bool = None
     parallel_attn_mlp: bool = False
     positional_embedding_type: str = "standard"
     rotary_dim: Optional[int] = None
@@ -44,99 +45,51 @@
     # Load HuggingFace model config
     #if 'llama' in official_model_name and 'open_llama' not in official_model_name:
     #    architecture = "LLaMAForCausalLM"
     #else:
     hf_config = AutoConfig.from_pretrained(official_model_name)
     architecture = hf_config.architectures[0]
 
-    if 'llama-7b' in official_model_name:
+    if architecture.lower() == "LlamaForCausalLM".lower():
         cfg_dict = {
-            "d_model": 4096,
-            "d_head": 4096 // 32,
-            "n_heads": 32,
-            "d_mlp": 11008,
-            "n_layers": 32,
-            "n_ctx": 2048,
-            "eps": 1e-6,
-            "d_vocab": 32000,
-            "act_fn": "silu",
-            "normalization_type": "RMS",
-            "positional_embedding_type": "rotary",
-            "rotary_dim": 4096 // 32,
-            "final_rms": True,
-            "gated_mlp": True,
-        }
-    elif 'llama-13b' in official_model_name:
-        cfg_dict = {
-            "d_model": 5120,
-            "d_head": 5120 // 40,
-            "n_heads": 40,
-            "d_mlp": 13824,
-            "n_layers": 40,
-            "n_ctx": 2048,
-            "eps": 1e-6,
-            "d_vocab": 32000,
-            "act_fn": "silu",
-            "normalization_type": "RMS",
-            "positional_embedding_type": "rotary",
-            "rotary_dim": 5120 // 40,
-            "final_rms": True,
-            "gated_mlp": True,
-        }
-    elif 'llama-30b' in official_model_name:
-        cfg_dict = {
-            "d_model": 6656,
-            "d_head": 6656 // 52,
-            "n_heads": 52,
-            "d_mlp": 17920,
-            "n_layers": 60,
-            "n_ctx": 2048,
-            "eps": 1e-6,
-            "d_vocab": 32000,
-            "act_fn": "silu",
-            "normalization_type": "RMS",
-            "positional_embedding_type": "rotary",
-            "rotary_dim": 6656 // 52,
-            "final_rms": True,
-            "gated_mlp": True,
-        }
-    elif 'llama-65b' in official_model_name:
-        cfg_dict = {
-            "d_model": 8192,
-            "d_head": 8192 // 64,
-            "n_heads": 64,
-            "d_mlp": 22016,
-            "n_layers": 80,
-            "n_ctx": 2048,
-            "eps": 1e-6,
-            "d_vocab": 32000,
-            "act_fn": "silu",
+            "d_model": hf_config.hidden_size,
+            "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
+            "n_heads": hf_config.num_attention_heads,
+            "d_mlp": hf_config.intermediate_size,
+            "n_layers": hf_config.num_hidden_layers,
+            "n_ctx": hf_config.max_position_embeddings,
+            "eps": hf_config.rms_norm_eps,
+            "d_vocab": hf_config.vocab_size,
+            "act_fn": hf_config.hidden_act,
             "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
-            "rotary_dim": 8192 // 64,
+            "rotary_dim": hf_config.hidden_size // hf_config.num_attention_heads, #?
             "final_rms": True,
             "gated_mlp": True,
         }
-    elif architecture.lower() == "LlamaForCausalLM".lower():
+    elif architecture == "MistralForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.intermediate_size,
             "n_layers": hf_config.num_hidden_layers,
             "n_ctx": hf_config.max_position_embeddings,
             "eps": hf_config.rms_norm_eps,
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.hidden_act,
             "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
+            "eps": hf_config.rms_norm_eps,
+            "n_key_value_heads": hf_config.num_key_value_heads,
             "rotary_dim": hf_config.hidden_size // hf_config.num_attention_heads, #?
-            "final_rms": True,
+            "use_local_attn": True,
             "gated_mlp": True,
         }
+
     elif architecture == "GPTNeoForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_heads,
             "n_heads": hf_config.num_heads,
             "d_mlp": hf_config.hidden_size * 4,
             "n_layers": hf_config.num_layers,
@@ -200,14 +153,15 @@
             "parallel_attn_mlp": True,
             "positional_embedding_type": "rotary",
             "rotary_dim": hf_config.rotary_dim,
             "normalization_type": "LN",
         }
     elif architecture == "GPTNeoXForCausalLM":
         cfg_dict = {
+            "model_type": "causal",
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.intermediate_size,
             "n_layers": hf_config.num_hidden_layers,
             "n_ctx": hf_config.max_position_embeddings,
             "eps": hf_config.layer_norm_eps,
@@ -387,21 +341,21 @@
         "attn.W_O_inv"  : "self_attn.inv_out_proj.weight",
         "attn.b_O_inv"  : "self_attn.inv_out_proj.inverse_bias",
 
         "ln2"           : "final_layer_norm",
         "ln2.w"         : "final_layer_norm.weight",
         "ln2.b"         : "final_layer_norm.bias",
 
-        "fc1"           : "fc1",
+        "mlp.in_proj"   : "fc1",
         "mlp.W_in"      : "fc1.weight",
         "mlp.b_in"      : "fc1.bias",
 
         "activation_fn" : "activation_fn",
 
-        "fc2"           : "fc2",
+        "mlp.out_proj"  : "fc2",
         "mlp.W_out"     : "fc2.weight",
         "mlp.b_out"     : "fc2.bias",
     }
     return opt_layer_map
 
 # LLaMa Models
 ##############
@@ -417,15 +371,15 @@
     "ln_final.w"      : "model.norm.weight",
     "unembed.W_U"     : "model.lm_head.weight.T",
     "unembed.b_U"     : None,
 }
 
 def build_llama_layer_map(cfg: ConfigClass):
     attn_proj_map = {"q": "q_proj", "k": "k_proj", "v": "v_proj", "o": "o_proj"}
-    mlp_proj_map = {"fc1": "up_proj", "fc2": "down_proj", "fc3": "gate_proj"}
+    mlp_proj_map = {"mlp.in_proj": "up_proj", "mlp.out_proj": "down_proj", "mlp.gate_proj": "gate_proj"}
 
     def llama_qkv_weight(layer, key: str, inpt: Optional[Any]=None):
         # Prepare shape changing
         their_shape = "(n_heads d_head) d_model"
         my_shape    = "n_heads d_head d_model"
         sizes = generate_sizes_dict(my_shape, cfg)
 
@@ -485,29 +439,129 @@
         "attn.W_O_inv"  : "self_attn.inv_out_proj.weight",
         "attn.b_O_inv"  : "self_attn.inv_out_proj.bias",
 
         "ln2"           : "post_attention_layernorm",
         "ln2.w"         : "post_attention_layernorm.weight",
         "ln2.b"         : None,
 
-        "fc1"           : "mlp.up_proj",
-        "fc3"           : "mlp.gate_proj",
+        "mlp.in_proj"   : "mlp.up_proj",
+        "mlp.gate_proj" : "mlp.gate_proj",
         "mlp.W_in"      : "mlp.up_proj.weight",
         "mlp.W_gate"    : "mlp.gate_proj.weight",
-        "mlp.b_in"      : lambda layer, _inpt=None: llama_mlp_bias(layer, "fc1", _inpt),
-        "mlp.b_gate"    : lambda layer, _inpt=None: llama_mlp_bias(layer, "fc3", _inpt),
+        "mlp.b_in"      : lambda layer, _inpt=None: llama_mlp_bias(layer, "mlp.in_proj", _inpt),
+        "mlp.b_gate"    : lambda layer, _inpt=None: llama_mlp_bias(layer, "mlp.out_proj", _inpt),
 
         "activation_fn" : "mlp.act_fn",
 
-        "fc2"           : "mlp.down_proj",
-        "mlp.W_out"     : "fc2.weight",
-        "mlp.b_out"     : lambda layer, _inpt=None: llama_mlp_bias(layer, "fc2", _inpt),
+        "mlp.out_proj"  : "mlp.down_proj",
+        "mlp.W_out"     : "mlp.down_proj.weight",
+        "mlp.b_out"     : lambda layer, _inpt=None: llama_mlp_bias(layer, "mlp.gate_proj", _inpt),
     }
     return llama_layer_map
 
+# Mistral Model
+###############
+
+mistral_model_map = {
+    "model"           : "model",
+    "layers"          : "model.layers",
+    "embed"           : "model.embed_tokens",
+    "embed.W_E"       : "model.embed.weights",
+    "pos_embed"       : "model.embed_positions",
+    "pos_embed.W"     : "model.embed_positions.weight",
+    "ln_final"        : "model.norm",
+    "ln_final.w"      : "model.norm.weight",
+    "unembed.W_U"     : "model.lm_head.weight.T",
+    "unembed.b_U"     : None,
+}
+
+def build_mistral_layer_map(cfg: ConfigClass):
+    attn_proj_map = {"q": "q_proj", "k": "k_proj", "v": "v_proj", "o": "o_proj"}
+    mlp_proj_map = {"mlp.in_proj": "up_proj", "mlp.out_proj": "down_proj", "mlp.gate_proj": "gate_proj"}
+
+    def mistral_qkv_weight(layer, key: str, inpt: Optional[Any]=None):
+        # Prepare shape changing
+        if key in ['k', 'v']:  # Adjust for Mistral's unique n_key_value_heads
+            their_shape = "(n_key_value_heads d_head) d_model"
+        else:
+            their_shape = "(n_heads d_head) d_model"
+        my_shape = "n_heads d_head d_model"
+        sizes = generate_sizes_dict(my_shape, cfg)
+
+        # Get attn proj module
+        attn = layer.self_attn
+        attn_proj = get_attrs(attn, attn_proj_map[key])
+
+        # Get mode
+        if inpt is None:
+            W = attn_proj.weight
+            W = einops.rearrange(W, f"{their_shape} -> {my_shape}", **sizes)
+            return W
+
+        # Set mode
+        W = einops.rearrange(inpt, f"{my_shape} -> {their_shape}", **sizes)
+        update_param(attn_proj, "weight", W)
+
+    def mistral_attn_bias(layer, key: str, _inpt: Optional[Any]=None):
+        # Create fake bias with zeros because is easier to handle
+        their_shape = "(n_heads d_head)"
+        my_shape = "n_heads d_head"
+        sizes = generate_sizes_dict(my_shape, cfg)
+
+        attn = layer.self_attn
+        _proj = get_attrs(attn, attn_proj_map[key]).weight
+        b = torch.zeros(_proj.shape[:-1], dtype=_proj.dtype, device=_proj.device)
+        if key == "o":
+            return b
+        return einops.rearrange(b, f"{their_shape} -> {my_shape}", **sizes)
+
+    def mistral_mlp_bias(layer, key: str, _inpt: Optional[Any]=None):
+        mlp = layer.mlp
+        _proj = get_attrs(mlp, mlp_proj_map[key]).weight
+        b = torch.zeros(_proj.shape[:-1], dtype=_proj.dtype, device=_proj.device)
+        return b
+
+    mistral_layer_map = {
+        "ln1"           : "input_layernorm",
+        "ln1.w"         : "input_layernorm.weight",
+        "ln1.b"         : None,
+
+        "attn"          : "self_attn",
+        "attn.q_proj"   : "self_attn.q_proj",
+        "attn.k_proj"   : "self_attn.k_proj",
+        "attn.v_proj"   : "self_attn.v_proj",
+
+        **generate_attn_qkv_functions(mistral_qkv_weight, mistral_attn_bias),
+
+        "attn.inv_out_proj" : "self_attn.inv_out_proj",
+        "attn.out_proj" : "self_attn.o_proj",
+        "attn.W_O"      : "self_attn.o_proj.weight",
+        "attn.b_O"      : lambda layer, _inpt=None: mistral_attn_bias(layer, "o", _inpt),
+
+        "ln2"           : "post_attention_layernorm",
+        "ln2.w"         : "post_attention_layernorm.weight",
+        "ln2.b"         : None,
+
+        "mlp.in_proj"   : "mlp.up_proj",
+        "mlp.gate_proj" : "mlp.gate_proj",
+        "mlp.W_in"      : "mlp.up_proj.weight",
+        "mlp.W_gate"    : "mlp.gate_proj.weight",
+        "mlp.b_in"      : lambda layer, _inpt=None: mistral_mlp_bias(layer, "mlp.in_proj", _inpt),
+        "mlp.b_gate"    : lambda layer, _inpt=None: mistral_mlp_bias(layer, "mlp.out_proj", _inpt),
+
+        "activation_fn" : "mlp.act_fn",
+
+        "mlp.out_proj"  : "mlp.down_proj",
+        "mlp.W_out"     : "mlp.down_proj.weight",
+        "mlp.b_out"     : lambda layer, _inpt=None: mistral_mlp_bias(layer, "mlp.gate_proj", _inpt),
+
+    }
+
+    return mistral_layer_map
+
 # GPT NEO X and Pythia Models
 #############################
 
 gpt_neox_model_map = {
     "model"           : "base_model",
     "layers"          : "base_model.layers",
     "embed"           : "base_model.embed_in",
@@ -585,16 +639,16 @@
         "attn.W_O_inv"      : "attention.inv_out_proj.weight",
         "attn.b_O_inv"      : "attention.inv_out_proj.inverse_bias",
 
         "ln2"       : "post_attention_layernorm",
         "ln2.w"     : "post_attention_layernorm.weight",
         "ln2.b"     : "post_attention_layernorm.bias",
 
-        "fc1"       : "mlp.dense_h_to_4h",
-        "fc2"       : "mlp.dense_4h_to_h",
+        "mlp.in_proj" : "mlp.dense_h_to_4h",
+        "mlp.out_proj": "mlp.dense_4h_to_h",
         "mlp.W_in"  : "mlp.dense_h_to_4h.weight",
         "mlp.W_out" : "mlp.dense_4h_to_h.weight",
         "mlp.b_in"  : "mlp.dense_h_to_4h.bias",
         "mlp.b_out" : "mlp.dense_4h_to_h.bias",
         "activation_fn" : "mlp.act",
     }
     return gpt_neox_layer_map
@@ -690,16 +744,16 @@
         "attn.b_O"      : "attn.c_proj.bias",
         "attn.inv_out_proj" : "attn.inv_out_proj",
         "attn.W_O_inv"      : "attn.inv_out_proj.weight",
         "attn.b_O_inv"      : "attn.inv_out_proj.inverse_bias",
         "ln2"       : "ln_2",
         "ln2.w"     : "ln_2.weight",
         "ln2.b"     : "ln_2.bias",
-        "fc1"       : "mlp.c_fc",
-        "fc2"       : "mlp.c_proj",
+        "mlp.in_proj" : "mlp.c_fc",
+        "mlp.out_proj": "mlp.c_proj",
         "mlp.W_in"  : lambda layer, inpt=None: gpt2_mlp_in_weight(layer, inpt),
         "mlp.W_out" : lambda layer, inpt=None: gpt2_mlp_out_weight(layer, inpt),
         "mlp.b_in"  : "mlp.c_fc.bias",
         "mlp.b_out" : "mlp.c_proj.bias",
         "activation_fn" : "mlp.act",
     }
     return gpt2_layer_map
@@ -794,21 +848,21 @@
         "attn.W_O_inv"  : "attention.inv_out_proj.weight",
         "attn.b_O_inv"  : "attention.inv_out_proj.inverse_bias",
 
         "ln2"           : "output.LayerNorm",
         "ln2.w"         : "output.LayerNorm.weight",
         "ln2.b"         : "output.LayerNorm.bias",
 
-        "fc1"           : "intermediate.dense",
+        "mlp.in_proj"   : "intermediate.dense",
         "mlp.W_in"      : "intermediate.dense.weight",
         "mlp.b_in"      : "intermediate.dense.bias",
 
         "activation_fn" : "intermediate.intermediate_act_fn",
 
-        "fc2"           : "output.dense",
+        "mlp.out_proj"  : "output.dense",
         "mlp.W_out"     : "output.dense.weight",
         "mlp.b_out"     : "output.dense.bias",
     }
     return opt_layer_map
 
 #####################################################################################
 # VISION TRANSFORMERS (eg: ViT)
@@ -900,21 +954,21 @@
         "attn.W_O_inv"  : "attention.inv_out_proj.weight",
         "attn.b_O_inv"  : "attention.inv_out_proj.inverse_bias",
 
         "ln2"           : "layernorm_after",
         "ln2.w"         : "layernorm_after.weight",
         "ln2.b"         : "layernorm_after.bias",
 
-        "fc1"           : "intermediate.dense",
+        "mlp.in_proj"   : "intermediate.dense",
         "mlp.W_in"      : "intermediate.dense.weight",
         "mlp.b_in"      : "intermediate.dense.bias",
 
         "activation_fn" : "intermediate.intermediate_act_fn",
 
-        "fc2"           : "output.dense",
+        "mlp.out_proj"  : "output.dense",
         "mlp.W_out"     : "output.dense.weight",
         "mlp.b_out"     : "output.dense.bias",
     }
 
     return vit_layer_map
 
 
@@ -934,14 +988,16 @@
 
 def get_model_key_map(config: ConfigClass):
     architecture = config.architecture
     if architecture == "OPTForCausalLM":
         return opt_model_map
     if architecture in ["LLaMAForCausalLM", "LlamaForCausalLM"]:
         return llama_model_map
+    if architecture == "MistralForCausalLM":
+        return mistral_model_map
     if architecture == "GPTNeoXForCausalLM":
         return gpt_neox_model_map
     if architecture == "GPT2LMHeadModel":
         return gpt2_model_map
     if architecture == "RobertaForMaskedLM":
         return roberta_model_map
     if architecture == "ViTForImageClassification":
@@ -952,14 +1008,16 @@
 def get_layer_key_map(config: ConfigClass):
     architecture = config.architecture
 
     if architecture == "OPTForCausalLM":
         return build_opt_layer_map(config)
     if architecture in ["LLaMAForCausalLM", "LlamaForCausalLM"]:
         return build_llama_layer_map(config)
+    if architecture == "MistralForCausalLM":
+        return build_mistral_layer_map(config)
     if architecture == "GPTNeoXForCausalLM":
         return build_gpt_neox_layer_map(config)
     if architecture == "GPT2LMHeadModel":
         return build_gpt2_layer_map(config)
     if architecture == "RobertaForMaskedLM":
         return build_roberta_layer_map(config)
     if architecture == "ViTForImageClassification":
```

### Comparing `taker-0.9.8/src/taker/model_repos.py` & `taker-0.9.9/src/taker/model_repos.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/nn.py` & `taker-0.9.9/src/taker/nn.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,18 @@
         self.param = torch.nn.Parameter(_vec)
 
     def get_bias(self, x):
         shape = x.shape
         bias  = self.param
         if self.shape == shape:
             return bias
-        bias = bias.view(shape[-1])
+        try:
+            bias = bias.view(shape[-1]) # normal shape
+        except:
+            bias = bias.view(-1, shape[-1]) # multi head attention shape
         return bias
 
     def forward(self, x):
         return x + self.get_bias(x)
 
 ######################################################################################
 # Define MLP Deletion functions
```

### Comparing `taker-0.9.8/src/taker/parser.py` & `taker-0.9.9/src/taker/parser.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/prune.py` & `taker-0.9.9/src/taker/prune.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/scoring.py` & `taker-0.9.9/src/taker/scoring.py`

 * *Files identical despite different names*

### Comparing `taker-0.9.8/src/taker/texts.py` & `taker-0.9.9/src/taker/texts.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
             dataset_image_label_key = "fine_label",
             dataset_filter=DatasetFilters.filter_rocket,
         ),
         EvalConfig("cifar100-rocketless",
             dataset_repo = "cifar100",
             dataset_type = "image-classification",
             dataset_split = "test",
+            streaming = False,
             is_train_mode = False,
             num_texts_to_skip = 1,
             dataset_image_key = "img",
             dataset_image_label_key = "fine_label",
             dataset_filter=DatasetFilters.filter_rocketless,
         ),
         EvalConfig("cifar100-rocket-mia",
@@ -277,14 +278,26 @@
             dataset_type = "image-classification",
             dataset_split = ["train", "test"],
             is_train_mode = True,
             dataset_image_key = "img",
             dataset_image_label_key = "coarse_label",
             dataset_filter=DatasetFilters.filter_veh2,
         ),
+        EvalConfig("bio",
+            dataset_repo           = "camel-ai/biology",
+            dataset_text_key       = "message_2",
+            dataset_has_test_split = False,
+        ),
+        EvalConfig("emotion",
+            dataset_repo = "dair-ai/emotion",
+            dataset_type = "text-classification",
+            dataset_text_key = "text",
+            dataset_text_label_key = "label",
+            dataset_has_test_split = True,
+        )
     ]
 
     # Convert into searchable dict
     labeled_eval_configs = dict([(c.dataset_name, c) for c in eval_configs])
 
     # Search the dict for config
     if dataset_name in labeled_eval_configs:
@@ -325,24 +338,24 @@
 
     else:
         _dataset = _dataset[split]
 
     # Apply filter if relevant
     if eval_config.dataset_filter is not None:
         _dataset = eval_config.dataset_filter(_dataset)
-
     # Skip n texts if relevant
     if eval_config.num_texts_to_skip >= 1:
         print(f"skipping {eval_config.num_texts_to_skip} texts in {eval_config.dataset_name}")
 
         # Skip only works for DatasetIterable. Kinda annoying ngl
         if hasattr(_dataset, "skip"):
             _dataset = _dataset.skip(eval_config.num_texts_to_skip) # Conservative skip limit
         else:
-            _dataset = _dataset[eval_config.num_texts_to_skip:]
+            indices = list(range(eval_config.num_texts_to_skip, len(_dataset)))
+            _dataset = _dataset.select(indices)
 
     # Skip tokens is no split
     if split == "train" and not eval_config.is_train_mode:
         skip_n = int(eval_config.num_tokens_to_skip//100)
         print( "Warning: 'pile_deduped' has no 'test' split.",
               f"Using 'train' split and skipping {skip_n} texts instead.")
         _dataset = _dataset.skip(skip_n) # Conservative skip limit
```

### Comparing `taker-0.9.8/PKG-INFO` & `taker-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: taker
-Version: 0.9.8
+Version: 0.9.9
 Summary: Tools for Transformer Activations Knowledge ExtRaction
 Home-page: https://github.com/nickypro/taker
 Author: Nicky Pochinkov
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: accelerate (>=0.21.0,<0.22.0)
 Requires-Dist: bitsandbytes (>=0.40.2,<0.41.0)
 Requires-Dist: celery (>=5.3.1,<6.0.0)
 Requires-Dist: datasets (>=2.9.0,<3.0.0)
 Requires-Dist: dict-deep (>=4.1.2,<5.0.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
@@ -25,17 +25,17 @@
 Requires-Dist: numexpr (>=2.7.0,<3.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: sentencepiece (>=0.1.99,<0.2.0)
 Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
 Requires-Dist: tensorboardx (>=2.5.1,<3.0.0)
-Requires-Dist: tokenizers (>=0.13.3,<0.14.0)
+Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: transformers (>=4.30.0,<5.0.0)
+Requires-Dist: transformers (>=4.33.0,<5.0.0)
 Requires-Dist: wandb (>=0.13.9,<0.14.0)
 Requires-Dist: welford-torch (>=0.2.1,<0.3.0)
 Requires-Dist: zstandard (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/nickypro/taker
 Description-Content-Type: text/markdown
 
 ![Tools for Lanugage Model Activations](https://github.com/nickypro/taker)
```

