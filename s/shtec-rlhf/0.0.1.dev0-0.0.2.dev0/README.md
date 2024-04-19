# Comparing `tmp/shtec-rlhf-0.0.1.dev0.tar.gz` & `tmp/shtec-rlhf-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shtec-rlhf-0.0.1.dev0.tar", last modified: Tue Apr 16 08:19:47 2024, max compression
+gzip compressed data, was "shtec-rlhf-0.0.2.dev0.tar", last modified: Fri Apr 19 03:10:48 2024, max compression
```

## Comparing `shtec-rlhf-0.0.1.dev0.tar` & `shtec-rlhf-0.0.2.dev0.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/PKG-INFO
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5303 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/pyproject.toml
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       38 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/setup.cfg
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-16 08:16:59.000000 shtec-rlhf-0.0.1.dev0/setup.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1005 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      591 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      450 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9251 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10049 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      423 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      484 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13680 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9018 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      448 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      503 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15371 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    18526 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      489 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      525 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    14472 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      702 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1233 2024-04-16 07:11:10.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/constants.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5026 2024-04-16 07:11:13.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/deepspeed_config.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      443 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/ds_eval_config_template.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      872 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/ds_train_config_template.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       66 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/fsdp_config.json
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2085 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15436 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/base.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/preference.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2648 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/prompt_only.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1228 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1180 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/alpaca.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      961 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/firefly.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4428 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/hh_rlhf.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4205 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/moss.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2582 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/safe_rlhf.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5352 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/safety_preference.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3925 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/supervised.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1674 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/utils.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      306 2024-04-16 06:55:53.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    19517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/arena.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:46.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      420 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6463 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/eval.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6635 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/model.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13385 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/cost.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:39.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      417 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/eval.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13213 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/problem.json
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9656 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/reward.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      452 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8849 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/deepspeed.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2822 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/huggingface.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      458 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2395 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7572 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/logger.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      584 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6565 2024-04-16 06:54:13.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/normalizer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7439 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/pretrained.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9326 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/bloom/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/bloom/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4143 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gemma/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gemma/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gemma/modeling_gemma.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt2/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt2/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6137 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt2/modeling_gpt2.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neo/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      390 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neo/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3919 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neo/modeling_gpt_neo.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neox/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      393 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neox/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3629 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neox/modeling_gpt_neox.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gptj/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gptj/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5867 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gptj/modeling_gptj.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/llama/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/llama/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/mistral/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      391 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/mistral/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3361 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/mistral/modeling_mistral.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/opt/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/opt/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3344 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.905182 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/phi/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/phi/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3325 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/phi/modeling_phi.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/qwen2/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       77 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/qwen2/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3537 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/qwen2/modeling_qwen2.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:51:12.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2803 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/arena.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11809 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/chatbot.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8659 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/cli.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      262 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4349 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/base.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    25698 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/rl_trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8535 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/supervised_trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9193 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/utils.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      179 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/__init__.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       83 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      176 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9733 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13712 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/trainer.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.909181 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      397 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/__init__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      487 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/__main__.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9753 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/main.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10744 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/trainer.py
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1439 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf/version.py
-drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-16 08:19:47.901182 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/PKG-INFO
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4077 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/SOURCES.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)        1 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/dependency_links.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      360 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/requires.txt
--rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       11 2024-04-16 08:19:47.000000 shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/top_level.txt
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/PKG-INFO
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5303 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/pyproject.toml
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       38 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/setup.cfg
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-16 08:16:59.000000 shtec-rlhf-0.0.2.dev0/setup.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1005 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      591 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      450 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9251 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10049 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      423 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      484 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13680 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9018 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      448 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      503 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15371 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    18526 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      489 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      525 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    14472 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      702 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1233 2024-04-16 07:11:10.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/constants.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5026 2024-04-16 07:11:13.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/deepspeed_config.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      443 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_eval_config_template.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      872 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_train_config_template.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       66 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/fsdp_config.json
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2085 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    15436 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/base.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/preference.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2648 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/prompt_only.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1228 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1180 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/alpaca.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      961 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/firefly.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4428 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/hh_rlhf.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4205 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/moss.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2582 2024-04-19 03:07:32.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/shtec_rlhf.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5352 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/safety_preference.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3925 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/supervised.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1674 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/utils.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      306 2024-04-16 06:55:53.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    19517 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/arena.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:46.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      420 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6463 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/eval.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6635 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/model.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13385 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/cost.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.118000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:54:39.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      417 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5801 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/eval.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13213 2024-04-16 06:27:36.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/problem.json
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9656 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/reward.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      452 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      475 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8849 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/deepspeed.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2822 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/huggingface.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      458 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2395 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7572 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/logger.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      584 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6565 2024-04-16 06:54:13.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/normalizer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     7439 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/pretrained.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9326 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4143 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/modeling_gemma.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     6137 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/modeling_gpt2.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      390 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3919 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/modeling_gpt_neo.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      393 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3629 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/modeling_gpt_neox.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      382 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     5867 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/modeling_gptj.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      385 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3651 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      391 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3361 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/modeling_mistral.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3344 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       71 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3325 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/modeling_phi.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       77 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     3537 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/modeling_qwen2.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      307 2024-04-16 06:51:12.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     2803 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/arena.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    11809 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/chatbot.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8659 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/cli.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      262 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4349 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/base.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    25698 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/rl_trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     8535 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/supervised_trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9193 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/utils.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.122000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      179 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/__init__.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       83 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      176 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9733 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    13712 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/trainer.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.126000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      397 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/__init__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      487 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/__main__.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     9753 2024-04-16 08:18:30.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/main.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)    10744 2024-04-16 08:14:54.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/trainer.py
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1439 2024-04-19 03:10:47.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf/version.py
+drwxrwxr-x   0 tcexeexe  (1000) tcexeexe  (1000)        0 2024-04-19 03:10:48.114000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     1300 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/PKG-INFO
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)     4078 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)        1 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)      360 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/requires.txt
+-rw-rw-r--   0 tcexeexe  (1000) tcexeexe  (1000)       11 2024-04-19 03:10:48.000000 shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/top_level.txt
```

### Comparing `shtec-rlhf-0.0.1.dev0/PKG-INFO` & `shtec-rlhf-0.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtec-rlhf
-Version: 0.0.1.dev0
+Version: 0.0.2.dev0
 Summary: shtec-rlhf: Safe Reinforcement Learning from Human Feedback
 Author: PKU-Alignment Team
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Repository, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Documentation, https://shtec-rlhf.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/shtec-rlhf
```

### Comparing `shtec-rlhf-0.0.1.dev0/pyproject.toml` & `shtec-rlhf-0.0.2.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/setup.py` & `shtec-rlhf-0.0.2.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/dpo/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/dpo/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_lag/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_lag/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__main__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/__main__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/algorithms/ppo_reward_shaping/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/constants.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/constants.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/deepspeed_config.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/deepspeed_config.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/configs/ds_train_config_template.json` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/configs/ds_train_config_template.json`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/base.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/base.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/preference.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/preference.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/prompt_only.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/prompt_only.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/alpaca.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/alpaca.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/firefly.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/firefly.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/hh_rlhf.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/moss.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/moss.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/raw/safe_rlhf.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/raw/shtec_rlhf.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/safety_preference.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/safety_preference.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/supervised.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/supervised.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/datasets/utils.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/arena.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/arena.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/eval.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/eval.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/bigbench/model.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/bigbench/model.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/cost.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/cost.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/eval.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/eval.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/gpt4/problem.json` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/gpt4/problem.json`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/evaluate/reward.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/evaluate/reward.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/deepspeed.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/deepspeed.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/huggingface.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/huggingface.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/finetune/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/finetune/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/logger.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/logger.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/normalizer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/normalizer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/pretrained.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/pretrained.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/__init__.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/__init__.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/bloom/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gemma/modeling_gemma.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gemma/modeling_gemma.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt2/modeling_gpt2.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neo/modeling_gpt_neo.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neo/modeling_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gpt_neox/modeling_gpt_neox.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gpt_neox/modeling_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/gptj/modeling_gptj.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/gptj/modeling_gptj.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/llama/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/mistral/modeling_mistral.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/mistral/modeling_mistral.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/opt/modeling_opt.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/phi/modeling_phi.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/phi/modeling_phi.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/models/score_model/qwen2/modeling_qwen2.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/models/score_model/qwen2/modeling_qwen2.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/arena.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/arena.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/chatbot.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/chatbot.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/serve/cli.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/serve/cli.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/base.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/base.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/rl_trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/rl_trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/trainers/supervised_trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/trainers/supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/utils.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/utils.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/cost/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/cost/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/main.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/main.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/values/reward/trainer.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/values/reward/trainer.py`

 * *Files identical despite different names*

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf/version.py` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  @date         04,2024
 #
 #  @par     Copyright (c) 2024, SHTEC
 # 
 # *******************************************************************************************************/
 """shtec-rlhf: Safe Reinforcement Learning with Human Feedback."""
 
-__version__ = '0.0.1dev0'
+__version__ = '0.0.2dev0'
 __license__ = 'Apache License, Version 2.0'
 __author__ = 'PKU-Alignment Team'
 __release__ = False
 
 if not __release__:
     import os
     import subprocess
```

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/PKG-INFO` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shtec-rlhf
-Version: 0.0.1.dev0
+Version: 0.0.2.dev0
 Summary: shtec-rlhf: Safe Reinforcement Learning from Human Feedback
 Author: PKU-Alignment Team
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Repository, https://github.com/PKU-Alignment/shtec-rlhf
 Project-URL: Documentation, https://shtec-rlhf.readthedocs.io
 Project-URL: Bug Report, https://github.com/PKU-Alignment/shtec-rlhf
```

### Comparing `shtec-rlhf-0.0.1.dev0/shtec_rlhf.egg-info/SOURCES.txt` & `shtec-rlhf-0.0.2.dev0/shtec_rlhf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 shtec_rlhf/datasets/supervised.py
 shtec_rlhf/datasets/utils.py
 shtec_rlhf/datasets/raw/__init__.py
 shtec_rlhf/datasets/raw/alpaca.py
 shtec_rlhf/datasets/raw/firefly.py
 shtec_rlhf/datasets/raw/hh_rlhf.py
 shtec_rlhf/datasets/raw/moss.py
-shtec_rlhf/datasets/raw/safe_rlhf.py
+shtec_rlhf/datasets/raw/shtec_rlhf.py
 shtec_rlhf/evaluate/__init__.py
 shtec_rlhf/evaluate/arena.py
 shtec_rlhf/evaluate/cost.py
 shtec_rlhf/evaluate/reward.py
 shtec_rlhf/evaluate/bigbench/__init__.py
 shtec_rlhf/evaluate/bigbench/__main__.py
 shtec_rlhf/evaluate/bigbench/eval.py
```

