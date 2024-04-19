# Comparing `tmp/moviechat-0.6.0.tar.gz` & `tmp/moviechat-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moviechat-0.6.0.tar", last modified: Fri Apr 19 12:38:51 2024, max compression
+gzip compressed data, was "moviechat-0.6.1.tar", last modified: Fri Apr 19 15:28:08 2024, max compression
```

## Comparing `moviechat-0.6.0.tar` & `moviechat-0.6.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.684219 moviechat-0.6.0/
--rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.6.0/LICENSE
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.676219 moviechat-0.6.0/MovieChat/
--rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 04:17:40.000000 moviechat-0.6.0/MovieChat/__init__.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/common/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    15080 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/config.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3620 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/dist_utils.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      815 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/gradcam.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6002 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/logger.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3517 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/optims.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9928 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/registry.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    13808 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/common/utils.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/conversation/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/conversation/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    10954 2024-04-17 09:12:13.000000 moviechat-0.6.0/MovieChat/conversation/conversation_video.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/datasets/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/__init__.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/datasets/builders/
--rw-rw-r--   0 exs       (1016) exs       (1016)     2162 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/builders/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8109 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/builders/base_dataset_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3004 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/builders/image_text_pair_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2393 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/builders/instruct_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      987 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/builders/video_caption_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6283 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/data_utils.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/datasets/datasets/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2067 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/base_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2602 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/caption_datasets.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     1669 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/cc_sbu_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4214 2024-04-17 09:11:31.000000 moviechat-0.6.0/MovieChat/datasets/datasets/dataloader_utils.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     1175 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/laion_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8785 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/llava_instruct_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9701 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/video_instruct_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4437 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/datasets/datasets/webvid_datasets.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/models/
--rw-rw-r--   0 exs       (1016) exs       (1016)    48450 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/Qformer.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4289 2024-04-19 03:58:05.000000 moviechat-0.6.0/MovieChat/models/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     7147 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/base_model.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     7795 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/blip2.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2331 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/blip2_outputs.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9161 2024-04-18 14:38:08.000000 moviechat-0.6.0/MovieChat/models/chat_model.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    18684 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/eva_vit.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    14489 2024-04-17 09:11:15.000000 moviechat-0.6.0/MovieChat/models/eva_vit_with_tome.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3989 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/helpers.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    33326 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/modeling_llama.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    31259 2024-04-19 12:32:33.000000 moviechat-0.6.0/MovieChat/models/moviechat.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    23136 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/multimodal_preprocessors.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    11438 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/models/process_video_data.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.680219 moviechat-0.6.0/MovieChat/processors/
--rw-rw-r--   0 exs       (1016) exs       (1016)      999 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      610 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/base_processor.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4008 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/blip_processors.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3924 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/functional_video.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    10960 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/randaugment.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     5017 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/transforms_video.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6959 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/processors/video_processor.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.684219 moviechat-0.6.0/MovieChat/runners/
--rw-rw-r--   0 exs       (1016) exs       (1016)      307 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/runners/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    22856 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/runners/runner_base.py
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/runners/test.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.684219 moviechat-0.6.0/MovieChat/tasks/
--rw-rw-r--   0 exs       (1016) exs       (1016)      837 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/tasks/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8799 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/tasks/base_task.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/tasks/image_text_pretrain.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.6.0/MovieChat/tasks/video_text_pretrain.py
--rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 12:38:51.684219 moviechat-0.6.0/PKG-INFO
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 12:38:51.684219 moviechat-0.6.0/moviechat.egg-info/
--rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 12:38:51.000000 moviechat-0.6.0/moviechat.egg-info/PKG-INFO
--rw-rw-r--   0 exs       (1016) exs       (1016)     2166 2024-04-19 12:38:51.000000 moviechat-0.6.0/moviechat.egg-info/SOURCES.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-19 12:38:51.000000 moviechat-0.6.0/moviechat.egg-info/dependency_links.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 12:38:51.000000 moviechat-0.6.0/moviechat.egg-info/requires.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)       10 2024-04-19 12:38:51.000000 moviechat-0.6.0/moviechat.egg-info/top_level.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)     1804 2024-04-19 12:35:22.000000 moviechat-0.6.0/pyproject.toml
--rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-19 12:38:51.684219 moviechat-0.6.0/setup.cfg
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.6.1/LICENSE
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 04:17:40.000000 moviechat-0.6.1/MovieChat/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/common/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    15080 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/config.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3620 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/dist_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      815 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/gradcam.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6002 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/logger.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3517 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/optims.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9928 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/registry.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    13808 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/common/utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/conversation/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/conversation/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10954 2024-04-17 09:12:13.000000 moviechat-0.6.1/MovieChat/conversation/conversation_video.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/datasets/builders/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2162 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/builders/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8109 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/builders/base_dataset_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3004 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/builders/image_text_pair_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2393 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/builders/instruct_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      987 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/builders/video_caption_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6283 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/data_utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.100828 moviechat-0.6.1/MovieChat/datasets/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2067 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/base_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2602 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/caption_datasets.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1669 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/cc_sbu_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4214 2024-04-17 09:11:31.000000 moviechat-0.6.1/MovieChat/datasets/datasets/dataloader_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1175 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/laion_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8785 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/llava_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9701 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/video_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4437 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/datasets/datasets/webvid_datasets.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/MovieChat/models/
+-rw-rw-r--   0 exs       (1016) exs       (1016)    48450 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/Qformer.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4289 2024-04-19 03:58:05.000000 moviechat-0.6.1/MovieChat/models/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7147 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/base_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7795 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/blip2.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2331 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/blip2_outputs.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9161 2024-04-18 14:38:08.000000 moviechat-0.6.1/MovieChat/models/chat_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    18684 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/eva_vit.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    14489 2024-04-17 09:11:15.000000 moviechat-0.6.1/MovieChat/models/eva_vit_with_tome.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3989 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/helpers.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    33326 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/modeling_llama.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    31970 2024-04-19 15:26:52.000000 moviechat-0.6.1/MovieChat/models/moviechat.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    23136 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/multimodal_preprocessors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    11438 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/models/process_video_data.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/MovieChat/processors/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      999 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      610 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/base_processor.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4008 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/blip_processors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3924 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/functional_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10960 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/randaugment.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     5017 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/transforms_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6959 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/processors/video_processor.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/MovieChat/runners/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      307 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/runners/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    22856 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/runners/runner_base.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/runners/test.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/MovieChat/tasks/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      837 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/tasks/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8799 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/tasks/base_task.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/tasks/image_text_pretrain.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.6.1/MovieChat/tasks/video_text_pretrain.py
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 15:28:08.104828 moviechat-0.6.1/PKG-INFO
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 15:28:08.104828 moviechat-0.6.1/moviechat.egg-info/
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 15:28:08.000000 moviechat-0.6.1/moviechat.egg-info/PKG-INFO
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2166 2024-04-19 15:28:08.000000 moviechat-0.6.1/moviechat.egg-info/SOURCES.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-19 15:28:08.000000 moviechat-0.6.1/moviechat.egg-info/dependency_links.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 15:28:08.000000 moviechat-0.6.1/moviechat.egg-info/requires.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)       10 2024-04-19 15:28:08.000000 moviechat-0.6.1/moviechat.egg-info/top_level.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1804 2024-04-19 15:27:47.000000 moviechat-0.6.1/pyproject.toml
+-rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-19 15:28:08.104828 moviechat-0.6.1/setup.cfg
```

### Comparing `moviechat-0.6.0/LICENSE` & `moviechat-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/__init__.py` & `moviechat-0.6.1/MovieChat/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/config.py` & `moviechat-0.6.1/MovieChat/common/config.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/dist_utils.py` & `moviechat-0.6.1/MovieChat/common/dist_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/gradcam.py` & `moviechat-0.6.1/MovieChat/common/gradcam.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/logger.py` & `moviechat-0.6.1/MovieChat/common/logger.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/optims.py` & `moviechat-0.6.1/MovieChat/common/optims.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/registry.py` & `moviechat-0.6.1/MovieChat/common/registry.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/common/utils.py` & `moviechat-0.6.1/MovieChat/common/utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/conversation/conversation_video.py` & `moviechat-0.6.1/MovieChat/conversation/conversation_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/builders/__init__.py` & `moviechat-0.6.1/MovieChat/datasets/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/builders/base_dataset_builder.py` & `moviechat-0.6.1/MovieChat/datasets/builders/base_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/builders/image_text_pair_builder.py` & `moviechat-0.6.1/MovieChat/datasets/builders/image_text_pair_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/builders/instruct_builder.py` & `moviechat-0.6.1/MovieChat/datasets/builders/instruct_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/builders/video_caption_builder.py` & `moviechat-0.6.1/MovieChat/datasets/builders/video_caption_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/data_utils.py` & `moviechat-0.6.1/MovieChat/datasets/data_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/base_dataset.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/caption_datasets.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/caption_datasets.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/cc_sbu_dataset.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/cc_sbu_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/dataloader_utils.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/laion_dataset.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/laion_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/llava_instruct_dataset.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/llava_instruct_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/video_instruct_dataset.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/video_instruct_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/datasets/datasets/webvid_datasets.py` & `moviechat-0.6.1/MovieChat/datasets/datasets/webvid_datasets.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/Qformer.py` & `moviechat-0.6.1/MovieChat/models/Qformer.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/__init__.py` & `moviechat-0.6.1/MovieChat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/base_model.py` & `moviechat-0.6.1/MovieChat/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/blip2.py` & `moviechat-0.6.1/MovieChat/models/blip2.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/blip2_outputs.py` & `moviechat-0.6.1/MovieChat/models/blip2_outputs.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/chat_model.py` & `moviechat-0.6.1/MovieChat/models/chat_model.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/eva_vit.py` & `moviechat-0.6.1/MovieChat/models/eva_vit.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/eva_vit_with_tome.py` & `moviechat-0.6.1/MovieChat/models/eva_vit_with_tome.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/helpers.py` & `moviechat-0.6.1/MovieChat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/modeling_llama.py` & `moviechat-0.6.1/MovieChat/models/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/moviechat.py` & `moviechat-0.6.1/MovieChat/models/moviechat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import torch
 from torch.cuda.amp import autocast as autocast
 import torch.nn as nn
 
 from MovieChat.common.registry import registry
 from MovieChat.models.blip2 import Blip2Base, disabled_train
 from MovieChat.models.modeling_llama import LlamaForCausalLM
+from MovieChat.common.dist_utils import download_cached_file
+from MovieChat.common.utils import is_url
 from transformers import LlamaTokenizer,BertConfig
 import einops
 import copy
 from MovieChat.models.Qformer import BertConfig, BertLMHeadModel
 
 
 import queue
@@ -155,16 +157,17 @@
 
         logging.info('Loading LLAMA proj')
         self.llama_proj = nn.Linear(
             self.Qformer.config.hidden_size, self.llama_model.config.hidden_size
         )
         if llama_proj_model:
             print("load llama proj weight: {}".format(llama_proj_model))
-            llama_proj_weight = torch.load(llama_proj_model, map_location="cpu")
-            msg = model.load_state_dict(llama_proj_weight['model'], strict=False)
+            # llama_proj_weight = torch.load(llama_proj_model, map_location="cpu")
+            # msg = model.load_state_dict(llama_proj_weight['model'], strict=False)
+            self.load_from_pretrained(url_or_filename=llama_proj_model)
 
         if frozen_llama_proj:
             #  todo frozen  llama_proj
             for name, param in self.llama_proj.named_parameters():
                 param.requires_grad = False
             logging.info('LLAMA proj is frozen')
         else:
@@ -409,16 +412,14 @@
                 query_embeds=video_query_tokens,
                 encoder_hidden_states=frame_hidden_state,
                 encoder_attention_mask=frame_atts,
                 return_dict=True,
             )
             video_hiddens=video_query_output.last_hidden_state 
 
-
-
         # a linear layer to project the output video representations into the same dimension as the text embeddings of LLMs
             inputs_llama = self.llama_proj(video_hiddens)
             atts_llama = torch.ones(inputs_llama.size()[:-1], dtype=torch.long).to(device) 
             return inputs_llama, atts_llama
 
     def encode_image(self, image):
         device = self.device
@@ -628,22 +629,20 @@
                     attention_mask=attention_mask,
                     return_dict=True,
                     labels=targets,
                 )
             loss = outputs.loss
 
         return {"loss": loss}
-
     @classmethod
-    def from_config(self, cls, device):
+    def from_config(cls, device):
         vit_model = "eva_clip_g"
         q_former_model = "https://storage.googleapis.com/sfr-vision-language-research/LAVIS/models/BLIP2/blip2_pretrained_flant5xxl.pth"
         img_size = 224
         num_query_token = 32
-        #TODO type in the path
         llama_model = "Enxin/MovieChat-vicuna"
         drop_path_rate = 0
         use_grad_checkpoint = False
         vit_precision = "fp16"
         freeze_vit = True
         freeze_qformer = True
         low_resource = False
@@ -652,19 +651,22 @@
         max_txt_len = 160
         end_sym = '###'
         frozen_llama_proj = True
         frozen_video_Qformer = True
         fusion_header_type = 'seqTransf'
         max_frame_pos = 32
         fusion_head_layers = 2
-        num_video_query_token =  32
+        num_video_query_token = 32
+        llama_proj_model = "https://huggingface.co/DAMO-NLP-SG/Video-LLaMA-Series/resolve/main/finetune-vicuna7b-v2.pth"
+
 
         model = cls(
             vit_model=vit_model,
             q_former_model=q_former_model,
+            llama_proj_model=llama_proj_model,
             img_size=img_size,
             drop_path_rate=drop_path_rate,
             use_grad_checkpoint=use_grad_checkpoint,
             vit_precision=vit_precision,
             freeze_vit=freeze_vit,
             freeze_qformer=freeze_qformer,
             num_query_token=num_query_token,
@@ -678,8 +680,16 @@
             fusion_header_type=fusion_header_type,
             max_frame_pos=max_frame_pos,
             fusion_head_layers=fusion_head_layers,
             frozen_llama_proj=frozen_llama_proj,
             frozen_video_Qformer=frozen_video_Qformer,
             num_video_query_token=num_video_query_token,
         )
+
+        ckpt_path = "https://huggingface.co/Enxin/MovieChat-proj/blob/main/pretrained_minigpt4.pth"  # load weights of MiniGPT-4
+        if ckpt_path:
+            print("Load first Checkpoint: {}".format(ckpt_path))
+            minigpt4_file = download_cached_file(
+                ckpt_path, check_hash=False, progress=True
+            )
+            msg = torch.load(minigpt4_file, map_location="cpu")
         return model
```

### Comparing `moviechat-0.6.0/MovieChat/models/multimodal_preprocessors.py` & `moviechat-0.6.1/MovieChat/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/models/process_video_data.py` & `moviechat-0.6.1/MovieChat/models/process_video_data.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/__init__.py` & `moviechat-0.6.1/MovieChat/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/base_processor.py` & `moviechat-0.6.1/MovieChat/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/blip_processors.py` & `moviechat-0.6.1/MovieChat/processors/blip_processors.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/functional_video.py` & `moviechat-0.6.1/MovieChat/processors/functional_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/randaugment.py` & `moviechat-0.6.1/MovieChat/processors/randaugment.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/transforms_video.py` & `moviechat-0.6.1/MovieChat/processors/transforms_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/processors/video_processor.py` & `moviechat-0.6.1/MovieChat/processors/video_processor.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/runners/runner_base.py` & `moviechat-0.6.1/MovieChat/runners/runner_base.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/tasks/__init__.py` & `moviechat-0.6.1/MovieChat/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/tasks/base_task.py` & `moviechat-0.6.1/MovieChat/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/tasks/image_text_pretrain.py` & `moviechat-0.6.1/MovieChat/tasks/image_text_pretrain.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/MovieChat/tasks/video_text_pretrain.py` & `moviechat-0.6.1/MovieChat/tasks/video_text_pretrain.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/PKG-INFO` & `moviechat-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviechat
-Version: 0.6.0
+Version: 0.6.1
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `moviechat-0.6.0/moviechat.egg-info/PKG-INFO` & `moviechat-0.6.1/moviechat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviechat
-Version: 0.6.0
+Version: 0.6.1
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `moviechat-0.6.0/moviechat.egg-info/SOURCES.txt` & `moviechat-0.6.1/moviechat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/moviechat.egg-info/requires.txt` & `moviechat-0.6.1/moviechat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moviechat-0.6.0/pyproject.toml` & `moviechat-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moviechat"
-version = "0.6.0"
+version = "0.6.1"
 description = "Long video understanding"
 authors = [
     { name = "Enxin Song", email = "enxin.song.dut@gmail.com" },
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7"
```

