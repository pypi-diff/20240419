# Comparing `tmp/llm_optimized_inference-0.1.3-py3-none-any.whl.zip` & `tmp/llm_optimized_inference-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,38 @@
-Zip file size: 66135 bytes, number of entries: 36
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-10 23:44 llm/__init__.py
--rw-rw-r--  2.0 unx      249 b- defN 24-Apr-10 23:44 llm/optimized/__init__.py
--rw-rw-r--  2.0 unx      703 b- defN 24-Apr-10 23:44 llm/optimized/inference/__init__.py
--rw-rw-r--  2.0 unx      204 b- defN 24-Apr-10 23:44 llm/optimized/inference/_version.py
--rw-rw-r--  2.0 unx    28124 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server.py
--rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-10 23:44 llm/optimized/inference/configs.py
--rw-rw-r--  2.0 unx     5210 b- defN 24-Apr-10 23:44 llm/optimized/inference/constants.py
--rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-10 23:44 llm/optimized/inference/conversation.py
--rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-10 23:44 llm/optimized/inference/fm_score.py
--rw-rw-r--  2.0 unx      664 b- defN 24-Apr-10 23:44 llm/optimized/inference/logging_config.py
--rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-10 23:44 llm/optimized/inference/managed_inference.py
--rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-10 23:44 llm/optimized/inference/model_config_factory.py
--rw-rw-r--  2.0 unx     6935 b- defN 24-Apr-10 23:44 llm/optimized/inference/model_utils.py
--rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-10 23:44 llm/optimized/inference/prompt_formatter.py
--rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-10 23:44 llm/optimized/inference/replica_manager.py
--rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-10 23:44 llm/optimized/inference/score.py
--rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-10 23:44 llm/optimized/inference/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/__init__.py
--rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/openapi.json
--rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-10 23:44 llm/optimized/inference/api_server_setup/protocol.py
--rw-rw-r--  2.0 unx      131 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/__init__.py
--rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
--rw-rw-r--  2.0 unx     8520 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
--rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-10 23:44 llm/optimized/inference/custom_model_configurations/schema_output.py
--rw-rw-r--  2.0 unx      259 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/__init__.py
--rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/_hf_predictors.py
--rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/engine.py
--rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/hf_engine.py
--rw-rw-r--  2.0 unx    10755 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/mii_engine.py
--rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/mii_engine_v2.py
--rw-rw-r--  2.0 unx    13820 b- defN 24-Apr-10 23:44 llm/optimized/inference/engine/vllm_engine.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        4 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-10 23:47 llm_optimized_inference-0.1.3.dist-info/RECORD
-36 files, 217700 bytes uncompressed, 60151 bytes compressed:  72.4%
+Zip file size: 66366 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-19 00:42 llm/__init__.py
+-rw-rw-r--  2.0 unx      249 b- defN 24-Apr-19 00:42 llm/optimized/__init__.py
+-rw-rw-r--  2.0 unx      703 b- defN 24-Apr-19 00:42 llm/optimized/inference/__init__.py
+-rw-rw-r--  2.0 unx      204 b- defN 24-Apr-19 00:42 llm/optimized/inference/_version.py
+-rw-rw-r--  2.0 unx    28243 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server.py
+-rw-rw-r--  2.0 unx     3203 b- defN 24-Apr-19 00:42 llm/optimized/inference/configs.py
+-rw-rw-r--  2.0 unx     5469 b- defN 24-Apr-19 00:42 llm/optimized/inference/constants.py
+-rw-rw-r--  2.0 unx     3255 b- defN 24-Apr-19 00:42 llm/optimized/inference/conversation.py
+-rw-rw-r--  2.0 unx     5802 b- defN 24-Apr-19 00:42 llm/optimized/inference/fm_score.py
+-rw-rw-r--  2.0 unx      664 b- defN 24-Apr-19 00:42 llm/optimized/inference/logging_config.py
+-rw-rw-r--  2.0 unx     9028 b- defN 24-Apr-19 00:42 llm/optimized/inference/managed_inference.py
+-rw-rw-r--  2.0 unx     1369 b- defN 24-Apr-19 00:42 llm/optimized/inference/model_config_factory.py
+-rw-rw-r--  2.0 unx     6638 b- defN 24-Apr-19 00:42 llm/optimized/inference/model_utils.py
+-rw-rw-r--  2.0 unx     1575 b- defN 24-Apr-19 00:42 llm/optimized/inference/prompt_formatter.py
+-rw-rw-r--  2.0 unx    12420 b- defN 24-Apr-19 00:42 llm/optimized/inference/replica_manager.py
+-rw-rw-r--  2.0 unx    18786 b- defN 24-Apr-19 00:42 llm/optimized/inference/score.py
+-rw-rw-r--  2.0 unx     4731 b- defN 24-Apr-19 00:42 llm/optimized/inference/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/__init__.py
+-rw-rw-r--  2.0 unx     9502 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/openapi.json
+-rw-rw-r--  2.0 unx     1878 b- defN 24-Apr-19 00:42 llm/optimized/inference/api_server_setup/protocol.py
+-rw-rw-r--  2.0 unx      131 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/__init__.py
+-rw-rw-r--  2.0 unx     2725 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py
+-rw-rw-r--  2.0 unx     8806 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py
+-rw-rw-r--  2.0 unx     1047 b- defN 24-Apr-19 00:42 llm/optimized/inference/custom_model_configurations/schema_output.py
+-rw-rw-r--  2.0 unx      259 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/__init__.py
+-rw-rw-r--  2.0 unx    38577 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/_hf_predictors.py
+-rw-rw-r--  2.0 unx     4583 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/engine.py
+-rw-rw-r--  2.0 unx     8617 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/hf_engine.py
+-rw-rw-r--  2.0 unx    10797 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/mii_engine.py
+-rw-rw-r--  2.0 unx     7971 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/mii_engine_v2.py
+-rw-rw-r--  2.0 unx    14278 b- defN 24-Apr-19 00:42 llm/optimized/inference/engine/vllm_engine.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3113 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        4 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3599 b- defN 24-Apr-19 00:45 llm_optimized_inference-0.1.4.dist-info/RECORD
+36 files, 218567 bytes uncompressed, 60382 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -87,23 +87,23 @@
 
 Filename: llm/optimized/inference/engine/mii_engine_v2.py
 Comment: 
 
 Filename: llm/optimized/inference/engine/vllm_engine.py
 Comment: 
 
-Filename: llm_optimized_inference-0.1.3.dist-info/LICENSE
+Filename: llm_optimized_inference-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: llm_optimized_inference-0.1.3.dist-info/METADATA
+Filename: llm_optimized_inference-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: llm_optimized_inference-0.1.3.dist-info/WHEEL
+Filename: llm_optimized_inference-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: llm_optimized_inference-0.1.3.dist-info/top_level.txt
+Filename: llm_optimized_inference-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_optimized_inference-0.1.3.dist-info/RECORD
+Filename: llm_optimized_inference-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## llm/optimized/inference/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
```

## llm/optimized/inference/api_server.py

```diff
@@ -59,14 +59,15 @@
 DEFAULT_MLFLOW_MODEL_PATH = "mlflow_model_folder/model"
 DEFAULT_TOKENIZER_PATH = "mlflow_model_folder/components/tokenizer"
 task_type = SupportedTask.TEXT_GENERATION
 g_fmscorer: FMScore = None
 g_model_signature = None
 g_served_model = None
 g_engine_config = None
+g_generation_config = {}
 
 # For apis
 app = FastAPI(openapi_url="/swagger.json", docs_url="/swagger.json")
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
@@ -330,22 +331,24 @@
     return AACS_error
 
 # endregion
 
 
 def get_generator_params(params: dict):
     """Return accumulated generator params."""
+    global g_generator_config
     updated_params = {}
     # map 'max_gen_len' to 'max_new_tokens' if present
     if "max_gen_len" in params:
         logger.warning("max_gen_len is deprecated. Use max_new_tokens")
         params["max_new_tokens"] = params["max_gen_len"]
         del params["max_gen_len"]
 
     updated_params.update(params)
+    updated_params.update(g_generation_config)
     return updated_params
 
 
 def _init_cuda_visible_devices():
     import torch
 
     if "CUDA_VISIBLE_DEVICES" in os.environ:
@@ -698,14 +701,16 @@
  
 def init_server(model_path: str, AACS_error: Union[None, Exception]):
     """Initialize text-generation-inference server and client."""
     global task_type
     global g_fmscorer
     global g_engine_config
     global g_model_signature
+    global g_generation_config
+
     try:
         tokenizer_path = os.path.join(
             os.getenv("AZUREML_MODEL_DIR", ""),
             DEFAULT_TOKENIZER_PATH,
         )
 
         # Maintain Backwards Compatibility with old file structure
@@ -728,15 +733,15 @@
         mlmodel = {}
         if abs_mlmodel_path and os.path.exists(abs_mlmodel_path):
             with open(abs_mlmodel_path) as f:
                 mlmodel = yaml.safe_load(f)
 
         if mlmodel:
             g_model_signature = mlmodel.get("signature", None)
-            g_engine_config, task_config, default_generator_configs, task_type = build_configs_from_model(
+            g_engine_config, task_config, g_generation_config, task_type = build_configs_from_model(
                 mlmodel,
                 model_path,
                 config_path,
                 tokenizer_path
             )
         
         config = {
@@ -746,15 +751,15 @@
 
         g_fmscorer = FMScore(config)
         g_fmscorer.init()
         if os.environ.get("LOGGING_WORKER_ID", "") == str(os.getpid()):
             for k, v in os.environ.items():
                 logger.info(f"env: {k} = {v}")
             logger.info(
-                f"updated default_generator_configs: " f"{default_generator_configs}",
+                f"updated generation_config: " f"{g_generation_config}",
             )
             if AACS_error:
                 logger.warning(f"AACS was not configured. Content moderation bypassed in setup. Error {AACS_error}")
         return None
     except Exception as e:
         return Exception(f"Error in creating client or server: {e}")
```

## llm/optimized/inference/constants.py

```diff
@@ -87,15 +87,17 @@
         "OLMoForCausalLM",
         "OPTForCausalLM",
         "OrionForCausalLM",
         "QWenLMHeadModel",
         "Qwen2ForCausalLM",
         "RWForCausalLM",
         "StableLmForCausalLM",
-        "DbrxForCausalLM"
+        "DbrxForCausalLM",
+        "Phi3MiniForCausalLM",
+        "PhiLongRoPEForCausalLM"
     }
 
 
 class MIISupportedModels:
     """MII Supported Models."""
 
     # TODO: Add more models from different tasks
@@ -122,15 +124,18 @@
     # TODO: Remove "RefinedWebModel" and "RefinedWeb" once falcon models are updated to latest huggingface commit
 
     Models = {
         "falcon": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWebModel": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "RefinedWeb": {"kwargs": {"gpu-memory-utilization": .95}, "args": ["trust-remote-code"]},
         "dbrx": {"args": ["trust-remote-code"]},
-        "deci_lm": {"args": ["trust-remote-code"]}
+        "deci_lm": {"args": ["trust-remote-code"]},
+        "phi3mini": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]},
+        "phi_longrope": {"kwargs": {"tensor-parallel-size": 1}, "args": ["trust-remote-code"]}
+
     }
 
     @classmethod
     def get_kwargs(cls, model_type: str):
         """Get the kwargs the vllm server needs for the model type."""
         params = cls.Models.get(model_type, {})
         return params.get("kwargs", {})
```

## llm/optimized/inference/model_utils.py

```diff
@@ -77,43 +77,36 @@
     engine_config["hf_config_path"] = os.path.dirname(config_path)
     engine_config["tokenizer"] = tokenizer_path
     task_config = {}
 
     if mlmodel:
         flavors = mlmodel.get("flavors", {})
 
+        # update default gen configs with model configs
+        model_generator_configs = {}
+        if os.path.exists(os.path.join(model_path, "generation_config.json")):
+            with open(os.path.join(model_path, "generation_config.json")) as f:
+                model_generator_configs.update(json.load(f))
+        default_generator_configs = get_generator_params(
+            model_generator_configs
+        )
+
         if "transformers" in flavors:
             task_type = flavors["transformers"]["task"]
             flavors_dict = flavors.get("transformers")
             ml_model_info = deepcopy(flavors_dict)
             if ml_model_info.get("tokenizer_type", None):
                 ml_model_info["hf_tokenizer_class"] = ml_model_info.get("tokenizer_type")
             if ml_model_info.get("pipeline_model_type", None):
                 ml_model_info["hf_pretrained_class"] = ml_model_info.get("pipeline_model_type")
-            model_generator_configs = {}
-            if os.path.exists(os.path.join(model_path, "generation_config.json")):
-                with open(os.path.join(model_path, "generation_config.json")) as f:
-                    model_generator_configs.update(json.load(f))
-            default_generator_configs = get_generator_params(
-                model_generator_configs
-            )
         elif "hftransformersv2" in flavors:
             task_type = flavors["hftransformersv2"]["task_type"]
-            model_generator_configs = flavors["hftransformersv2"].get(
-                "generator_config",
-                {},
-            )
             ml_model_info = flavors["hftransformersv2"].copy()
             if task_type not in ALL_TASKS:
                 raise Exception(f"Unsupported task_type {task_type}")
-
-            # update default gen configs with model configs
-            default_generator_configs = get_generator_params(
-                model_generator_configs,
-            )
         elif "python_function" in flavors:
             task_type = mlmodel["metadata"]["base_model_task"]
             if task_type not in [TaskType.TEXT_TO_IMAGE, TaskType.TEXT_TO_IMAGE_INPAINTING]:
                 raise Exception(f"Unsupported task_type {task_type}")
 
             model_type = mlmodel["metadata"].get("model_type", "")
```

## llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py

```diff
@@ -78,36 +78,38 @@
         return {
             "deployment_name": os.getenv("DEPLOYMENT_NAME", default_deployment_name),
             "mii_configs": {},
         }
 
     @staticmethod
     def _post_processing_text_to_image(
-        responses: "ImageResponse", inference_time: float, prompts: List[str] = None
+        responses: "ImageResponse", inference_time: float, prompts: List[str] = None, num_images_per_prompt: int = 1
     ) -> List[ImageTaskInferenceResult]:
         """Post processing for text to image task.
 
         :param responses: response from mii server
         :type responses: ImageResponse
         :param inference_time: inference time in milliseconds
         :type inference_time: float
         :param prompts: input prompts, defaults to None
         :type prompts: List[str], optional
+        :param num_images_per_prompt: number of images per prompt, defaults to 1
+        :type num_images_per_prompt: int, optional
         :return: Image Task prediction output
         :rtype: List[ImageTaskInferenceResult]
         """
         result = []
         images = responses.images
         nsfw_content_detected = responses.nsfw_content_detected
         for i in range(len(images)):
             result.append(
                 ImageTaskInferenceResult(
                     response=TextToImageSchema(
                         generated_image=images[i],
-                        prompt=prompts[i][0] if prompts else None,
+                        prompt=prompts[i // num_images_per_prompt][0] if prompts else None,
                         nsfw_content_detected=nsfw_content_detected[i] if nsfw_content_detected else None,
                     ),
                     inference_time_ms=inference_time,
                 )
             )
         return result
 
@@ -123,15 +125,16 @@
         :return: processed model response
         :rtype: List of ImageTaskInferenceResult
         """
         TASK_POST_PROCESSING_MAP = {TaskType.TEXT_TO_IMAGE: self._post_processing_text_to_image,
                                     TaskType.TEXT_TO_IMAGE_INPAINTING: self._post_processing_text_to_image
                                     }
         prompts = kwargs.get("prompts")
-        result = TASK_POST_PROCESSING_MAP[self._task](responses, inference_time, prompts)
+        num_images_per_prompt = kwargs.get("num_images_per_prompt", 1)
+        result = TASK_POST_PROCESSING_MAP[self._task](responses, inference_time, prompts, num_images_per_prompt)
         return result
 
     def update_mii_model_config(self, model_config: "ModelConfig") -> None:
         """Override the default MII model configuration depending on task and GPU compute capability.
 
         :param model_config: MII model configuration
         :type model_config: ModelConfig
```

## llm/optimized/inference/engine/mii_engine.py

```diff
@@ -77,15 +77,17 @@
         try:
             responses = await self.model._request_async_response(queries, **params)
         except Exception as e:
             raise Exception(json.dumps({"error": "Error in processing request", "exception": str(e)}))
         inference_time_ms = (time.time() - start_time) * 1000
 
         if self.custom_model_config_builder is not None:
-            return self.custom_model_config_builder.post_processing(responses, inference_time_ms, prompts=prompts)
+            return self.custom_model_config_builder.post_processing(
+                responses, inference_time_ms, prompts=prompts, **params
+            )
 
         inference_results = []  # type: List[InferenceResult]
         return_full_text = params.pop("return_full_text", True)
         for i, res in enumerate(responses.response):
             generated_text = res
             generated_text = self._del_prompt_if_req(prompts[i], generated_text, return_full_text=return_full_text)
             response_tokens = self.get_tokens(generated_text)
```

## llm/optimized/inference/engine/vllm_engine.py

```diff
@@ -188,14 +188,23 @@
         if "use_beam_search" in params and params["use_beam_search"]:
             logger.info("Beam search is enabled, setting temperature to 0.")
             params["temperature"] = 0.0
 
             if "best_of" not in params:
                 logger.info("Beam search is enabled, setting best_of to 2.")
                 params["best_of"] = 2
+        
+        if "eos_token_id" in params:
+            eos_token_id = params["eos_token_id"]
+            # eos_token_id in GenerationConfig is (Union[int, List[int]], optional) 
+            # while vLLM SamplingParams is (Optional[List[int]])
+            if not isinstance(eos_token_id, list):
+                params["stop_token_ids"] = [params["eos_token_id"]]
+            else:
+                params["stop_token_ids"] = params["eos_token_id"]
 
         # Remove unsupported keys and log a warning for each
         unsupported_keys = set(params.keys()) - set(VLLM_SAMPLING_PARAMS.keys())
         for key in unsupported_keys:
             logger.warning(
                 f"Warning: Parameter '{key}' is not supported by VLLM and will be removed.",
             )
```

## Comparing `llm_optimized_inference-0.1.3.dist-info/METADATA` & `llm_optimized_inference-0.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-optimized-inference
-Version: 0.1.3
+Version: 0.1.4
 Home-page: 
 Author: Microsoft
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 License-File: LICENSE
 Requires-Dist: deepspeed ==0.13.2
 Requires-Dist: deepspeed-mii ==0.2.2
 Requires-Dist: vllm ==0.4.0.post1
 Requires-Dist: deepspeed-kernels ==0.0.1.dev1698255861
 Requires-Dist: diffusers ==0.26.2
 Requires-Dist: pandas ~=2.1.4
-Requires-Dist: transformers ~=4.39.1
+Requires-Dist: transformers ~=4.40.0
 Requires-Dist: aiolimiter ~=1.1.0
 Requires-Dist: azure-ai-contentsafety ==1.0.0b1
 Requires-Dist: azure-ai-ml ==1.12.1
 Requires-Dist: azure-identity ==1.15.0
 Requires-Dist: azureml-ai-monitoring ==0.1.0b4
 Requires-Dist: azureml-inference-server-http
 Requires-Dist: azureml-mlflow
```

## Comparing `llm_optimized_inference-0.1.3.dist-info/RECORD` & `llm_optimized_inference-0.1.4.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 llm/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/__init__.py,sha256=ybCtCrXNS3six25SvldGKjcl-9eR9CzOMgoUjbRBdBQ,249
 llm/optimized/inference/__init__.py,sha256=rGZODP-qE2NOlUgdbmxhfuS3svmx9gM-kU97d9-jb50,703
-llm/optimized/inference/_version.py,sha256=nyTOHBjjPDYAxYwXKh0e_MQds1g4eK__bGQIqfBzN7U,204
-llm/optimized/inference/api_server.py,sha256=JokKFHQWG6yQKdC_aYhiGX_THF3XI31CdK_Xy47DLYU,28124
+llm/optimized/inference/_version.py,sha256=xTMdyihKrF9Wwzf6EEZPWUMcTZtCY6fmsZCX3oPpH4o,204
+llm/optimized/inference/api_server.py,sha256=kyUIykJuk9jPajQyUqqMl4FEQKLZV57LykfGY0Z99Ak,28243
 llm/optimized/inference/configs.py,sha256=d5NKbQlfYVkUQ4SL03KVBQekdOG4VrcD0xGxVeHESeQ,3203
-llm/optimized/inference/constants.py,sha256=3JodVG32H9cRiBmyQ2WwFaa41Eh15zNM4T3eyZQFH7k,5210
+llm/optimized/inference/constants.py,sha256=1MgHKQg67k-swDkfhsrRDRpMabW82ZKNfvdhSyP61vE,5469
 llm/optimized/inference/conversation.py,sha256=cBrHv1sI1hrOQB57sSZKAarplKRgqQWqmYxT-wkZHLM,3255
 llm/optimized/inference/fm_score.py,sha256=7z7ZbLMXUXH6gp1-G_l3rOus9r9vSpIm5-wOj5X17aQ,5802
 llm/optimized/inference/logging_config.py,sha256=egtAiGCNVNoU8E_JPhp2aGJVIJ_QkTwLhkNjpVKjICI,664
 llm/optimized/inference/managed_inference.py,sha256=O_HlOPNl24Uoy68gFKrSM_gOG-rg4P_lishBQFAXyC8,9028
 llm/optimized/inference/model_config_factory.py,sha256=EpHH8QyUaE5DC6A5O5nKbie_kMEpfeqmufbOn0U6jFI,1369
-llm/optimized/inference/model_utils.py,sha256=WRo4cmiMlK5tGUd7UDXRJzdXjQi5Lb0uECPijbVPdaQ,6935
+llm/optimized/inference/model_utils.py,sha256=W9nLxInrhuPnmhvZldBpS2POB7-u_SST7ostxatAYrA,6638
 llm/optimized/inference/prompt_formatter.py,sha256=xxM4MbvvPL6jQcLB37uKA9-wCHXTZUL9l5GiUu3r964,1575
 llm/optimized/inference/replica_manager.py,sha256=AUQn9IWFgdsHEQpHDqQVMjnGdZFdzr55IQnVmXFHefA,12420
 llm/optimized/inference/score.py,sha256=RWEaCZ4Akig88ErqshDD8KFCF-YDwMJvsRJjeBWR-WM,18786
 llm/optimized/inference/utils.py,sha256=STENfqDoR8otc2Ig8MN-nERR-y6O6Nl3gpIOZ8A8fbo,4731
 llm/optimized/inference/api_server_setup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 llm/optimized/inference/api_server_setup/openapi.json,sha256=SMtuKvJK58zuxDig48iZ2GMggHxvCpBx5KgYXVAWtoA,9502
 llm/optimized/inference/api_server_setup/protocol.py,sha256=0WmY2-1iQrCsDXXanqIwM7klNBU3skm6tZMxOMPTrWk,1878
 llm/optimized/inference/custom_model_configurations/__init__.py,sha256=D0zlB3WPH212MfcHh1Wz6TRe6Igcg-0Wh0hHA8Kl_l0,131
 llm/optimized/inference/custom_model_configurations/base_configuration_builder.py,sha256=pX9BNG70Rts3TY5p_Smuq4x8ZDG0DG1-6kLfY90Jht0,2725
-llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py,sha256=umom7rGh5HBt43iQYWIKJa_gqJqSxfn35Ezu4D7O0-I,8520
+llm/optimized/inference/custom_model_configurations/diffusion_configuration_builder.py,sha256=oPY_h5WDdopurQzsfaR95DHLjgFSNgq4coE2ETo-j2o,8806
 llm/optimized/inference/custom_model_configurations/schema_output.py,sha256=JIpThLkAPoO7MlhaJVSxP2RYVwYzIpw3R3k-nraLq9k,1047
 llm/optimized/inference/engine/__init__.py,sha256=8GqGW53dbRlGShwO11h5HQH4KjnUzoW0t0cChUUFDPY,259
 llm/optimized/inference/engine/_hf_predictors.py,sha256=AwQTIpmOHb7h31H2DF2Jx-9b03lcB5DOrgSbXGpamIk,38577
 llm/optimized/inference/engine/engine.py,sha256=xbpEVJBjovFyACw6WF8uqnmyodRWqb52oaR3s3pr8Sc,4583
 llm/optimized/inference/engine/hf_engine.py,sha256=4rRldNod-pMDJ_-3q0RDWEkigCTr6I62HyJspb01lAs,8617
-llm/optimized/inference/engine/mii_engine.py,sha256=oL426rosTUkhnn7P2K37sEyNLRAvIfNj616jyhDDBjk,10755
+llm/optimized/inference/engine/mii_engine.py,sha256=TBfc_wt4-NKTzkjHCie5YpqRGS6pvBNigyYpTHt_jII,10797
 llm/optimized/inference/engine/mii_engine_v2.py,sha256=rI4tjRyj-dCZBDAiN0YNPKMBtkD3MXxcbucuSlHg6lI,7971
-llm/optimized/inference/engine/vllm_engine.py,sha256=fssm9SzWYcxBp4KxxhKORhe4BdsulxXUozNfz5BTRyw,13820
-llm_optimized_inference-0.1.3.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-llm_optimized_inference-0.1.3.dist-info/METADATA,sha256=6H6ShACnFiHk-Du8NG04ZuALNWeKavohRldaKVXziMg,3113
-llm_optimized_inference-0.1.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-llm_optimized_inference-0.1.3.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
-llm_optimized_inference-0.1.3.dist-info/RECORD,,
+llm/optimized/inference/engine/vllm_engine.py,sha256=IZDkMxOTMhsn7qCmsSAfIE8DFll4dfDRIWd5FU6_a3c,14278
+llm_optimized_inference-0.1.4.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+llm_optimized_inference-0.1.4.dist-info/METADATA,sha256=z3BdPc8OhIo4ByRfgRnJtPYq2shTK66a8dgLk162wr0,3113
+llm_optimized_inference-0.1.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+llm_optimized_inference-0.1.4.dist-info/top_level.txt,sha256=TwpEQXP3b1MS9Y2XuGgRuo9-Kny507xt2HFZgJ5TSIY,4
+llm_optimized_inference-0.1.4.dist-info/RECORD,,
```

