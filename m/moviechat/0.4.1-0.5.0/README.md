# Comparing `tmp/moviechat-0.4.1.tar.gz` & `tmp/moviechat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moviechat-0.4.1.tar", last modified: Fri Apr 19 04:19:00 2024, max compression
+gzip compressed data, was "moviechat-0.5.0.tar", last modified: Fri Apr 19 08:09:48 2024, max compression
```

## Comparing `moviechat-0.4.1.tar` & `moviechat-0.5.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/
--rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.4.1/LICENSE
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/
--rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 04:17:40.000000 moviechat-0.4.1/MovieChat/__init__.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/common/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    15080 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/config.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3620 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/dist_utils.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      815 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/gradcam.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6002 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/logger.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3517 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/optims.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9928 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/registry.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    13808 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/common/utils.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/conversation/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/conversation/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    10954 2024-04-17 09:12:13.000000 moviechat-0.4.1/MovieChat/conversation/conversation_video.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/datasets/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/__init__.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/datasets/builders/
--rw-rw-r--   0 exs       (1016) exs       (1016)     2162 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/builders/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8109 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/builders/base_dataset_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3004 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/builders/image_text_pair_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2393 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/builders/instruct_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      987 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/builders/video_caption_builder.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6283 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/data_utils.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.737846 moviechat-0.4.1/MovieChat/datasets/datasets/
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2067 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/base_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2602 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/caption_datasets.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     1669 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/cc_sbu_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4214 2024-04-17 09:11:31.000000 moviechat-0.4.1/MovieChat/datasets/datasets/dataloader_utils.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     1175 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/laion_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8785 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/llava_instruct_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9701 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/video_instruct_dataset.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4437 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/datasets/datasets/webvid_datasets.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/MovieChat/models/
--rw-rw-r--   0 exs       (1016) exs       (1016)    48450 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/Qformer.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4289 2024-04-19 03:58:05.000000 moviechat-0.4.1/MovieChat/models/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     7147 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/base_model.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     7795 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/blip2.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     2331 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/blip2_outputs.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     9161 2024-04-18 14:38:08.000000 moviechat-0.4.1/MovieChat/models/chat_model.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    18684 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/eva_vit.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    14489 2024-04-17 09:11:15.000000 moviechat-0.4.1/MovieChat/models/eva_vit_with_tome.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3989 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/helpers.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    33326 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/modeling_llama.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    32438 2024-04-18 14:38:48.000000 moviechat-0.4.1/MovieChat/models/moviechat.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    23136 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/multimodal_preprocessors.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    11438 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/models/process_video_data.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/MovieChat/processors/
--rw-rw-r--   0 exs       (1016) exs       (1016)      999 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      610 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/base_processor.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     4008 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/blip_processors.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     3924 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/functional_video.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    10960 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/randaugment.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     5017 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/transforms_video.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     6959 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/processors/video_processor.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/MovieChat/runners/
--rw-rw-r--   0 exs       (1016) exs       (1016)      307 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/runners/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)    22856 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/runners/runner_base.py
--rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/runners/test.py
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/MovieChat/tasks/
--rw-rw-r--   0 exs       (1016) exs       (1016)      837 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/tasks/__init__.py
--rw-rw-r--   0 exs       (1016) exs       (1016)     8799 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/tasks/base_task.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/tasks/image_text_pretrain.py
--rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.4.1/MovieChat/tasks/video_text_pretrain.py
--rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 04:19:00.741846 moviechat-0.4.1/PKG-INFO
-drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 04:19:00.741846 moviechat-0.4.1/moviechat.egg-info/
--rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 04:19:00.000000 moviechat-0.4.1/moviechat.egg-info/PKG-INFO
--rw-rw-r--   0 exs       (1016) exs       (1016)     2166 2024-04-19 04:19:00.000000 moviechat-0.4.1/moviechat.egg-info/SOURCES.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-19 04:19:00.000000 moviechat-0.4.1/moviechat.egg-info/dependency_links.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 04:19:00.000000 moviechat-0.4.1/moviechat.egg-info/requires.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)       10 2024-04-19 04:19:00.000000 moviechat-0.4.1/moviechat.egg-info/top_level.txt
--rw-rw-r--   0 exs       (1016) exs       (1016)     1804 2024-04-19 04:18:28.000000 moviechat-0.4.1/pyproject.toml
--rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-19 04:19:00.741846 moviechat-0.4.1/setup.cfg
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1501 2024-04-17 05:16:47.000000 moviechat-0.5.0/LICENSE
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 04:17:40.000000 moviechat-0.5.0/MovieChat/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/common/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    15080 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/config.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3620 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/dist_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      815 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/gradcam.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6002 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/logger.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3517 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/optims.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9928 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/registry.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    13808 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/common/utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/conversation/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/conversation/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10954 2024-04-17 09:12:13.000000 moviechat-0.5.0/MovieChat/conversation/conversation_video.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/__init__.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/datasets/builders/
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2162 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/builders/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8109 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/builders/base_dataset_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3004 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/builders/image_text_pair_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2393 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/builders/instruct_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      987 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/builders/video_caption_builder.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6283 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/data_utils.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.153642 moviechat-0.5.0/MovieChat/datasets/datasets/
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2067 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/base_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2602 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/caption_datasets.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1669 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/cc_sbu_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4214 2024-04-17 09:11:31.000000 moviechat-0.5.0/MovieChat/datasets/datasets/dataloader_utils.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1175 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/laion_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8785 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/llava_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9701 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/video_instruct_dataset.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4437 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/datasets/datasets/webvid_datasets.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/MovieChat/models/
+-rw-rw-r--   0 exs       (1016) exs       (1016)    48450 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/Qformer.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4289 2024-04-19 03:58:05.000000 moviechat-0.5.0/MovieChat/models/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7147 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/base_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     7795 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/blip2.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2331 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/blip2_outputs.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     9161 2024-04-18 14:38:08.000000 moviechat-0.5.0/MovieChat/models/chat_model.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    18684 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/eva_vit.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    14489 2024-04-17 09:11:15.000000 moviechat-0.5.0/MovieChat/models/eva_vit_with_tome.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3989 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/helpers.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    33326 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/modeling_llama.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    31253 2024-04-19 08:09:06.000000 moviechat-0.5.0/MovieChat/models/moviechat.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    23136 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/multimodal_preprocessors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    11438 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/models/process_video_data.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/MovieChat/processors/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      999 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      610 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/base_processor.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     4008 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/blip_processors.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     3924 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/functional_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    10960 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/randaugment.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     5017 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/transforms_video.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     6959 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/processors/video_processor.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/MovieChat/runners/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      307 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/runners/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)    22856 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/runners/runner_base.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)        0 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/runners/test.py
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/MovieChat/tasks/
+-rw-rw-r--   0 exs       (1016) exs       (1016)      837 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/tasks/__init__.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)     8799 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/tasks/base_task.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/tasks/image_text_pretrain.py
+-rw-rw-r--   0 exs       (1016) exs       (1016)      540 2024-04-17 05:16:51.000000 moviechat-0.5.0/MovieChat/tasks/video_text_pretrain.py
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 08:09:48.157642 moviechat-0.5.0/PKG-INFO
+drwxrwxr-x   0 exs       (1016) exs       (1016)        0 2024-04-19 08:09:48.157642 moviechat-0.5.0/moviechat.egg-info/
+-rw-r--r--   0 exs       (1016) exs       (1016)     2047 2024-04-19 08:09:48.000000 moviechat-0.5.0/moviechat.egg-info/PKG-INFO
+-rw-rw-r--   0 exs       (1016) exs       (1016)     2166 2024-04-19 08:09:48.000000 moviechat-0.5.0/moviechat.egg-info/SOURCES.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)        1 2024-04-19 08:09:48.000000 moviechat-0.5.0/moviechat.egg-info/dependency_links.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)      905 2024-04-19 08:09:48.000000 moviechat-0.5.0/moviechat.egg-info/requires.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)       10 2024-04-19 08:09:48.000000 moviechat-0.5.0/moviechat.egg-info/top_level.txt
+-rw-rw-r--   0 exs       (1016) exs       (1016)     1804 2024-04-19 08:09:29.000000 moviechat-0.5.0/pyproject.toml
+-rw-rw-r--   0 exs       (1016) exs       (1016)       38 2024-04-19 08:09:48.157642 moviechat-0.5.0/setup.cfg
```

### Comparing `moviechat-0.4.1/LICENSE` & `moviechat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/__init__.py` & `moviechat-0.5.0/MovieChat/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/config.py` & `moviechat-0.5.0/MovieChat/common/config.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/dist_utils.py` & `moviechat-0.5.0/MovieChat/common/dist_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/gradcam.py` & `moviechat-0.5.0/MovieChat/common/gradcam.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/logger.py` & `moviechat-0.5.0/MovieChat/common/logger.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/optims.py` & `moviechat-0.5.0/MovieChat/common/optims.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/registry.py` & `moviechat-0.5.0/MovieChat/common/registry.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/common/utils.py` & `moviechat-0.5.0/MovieChat/common/utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/conversation/conversation_video.py` & `moviechat-0.5.0/MovieChat/conversation/conversation_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/builders/__init__.py` & `moviechat-0.5.0/MovieChat/datasets/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/builders/base_dataset_builder.py` & `moviechat-0.5.0/MovieChat/datasets/builders/base_dataset_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/builders/image_text_pair_builder.py` & `moviechat-0.5.0/MovieChat/datasets/builders/image_text_pair_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/builders/instruct_builder.py` & `moviechat-0.5.0/MovieChat/datasets/builders/instruct_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/builders/video_caption_builder.py` & `moviechat-0.5.0/MovieChat/datasets/builders/video_caption_builder.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/data_utils.py` & `moviechat-0.5.0/MovieChat/datasets/data_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/base_dataset.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/caption_datasets.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/caption_datasets.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/cc_sbu_dataset.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/cc_sbu_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/dataloader_utils.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/laion_dataset.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/laion_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/llava_instruct_dataset.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/llava_instruct_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/video_instruct_dataset.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/video_instruct_dataset.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/datasets/datasets/webvid_datasets.py` & `moviechat-0.5.0/MovieChat/datasets/datasets/webvid_datasets.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/Qformer.py` & `moviechat-0.5.0/MovieChat/models/Qformer.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/__init__.py` & `moviechat-0.5.0/MovieChat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/base_model.py` & `moviechat-0.5.0/MovieChat/models/base_model.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/blip2.py` & `moviechat-0.5.0/MovieChat/models/blip2.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/blip2_outputs.py` & `moviechat-0.5.0/MovieChat/models/blip2_outputs.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/chat_model.py` & `moviechat-0.5.0/MovieChat/models/chat_model.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/eva_vit.py` & `moviechat-0.5.0/MovieChat/models/eva_vit.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/eva_vit_with_tome.py` & `moviechat-0.5.0/MovieChat/models/eva_vit_with_tome.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/helpers.py` & `moviechat-0.5.0/MovieChat/models/helpers.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/modeling_llama.py` & `moviechat-0.5.0/MovieChat/models/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/moviechat.py` & `moviechat-0.5.0/MovieChat/models/moviechat.py`

 * *Files 6% similar despite different names*

```diff
@@ -630,43 +630,38 @@
                     labels=targets,
                 )
             loss = outputs.loss
 
         return {"loss": loss}
 
     @classmethod
-    def from_config(cls, cfg, device):
-        vit_model = cfg.get("vit_model", "eva_clip_g")
-        q_former_model = cfg.get("q_former_model", "https://storage.googleapis.com/sfr-vision-language-research/LAVIS/models/BLIP2/blip2_pretrained_flant5xxl.pth")
-        img_size = cfg.get("image_size")
-        num_query_token = cfg.get("num_query_token")
-        llama_model = cfg.get("llama_model")
+    def from_config(cls, device):
+        vit_model = "eva_clip_g"
+        q_former_model = "https://storage.googleapis.com/sfr-vision-language-research/LAVIS/models/BLIP2/blip2_pretrained_flant5xxl.pth"
+        img_size = 224
+        num_query_token = 32
+        #TODO type in the path
+        llama_model = "Enxin/MovieChat-vicuna"
+        drop_path_rate = 0
+        use_grad_checkpoint = False
+        vit_precision = "fp16"
+        freeze_vit = True
+        freeze_qformer = True
+        low_resource = False
+        prompt_path = ""
+        prompt_template = ""
+        max_txt_len = 160
+        end_sym = '###'
+        frozen_llama_proj = True
+        frozen_video_Qformer = True
+        fusion_header_type = 'seqTransf'
+        max_frame_pos = 32
+        fusion_head_layers = 2
+        num_video_query_token =  32
 
-        drop_path_rate = cfg.get("drop_path_rate", 0)
-        use_grad_checkpoint = cfg.get("use_grad_checkpoint", False)
-        vit_precision = cfg.get("vit_precision", "fp16")
-        freeze_vit = cfg.get("freeze_vit", True)
-        freeze_qformer = cfg.get("freeze_qformer", True)
-        low_resource = cfg.get("low_resource", False)
-        device_8bit = cfg.get("device_8bit", 0)
-
-        prompt_path = cfg.get("prompt_path", "")
-        prompt_template = cfg.get("prompt_template", "")
-        max_txt_len = cfg.get("max_txt_len", 32)
-        end_sym = cfg.get("end_sym", '\n')
-        
-        frozen_llama_proj = cfg.get("frozen_llama_proj", True)
-        frozen_video_Qformer = cfg.get("frozen_video_Qformer", True)
-
-        llama_proj_model = cfg.get("llama_proj_model", '')
-
-        fusion_header_type = cfg.get("fusion_header_type", 'seqTransf')
-        max_frame_pos = cfg.get("max_frame_pos", 32)
-        fusion_head_layers = cfg.get("fusion_head_layers", 2)
-        num_video_query_token =  cfg.get("num_video_query_token", 32)
         model = cls(
             vit_model=vit_model,
             q_former_model=q_former_model,
             img_size=img_size,
             drop_path_rate=drop_path_rate,
             use_grad_checkpoint=use_grad_checkpoint,
             vit_precision=vit_precision,
@@ -675,27 +670,16 @@
             num_query_token=num_query_token,
             llama_model=llama_model,
             prompt_path=prompt_path,
             prompt_template=prompt_template,
             max_txt_len=max_txt_len,
             end_sym=end_sym,
             low_resource=low_resource,
-            device_8bit=device_8bit,
+            device_8bit=device,
             fusion_header_type=fusion_header_type,
             max_frame_pos=max_frame_pos,
             fusion_head_layers=fusion_head_layers,
             frozen_llama_proj=frozen_llama_proj,
             frozen_video_Qformer=frozen_video_Qformer,
             num_video_query_token=num_video_query_token,
         )
-
-        ckpt_path = cfg.get("ckpt", "")  # load weights of MiniGPT-4
-        if ckpt_path:
-            print("Load first Checkpoint: {}".format(ckpt_path))
-            ckpt = torch.load(ckpt_path, map_location=device)
-            msg = model.load_state_dict(ckpt['model'], strict=False)
-        ckpt_path_2 = cfg.get("ckpt_2", "")  
-        if ckpt_path_2:
-            print("Load second Checkpoint: {}".format(ckpt_path_2))
-            ckpt = torch.load(ckpt_path_2, map_location=device)
-            msg = model.load_state_dict(ckpt['model'], strict=False)
         return model
```

### Comparing `moviechat-0.4.1/MovieChat/models/multimodal_preprocessors.py` & `moviechat-0.5.0/MovieChat/models/multimodal_preprocessors.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/models/process_video_data.py` & `moviechat-0.5.0/MovieChat/models/process_video_data.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/__init__.py` & `moviechat-0.5.0/MovieChat/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/base_processor.py` & `moviechat-0.5.0/MovieChat/processors/base_processor.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/blip_processors.py` & `moviechat-0.5.0/MovieChat/processors/blip_processors.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/functional_video.py` & `moviechat-0.5.0/MovieChat/processors/functional_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/randaugment.py` & `moviechat-0.5.0/MovieChat/processors/randaugment.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/transforms_video.py` & `moviechat-0.5.0/MovieChat/processors/transforms_video.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/processors/video_processor.py` & `moviechat-0.5.0/MovieChat/processors/video_processor.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/runners/runner_base.py` & `moviechat-0.5.0/MovieChat/runners/runner_base.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/tasks/__init__.py` & `moviechat-0.5.0/MovieChat/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/tasks/base_task.py` & `moviechat-0.5.0/MovieChat/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/tasks/image_text_pretrain.py` & `moviechat-0.5.0/MovieChat/tasks/image_text_pretrain.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/MovieChat/tasks/video_text_pretrain.py` & `moviechat-0.5.0/MovieChat/tasks/video_text_pretrain.py`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/PKG-INFO` & `moviechat-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviechat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `moviechat-0.4.1/moviechat.egg-info/PKG-INFO` & `moviechat-0.5.0/moviechat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moviechat
-Version: 0.4.1
+Version: 0.5.0
 Summary: Long video understanding
 Author-email: Enxin Song <enxin.song.dut@gmail.com>
 License: MIT License
 Project-URL: homepage, https://rese1f.github.io/MovieChat/
 Project-URL: repository, https://github.com/rese1f/MovieChat
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `moviechat-0.4.1/moviechat.egg-info/SOURCES.txt` & `moviechat-0.5.0/moviechat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/moviechat.egg-info/requires.txt` & `moviechat-0.5.0/moviechat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moviechat-0.4.1/pyproject.toml` & `moviechat-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moviechat"
-version = "0.4.1"
+version = "0.5.0"
 description = "Long video understanding"
 authors = [
     { name = "Enxin Song", email = "enxin.song.dut@gmail.com" },
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7"
```

