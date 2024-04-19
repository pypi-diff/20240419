# Comparing `tmp/alpaca_eval-0.6.1.tar.gz` & `tmp/alpaca_eval-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.6.1.tar", last modified: Sat Apr 13 05:40:52 2024, max compression
+gzip compressed data, was "alpaca_eval-0.6.2.tar", last modified: Fri Apr 19 06:28:05 2024, max compression
```

## Comparing `alpaca_eval-0.6.1.tar` & `alpaca_eval-0.6.2.tar`

### file list

```diff
@@ -1,566 +1,577 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.591073 alpaca_eval-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-04-13 05:40:19.000000 alpaca_eval-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 05:40:19.000000 alpaca_eval-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    87001 2024-04-13 05:40:52.591073 alpaca_eval-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    83777 2024-04-13 05:40:19.000000 alpaca_eval-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.519073 alpaca_eval-0.6.1/example/
--rw-r--r--   0 runner    (1001) docker     (127)   500735 2024-04-13 05:40:19.000000 alpaca_eval-0.6.1/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:40:52.591073 alpaca_eval-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.491073 alpaca_eval-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.519073 alpaca_eval-0.6.1/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 05:40:31.000000 alpaca_eval-0.6.1/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25664 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.523073 alpaca_eval-0.6.1/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.523073 alpaca_eval-0.6.1/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/bedrock_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/jinachat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/decoders/vllm_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0314/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0314/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0613/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0613/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.527073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/bedrock_claude/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/bedrock_claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/bedrock_claude_2/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/bedrock_claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.531073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt35_turbo_instruct/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt35_turbo_instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/basic_clf_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/basic_clf_cot_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.535073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/mistral-large-2402_ranking/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/mistral-large-2402_ranking/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.495073 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_cot_gpt4_turbo_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_gpt4_turbo_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/claude_3_opus_ranking_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/mistral-large-2402_ranking_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17446 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/weighted_alpaca_eval_gpt4_turbo_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28388 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/metrics/glm_winrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/metrics/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/metrics/winrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.515073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.539073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Conifer-7B-DPO/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Conifer-7B-DPO/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Conifer-7B-DPO/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Ein-70B-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Ein-70B-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Ein-70B-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mistral-7B-Instruct-v0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mistral-7B-Instruct-v0.2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/togetherai_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/togetherai_prompt_concise.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/togetherai_prompt_verbose.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/togetherai_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.543073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen-14B-Chat/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen-14B-Chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen-14B-Chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.2-best-of-16/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Samba-CoE-v0.2-best-of-16/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-13B-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-13B-v0.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.547073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b-neft/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b-neft/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b-neft/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b_concise/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-7b_verbose/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baichuan-13b-chat/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/bedrock_claude/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/bedrock_claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/bedrock_claude_2/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/bedrock_claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.551073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/causallm-14b/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/causallm-14b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/causallm-14b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/chatglm2-6b/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_concise/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_concise/prompt_concise.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_verbose/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-2.1_verbose/prompt_verbose.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-3-opus-20240229/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-3-opus-20240229/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/prompt_chatml.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-instant-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude-instant-1.2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude2-alpaca-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/claude2-alpaca-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cut-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cut-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/cut-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/dbrx-instruct/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/dbrx-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/deita-7b-v1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/deita-7b-v1.0/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/dolphin-2.2.1-mistral-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/dolphin-2.2.1-mistral-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/evo-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/evo-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.555073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/evo-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/evo-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemini-pro/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemini-pro/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemini-pro/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemma-2b-it/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemma-2b-it/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemma-7b-it/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gemma-7b-it/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-0301/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-0301/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-0613/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-0613/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_concise/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_verbose/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-16k-0613/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-3.5-turbo-16k-0613/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-4-0125-preview/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-4-0125-preview/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-4-turbo-2024-04-09/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt-4-turbo-2024-04-09/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt35_turbo_instruct/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt35_turbo_instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0314/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0314/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613_concise/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_0613_verbose/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.559073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/chatml_prompt_concise.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/chatml_prompt_verbose.txt
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_gamed/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/gpt4_gamed/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-33b-api/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/humpback-llama-65b/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/humpback-llama-65b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/humpback-llama-65b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/humpback-llama2-70b/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/humpback-llama2-70b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/jina-chat/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/jina-chat/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/jina-chat/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.563073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minichat-1.5-3b/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minichat-1.5-3b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minichat-3b/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minichat-3b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minichat-3b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-large-2402/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-large-2402/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-medium/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-medium/basic_chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-medium/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-orpo-beta/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-orpo-beta/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/mistral-orpo-beta/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.567073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v3.1-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.571073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-dpo/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-dpo/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-dpo/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-sft/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-sft/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/phi-2-sft/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/platolm-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/platolm-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/platolm-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v1.0/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v2.0/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-70b/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-70b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-70b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.575073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/tulu-2-dpo-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b-v1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-13b-v1.5/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b-v1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/vicuna-7b-v1.5/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.579073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-70b/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/wizardlm-70b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-13b-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-13b-v0.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-70b-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-70b-v0.1/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-70b-v0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-70b-v0.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/zephyr-7b-alpha/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/zephyr-7b-alpha/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/zephyr-7b-alpha/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/zephyr-7b-beta/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/models_configs/zephyr-7b-beta/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30592 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    22523 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    87001 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 05:40:52.000000 alpaca_eval-0.6.1/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:40:52.583073 alpaca_eval-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-13 05:40:23.000000 alpaca_eval-0.6.1/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.967802 alpaca_eval-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-04-19 06:27:31.000000 alpaca_eval-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-19 06:27:31.000000 alpaca_eval-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    87001 2024-04-19 06:28:05.967802 alpaca_eval-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    83777 2024-04-19 06:27:31.000000 alpaca_eval-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.907803 alpaca_eval-0.6.2/example/
+-rw-r--r--   0 runner    (1001) docker     (127)   500735 2024-04-19 06:27:31.000000 alpaca_eval-0.6.2/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 06:28:05.967802 alpaca_eval-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.875803 alpaca_eval-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.911803 alpaca_eval-0.6.2/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 06:27:42.000000 alpaca_eval-0.6.2/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25709 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.911803 alpaca_eval-0.6.2/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/bedrock_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/jinachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/decoders/vllm_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0314/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0314/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0613/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_0613/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.915803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/bedrock_claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/bedrock_claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/bedrock_claude_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/bedrock_claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.919803 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt35_turbo_instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt35_turbo_instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/basic_clf_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/basic_clf_cot_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.923802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/mistral-large-2402_ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/mistral-large-2402_ranking/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo_new/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo_new/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.883803 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_cot_gpt4_turbo_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_gpt4_turbo_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/claude_3_opus_ranking_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/mistral-large-2402_ranking_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17837 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/weighted_alpaca_eval_gpt4_turbo_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28388 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/metrics/glm_winrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/metrics/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/metrics/winrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.907803 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Conifer-7B-DPO/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Conifer-7B-DPO/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Conifer-7B-DPO/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.927802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Ein-70B-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Ein-70B-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Ein-70B-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Meta-Llama-3-70B-Instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Meta-Llama-3-70B-Instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Meta-Llama-3-8B-Instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Meta-Llama-3-8B-Instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mistral-7B-Instruct-v0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mistral-7B-Instruct-v0.2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x22B-Instruct-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x22B-Instruct-v0.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/togetherai_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/togetherai_prompt_concise.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/togetherai_prompt_verbose.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige-Plus-Chat-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige-Plus-Chat-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige-Plus-Chat-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/togetherai_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen-14B-Chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen-14B-Chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen-14B-Chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.931802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.2-best-of-16/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Samba-CoE-v0.2-best-of-16/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Starling-LM-7B-alpha/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-13B-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-13B-v0.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-70B-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Yi-34B-Chat-Verified/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_claude-3-opus-20240229/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/aligner-2b_qwen1.5-72b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.935802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b-neft/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b-neft/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b-neft/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b_concise/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-7b_verbose/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baichuan-13b-chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baichuan-13b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baichuan-13b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/bedrock_claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/bedrock_claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/bedrock_claude_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/bedrock_claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/causallm-14b/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/causallm-14b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/causallm-14b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/chatglm2-6b/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/chatglm2-6b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/chatglm2-6b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_concise/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_concise/prompt_concise.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_verbose/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-2.1_verbose/prompt_verbose.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-3-opus-20240229/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-3-opus-20240229/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-3-sonnet-20240229/prompt_chatml.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-instant-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude-instant-1.2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude2-alpaca-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/claude2-alpaca-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.939802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cut-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cut-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/cut-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/dbrx-instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/dbrx-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/deepseek-llm-67b-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/deita-7b-v1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/deita-7b-v1.0/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/dolphin-2.2.1-mistral-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/dolphin-2.2.1-mistral-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/evo-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/evo-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/evo-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/evo-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemini-pro/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemini-pro/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemini-pro/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemma-2b-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemma-2b-it/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemma-7b-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gemma-7b-it/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-0301/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-0301/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-0613/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-0613/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_concise/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-1106_verbose/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-16k-0613/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-3.5-turbo-16k-0613/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-4-0125-preview/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-4-0125-preview/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-4-turbo-2024-04-09/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt-4-turbo-2024-04-09/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt35_turbo_instruct/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt35_turbo_instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0314/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0314/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613_concise/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.943802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_0613_verbose/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/chatml_prompt_concise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_concise/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/chatml_prompt_verbose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_1106_preview_verbose/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_gamed/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/gpt4_gamed/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-33b-api/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-33b-api/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/humpback-llama-65b/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/humpback-llama-65b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/humpback-llama-65b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/humpback-llama2-70b/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/humpback-llama2-70b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/internlm2-chat-20b-ppo/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/jina-chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/jina-chat/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/jina-chat/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-13b-chat-hf/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-70b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-chat-7b-evol70k-neft/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.947802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minichat-1.5-3b/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minichat-1.5-3b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minichat-3b/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minichat-3b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minichat-3b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-large-2402/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-large-2402/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-medium/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-medium/basic_chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-medium/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-orpo-beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-orpo-beta/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/mistral-orpo-beta/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.951802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v3.1-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat-v3.1-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-dpo/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-dpo/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-dpo/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-sft/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-sft/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/phi-2-sft/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/platolm-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/platolm-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/platolm-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v1.0/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/recycled-wizardlm-7b-v2.0/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-70b/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-70b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-70b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/tulu-2-dpo-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.955802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b-v1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-13b-v1.5/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b-v1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/vicuna-7b-v1.5/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-70b/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/wizardlm-70b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-13b-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-13b-v0.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-70b-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-70b-v0.1/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-70b-v0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-70b-v0.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/xwinlm-7b-v0.1/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/zephyr-7b-alpha/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/zephyr-7b-alpha/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/zephyr-7b-alpha/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.959802 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/zephyr-7b-beta/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/models_configs/zephyr-7b-beta/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30592 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22523 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.963802 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    87001 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 06:28:05.000000 alpaca_eval-0.6.2/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:28:05.963802 alpaca_eval-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-19 06:27:34.000000 alpaca_eval-0.6.2/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.6.1/LICENSE` & `alpaca_eval-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/PKG-INFO` & `alpaca_eval-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.6.1
+Version: 0.6.2
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -1327,15 +1327,15 @@
 Length controlled (LC) win-rates are a debiased version of the win-rates that control for the length of the outputs.
 
 The main idea is that for each model we will fit a logistic regression to  predict the preference of the autoannotator given: (1) the instruction, (2) the model, and (3) the difference of length between the baseline and model output. 
 Given such a logistic regression we can then try to predict the counterfactual "what would the preference be if the model's output had the same length as the baseline" by setting the length difference to 0.
 By averaging over this length-controlled preference, we then obtain the length-controlled win-rate.
 The exact form of the logistic regression is taken such that the interpretation of LC win rates is similar to the raw win rates, for example for any model `m1` and `m2` we have `win_rate(m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`. 
 Length controlled win-rates increase the correlation between AlpacaEval's leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while significantly decreasing the length gameability of the annotator**.
-For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_correction.ipynb).
+For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_controlled.ipynb).
 
 This idea of estimating the controlled direct effect, by predicting the outcome while conditioning on the mediator (the length difference), is common in statistical inference.
 
 To get LC win rates on previously annotated models, you can use the following command:
 
 ```bash
 pip install -U alpaca_eval
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.6.1 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.6.2 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -893,15 +893,15 @@
 the raw win rates, for example for any model `m1` and `m2` we have `win_rate
 (m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`.
 Length controlled win-rates increase the correlation between AlpacaEval's
 leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while
 significantly decreasing the length gameability of the annotator**. For more
 information and results about length controlled win-rates see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
-length_correction.ipynb). This idea of estimating the controlled direct effect,
+length_controlled.ipynb). This idea of estimating the controlled direct effect,
 by predicting the outcome while conditioning on the mediator (the length
 difference), is common in statistical inference. To get LC win rates on
 previously annotated models, you can use the following command: ```bash pip
 install -U alpaca_eval alpaca_eval --model_outputs â¦ --
 is_recompute_metrics_only True ```
 ********** AAllppaaccaaEEvvaall 22..00 **********
 AlpacaEval 2.0 is a new version of AlpacaEval. Here are the differences: -
```

### Comparing `alpaca_eval-0.6.1/README.md` & `alpaca_eval-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1244,15 +1244,15 @@
 Length controlled (LC) win-rates are a debiased version of the win-rates that control for the length of the outputs.
 
 The main idea is that for each model we will fit a logistic regression to  predict the preference of the autoannotator given: (1) the instruction, (2) the model, and (3) the difference of length between the baseline and model output. 
 Given such a logistic regression we can then try to predict the counterfactual "what would the preference be if the model's output had the same length as the baseline" by setting the length difference to 0.
 By averaging over this length-controlled preference, we then obtain the length-controlled win-rate.
 The exact form of the logistic regression is taken such that the interpretation of LC win rates is similar to the raw win rates, for example for any model `m1` and `m2` we have `win_rate(m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`. 
 Length controlled win-rates increase the correlation between AlpacaEval's leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while significantly decreasing the length gameability of the annotator**.
-For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_correction.ipynb).
+For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_controlled.ipynb).
 
 This idea of estimating the controlled direct effect, by predicting the outcome while conditioning on the mediator (the length difference), is common in statistical inference.
 
 To get LC win rates on previously annotated models, you can use the following command:
 
 ```bash
 pip install -U alpaca_eval
```

#### html2text {}

```diff
@@ -850,15 +850,15 @@
 the raw win rates, for example for any model `m1` and `m2` we have `win_rate
 (m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`.
 Length controlled win-rates increase the correlation between AlpacaEval's
 leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while
 significantly decreasing the length gameability of the annotator**. For more
 information and results about length controlled win-rates see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
-length_correction.ipynb). This idea of estimating the controlled direct effect,
+length_controlled.ipynb). This idea of estimating the controlled direct effect,
 by predicting the outcome while conditioning on the mediator (the length
 difference), is common in statistical inference. To get LC win rates on
 previously annotated models, you can use the following command: ```bash pip
 install -U alpaca_eval alpaca_eval --model_outputs â¦ --
 is_recompute_metrics_only True ```
 ********** AAllppaaccaaEEvvaall 22..00 **********
 AlpacaEval 2.0 is a new version of AlpacaEval. Here are the differences: -
```

### Comparing `alpaca_eval-0.6.1/example/outputs.json` & `alpaca_eval-0.6.2/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/setup.py` & `alpaca_eval-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/analyze.py` & `alpaca_eval-0.6.2/src/alpaca_eval/analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
             Correlations between different methods.
         """
 
         annotations_1 = self._get_annotations(annotations_1)
         is_add_generator = annotations_2 == "gold_crossannotations"
         annotations_2 = self._get_annotations(annotations_2)
 
-        if is_add_generator:
+        if "generator" not in annotations_2.columns and is_add_generator:
             # TODO clean: following is because we don't save generator in HF crossannotation dataset => reconstructs it.
             # takes only eval set for the leaderboard
             merge_kwargs = dict(right=self.df_gold_annotations[self.keys + ["generator"]], on=self.keys)
             annotations_2 = annotations_2.query("datasplit == 'eval'").merge(**merge_kwargs)
             annotations_1 = annotations_1.query("datasplit == 'eval'").merge(**merge_kwargs)
             n_per_generator = annotations_2.groupby("generator").size()
             n_annotated = 100  # we annotated around 140 per generator, there are other generators due to same outputs
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.6.2/src/alpaca_eval/annotators/base.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.6.2/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.6.2/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/constants.py` & `alpaca_eval-0.6.2/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/bedrock_anthropic.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/bedrock_anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/google.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/google.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/jinachat.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/jinachat.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
 
 def _get_price_per_token(model, price_per_token=None):
     """Returns the price per token for a given model"""
     if price_per_token is not None:
         return float(price_per_token)
     if "gpt-4-turbo" in model:
-        return 0.001 / 1000
+        return 0.01 / 1000
     elif "gpt-4-1106" in model:
         return (
             0.01 / 1000
         )  # that's not completely true because decoding is 0.03 but close enough given that most is context
     elif "gpt-4" in model:
         return (
             0.03 / 1000
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/replicate.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/replicate.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/decoders/vllm_local.py` & `alpaca_eval-0.6.2/src/alpaca_eval/decoders/vllm_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_cot_gpt4_turbo/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/configs.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-alpaca_eval_clf_cot_gpt4_turbo:
-  prompt_template: "alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt"
+alpaca_eval_clf_gpt4_turbo:
+  prompt_template: "alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
-    model_name: "gpt-4-turbo"
-    max_tokens: 300
+    model_name: "gpt-4-1106-preview"
+    max_tokens: 1
     temperature: 1 # temperature should be applied for sampling, so that should make no effect.
     logprobs: true
     top_logprobs: 5
   fn_completion_parser: "logprob_parser"
   completion_parser_kwargs:
     numerator_token: "m"
     denominator_tokens: ["m", "M"]
     is_binarize: true
-    log_prob_index: -1
   completion_key: "completions_all"
   batch_size: 1
-  processors_to_kwargs:
-    ChainOfThoughtProcessor: {}
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_clf_gpt4_turbo/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/configs.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-alpaca_eval_clf_gpt4_turbo:
-  prompt_template: "alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt"
+gpt4_turbo_logprob:
+  prompt_template: "gpt4_turbo_clf/basic_clf_prompt.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
-    model_name: "gpt-4-turbo"
+    model_name: "gpt-4-1106-preview"
     max_tokens: 1
     temperature: 1 # temperature should be applied for sampling, so that should make no effect.
     logprobs: true
     top_logprobs: 5
   fn_completion_parser: "logprob_parser"
   completion_parser_kwargs:
-    numerator_token: "m"
-    denominator_tokens: ["m", "M"]
-    is_binarize: true
+    numerator_token: "A"
+    denominator_tokens: [ "A", "B" ]
+    is_binarize: false
   completion_key: "completions_all"
-  batch_size: 1
+  batch_size: 1
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_cot_gpt4_turbo_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_turbo_fn/configs.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 alpaca_eval_gpt4_turbo_fn:
   prompt_template: "alpaca_eval_gpt4_turbo_fn/alpaca_eval_fn.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
-    model_name: "gpt-4-turbo"
+    model_name: "gpt-4-1106-preview"
     max_tokens: 100
     temperature: 0
     function_call:
       name: "make_partial_leaderboard"
     functions:
       - name: "make_partial_leaderboard"
         description: "Make a leaderboard of models given a list of the models ordered by the preference of their outputs."
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/ranking_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_3_opus_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/ranking_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt-3.5-turbo-1106_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/basic_clf_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/basic_clf_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_clf/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/basic_clf_cot_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/basic_clf_cot_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_clf/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/gpt4_turbo_cot_logprob/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/gpt4_turbo_logprob/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/configs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-gpt4_turbo_logprob:
-  prompt_template: "gpt4_turbo_clf/basic_clf_prompt.txt"
+weighted_alpaca_eval_cot_gpt4_turbo:
+  prompt_template: "alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
     model_name: "gpt-4-1106-preview"
-    max_tokens: 1
+    max_tokens: 300
     temperature: 1 # temperature should be applied for sampling, so that should make no effect.
     logprobs: true
     top_logprobs: 5
   fn_completion_parser: "logprob_parser"
   completion_parser_kwargs:
-    numerator_token: "A"
-    denominator_tokens: [ "A", "B" ]
+    numerator_token: "m"
+    denominator_tokens: ["m", "M"]
     is_binarize: false
+    log_prob_index: -1
   completion_key: "completions_all"
-  batch_size: 1
+  batch_size: 1
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/configs.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-weighted_alpaca_eval_cot_gpt4_turbo:
-  prompt_template: "alpaca_eval_clf_cot_gpt4_turbo/alpaca_eval_clf_cot.txt"
+weighted_alpaca_eval_gpt4_turbo:
+  prompt_template: "alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
-    model_name: "gpt-4-turbo"
-    max_tokens: 300
+    model_name: "gpt-4-1106-preview"
+    max_tokens: 1
     temperature: 1 # temperature should be applied for sampling, so that should make no effect.
     logprobs: true
     top_logprobs: 5
   fn_completion_parser: "logprob_parser"
   completion_parser_kwargs:
     numerator_token: "m"
     denominator_tokens: ["m", "M"]
     is_binarize: false
-    log_prob_index: -1
   completion_key: "completions_all"
   batch_size: 1
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo_new/configs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-weighted_alpaca_eval_gpt4_turbo:
+weighted_alpaca_eval_gpt4_turbo_new:
   prompt_template: "alpaca_eval_clf_gpt4_turbo/alpaca_eval_clf.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
     model_name: "gpt-4-turbo"
     max_tokens: 1
     temperature: 1 # temperature should be applied for sampling, so that should make no effect.
     logprobs: true
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_cot_gpt4_turbo_fn_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_cot_gpt4_turbo_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_gpt4_turbo_fn_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_gpt4_turbo_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/claude_3_opus_ranking_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/claude_3_opus_ranking_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/mistral-large-2402_ranking_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/mistral-large-2402_ranking_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/data_AlpacaEval_2/weighted_alpaca_eval_gpt4_turbo_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/data_AlpacaEval_2/weighted_alpaca_eval_gpt4_turbo_leaderboard.csv`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 ,win_rate,standard_error,n_wins,n_wins_base,n_draws,n_total,discrete_win_rate,mode,avg_length,length_controlled_winrate
-gpt-4-0125-preview,51.22356403608144,1.5925964020631154,408,388,9,805,51.24223602484472,verified,2018,52.71305126323133
-gpt-4-turbo-2024-04-09,42.6755010801893,1.601975204819872,334,463,8,805,41.98757763975156,minimal,1802,51.9269770895354
+gpt-4-turbo-2024-04-09,46.11526538763708,1.474073957743638,370,426,9,805,46.52173913043478,minimal,1802,55.01530093647852
 gpt4_1106_preview_verbose,64.30360147101865,1.3348590089025316,525,268,12,805,65.96273291925466,dev,2402,51.57500797967598
 gpt4_1106_preview,50.0,0.0,0,0,805,805,50.0,minimal,2049,50.0
+Nanbeige-Plus-Chat-v0.1,56.70300973017392,1.482841874951873,456,347,2,805,56.77018633540373,community,2587,44.45966240337981
 gpt4_1106_preview_concise,22.92019444047205,1.232517714329424,172,622,11,805,22.049689440993788,dev,1136,41.896601591245386
 aligner-2b_claude-3-opus-20240229,34.46337362321739,1.314666526302454,225,475,105,805,34.47204968944099,community,1669,41.823071715247664
-claude-3-opus-20240229,29.04176413403727,1.3942602231385623,223,580,2,805,27.82608695652174,minimal,1388,40.39177606350116
-gpt4,23.576789314782605,1.275704201206918,179,618,8,805,22.732919254658384,minimal,1365,38.12808974440021
+claude-3-opus-20240229,29.10526953334248,1.3941539442369442,223,579,3,805,27.888198757763977,minimal,1388,40.5095080124761
+gpt4,23.576789314782605,1.275704201206918,179,618,8,805,22.732919254658384,verified,1365,38.12808974440021
 aligner-2b_qwen1.5-72b-chat,31.773037737123104,1.2392772646245978,180,473,152,805,31.801242236024844,community,1812,36.725868878524274
 Qwen1.5-72B-Chat,26.49828339562733,1.304236164893057,201,600,4,805,25.217391304347824,community,1549,36.571754111987296
 gpt4_0314,22.073258928708075,1.2466725494608204,172,627,6,805,21.73913043478261,verified,1371,35.30706121640206
 Ein-70B-v0.1,24.84472049689441,1.521406431103307,199,604,2,805,24.84472049689441,community,1467,35.029054008520646
-claude-3-sonnet-20240229,25.556325292273296,1.3419811051815638,193,608,4,805,24.22360248447205,verified,1420,34.87247436243302
+claude-3-sonnet-20240229,25.556325292273296,1.3419811051815638,193,608,4,805,24.22360248447205,minimal,1420,34.87247436243302
+Meta-Llama-3-70B-Instruct,33.17785695886864,1.3886514096065603,266,537,2,805,33.16770186335404,minimal,1919,34.42459717459881
 gpt4_0613_verbose,23.237360043453418,1.283539505582624,171,630,4,805,21.490683229813666,dev,1473,33.82126688658535
-mistral-large-2402,21.43877598137888,1.2485232545097724,166,638,1,805,20.6832298136646,minimal,1362,32.65207998531868
+mistral-large-2402,21.43877598137888,1.2485232545097724,166,638,1,805,20.6832298136646,verified,1362,32.65207998531868
 Samba-CoE-v0.2-best-of-16,26.988254318335404,1.3189030000371738,201,601,3,805,25.15527950310559,community,1578,31.506544268148147
+Mixtral-8x22B-Instruct-v0.1,22.21017054750302,1.2780740057417268,174,628,3,805,21.801242236024844,verified,1445,30.878810294279383
 claude-2.1_verbose,24.35407109006212,1.293586209982439,191,613,1,805,23.7888198757764,dev,1414,30.29117916664986
 gpt4_0613,15.75503808763975,1.0754642482396215,117,684,4,805,14.782608695652174,verified,1140,30.18332231673423
 Snorkel-Mistral-PairRM-DPO-best-of-16,34.8601328912795,1.3599450436840308,270,533,2,805,33.66459627329193,community,2616,29.974321613074405
 Contextual-KTO-Mistral-PairRM,33.227355200024846,1.3779687477923963,260,544,1,805,32.36024844720497,verified,2521,29.705808939683976
 pairrm-Yi-34B-Chat,31.24128294680746,1.34824373994879,239,563,3,805,29.87577639751553,community,2195,28.81484086684313
 mistral-medium,21.855772543652176,1.2682402187223842,164,639,2,805,20.496894409937887,verified,1500,28.614337401726104
 claude-2,17.188240356708075,1.17482825615589,131,673,1,805,16.335403726708076,verified,1069,28.155196141629148
 Samba-CoE-v0.2,21.847378669267083,1.2171089783436106,159,645,1,805,19.81366459627329,community,1469,27.62426735006872
 claude,16.98534361236025,1.1687959793014906,129,676,0,805,16.024844720496894,verified,1082,27.289504443727107
 Yi-34B-Chat,29.65994671879504,1.3225712597906096,219,582,4,805,27.45341614906832,verified,2123,27.19054787762733
 Snorkel-Mistral-PairRM-DPO,30.220052700671644,1.3328273012530358,231,572,1,804,28.79353233830846,community,2736,26.39144645733206
 claude-instant-1.2,16.12739962159006,1.1341036838301686,120,682,3,805,15.093167701863356,community,1112,25.61225902543337
-dbrx-instruct,18.448348984074535,1.255388020324377,150,655,0,805,18.633540372670808,verified,1450,25.375449740444473
+dbrx-instruct,18.44834898407453,1.255388020324377,150,655,0,805,18.633540372670808,verified,1450,25.37544974044448
 claude-2.1,15.733506736409938,1.120315865445773,115,688,2,805,14.409937888198757,verified,1096,25.251943886133027
 Nanbeige2-8B-Chat,39.35450207219922,1.4524224245579649,323,480,2,805,40.24844720496895,community,2709,25.24207090175315
 xwinlm-70b-v0.1,21.812957073875776,1.230327447605842,166,635,4,805,20.869565217391305,community,1775,24.649686057119272
-gemini-pro,18.177644540571432,1.158850379070738,135,665,5,805,17.080745341614907,community,1456,24.38177610802152
+gemini-pro,18.177644540571432,1.158850379070738,135,665,5,805,17.080745341614907,minimal,1456,24.38177610802152
 Mixtral-8x7B-Instruct-v0.1,18.25531762637268,1.1885585968848205,135,668,2,805,16.8944099378882,minimal,1465,23.68848260134481
 evo-v2-7b,20.834113022583853,1.2159901798146158,158,644,3,805,19.81366459627329,community,1754,23.35770570204821
 Mixtral-8x7B-Instruct-v0.1_verbose,24.61406305018634,1.2975757385881228,194,609,2,805,24.22360248447205,dev,2083,23.223120780856064
 Mixtral-8x7B-Instruct-v0.1_concise,13.744040154795034,1.071868299237546,105,700,0,805,13.043478260869565,dev,910,22.962609472758643
+Meta-Llama-3-8B-Instruct,22.56990260938061,1.257580233106669,176,626,3,805,22.049689440993788,minimal,1899,22.918784673210016
 Samba-CoE-v0.1,16.835501870062114,1.1180386124646702,124,680,1,805,15.46583850931677,community,1316,22.865837334795227
 gpt-3.5-turbo-16k-0613,14.13239070746584,1.027579400264853,96,704,5,805,12.236024844720497,verified,1328,22.720189163383225
 gpt-3.5-turbo-0613,14.09579857390062,1.0371186215049395,99,700,6,805,12.670807453416147,community,1331,22.35251298054288
 gpt-3.5-turbo-1106_verbose,12.76316981026087,1.044246819212278,94,709,2,805,11.801242236024844,dev,1058,22.00093702171442
 gpt4_0613_concise,9.400320574596272,0.901021275896262,71,729,5,805,9.130434782608695,dev,627,21.57799091454269
 pairrm-tulu-2-70b,18.638962967441,1.1924966700012911,140,665,0,805,17.391304347826086,community,1607,21.428403975507223
 tulu-2-dpo-70b,15.982854374136648,1.1457861368237434,119,683,3,805,14.96894409937888,verified,1418,21.238610038371124
@@ -58,15 +61,15 @@
 Conifer-7B-DPO,11.31358564916222,0.9870897936343656,87,717,1,805,10.869565217391305,community,1253,17.11249588276248
 Mistral-7B-Instruct-v0.2,14.722772657714286,1.0785266446729775,113,691,1,805,14.09937888198758,minimal,1676,17.111251846021165
 evo-7b,15.577437399527952,1.0835570388658722,112,689,4,805,14.161490683229813,community,1774,16.489386004239325
 humpback-llama2-70b,10.121771502645965,0.9401806122130112,77,727,1,805,9.627329192546584,community,1107,16.249164231428974
 OpenHermes-2.5-Mistral-7B,10.340415705751552,0.935655389929366,75,727,3,805,9.503105590062113,verified,1107,16.248577696674843
 deita-7b-v1.0,12.646639472385097,1.0352555320811423,96,708,1,805,11.987577639751551,community,1417,16.05901353966741
 jina-chat,7.786130393366459,0.8398450575524877,59,743,3,805,7.515527950310559,community,676,15.866004049505932
-TempNet-LLaMA2-Chat-70B-v0.1,15.051894420220444,1.08015075807378,111,691,2,804,13.930348258706468,minimal,1830,15.831162778430024
+TempNet-LLaMA2-Chat-70B-v0.1,15.051894420220444,1.08015075807378,111,691,2,804,13.930348258706468,community,1830,15.831162778430024
 gpt-3.5-turbo-1106_concise,7.41586497762733,0.8374438113826953,57,744,4,805,7.329192546583851,dev,431,15.769520983894386
 causallm-14b,11.146160869950313,0.9544127300795228,81,720,4,805,10.31055900621118,community,1391,15.72032518895564
 pairrm-zephyr-7b-beta,12.84127825562733,1.0535874941903722,98,706,1,805,12.236024844720497,community,1487,15.529867294986612
 mistral-orpo-beta,12.565408794559003,0.9929774686147969,95,707,3,805,11.987577639751551,community,1636,14.716749430705242
 Starling-LM-7B-alpha,14.24592352162733,1.0685460609395083,102,702,1,805,12.732919254658384,community,1895,14.690471079424972
 llama-2-70b-chat-hf,13.88825834374378,1.079984772728814,104,700,0,804,12.935323383084576,verified,1790,14.689648588392544
 openchat-v3.1-13b,11.082230489416148,0.9501308701291292,80,720,5,805,10.248447204968944,community,1484,14.50338795683784
@@ -124,15 +127,15 @@
 baize-v2-13b,4.590545330645964,0.6497033226861672,32,770,3,805,4.161490683229814,community,930,7.012247205044542
 recycled-wizardlm-7b-v1.0,6.632749960459629,0.7713329913775592,53,752,0,805,6.583850931677018,community,1494,6.9014773220018215
 alpaca-7b_verbose,2.9331016025062344,0.5302092824422211,22,778,2,802,2.8678304239401498,dev,537,6.816306816367379
 alpaca-farm-ppo-human,4.100426814981367,0.6304721406855217,32,770,3,805,4.161490683229814,verified,803,6.418603294911531
 vicuna-7b,4.16261116226087,0.6135107768217068,28,775,2,805,3.602484472049689,verified,1044,6.277217738516609
 alpaca-7b,2.591450540223603,0.4870855382635108,17,785,3,805,2.298136645962733,minimal,396,5.875487163278986
 phi-2-sft,3.977567775217392,0.6098271417287373,28,777,0,805,3.4782608695652173,verified,1068,5.853787690603355
-TempNet-LLaMA2-Chat-7B-v0.1,5.430143264670806,0.7210775889233014,39,765,1,805,4.906832298136646,minimal,1512,5.739613836715224
+TempNet-LLaMA2-Chat-7B-v0.1,5.430143264670806,0.7210775889233014,39,765,1,805,4.906832298136646,community,1512,5.739613836715224
 minichat-3b,3.0071507063602487,0.504124596172496,22,779,4,805,2.981366459627329,community,868,5.729332875896306
 guanaco-33b,5.002493724956522,0.6697115752218856,37,768,0,805,4.596273291925466,verified,1311,5.690019090866207
 falcon-40b-instruct,3.3429188224720505,0.5541127159067186,27,777,1,805,3.4161490683229814,verified,662,5.6075325447394455
 gemma-2b-it,3.4019714381366457,0.5389981250162534,23,782,0,805,2.857142857142857,verified,1041,5.437453620377121
 llama-2-7b-chat-hf,4.961339547167702,0.6691754516864777,38,766,1,805,4.782608695652174,verified,1479,5.354821279508294
 openbuddy-falcon-7b-v6,3.521174371975156,0.5655836442881659,27,778,0,805,3.354037267080745,community,1152,4.8261244822302976
 alpaca-7b_concise,1.9911763835447769,0.4437510223659489,15,787,2,804,1.9900497512437807,dev,351,4.467251679930348
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.6.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/main.py` & `alpaca_eval-0.6.2/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/metrics/glm_winrate.py` & `alpaca_eval-0.6.2/src/alpaca_eval/metrics/glm_winrate.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/metrics/helpers.py` & `alpaca_eval-0.6.2/src/alpaca_eval/metrics/helpers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/metrics/winrate.py` & `alpaca_eval-0.6.2/src/alpaca_eval/metrics/winrate.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 
 
 # backward compatibility
 def pairwise_to_winrate(preferences: Union[pd.DataFrame, Sequence]) -> dict[str, float]:
     """Extract head2head metrics (n_wins, n_counts, win_rate) from a sequence preference.
     This assumes that the preference is encoded as 0 or 1.5 for draw, 1 for base win, 2 when the model to compare wins.
     """
-    return get_winrate(annotations=[dict(preferences=p) for p in preferences])
+    return get_winrate(annotations=[dict(preference=p) for p in preferences])
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Ein-70B-v0.1/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Ein-70B-v0.1/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/Snorkel-Mistral-PairRM-DPO-best-of-16/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/TempNet-LLaMA2-Chat-7B-v0.1/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/llama-2-7b-chat-hf/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-40b-v9/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-falcon-7b-v6/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-30b-v7.1/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama-65b-v8/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-13b-v11.1/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/prompt.txt` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/openbuddy-llama2-70b-v10.1/prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-Yi-34B-Chat/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-13b/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-tulu-2-70b/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/pairrm-zephyr-7b-beta/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-best-of-16/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/configs.yaml` & `alpaca_eval-0.6.2/src/alpaca_eval/models_configs/ultralm-13b-v2.0-best-of-16/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/plotting.py` & `alpaca_eval-0.6.2/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/processors.py` & `alpaca_eval-0.6.2/src/alpaca_eval/processors.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval/utils.py` & `alpaca_eval-0.6.2/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.6.2/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.6.1
+Version: 0.6.2
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -1327,15 +1327,15 @@
 Length controlled (LC) win-rates are a debiased version of the win-rates that control for the length of the outputs.
 
 The main idea is that for each model we will fit a logistic regression to  predict the preference of the autoannotator given: (1) the instruction, (2) the model, and (3) the difference of length between the baseline and model output. 
 Given such a logistic regression we can then try to predict the counterfactual "what would the preference be if the model's output had the same length as the baseline" by setting the length difference to 0.
 By averaging over this length-controlled preference, we then obtain the length-controlled win-rate.
 The exact form of the logistic regression is taken such that the interpretation of LC win rates is similar to the raw win rates, for example for any model `m1` and `m2` we have `win_rate(m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`. 
 Length controlled win-rates increase the correlation between AlpacaEval's leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while significantly decreasing the length gameability of the annotator**.
-For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_correction.ipynb).
+For more information and results about length controlled win-rates see [this notebook](https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/length_controlled.ipynb).
 
 This idea of estimating the controlled direct effect, by predicting the outcome while conditioning on the mediator (the length difference), is common in statistical inference.
 
 To get LC win rates on previously annotated models, you can use the following command:
 
 ```bash
 pip install -U alpaca_eval
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.6.1 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.6.2 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
@@ -893,15 +893,15 @@
 the raw win rates, for example for any model `m1` and `m2` we have `win_rate
 (m1, m2) = 1 - win_rate(m2, m1) \in [0,100]` and `win_rate(m1, m1) = 0.5`.
 Length controlled win-rates increase the correlation between AlpacaEval's
 leaderboard and Chat Arena from **0.93 to 0.98 Spearman correlation, while
 significantly decreasing the length gameability of the annotator**. For more
 information and results about length controlled win-rates see [this notebook]
 (https://github.com/tatsu-lab/alpaca_eval/blob/main/notebooks/
-length_correction.ipynb). This idea of estimating the controlled direct effect,
+length_controlled.ipynb). This idea of estimating the controlled direct effect,
 by predicting the outcome while conditioning on the mediator (the length
 difference), is common in statistical inference. To get LC win rates on
 previously annotated models, you can use the following command: ```bash pip
 install -U alpaca_eval alpaca_eval --model_outputs â¦ --
 is_recompute_metrics_only True ```
 ********** AAllppaaccaaEEvvaall 22..00 **********
 AlpacaEval 2.0 is a new version of AlpacaEval. Here are the differences: -
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.6.2/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
 src/alpaca_eval/evaluators_configs/test/configs.yaml
 src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
 src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
 src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_cot_gpt4_turbo/configs.yaml
 src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo/configs.yaml
+src/alpaca_eval/evaluators_configs/weighted_alpaca_eval_gpt4_turbo_new/configs.yaml
 src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_cot_gpt4_turbo_fn_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval_2/alpaca_eval_gpt4_turbo_fn_leaderboard.csv
 src/alpaca_eval/leaderboards/data_AlpacaEval_2/claude_3_opus_ranking_leaderboard.csv
@@ -123,23 +124,28 @@
 src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM/prompt.txt
 src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/configs.yaml
 src/alpaca_eval/models_configs/Contextual-KTO-Mistral-PairRM-Verified/prompt.txt
 src/alpaca_eval/models_configs/Ein-70B-v0.1/configs.yaml
 src/alpaca_eval/models_configs/Ein-70B-v0.1/prompt.txt
 src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/configs.yaml
 src/alpaca_eval/models_configs/LMCocktail-10.7B-v1/prompt.txt
+src/alpaca_eval/models_configs/Meta-Llama-3-70B-Instruct/configs.yaml
+src/alpaca_eval/models_configs/Meta-Llama-3-8B-Instruct/configs.yaml
 src/alpaca_eval/models_configs/Mistral-7B-Instruct-v0.2/configs.yaml
 src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/configs.yaml
 src/alpaca_eval/models_configs/Mistral-7B-ReMax-v0.1/prompt.txt
+src/alpaca_eval/models_configs/Mixtral-8x22B-Instruct-v0.1/configs.yaml
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/configs.yaml
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1/togetherai_prompt.txt
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/configs.yaml
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_concise/togetherai_prompt_concise.txt
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/configs.yaml
 src/alpaca_eval/models_configs/Mixtral-8x7B-Instruct-v0.1_verbose/togetherai_prompt_verbose.txt
+src/alpaca_eval/models_configs/Nanbeige-Plus-Chat-v0.1/configs.yaml
+src/alpaca_eval/models_configs/Nanbeige-Plus-Chat-v0.1/prompt.txt
 src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/configs.yaml
 src/alpaca_eval/models_configs/Nanbeige2-8B-Chat/prompt.txt
 src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/configs.yaml
 src/alpaca_eval/models_configs/OpenHermes-2.5-Mistral-7B/togetherai_prompt.txt
 src/alpaca_eval/models_configs/Qwen-14B-Chat/configs.yaml
 src/alpaca_eval/models_configs/Qwen-14B-Chat/prompt.txt
 src/alpaca_eval/models_configs/Qwen1.5-72B-Chat/configs.yaml
```

### Comparing `alpaca_eval-0.6.1/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.6.2/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/tests/test_analyze.py` & `alpaca_eval-0.6.2/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/tests/test_decoders_unit.py` & `alpaca_eval-0.6.2/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/tests/test_main.py` & `alpaca_eval-0.6.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.6.1/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.6.2/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

