# Comparing `tmp/wonder-diffusion-sdk-0.0.4.dev0.tar.gz` & `tmp/wonder-diffusion-sdk-0.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wonder-diffusion-sdk-0.0.4.dev0.tar", last modified: Wed Apr 17 12:21:27 2024, max compression
+gzip compressed data, was "wonder-diffusion-sdk-0.0.4.dev1.tar", last modified: Fri Apr 19 07:13:35 2024, max compression
```

## Comparing `wonder-diffusion-sdk-0.0.4.dev0.tar` & `wonder-diffusion-sdk-0.0.4.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.921681 wonder-diffusion-sdk-0.0.4.dev0/
--rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.4.dev0/LICENCE
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-17 12:21:27.921507 wonder-diffusion-sdk-0.0.4.dev0/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-17 12:21:27.921743 wonder-diffusion-sdk-0.0.4.dev0/setup.cfg
--rw-r--r--   0 basri      (501) staff       (20)      319 2024-04-17 12:21:17.000000 wonder-diffusion-sdk-0.0.4.dev0/setup.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.917051 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/
--rw-r--r--   0 basri      (501) staff       (20)    10544 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/__init__.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.918971 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/
--rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/deepcache.py
--rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/dotdict.py
--rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/lightning.py
--rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/logger.py
--rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/safety_checker.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.920345 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/
--rw-r--r--   0 basri      (501) staff       (20)      183 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/globals.py
--rw-r--r--   0 basri      (501) staff       (20)      981 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/lora_config.py
--rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/model_config.py
--rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/sdk_config.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.921275 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/
--rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/__init__.py
--rw-r--r--   0 basri      (501) staff       (20)      465 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/pipeline_type.py
--rw-r--r--   0 basri      (501) staff       (20)     2526 2024-04-03 11:08:09.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/pipelines.py
--rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/scheduler_type.py
--rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/schedulers.py
-drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-17 12:21:27.917949 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/
--rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-17 12:21:27.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/PKG-INFO
--rw-r--r--   0 basri      (501) staff       (20)      954 2024-04-17 12:21:27.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-17 12:21:27.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-17 12:21:27.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/requires.txt
--rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-17 12:21:27.000000 wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.760731 wonder-diffusion-sdk-0.0.4.dev1/
+-rw-r--r--   0 basri      (501) staff       (20)     1080 2024-01-31 06:15:26.000000 wonder-diffusion-sdk-0.0.4.dev1/LICENCE
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-19 07:13:35.760555 wonder-diffusion-sdk-0.0.4.dev1/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)       38 2024-04-19 07:13:35.760889 wonder-diffusion-sdk-0.0.4.dev1/setup.cfg
+-rw-r--r--   0 basri      (501) staff       (20)      319 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/setup.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.754094 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/
+-rw-r--r--   0 basri      (501) staff       (20)    10595 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/__init__.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.756757 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/
+-rw-r--r--   0 basri      (501) staff       (20)      199 2024-03-22 14:04:45.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      402 2024-03-22 14:04:23.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/deepcache.py
+-rw-r--r--   0 basri      (501) staff       (20)      117 2024-02-28 08:41:39.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/dotdict.py
+-rw-r--r--   0 basri      (501) staff       (20)      914 2024-04-17 08:38:18.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/lightning.py
+-rw-r--r--   0 basri      (501) staff       (20)     1137 2024-03-11 09:11:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/logger.py
+-rw-r--r--   0 basri      (501) staff       (20)     3207 2024-02-27 13:23:11.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/safety_checker.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.758331 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/
+-rw-r--r--   0 basri      (501) staff       (20)      183 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)       70 2024-03-20 09:12:50.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/globals.py
+-rw-r--r--   0 basri      (501) staff       (20)      996 2024-04-19 07:12:53.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/lora_config.py
+-rw-r--r--   0 basri      (501) staff       (20)     1503 2024-03-22 14:14:11.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/model_config.py
+-rw-r--r--   0 basri      (501) staff       (20)      197 2024-03-22 14:06:09.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/sdk_config.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.759969 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/
+-rw-r--r--   0 basri      (501) staff       (20)      167 2024-03-11 10:04:17.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/__init__.py
+-rw-r--r--   0 basri      (501) staff       (20)      465 2024-04-17 12:15:34.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipeline_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     2526 2024-04-03 11:08:09.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipelines.py
+-rw-r--r--   0 basri      (501) staff       (20)      815 2024-03-12 10:17:49.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/scheduler_type.py
+-rw-r--r--   0 basri      (501) staff       (20)     3174 2024-03-22 13:38:15.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/schedulers.py
+drwxr-xr-x   0 basri      (501) staff       (20)        0 2024-04-19 07:13:35.754969 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/
+-rw-r--r--   0 basri      (501) staff       (20)      190 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 basri      (501) staff       (20)      954 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 basri      (501) staff       (20)        1 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 basri      (501) staff       (20)       18 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/requires.txt
+-rw-r--r--   0 basri      (501) staff       (20)       21 2024-04-19 07:13:35.000000 wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/top_level.txt
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/LICENCE` & `wonder-diffusion-sdk-0.0.4.dev1/LICENCE`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/__init__.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,26 +194,26 @@
             _pipeline = pipeline
         elif hasattr(self, 'pipeline'):
             _pipeline = self.pipeline
 
         # Single Lora
         if len(config.loras) == 1:
             _pipeline.load_lora_weights(
-                lora.path, weight_name=config.loras[0].weight_name)
+                config.loras[0].path, weight_name=config.loras[0].weight_name)
         # Multiple Loras
         else:
             if config.use_peft:
                 self.load_loras_with_peft(_pipeline, config)
             else:
                 adapters = []
                 adapter_weights = []
                 for lora in config.loras:
                     _pipeline.load_lora_weights(
-                        lora.path, weight_name=lora.weight_name, adapter_name=lora.adapter)
-                    adapters.append(lora.adapter)
+                        lora.path, weight_name=lora.weight_name, adapter_name=lora.adapter_name)
+                    adapters.append(lora.adapter_name)
                     adapter_weights.append(lora.adapter_weight)
                 _pipeline.set_adapters(
                     adapters, adapter_weights=adapter_weights)
 
     def load_loras_with_peft(self, pipeline: DiffusionPipeline, config: WonderLoraConfig):
         try:
             from peft import get_peft_model, PeftModel
@@ -240,31 +240,31 @@
                 lora.base_model_name_or_path,
                 torch_dtype=torch.float16,
                 variant="fp16",
                 unet=unet
             ).to(DEVICE)
 
             temp_pipeline.load_lora_weights(
-                lora.path, weight_name=lora.weight_name, adapter_name=lora.adapter)
-            temp_pipeline.set_adapters(adapter_names=lora.adapter)
+                lora.path, weight_name=lora.weight_name, adapter_name=lora.adapter_name)
+            temp_pipeline.set_adapters(adapter_names=lora.adapter_name)
 
-            adapters.append(lora.adapter)
+            adapters.append(lora.adapter_name)
             adapter_weights.append(lora.adapter_weight)
 
             unet_copy = copy.deepcopy(unet)
             peft_model = get_peft_model(
                 unet_copy,
-                temp_pipeline.unet.peft_config[lora.adapter],
-                adapter_name=lora.adapter
+                temp_pipeline.unet.peft_config[lora.adapter_name],
+                adapter_name=lora.adapter_name
             )
 
             original_state_dict = {f"base_model.model.{k}": v for k,
                                    v in temp_pipeline.unet.state_dict().items()}
             peft_model.load_state_dict(original_state_dict, strict=True)
-            peft_model.save_pretrained(f'peft_models/{lora.adapter}')
+            peft_model.save_pretrained(f'peft_models/{lora.adapter_name}')
 
             peft_models.append(peft_model)
 
             del unet, unet_copy, temp_pipeline, peft_model
             torch.cuda.empty_cache()
 
         model = PeftModel.from_pretrained(
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/lightning.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/lightning.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/logger.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/logger.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/components/safety_checker.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/components/safety_checker.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/lora_config.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/lora_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
         - `base_model_name_or_path` is required when loading multiple Loras with peft.
     """
 
     def __init__(
         self,
         path: str | os.PathLike = None,
         weight_name: str = None,
-        adapter: str = None,
+        adapter_name: str = None,
         adapter_weight: float = None,
         base_model_name_or_path: str = None,
     ):
         self.path = path
         self.weight_name = weight_name
-        self.adapter = adapter
+        self.adapter_name = adapter_name
         self.adapter_weight = adapter_weight
         self.base_model_name_or_path = base_model_name_or_path
 
 
 class WonderLoraConfig:
     """
     NOTES:
```

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/config/model_config.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/config/model_config.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/pipelines.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/pipelines.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/scheduler_type.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/scheduler_type.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk/types/schedulers.py` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk/types/schedulers.py`

 * *Files identical despite different names*

### Comparing `wonder-diffusion-sdk-0.0.4.dev0/wonder_diffusion_sdk.egg-info/SOURCES.txt` & `wonder-diffusion-sdk-0.0.4.dev1/wonder_diffusion_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

