# Comparing `tmp/tipo-kgen-0.0.5.tar.gz` & `tmp/tipo-kgen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipo-kgen-0.0.5.tar", last modified: Thu Apr 18 16:03:44 2024, max compression
+gzip compressed data, was "tipo-kgen-0.0.6.tar", last modified: Fri Apr 19 03:20:20 2024, max compression
```

## Comparing `tipo-kgen-0.0.5.tar` & `tipo-kgen-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 16:03:44.927894 tipo-kgen-0.0.5/
--rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      409 2024-04-18 16:03:44.927390 tipo-kgen-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 16:03:44.910800 tipo-kgen-0.0.5/kgen/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.5/kgen/__init__.py
--rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.5/kgen/formatter.py
--rw-rw-rw-   0        0        0     4328 2024-04-18 15:58:06.000000 tipo-kgen-0.0.5/kgen/generate.py
--rw-rw-rw-   0        0        0     1153 2024-04-17 17:47:41.000000 tipo-kgen-0.0.5/kgen/logging.py
--rw-rw-rw-   0        0        0     1072 2024-04-18 15:58:40.000000 tipo-kgen-0.0.5/kgen/metainfo.py
--rw-rw-rw-   0        0        0     2469 2024-04-18 16:03:10.000000 tipo-kgen-0.0.5/kgen/models.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:03:44.918768 tipo-kgen-0.0.5/kgen/tag-list/
--rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.5/kgen/tag-list/__init__.py
--rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.5/kgen/tag-list/artist.txt
--rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.5/kgen/tag-list/characters.txt
--rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.5/kgen/tag-list/copyrights.txt
--rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.5/kgen/tag-list/meta.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 16:03:44.927894 tipo-kgen-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      603 2024-04-18 16:03:36.000000 tipo-kgen-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 16:03:44.927390 tipo-kgen-0.0.5/tipo_kgen.egg-info/
--rw-rw-rw-   0        0        0      409 2024-04-18 16:03:44.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2024-04-18 16:03:44.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 16:03:44.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2024-04-18 16:03:44.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-18 16:03:44.000000 tipo-kgen-0.0.5/tipo_kgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 03:20:20.657808 tipo-kgen-0.0.6/
+-rw-rw-rw-   0        0        0    11540 2024-03-23 06:06:25.000000 tipo-kgen-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      409 2024-04-19 03:20:20.656803 tipo-kgen-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2352 2024-04-18 03:16:31.000000 tipo-kgen-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 03:20:20.635401 tipo-kgen-0.0.6/kgen/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:02:12.000000 tipo-kgen-0.0.6/kgen/__init__.py
+-rw-rw-rw-   0        0        0     4111 2024-04-17 18:14:56.000000 tipo-kgen-0.0.6/kgen/formatter.py
+-rw-rw-rw-   0        0        0     4254 2024-04-19 03:08:22.000000 tipo-kgen-0.0.6/kgen/generate.py
+-rw-rw-rw-   0        0        0     1153 2024-04-19 03:08:01.000000 tipo-kgen-0.0.6/kgen/logging.py
+-rw-rw-rw-   0        0        0     1072 2024-04-18 15:58:40.000000 tipo-kgen-0.0.6/kgen/metainfo.py
+-rw-rw-rw-   0        0        0     2937 2024-04-19 03:14:34.000000 tipo-kgen-0.0.6/kgen/models.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:20:20.641910 tipo-kgen-0.0.6/kgen/tag-list/
+-rw-rw-rw-   0        0        0        0 2024-04-17 16:47:26.000000 tipo-kgen-0.0.6/kgen/tag-list/__init__.py
+-rw-rw-rw-   0        0        0  4459440 2024-04-17 15:02:11.000000 tipo-kgen-0.0.6/kgen/tag-list/artist.txt
+-rw-rw-rw-   0        0        0  4079093 2024-04-17 15:02:11.000000 tipo-kgen-0.0.6/kgen/tag-list/characters.txt
+-rw-rw-rw-   0        0        0   823337 2024-04-17 15:02:11.000000 tipo-kgen-0.0.6/kgen/tag-list/copyrights.txt
+-rw-rw-rw-   0        0        0     8830 2024-04-17 15:02:11.000000 tipo-kgen-0.0.6/kgen/tag-list/meta.txt
+-rw-rw-rw-   0        0        0      204 2024-04-19 03:04:45.000000 tipo-kgen-0.0.6/kgen/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-19 03:20:20.657808 tipo-kgen-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      603 2024-04-19 03:20:13.000000 tipo-kgen-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 03:20:20.656803 tipo-kgen-0.0.6/tipo_kgen.egg-info/
+-rw-rw-rw-   0        0        0      409 2024-04-19 03:20:20.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-19 03:20:20.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 03:20:20.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 17:29:04.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2024-04-19 03:20:20.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-19 03:20:20.000000 tipo-kgen-0.0.6/tipo_kgen.egg-info/top_level.txt
```

### Comparing `tipo-kgen-0.0.5/LICENSE` & `tipo-kgen-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/README.md` & `tipo-kgen-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/formatter.py` & `tipo-kgen-0.0.6/kgen/formatter.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/generate.py` & `tipo-kgen-0.0.6/kgen/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import regex as re
-import random
 from contextlib import nullcontext
 from random import shuffle
 
 import torch
 
 try:
     from llama_cpp import Llama
 except ImportError:
 
     class Llama:
         pass
 
-
 from transformers import (
     GenerationConfig,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     set_seed,
 )
 
+from .utils import same_order_deduplicate
+
 
 def generate(
     model: PreTrainedModel | Llama,
     tokenizer: PreTrainedTokenizerBase,
     prompt="",
     temperature=0.5,
     top_p=0.95,
@@ -40,15 +40,14 @@
             temperature=temperature,
             top_p=top_p,
             top_k=top_k,
             max_tokens=max_new_tokens,
             repeat_penalty=repetition_penalty or 1,
             seed=kwargs.get("seed", None),
         )
-        # print(prompt, "===", result["choices"][0]["text"])
         return prompt + result["choices"][0]["text"]
     if "seed" in kwargs:
         set_seed(kwargs["seed"])
 
     torch.cuda.empty_cache()
     inputs = tokenizer(prompt, return_tensors="pt")
     input_ids = inputs["input_ids"].to(next(model.parameters()).device)
@@ -122,23 +121,20 @@
             eos_token_id=getattr(tokenizer, "eos_token_id", None),
             seed=seed + iter_count,
         )
         iter_count += 1
         llm_gen = llm_gen.replace("</s>", "").replace("<s>", "")
         orig_prompt = llm_gen.split("<|input_end|>")[0]
         extra = llm_gen.split("<|input_end|>")[-1].strip().strip(",")
-        extra_tokens = sorted(
-            set(
-                [
-                    tok.strip()
-                    for tok in extra.split(",")
-                    if not black_list_match(tok.strip(), black_list)
-                ]
-            )
-        )
+        extra_tokens = [
+            tok.strip()
+            for tok in extra.split(",")
+            if not black_list_match(tok.strip(), black_list)
+        ]
+        extra_tokens = same_order_deduplicate(extra_tokens)
         llm_gen = llm_gen.replace(extra, ", ".join(extra_tokens))
 
         yield llm_gen, extra_tokens, iter_count
 
         if set(extra_tokens) == prev_output:
             same_output_count += 1
             retry += 1
```

### Comparing `tipo-kgen-0.0.5/kgen/logging.py` & `tipo-kgen-0.0.6/kgen/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         levelname = colored_record.levelname
         seq = self.COLORS.get(levelname, self.COLORS["RESET"])
         colored_record.levelname = f"{seq}{levelname}{self.COLORS['RESET']}"
         return super().format(colored_record)
 
 
 # Create a new logger
-logger = logging.getLogger("TOPI-KGen")
+logger = logging.getLogger("TIPO-KGen")
 logger.propagate = False
 
 # Add handler if we don't have one.
 if not logger.handlers:
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(
         ColoredFormatter(
```

### Comparing `tipo-kgen-0.0.5/kgen/metainfo.py` & `tipo-kgen-0.0.6/kgen/metainfo.py`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/models.py` & `tipo-kgen-0.0.6/kgen/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -54,28 +54,36 @@
         str(model_dir / file)
         for file in os.listdir(model_dir)
         if file.endswith(".gguf")
     ]
     return files
 
 
-def load_model(model_name=model_list[0], gguf=False):
+def load_model(model_name=model_list[0], gguf=False, device="cpu"):
     global text_model, tokenizer
     if gguf:
         try:
             assert Llama is not None
             model_name = os.path.basename(model_name)
             text_model = Llama(
                 str(model_dir / model_name),
                 n_ctx=384,
-                n_gpu_layers=100,
+                n_gpu_layers=0 if device == "cpu" else 1000,
                 verbose=False,
             )
             tokenizer = None
             logger.info(f"Llama-cpp-python/gguf model {model_name} loaded")
+            if device=="cuda":
+                logger.warning(
+                    "llama.cpp have reproducibility issue on cuda "
+                    "(https://github.com/ggerganov/llama.cpp/pull/1346) "
+                    "It is suggested to use cpu or "
+                    "compile llama-cpp-python by yourself "
+                    "and set GGML_CUDA_MAX_STREAMS in the file ggml-cuda.cu to 1."
+                )
             return
         except Exception as e:
             logger.warning(f"Llama-cpp-python/gguf model {model_name} load failed")
             model_name = model_list[0]
     logger.info(f"Using transformers model {model_name}")
     text_model = LlamaForCausalLM.from_pretrained(model_name).eval().half()
     tokenizer = LlamaTokenizer.from_pretrained(model_name)
```

### Comparing `tipo-kgen-0.0.5/kgen/tag-list/artist.txt` & `tipo-kgen-0.0.6/kgen/tag-list/artist.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/tag-list/characters.txt` & `tipo-kgen-0.0.6/kgen/tag-list/characters.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/tag-list/copyrights.txt` & `tipo-kgen-0.0.6/kgen/tag-list/copyrights.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/kgen/tag-list/meta.txt` & `tipo-kgen-0.0.6/kgen/tag-list/meta.txt`

 * *Files identical despite different names*

### Comparing `tipo-kgen-0.0.5/setup.py` & `tipo-kgen-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="tipo-kgen",
     packages=find_packages(),
-    version="0.0.5",
+    version="0.0.6",
     license="Apache 2.0",
     url="https://github.com/KohakuBlueleaf/KGen",
     description=(
         "TIPO: Text to Image genration through "
         "text Presampling with LLMs for Optimal prompting"
     ),
     author="Shih-Ying Yeh(KohakuBlueLeaf)",
```

