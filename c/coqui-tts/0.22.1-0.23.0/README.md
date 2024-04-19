# Comparing `tmp/coqui-tts-0.22.1.tar.gz` & `tmp/coqui_tts-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coqui-tts-0.22.1.tar", last modified: Wed Apr  3 12:59:50 2024, max compression
+gzip compressed data, was "coqui_tts-0.23.0.tar", last modified: Fri Apr 19 12:26:04 2024, max compression
```

## Comparing `coqui-tts-0.22.1.tar` & `coqui_tts-0.23.0.tar`

### file list

```diff
@@ -1,390 +1,390 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.539300 coqui-tts-0.22.1/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-04-03 12:59:50.539300 coqui-tts-0.22.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.487300 coqui-tts-0.22.1/TTS/
--rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/.models.json
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20568 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.487300 coqui-tts-0.22.1/TTS/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/collect_env_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/compute_attention_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/compute_embeddings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3175 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/compute_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/eval_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9486 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/extract_tts_spectrograms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/find_unique_chars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/find_unique_phonemes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4263 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/remove_silence_using_vad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/resample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16167 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12251 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/train_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/train_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/train_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/bin/tune_wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/config/shared_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.479300 coqui-tts-0.22.1/TTS/demos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/utils/gpt_train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14796 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/xtts_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/encoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/encoder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/configs/base_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/configs/emotion_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/configs/speaker_encoder_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/encoder/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/models/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/models/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/encoder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/utils/prepare_voxceleb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/encoder/utils/visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.491300 coqui-tts-0.22.1/TTS/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/static/coqui-log-green-TTS.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.495300 coqui-tts-0.22.1/TTS/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/templates/details.html
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.495300 coqui-tts-0.22.1/TTS/tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.495300 coqui-tts-0.22.1/TTS/tts/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/align_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/bark_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/delightful_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/fast_pitch_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/fast_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/fastspeech2_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/glow_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/neuralhmm_tts_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/overflow_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/speedy_speech_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/tacotron2_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/tacotron_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/tortoise_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/vits_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/configs/xtts_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.495300 coqui-tts-0.22.1/TTS/tts/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38166 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    27943 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/datasets/formatters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.495300 coqui-tts-0.22.1/TTS/tts/layers/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.499300 coqui-tts-0.22.1/TTS/tts/layers/align_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/align_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/align_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/align_tts/mdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.499300 coqui-tts-0.22.1/TTS/tts/layers/bark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.499300 coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/hubert_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/kmeans_hubert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/inference_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/bark/model_fine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.499300 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23482 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/acoustic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/conformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/conv_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/energy_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/kernel_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/pitch_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/variance_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.499300 coqui-tts-0.22.1/TTS/tts/layers/feed_forward/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/feed_forward/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/feed_forward/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/feed_forward/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/feed_forward/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.503300 coqui-tts-0.22.1/TTS/tts/layers/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/aligner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/pos_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/res_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/time_depth_sep_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/generic/wavenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.503300 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/glow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/glow_tts/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.503300 coqui-tts-0.22.1/TTS/tts/layers/overflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/overflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11736 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/overflow/common_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/overflow/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/overflow/neural_hmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/overflow/plotting_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.503300 coqui-tts-0.22.1/TTS/tts/layers/tacotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/attentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/capacitron_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/common_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/gst_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18785 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15855 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tacotron/tacotron2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.507300 coqui-tts-0.22.1/TTS/tts/layers/tortoise/
--rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/arch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/audio_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/autoregressive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/clvp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51012 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/diffusion_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    72285 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/random_latent_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/wav2vec_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    41480 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/tortoise/xtransformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.507300 coqui-tts-0.22.1/TTS/tts/layers/vits/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/vits/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/vits/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/vits/stochastic_duration_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/vits/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.511300 coqui-tts-0.22.1/TTS/tts/layers/xtts/
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/dvae.py
--rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/gpt_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/hifigan_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/latent_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/perceiver_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46561 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/stream_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    30757 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.511300 coqui-tts-0.22.1/TTS/tts/layers/xtts/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/trainer/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20516 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/trainer/gpt_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/xtts_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    59330 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/layers/xtts/zh_num2words.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.511300 coqui-tts-0.22.1/TTS/tts/models/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/align_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/bark.py
--rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/base_tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    20130 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/base_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    70316 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/delightful_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    35609 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/forward_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/glow_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17346 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/neuralhmm_tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/overflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/tacotron.py
--rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/tacotron2.py
--rw-r--r--   0 runner    (1001) docker     (127)    42355 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/tortoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    81919 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/vits.py
--rw-r--r--   0 runner    (1001) docker     (127)    32343 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/models/xtts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.479300 coqui-tts-0.22.1/TTS/tts/utils/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/assets/tortoise/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/assets/tortoise/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/fairseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   868695 2024-04-03 12:59:49.000000 coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     9625 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/speakers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/ssim.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/text/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/text/bangla/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/bangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/bangla/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.515300 coqui-tts-0.22.1/TTS/tts/utils/text/belarusian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/belarusian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/belarusian/phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16571 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/characters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/cmudict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/english/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/english/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/english/abbreviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/english/number_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/english/time_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/french/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/french/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/french/abbreviations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/japanese/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/japanese/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/japanese/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/korean/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/korean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/korean/ko_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/korean/korean.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/korean/phonemizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.519300 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/text/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/tts/utils/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/utils/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/audio/numpy_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    23635 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/audio/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/audio/torch_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/capacitron_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/distribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/radam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22890 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/synthesizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/utils/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.483300 coqui-tts-0.22.1/TTS/vc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/vc/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/configs/freevc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/configs/shared_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/vc/models/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/models/base_vc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/models/freevc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/vc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.523300 coqui-tts-0.22.1/TTS/vc/modules/freevc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/mel_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.527300 coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.527300 coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/wavlm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.527300 coqui-tts-0.22.1/TTS/vocoder/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.527300 coqui-tts-0.22.1/TTS/vocoder/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/fullband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/hifigan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/multiband_melgan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/parallel_wavegan_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/shared_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/univnet_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/wavegrad_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/configs/wavernn_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.527300 coqui-tts-0.22.1/TTS/vocoder/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/datasets/gan_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/datasets/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/datasets/wavegrad_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/datasets/wavernn_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.531300 coqui-tts-0.22.1/TTS/vocoder/layers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/hifigan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/lvc_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/melgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/parallel_wavegan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/pqmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/layers/wavegrad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.531300 coqui-tts-0.22.1/TTS/vocoder/models/
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/base_vocoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/fullband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14587 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/hifigan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/hifigan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/melgan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/melgan_multiscale_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/multiband_melgan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/parallel_wavegan_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/parallel_wavegan_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/random_window_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/univnet_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/univnet_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/wavegrad.py
--rw-r--r--   0 runner    (1001) docker     (127)    25233 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/models/wavernn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.531300 coqui-tts-0.22.1/TTS/vocoder/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/utils/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/TTS/vocoder/utils/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.535300 coqui-tts-0.22.1/coqui_tts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:59:49.000000 coqui-tts-0.22.1/coqui_tts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 12:59:50.000000 coqui-tts-0.22.1/coqui_tts.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:59:50.535300 coqui-tts-0.22.1/images/
--rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/images/coqui-log-green-TTS.png
--rw-r--r--   0 runner    (1001) docker     (127)   474464 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/images/example_model_output.png
--rw-r--r--   0 runner    (1001) docker     (127)   149914 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/images/model.png
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/requirements.ja.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/requirements.notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 12:59:50.539300 coqui-tts-0.22.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-03 12:59:37.000000 coqui-tts-0.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.784660 coqui_tts-0.23.0/TTS/
+-rw-r--r--   0 runner    (1001) docker     (127)    44046 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/.models.json
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20591 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/collect_env_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_attention_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_embeddings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/compute_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/eval_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9602 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/extract_tts_spectrograms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/find_unique_chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/find_unique_phonemes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4433 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/remove_silence_using_vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16672 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/synthesize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/train_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/bin/tune_wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/config/shared_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.772660 coqui_tts-0.23.0/TTS/demos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/gpt_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/xtts_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.788660 coqui_tts-0.23.0/TTS/encoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/base_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/emotion_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/configs/speaker_encoder_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/encoder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/models/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/encoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/prepare_voxceleb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/encoder/utils/visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/static/coqui-log-green-TTS.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.792660 coqui_tts-0.23.0/TTS/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/align_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/bark_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/delightful_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fast_pitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fast_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/fastspeech2_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/glow_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/neuralhmm_tts_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/overflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/speedy_speech_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tacotron2_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tacotron_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/tortoise_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/vits_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/configs/xtts_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37839 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28004 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/datasets/formatters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/align_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/align_tts/mdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.796660 coqui_tts-0.23.0/TTS/tts/layers/bark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/hubert_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/kmeans_hubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26202 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/inference_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/bark/model_fine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/acoustic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17806 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23945 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conv_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/energy_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/kernel_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/pitch_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/variance_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.800660 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/feed_forward/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/aligner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/pos_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/res_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/time_depth_sep_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/generic/wavenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/glow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/glow_tts/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35686 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/overflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/common_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/neural_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/overflow/plotting_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.804660 coqui_tts-0.23.0/TTS/tts/layers/tacotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/attentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/capacitron_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/common_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/gst_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.808660 coqui_tts-0.23.0/TTS/tts/layers/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (127)    14530 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/arch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/audio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/autoregressive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/clvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51012 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72348 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/random_latent_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14445 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/wav2vec_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41480 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/tortoise/xtransformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.808660 coqui_tts-0.23.0/TTS/tts/layers/vits/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/stochastic_duration_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/vits/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.812660 coqui_tts-0.23.0/TTS/tts/layers/xtts/
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/dvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23051 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25094 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/hifigan_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/latent_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/perceiver_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46561 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/stream_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31005 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.812660 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/gpt_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/xtts_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59442 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/layers/xtts/zh_num2words.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/align_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10480 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/bark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/base_tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20192 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/base_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70351 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/delightful_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/forward_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24259 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/glow_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17382 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/neuralhmm_tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/overflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tacotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19645 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tacotron2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42373 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/tortoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81986 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/vits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32412 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/models/xtts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.776660 coqui_tts-0.23.0/TTS/tts/utils/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.816660 coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/fairseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   868695 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/speakers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14962 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/bangla/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/cmudict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.820660 coqui_tts-0.23.0/TTS/tts/utils/text/english/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/abbreviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/number_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/english/time_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/french/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/french/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/french/abbreviations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/japanese/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/korean/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/ko_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/korean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/korean/phonemizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.824660 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/text/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/tts/utils/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/utils/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/numpy_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/audio/torch_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/capacitron_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/distribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28269 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/radam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22967 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/synthesizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/utils/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.780660 coqui_tts-0.23.0/TTS/vc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/freevc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/configs/shared_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18826 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/base_vc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/models/freevc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.828660 coqui_tts-0.23.0/TTS/vc/modules/freevc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/mel_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/wavlm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.832660 coqui_tts-0.23.0/TTS/vocoder/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/fullband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/hifigan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/multiband_melgan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/parallel_wavegan_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/shared_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/univnet_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/wavegrad_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/configs/wavernn_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.836660 coqui_tts-0.23.0/TTS/vocoder/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/gan_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/wavegrad_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/datasets/wavernn_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.836660 coqui_tts-0.23.0/TTS/vocoder/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/lvc_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/melgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/parallel_wavegan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/pqmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/layers/wavegrad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/TTS/vocoder/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/base_vocoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/fullband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14527 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/hifigan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10678 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/hifigan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/melgan_multiscale_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/multiband_melgan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/random_window_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/univnet_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/univnet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/wavegrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25204 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/models/wavernn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/TTS/vocoder/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/TTS/vocoder/utils/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/coqui_tts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20190 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11216 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 12:26:04.000000 coqui_tts-0.23.0/coqui_tts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:26:04.840660 coqui_tts-0.23.0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    61564 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/coqui-log-green-TTS.png
+-rw-r--r--   0 runner    (1001) docker     (127)   474464 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/example_model_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)   149914 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/images/model.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.ja.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 12:26:04.844660 coqui_tts-0.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-19 12:25:50.000000 coqui_tts-0.23.0/setup.py
```

### Comparing `coqui-tts-0.22.1/CITATION.cff` & `coqui_tts-0.23.0/CITATION.cff`

 * *Files 27% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 authors:
   - family-names: "Eren"
     given-names: "Gölge"
   - name: "The Coqui TTS Team"
 version: 1.4
 doi: 10.5281/zenodo.6334862
 license: "MPL-2.0"
-url: "https://github.com/eginhard/coqui-tts"
-repository-code: "https://github.com/eginhard/coqui-tts"
+url: "https://github.com/idiap/coqui-ai-TTS"
+repository-code: "https://github.com/idiap/coqui-ai-TTS"
 keywords:
   - machine learning
   - deep learning
   - artificial intelligence
   - text to speech
   - TTS
```

### Comparing `coqui-tts-0.22.1/LICENSE.txt` & `coqui_tts-0.23.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/PKG-INFO` & `coqui_tts-0.23.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: coqui-tts
-Version: 0.22.1
+Version: 0.23.0
 Summary: Deep learning for Text to Speech.
-Home-page: https://github.com/eginhard/coqui-tts
+Home-page: https://github.com/idiap/coqui-ai-TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://coqui-tts.readthedocs.io
-Project-URL: Tracker, https://github.com/eginhard/coqui-tts/issues
-Project-URL: Repository, https://github.com/eginhard/coqui-tts
-Project-URL: Discussions, https://github.com/eginhard/coqui-tts/discussions
+Project-URL: Tracker, https://github.com/idiap/coqui-ai-TTS/issues
+Project-URL: Repository, https://github.com/idiap/coqui-ai-TTS
+Project-URL: Discussions, https://github.com/idiap/coqui-ai-TTS/discussions
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -86,48 +86,49 @@
 Requires-Dist: flask>=2.0.1; extra == "server"
 Provides-Extra: ja
 Requires-Dist: mecab-python3==1.0.6; extra == "ja"
 Requires-Dist: unidic-lite==1.0.8; extra == "ja"
 Requires-Dist: cutlet; extra == "ja"
 
 
-## 🐸Coqui.ai News
+## 🐸Coqui TTS News
+- 📣 Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)
 - 📣 ⓍTTSv2 is here with 16 languages and better performance across the board.
-- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/eginhard/coqui-tts/tree/dev/recipes/ljspeech).
+- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/idiap/coqui-ai-TTS/tree/dev/recipes/ljspeech).
 - 📣 ⓍTTS can now stream with <200ms latency.
 - 📣 ⓍTTS, our production TTS model that can speak 13 languages, is released [Blog Post](https://coqui.ai/blog/tts/open_xtts), [Demo](https://huggingface.co/spaces/coqui/xtts), [Docs](https://coqui-tts.readthedocs.io/en/dev/models/xtts.html)
 - 📣 [🐶Bark](https://github.com/suno-ai/bark) is now available for inference with unconstrained voice cloning. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/bark.html)
 - 📣 You can use [~1100 Fairseq models](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) with 🐸TTS.
 - 📣 🐸TTS now supports 🐢Tortoise with faster inference. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/tortoise.html)
 
 <div align="center">
 <img src="https://static.scarf.sh/a.png?x-pxid=cf317fe7-2188-4721-bc01-124bb5d5dbb2" />
 
-## <img src="https://raw.githubusercontent.com/eginhard/coqui-tts/main/images/coqui-log-green-TTS.png" height="56"/>
+## <img src="https://raw.githubusercontent.com/idiap/coqui-ai-TTS/main/images/coqui-log-green-TTS.png" height="56"/>
 
 
 **🐸TTS is a library for advanced Text-to-Speech generation.**
 
 🚀 Pretrained models in +1100 languages.
 
 🛠️ Tools for training new models and fine-tuning existing models in any language.
 
 📚 Utilities for dataset analysis and curation.
 ______________________________________________________________________
 
 [![Discord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
-[![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
-[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/eginhard/coqui-tts/blob/main/CODE_OF_CONDUCT.md)
-[![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
+[![PyPI version](https://badge.fury.io/py/coqui-tts.svg)](https://badge.fury.io/py/coqui-tts)
+[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/idiap/coqui-ai-TTS/blob/main/CODE_OF_CONDUCT.md)
+[![Downloads](https://pepy.tech/badge/coqui-tts)](https://pepy.tech/project/coqui-tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/tests.yml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/docker.yaml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/style_check.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/tests.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/docker.yaml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/style_check.yml/badge.svg)
 [![Docs](<https://readthedocs.org/projects/coqui-tts/badge/?version=latest&style=plastic>)](https://coqui-tts.readthedocs.io/en/latest/)
 
 </div>
 
 ______________________________________________________________________
 
 ## 💬 Where to ask questions
@@ -136,28 +137,28 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
 | 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
-[github issue tracker]: https://github.com/eginhard/coqui-tts/issues
-[github discussions]: https://github.com/eginhard/coqui-tts/discussions
+[github issue tracker]: https://github.com/idiap/coqui-ai-TTS/issues
+[github discussions]: https://github.com/idiap/coqui-ai-TTS/discussions
 [discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://coqui-tts.readthedocs.io/en/latest/)
-| 💾 **Installation**               | [TTS/README.md](https://github.com/eginhard/coqui-tts/tree/dev#installation)|
-| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/eginhard/coqui-tts/blob/main/CONTRIBUTING.md)|
+| 💾 **Installation**               | [TTS/README.md](https://github.com/idiap/coqui-ai-TTS/tree/dev#installation)|
+| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/idiap/coqui-ai-TTS/blob/main/CONTRIBUTING.md)|
 | 📌 **Road Map**                   | [Main Development Plans](https://github.com/coqui-ai/TTS/issues/378)
-| 🚀 **Released Models**            | [Standard models](https://github.com/eginhard/coqui-tts/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/eginhard/coqui-tts#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
+| 🚀 **Released Models**            | [Standard models](https://github.com/idiap/coqui-ai-TTS/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/idiap/coqui-ai-TTS#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
 | 📰 **Papers**                    | [TTS Papers](https://github.com/erogol/TTS-papers)|
 
 ## Features
 - High-performance Deep Learning models for Text2Speech tasks.
     - Text2Spec models (Tacotron, Tacotron2, Glow-TTS, SpeedySpeech).
     - Speaker Encoder to compute speaker embeddings efficiently.
     - Vocoder models (MelGAN, Multiband-MelGAN, GAN-TTS, ParallelWaveGAN, WaveGrad, WaveRNN)
@@ -217,26 +218,26 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 18.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
 
 If you plan to code or train models, clone 🐸TTS and install it locally.
 
 ```bash
-git clone https://github.com/eginhard/coqui-tts
+git clone https://github.com/idiap/coqui-ai-TTS
 pip install -e .[all,dev,notebooks,server]  # Select the relevant extras
 ```
 
 If you are on Ubuntu (Debian), you can also run following commands for installation.
 
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
```

### Comparing `coqui-tts-0.22.1/README.md` & `coqui_tts-0.23.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 
-## 🐸Coqui.ai News
+## 🐸Coqui TTS News
+- 📣 Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)
 - 📣 ⓍTTSv2 is here with 16 languages and better performance across the board.
-- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/eginhard/coqui-tts/tree/dev/recipes/ljspeech).
+- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/idiap/coqui-ai-TTS/tree/dev/recipes/ljspeech).
 - 📣 ⓍTTS can now stream with <200ms latency.
 - 📣 ⓍTTS, our production TTS model that can speak 13 languages, is released [Blog Post](https://coqui.ai/blog/tts/open_xtts), [Demo](https://huggingface.co/spaces/coqui/xtts), [Docs](https://coqui-tts.readthedocs.io/en/dev/models/xtts.html)
 - 📣 [🐶Bark](https://github.com/suno-ai/bark) is now available for inference with unconstrained voice cloning. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/bark.html)
 - 📣 You can use [~1100 Fairseq models](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) with 🐸TTS.
 - 📣 🐸TTS now supports 🐢Tortoise with faster inference. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/tortoise.html)
 
 <div align="center">
 <img src="https://static.scarf.sh/a.png?x-pxid=cf317fe7-2188-4721-bc01-124bb5d5dbb2" />
 
-## <img src="https://raw.githubusercontent.com/eginhard/coqui-tts/main/images/coqui-log-green-TTS.png" height="56"/>
+## <img src="https://raw.githubusercontent.com/idiap/coqui-ai-TTS/main/images/coqui-log-green-TTS.png" height="56"/>
 
 
 **🐸TTS is a library for advanced Text-to-Speech generation.**
 
 🚀 Pretrained models in +1100 languages.
 
 🛠️ Tools for training new models and fine-tuning existing models in any language.
 
 📚 Utilities for dataset analysis and curation.
 ______________________________________________________________________
 
 [![Discord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
-[![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
-[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/eginhard/coqui-tts/blob/main/CODE_OF_CONDUCT.md)
-[![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
+[![PyPI version](https://badge.fury.io/py/coqui-tts.svg)](https://badge.fury.io/py/coqui-tts)
+[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/idiap/coqui-ai-TTS/blob/main/CODE_OF_CONDUCT.md)
+[![Downloads](https://pepy.tech/badge/coqui-tts)](https://pepy.tech/project/coqui-tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/tests.yml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/docker.yaml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/style_check.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/tests.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/docker.yaml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/style_check.yml/badge.svg)
 [![Docs](<https://readthedocs.org/projects/coqui-tts/badge/?version=latest&style=plastic>)](https://coqui-tts.readthedocs.io/en/latest/)
 
 </div>
 
 ______________________________________________________________________
 
 ## 💬 Where to ask questions
@@ -45,28 +46,28 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
 | 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
-[github issue tracker]: https://github.com/eginhard/coqui-tts/issues
-[github discussions]: https://github.com/eginhard/coqui-tts/discussions
+[github issue tracker]: https://github.com/idiap/coqui-ai-TTS/issues
+[github discussions]: https://github.com/idiap/coqui-ai-TTS/discussions
 [discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://coqui-tts.readthedocs.io/en/latest/)
-| 💾 **Installation**               | [TTS/README.md](https://github.com/eginhard/coqui-tts/tree/dev#installation)|
-| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/eginhard/coqui-tts/blob/main/CONTRIBUTING.md)|
+| 💾 **Installation**               | [TTS/README.md](https://github.com/idiap/coqui-ai-TTS/tree/dev#installation)|
+| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/idiap/coqui-ai-TTS/blob/main/CONTRIBUTING.md)|
 | 📌 **Road Map**                   | [Main Development Plans](https://github.com/coqui-ai/TTS/issues/378)
-| 🚀 **Released Models**            | [Standard models](https://github.com/eginhard/coqui-tts/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/eginhard/coqui-tts#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
+| 🚀 **Released Models**            | [Standard models](https://github.com/idiap/coqui-ai-TTS/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/idiap/coqui-ai-TTS#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
 | 📰 **Papers**                    | [TTS Papers](https://github.com/erogol/TTS-papers)|
 
 ## Features
 - High-performance Deep Learning models for Text2Speech tasks.
     - Text2Spec models (Tacotron, Tacotron2, Glow-TTS, SpeedySpeech).
     - Speaker Encoder to compute speaker embeddings efficiently.
     - Vocoder models (MelGAN, Multiband-MelGAN, GAN-TTS, ParallelWaveGAN, WaveGrad, WaveRNN)
@@ -126,26 +127,26 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 18.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
 
 If you plan to code or train models, clone 🐸TTS and install it locally.
 
 ```bash
-git clone https://github.com/eginhard/coqui-tts
+git clone https://github.com/idiap/coqui-ai-TTS
 pip install -e .[all,dev,notebooks,server]  # Select the relevant extras
 ```
 
 If you are on Ubuntu (Debian), you can also run following commands for installation.
 
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
```

### Comparing `coqui-tts-0.22.1/TTS/.models.json` & `coqui_tts-0.23.0/TTS/.models.json`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/api.py` & `coqui_tts-0.23.0/TTS/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import logging
 import tempfile
 import warnings
 from pathlib import Path
 
 from torch import nn
 
 from TTS.config import load_config
 from TTS.utils.audio.numpy_transforms import save_wav
 from TTS.utils.manage import ModelManager
 from TTS.utils.synthesizer import Synthesizer
 
+logger = logging.getLogger(__name__)
+
 
 class TTS(nn.Module):
     """TODO: Add voice conversion and Capacitron support."""
 
     def __init__(
         self,
         model_name: str = "",
@@ -55,15 +58,15 @@
             config_path (str, optional): Path to the model config. Defaults to None.
             vocoder_path (str, optional): Path to the vocoder checkpoint. Defaults to None.
             vocoder_config_path (str, optional): Path to the vocoder config. Defaults to None.
             progress_bar (bool, optional): Whether to pring a progress bar while downloading a model. Defaults to True.
             gpu (bool, optional): Enable/disable GPU. Some models might be too slow on CPU. Defaults to False.
         """
         super().__init__()
-        self.manager = ModelManager(models_file=self.get_models_file_path(), progress_bar=progress_bar, verbose=False)
+        self.manager = ModelManager(models_file=self.get_models_file_path(), progress_bar=progress_bar)
         self.config = load_config(config_path) if config_path else None
         self.synthesizer = None
         self.voice_converter = None
         self.model_name = ""
         if gpu:
             warnings.warn("`gpu` will be deprecated. Please use `tts.to(device)` instead.")
 
@@ -118,15 +121,15 @@
 
     @staticmethod
     def get_models_file_path():
         return Path(__file__).parent / ".models.json"
 
     @staticmethod
     def list_models():
-        return ModelManager(models_file=TTS.get_models_file_path(), progress_bar=False, verbose=False).list_models()
+        return ModelManager(models_file=TTS.get_models_file_path(), progress_bar=False).list_models()
 
     def download_model_by_name(self, model_name: str):
         model_path, config_path, model_item = self.manager.download_model(model_name)
         if "fairseq" in model_name or (model_item is not None and isinstance(model_item["model_url"], list)):
             # return model directory if there are multiple files
             # we assume that the model knows how to load itself
             return None, None, None, None, model_path
```

### Comparing `coqui-tts-0.22.1/TTS/bin/collect_env_info.py` & `coqui_tts-0.23.0/TTS/bin/collect_env_info.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/bin/compute_attention_masks.py` & `coqui_tts-0.23.0/TTS/bin/compute_attention_masks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import argparse
 import importlib
+import logging
 import os
 from argparse import RawTextHelpFormatter
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from TTS.config import load_config
 from TTS.tts.datasets.TTSDataset import TTSDataset
 from TTS.tts.models import setup_model
 from TTS.tts.utils.text.characters import make_symbols, phonemes, symbols
 from TTS.utils.audio import AudioProcessor
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 from TTS.utils.io import load_checkpoint
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     # pylint: disable=bad-option-value
     parser = argparse.ArgumentParser(
         description="""Extract attention masks from trained Tacotron/Tacotron2 models.
 These masks can be used for different purposes including training a TTS model with a Duration Predictor.\n\n"""
         """Each attention mask is written to the same path as the input wav file with ".npy" file extension.
 (e.g. path/bla.wav (wav file) --> path/bla.npy (attention mask))\n"""
         """
```

### Comparing `coqui-tts-0.22.1/TTS/bin/compute_embeddings.py` & `coqui_tts-0.23.0/TTS/bin/compute_embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import argparse
+import logging
 import os
 from argparse import RawTextHelpFormatter
 
 import torch
 from tqdm import tqdm
 
 from TTS.config import load_config
 from TTS.config.shared_configs import BaseDatasetConfig
 from TTS.tts.datasets import load_tts_samples
 from TTS.tts.utils.managers import save_file
 from TTS.tts.utils.speakers import SpeakerManager
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 def compute_embeddings(
     model_path,
     config_path,
     output_path,
     old_speakers_file=None,
@@ -96,14 +98,16 @@
             os.makedirs(os.path.dirname(mapping_file_path), exist_ok=True)
 
         save_file(speaker_mapping, mapping_file_path)
         print("Speaker embeddings saved at:", mapping_file_path)
 
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser(
         description="""Compute embedding vectors for each audio file in a dataset and store them keyed by `{dataset_name}#{file_path}` in a .pth file\n\n"""
         """
         Example runs:
         python TTS/bin/compute_embeddings.py --model_path speaker_encoder_model.pth --config_path speaker_encoder_config.json  --config_dataset_path dataset_config.json
 
         python TTS/bin/compute_embeddings.py --model_path speaker_encoder_model.pth --config_path speaker_encoder_config.json  --formatter_name coqui --dataset_path /path/to/vctk/dataset --dataset_name my_vctk --meta_file_train /path/to/vctk/metafile_train.csv --meta_file_val /path/to/vctk/metafile_eval.csv
```

### Comparing `coqui-tts-0.22.1/TTS/bin/compute_statistics.py` & `coqui_tts-0.23.0/TTS/bin/compute_statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
 import glob
+import logging
 import os
 
 import numpy as np
 from tqdm import tqdm
 
 # from TTS.utils.io import load_config
 from TTS.config import load_config
 from TTS.tts.datasets import load_tts_samples
 from TTS.utils.audio import AudioProcessor
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 def main():
     """Run preprocessing process."""
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser(description="Compute mean and variance of spectrogtram features.")
     parser.add_argument("config_path", type=str, help="TTS config file path to define audio processin parameters.")
     parser.add_argument("out_path", type=str, help="save path (directory and filename).")
     parser.add_argument(
         "--data_path",
         type=str,
         required=False,
```

### Comparing `coqui-tts-0.22.1/TTS/bin/eval_encoder.py` & `coqui_tts-0.23.0/TTS/bin/eval_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
+import logging
 from argparse import RawTextHelpFormatter
 
 import torch
 from tqdm import tqdm
 
 from TTS.config import load_config
 from TTS.tts.datasets import load_tts_samples
 from TTS.tts.utils.speakers import SpeakerManager
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 def compute_encoder_accuracy(dataset_items, encoder_manager):
     class_name_key = encoder_manager.encoder_config.class_name_key
     map_classid_to_classname = getattr(encoder_manager.encoder_config, "map_classid_to_classname", None)
 
     class_acc_dict = {}
@@ -47,14 +49,16 @@
         print("Class", key, "Accuracy:", acc)
         acc_avg += acc
 
     print("Average Accuracy:", acc_avg / len(class_acc_dict))
 
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser(
         description="""Compute the accuracy of the encoder.\n\n"""
         """
         Example runs:
         python TTS/bin/eval_encoder.py emotion_encoder_model.pth emotion_encoder_config.json  dataset_config.json
         """,
         formatter_class=RawTextHelpFormatter,
```

### Comparing `coqui-tts-0.22.1/TTS/bin/extract_tts_spectrograms.py` & `coqui_tts-0.23.0/TTS/bin/extract_tts_spectrograms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """Extract Mel spectrograms with teacher forcing."""
 
 import argparse
+import logging
 import os
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 from trainer.generic_utils import count_parameters
@@ -13,19 +14,20 @@
 from TTS.config import load_config
 from TTS.tts.datasets import TTSDataset, load_tts_samples
 from TTS.tts.models import setup_model
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.utils.audio import AudioProcessor
 from TTS.utils.audio.numpy_transforms import quantize
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 use_cuda = torch.cuda.is_available()
 
 
-def setup_loader(ap, r, verbose=False):
+def setup_loader(ap, r):
     tokenizer, _ = TTSTokenizer.init_from_config(c)
     dataset = TTSDataset(
         outputs_per_step=r,
         compute_linear_spec=False,
         samples=meta_data,
         tokenizer=tokenizer,
         ap=ap,
@@ -33,15 +35,14 @@
         min_text_len=c.min_text_len,
         max_text_len=c.max_text_len,
         min_audio_len=c.min_audio_len,
         max_audio_len=c.max_audio_len,
         phoneme_cache_path=c.phoneme_cache_path,
         precompute_num_workers=0,
         use_noise_augment=False,
-        verbose=verbose,
         speaker_id_mapping=speaker_manager.name_to_id if c.use_speaker_embedding else None,
         d_vector_mapping=speaker_manager.embeddings if c.use_d_vector_file else None,
     )
 
     if c.use_phonemes and c.compute_input_seq_cache:
         # precompute phonemes to have a better estimate of sequence lengths.
         dataset.compute_input_seq(c.num_loader_workers)
@@ -253,29 +254,31 @@
     if use_cuda:
         model.cuda()
 
     num_params = count_parameters(model)
     print("\n > Model has {} parameters".format(num_params), flush=True)
     # set r
     r = 1 if c.model.lower() == "glow_tts" else model.decoder.r
-    own_loader = setup_loader(ap, r, verbose=True)
+    own_loader = setup_loader(ap, r)
 
     extract_spectrograms(
         own_loader,
         model,
         ap,
         args.output_path,
         quantize_bits=args.quantize_bits,
         save_audio=args.save_audio,
         debug=args.debug,
         metada_name="metada.txt",
     )
 
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser()
     parser.add_argument("--config_path", type=str, help="Path to config file for training.", required=True)
     parser.add_argument("--checkpoint_path", type=str, help="Model file to be restored.", required=True)
     parser.add_argument("--output_path", type=str, help="Path to save mel specs", required=True)
     parser.add_argument("--debug", default=False, action="store_true", help="Save audio files for debug")
     parser.add_argument("--save_audio", default=False, action="store_true", help="Save audio files")
     parser.add_argument("--quantize_bits", type=int, default=0, help="Save quantized audio files if non-zero")
```

### Comparing `coqui-tts-0.22.1/TTS/bin/find_unique_chars.py` & `coqui_tts-0.23.0/TTS/bin/find_unique_chars.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Find all the unique characters in a dataset"""
 
 import argparse
+import logging
 from argparse import RawTextHelpFormatter
 
 from TTS.config import load_config
 from TTS.tts.datasets import find_unique_chars, load_tts_samples
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 def main():
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     # pylint: disable=bad-option-value
     parser = argparse.ArgumentParser(
         description="""Find all the unique characters or phonemes in a dataset.\n\n"""
         """
     Example runs:
 
     python TTS/bin/find_unique_chars.py --config_path config.json
```

### Comparing `coqui-tts-0.22.1/TTS/bin/find_unique_phonemes.py` & `coqui_tts-0.23.0/TTS/bin/find_unique_phonemes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Find all the unique characters in a dataset"""
 
 import argparse
+import logging
 import multiprocessing
 from argparse import RawTextHelpFormatter
 
 from tqdm.contrib.concurrent import process_map
 
 from TTS.config import load_config
 from TTS.tts.datasets import load_tts_samples
 from TTS.tts.utils.text.phonemizers import Gruut
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 def compute_phonemes(item):
     text = item["text"]
     ph = phonemizer.phonemize(text).replace("|", "")
     return set(ph)
 
 
 def main():
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     # pylint: disable=W0601
     global c, phonemizer
     # pylint: disable=bad-option-value
     parser = argparse.ArgumentParser(
         description="""Find all the unique characters or phonemes in a dataset.\n\n"""
         """
     Example runs:
```

### Comparing `coqui-tts-0.22.1/TTS/bin/remove_silence_using_vad.py` & `coqui_tts-0.23.0/TTS/bin/remove_silence_using_vad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import glob
+import logging
 import multiprocessing
 import os
 import pathlib
 
 import torch
 from tqdm import tqdm
 
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 from TTS.utils.vad import get_vad_model_and_utils, remove_silence
 
 torch.set_num_threads(1)
 
 
 def adjust_path_and_remove_silence(audio_path):
     output_path = audio_path.replace(os.path.join(args.input_dir, ""), os.path.join(args.output_dir, ""))
@@ -71,14 +73,16 @@
             for file in filtered_files:
                 f.write(str(file) + "\n")
     else:
         print("> No files Found !")
 
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser(
         description="python TTS/bin/remove_silence_using_vad.py -i=VCTK-Corpus/ -o=VCTK-Corpus-removed-silence/ -g=wav48_silence_trimmed/*/*_mic1.flac --trim_just_beginning_and_end True"
     )
     parser.add_argument("-i", "--input_dir", type=str, help="Dataset root dir", required=True)
     parser.add_argument("-o", "--output_dir", type=str, help="Output Dataset dir", default="")
     parser.add_argument("-f", "--force", default=False, action="store_true", help="Force the replace of exists files")
     parser.add_argument(
```

### Comparing `coqui-tts-0.22.1/TTS/bin/resample.py` & `coqui_tts-0.23.0/TTS/bin/resample.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/bin/synthesize.py` & `coqui_tts-0.23.0/TTS/bin/synthesize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
 import contextlib
+import logging
 import sys
 from argparse import RawTextHelpFormatter
 
 # pylint: disable=redefined-outer-name, unused-argument
 from pathlib import Path
 
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
+
+logger = logging.getLogger(__name__)
+
 description = """
 Synthesize speech on command line.
 
 You can either use your trained model or choose a model from the provided list.
 
 If you don't specify any models, then it uses LJSpeech based English model.
 
@@ -138,14 +143,16 @@
         return True
     if v.lower() in ("no", "false", "f", "n", "0"):
         return False
     raise argparse.ArgumentTypeError("Boolean value expected.")
 
 
 def main():
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser(
         description=description.replace("    ```\n", ""),
         formatter_class=RawTextHelpFormatter,
     )
 
     parser.add_argument(
         "--list_models",
@@ -431,39 +438,45 @@
             vc_config_path,
             model_dir,
             args.voice_dir,
         ).to(device)
 
         # query speaker ids of a multi-speaker model.
         if args.list_speaker_idxs:
-            print(
-                " > Available speaker ids: (Set --speaker_idx flag to one of these values to use the multi-speaker model."
+            if synthesizer.tts_model.speaker_manager is None:
+                logger.info("Model only has a single speaker.")
+                return
+            logger.info(
+                "Available speaker ids: (Set --speaker_idx flag to one of these values to use the multi-speaker model."
             )
-            print(synthesizer.tts_model.speaker_manager.name_to_id)
+            logger.info(synthesizer.tts_model.speaker_manager.name_to_id)
             return
 
         # query langauge ids of a multi-lingual model.
         if args.list_language_idxs:
-            print(
-                " > Available language ids: (Set --language_idx flag to one of these values to use the multi-lingual model."
+            if synthesizer.tts_model.language_manager is None:
+                logger.info("Monolingual model.")
+                return
+            logger.info(
+                "Available language ids: (Set --language_idx flag to one of these values to use the multi-lingual model."
             )
-            print(synthesizer.tts_model.language_manager.name_to_id)
+            logger.info(synthesizer.tts_model.language_manager.name_to_id)
             return
 
         # check the arguments against a multi-speaker model.
         if synthesizer.tts_speakers_file and (not args.speaker_idx and not args.speaker_wav):
-            print(
-                " [!] Looks like you use a multi-speaker model. Define `--speaker_idx` to "
+            logger.error(
+                "Looks like you use a multi-speaker model. Define `--speaker_idx` to "
                 "select the target speaker. You can list the available speakers for this model by `--list_speaker_idxs`."
             )
             return
 
         # RUN THE SYNTHESIS
         if args.text:
-            print(" > Text: {}".format(args.text))
+            logger.info("Text: %s", args.text)
 
         # kick it
         if tts_path is not None:
             wav = synthesizer.tts(
                 args.text,
                 speaker_name=args.speaker_idx,
                 language_name=args.language_idx,
@@ -480,13 +493,13 @@
             )
         elif model_dir is not None:
             wav = synthesizer.tts(
                 args.text, speaker_name=args.speaker_idx, language_name=args.language_idx, speaker_wav=args.speaker_wav
             )
 
         # save the results
-        print(" > Saving output to {}".format(args.out_path))
         synthesizer.save_wav(wav, args.out_path, pipe_out=pipe_out)
+        logger.info("Saved output to %s", args.out_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `coqui-tts-0.22.1/TTS/bin/train_encoder.py` & `coqui_tts-0.23.0/TTS/bin/train_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import logging
 import os
 import sys
 import time
 import traceback
 
 import torch
 from torch.utils.data import DataLoader
@@ -15,38 +16,38 @@
 
 from TTS.encoder.dataset import EncoderDataset
 from TTS.encoder.utils.generic_utils import setup_encoder_model
 from TTS.encoder.utils.training import init_training
 from TTS.encoder.utils.visual import plot_embeddings
 from TTS.tts.datasets import load_tts_samples
 from TTS.utils.audio import AudioProcessor
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 from TTS.utils.samplers import PerfectBatchSampler
 from TTS.utils.training import check_update
 
 torch.backends.cudnn.enabled = True
 torch.backends.cudnn.benchmark = True
 torch.manual_seed(54321)
 use_cuda = torch.cuda.is_available()
 num_gpus = torch.cuda.device_count()
 print(" > Using CUDA: ", use_cuda)
 print(" > Number of GPUs: ", num_gpus)
 
 
-def setup_loader(ap: AudioProcessor, is_val: bool = False, verbose: bool = False):
+def setup_loader(ap: AudioProcessor, is_val: bool = False):
     num_utter_per_class = c.num_utter_per_class if not is_val else c.eval_num_utter_per_class
     num_classes_in_batch = c.num_classes_in_batch if not is_val else c.eval_num_classes_in_batch
 
     dataset = EncoderDataset(
         c,
         ap,
         meta_data_eval if is_val else meta_data_train,
         voice_len=c.voice_len,
         num_utter_per_class=num_utter_per_class,
         num_classes_in_batch=num_classes_in_batch,
-        verbose=verbose,
         augmentation_config=c.audio_augmentation if not is_val else None,
         use_torch_spec=c.model_params.get("use_torch_spec", False),
     )
     # get classes list
     classes = dataset.get_class_list()
 
     sampler = PerfectBatchSampler(
@@ -274,17 +275,17 @@
     model = setup_encoder_model(c)
 
     optimizer = get_optimizer(c.optimizer, c.optimizer_params, c.lr, model)
 
     # pylint: disable=redefined-outer-name
     meta_data_train, meta_data_eval = load_tts_samples(c.datasets, eval_split=True)
 
-    train_data_loader, train_classes, map_classid_to_classname = setup_loader(ap, is_val=False, verbose=True)
+    train_data_loader, train_classes, map_classid_to_classname = setup_loader(ap, is_val=False)
     if c.run_eval:
-        eval_data_loader, _, _ = setup_loader(ap, is_val=True, verbose=True)
+        eval_data_loader, _, _ = setup_loader(ap, is_val=True)
     else:
         eval_data_loader = None
 
     num_classes = len(train_classes)
     criterion = model.get_criterion(c, num_classes)
 
     if c.loss == "softmaxproto" and c.model != "speaker_encoder":
@@ -312,14 +313,16 @@
         criterion.cuda()
 
     global_step = args.restore_step
     _, global_step = train(model, optimizer, scheduler, criterion, train_data_loader, eval_data_loader, global_step)
 
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     args, c, OUT_PATH, AUDIO_PATH, c_logger, dashboard_logger = init_training()
 
     try:
         main(args)
     except KeyboardInterrupt:
         remove_experiment_folder(OUT_PATH)
         try:
```

### Comparing `coqui-tts-0.22.1/TTS/bin/train_tts.py` & `coqui_tts-0.23.0/TTS/bin/train_tts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import logging
 import os
 from dataclasses import dataclass, field
 
 from trainer import Trainer, TrainerArgs
 
 from TTS.config import load_config, register_config
 from TTS.tts.datasets import load_tts_samples
 from TTS.tts.models import setup_model
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 
 
 @dataclass
 class TrainTTSArgs(TrainerArgs):
     config_path: str = field(default=None, metadata={"help": "Path to the config file."})
 
 
 def main():
     """Run `tts` model training directly by a `config.json` file."""
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     # init trainer args
     train_args = TrainTTSArgs()
     parser = train_args.init_argparse(arg_prefix="")
 
     # override trainer args from comman-line args
     args, config_overrides = parser.parse_known_args()
     train_args.parse_args(args)
```

### Comparing `coqui-tts-0.22.1/TTS/bin/train_vocoder.py` & `coqui_tts-0.23.0/TTS/bin/train_vocoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import logging
 import os
 from dataclasses import dataclass, field
 
 from trainer import Trainer, TrainerArgs
 
 from TTS.config import load_config, register_config
 from TTS.utils.audio import AudioProcessor
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 from TTS.vocoder.datasets.preprocess import load_wav_data, load_wav_feat_data
 from TTS.vocoder.models import setup_model
 
 
 @dataclass
 class TrainVocoderArgs(TrainerArgs):
     config_path: str = field(default=None, metadata={"help": "Path to the config file."})
 
 
 def main():
     """Run `tts` model training directly by a `config.json` file."""
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     # init trainer args
     train_args = TrainVocoderArgs()
     parser = train_args.init_argparse(arg_prefix="")
 
     # override trainer args from comman-line args
     args, config_overrides = parser.parse_known_args()
     train_args.parse_args(args)
```

### Comparing `coqui-tts-0.22.1/TTS/bin/tune_wavegrad.py` & `coqui_tts-0.23.0/TTS/bin/tune_wavegrad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """Search a good noise schedule for WaveGrad for a given number of inference iterations"""
 
 import argparse
+import logging
 from itertools import product as cartesian_product
 
 import numpy as np
 import torch
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from TTS.config import load_config
 from TTS.utils.audio import AudioProcessor
+from TTS.utils.generic_utils import ConsoleFormatter, setup_logger
 from TTS.vocoder.datasets.preprocess import load_wav_data
 from TTS.vocoder.datasets.wavegrad_dataset import WaveGradDataset
 from TTS.vocoder.models import setup_model
 
 if __name__ == "__main__":
+    setup_logger("TTS", level=logging.INFO, screen=True, formatter=ConsoleFormatter())
+
     parser = argparse.ArgumentParser()
     parser.add_argument("--model_path", type=str, help="Path to model checkpoint.")
     parser.add_argument("--config_path", type=str, help="Path to model config file.")
     parser.add_argument("--data_path", type=str, help="Path to data directory.")
     parser.add_argument("--output_path", type=str, help="path for output file including file name and extension.")
     parser.add_argument(
         "--num_iter",
@@ -51,15 +55,14 @@
         hop_len=ap.hop_length,
         pad_short=config.pad_short,
         conv_pad=config.conv_pad,
         is_training=True,
         return_segments=False,
         use_noise_augment=False,
         use_cache=False,
-        verbose=True,
     )
     loader = DataLoader(
         dataset,
         batch_size=1,
         shuffle=False,
         collate_fn=dataset.collate_full_clips,
         drop_last=False,
```

### Comparing `coqui-tts-0.22.1/TTS/config/__init__.py` & `coqui_tts-0.23.0/TTS/config/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/config/shared_configs.py` & `coqui_tts-0.23.0/TTS/config/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/utils/formatter.py` & `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/utils/gpt_train.py` & `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/utils/gpt_train.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/demos/xtts_ft_demo/xtts_demo.py` & `coqui_tts-0.23.0/TTS/demos/xtts_ft_demo/xtts_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
                     "nl",
                     "cs",
                     "ar",
                     "zh",
                     "hu",
                     "ko",
                     "ja",
+                    "hi",
                 ],
             )
             progress_data = gr.Label(label="Progress:")
             logs = gr.Textbox(
                 label="Logs:",
                 interactive=False,
             )
@@ -366,14 +367,15 @@
                             "nl",
                             "cs",
                             "ar",
                             "zh",
                             "hu",
                             "ko",
                             "ja",
+                            "hi",
                         ],
                     )
                     tts_text = gr.Textbox(
                         label="Input Text.",
                         value="This model sounds really good and above all, it's reasonably fast.",
                     )
                     tts_btn = gr.Button(value="Step 4 - Inference")
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/README.md` & `coqui_tts-0.23.0/TTS/encoder/README.md`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/encoder/configs/base_encoder_config.py` & `coqui_tts-0.23.0/TTS/encoder/configs/base_encoder_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/encoder/dataset.py` & `coqui_tts-0.23.0/TTS/encoder/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
+import logging
 import random
 
 import torch
 from torch.utils.data import Dataset
 
 from TTS.encoder.utils.generic_utils import AugmentWAV
 
+logger = logging.getLogger(__name__)
+
 
 class EncoderDataset(Dataset):
     def __init__(
         self,
         config,
         ap,
         meta_data,
         voice_len=1.6,
         num_classes_in_batch=64,
         num_utter_per_class=10,
-        verbose=False,
         augmentation_config=None,
         use_torch_spec=None,
     ):
         """
         Args:
             ap (TTS.tts.utils.AudioProcessor): audio processor object.
             meta_data (list): list of dataset instances.
             seq_len (int): voice segment length in seconds.
-            verbose (bool): print diagnostic information.
         """
         super().__init__()
         self.config = config
         self.items = meta_data
         self.sample_rate = ap.sample_rate
         self.seq_len = int(voice_len * self.sample_rate)
         self.num_utter_per_class = num_utter_per_class
         self.ap = ap
-        self.verbose = verbose
         self.use_torch_spec = use_torch_spec
         self.classes, self.items = self.__parse_items()
 
         self.classname_to_classid = {key: i for i, key in enumerate(self.classes)}
 
         # Data Augmentation
         self.augmentator = None
@@ -46,21 +46,20 @@
             self.data_augmentation_p = augmentation_config["p"]
             if self.data_augmentation_p and ("additive" in augmentation_config or "rir" in augmentation_config):
                 self.augmentator = AugmentWAV(ap, augmentation_config)
 
             if "gaussian" in augmentation_config.keys():
                 self.gaussian_augmentation_config = augmentation_config["gaussian"]
 
-        if self.verbose:
-            print("\n > DataLoader initialization")
-            print(f" | > Classes per Batch: {num_classes_in_batch}")
-            print(f" | > Number of instances : {len(self.items)}")
-            print(f" | > Sequence length: {self.seq_len}")
-            print(f" | > Num Classes: {len(self.classes)}")
-            print(f" | > Classes: {self.classes}")
+        logger.info("DataLoader initialization")
+        logger.info(" | Classes per batch: %d", num_classes_in_batch)
+        logger.info(" | Number of instances: %d", len(self.items))
+        logger.info(" | Sequence length: %d", self.seq_len)
+        logger.info(" | Number of classes: %d", len(self.classes))
+        logger.info(" | Classes: %d", self.classes)
 
     def load_wav(self, filename):
         audio = self.ap.load_wav(filename, sr=self.ap.sample_rate)
         return audio
 
     def __parse_items(self):
         class_to_utters = {}
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/losses.py` & `coqui_tts-0.23.0/TTS/encoder/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import logging
+
 import torch
 import torch.nn.functional as F
 from torch import nn
 
+logger = logging.getLogger(__name__)
+
 
 # adapted from https://github.com/cvqluu/GE2E-Loss
 class GE2ELoss(nn.Module):
     def __init__(self, init_w=10.0, init_b=-5.0, loss_method="softmax"):
         """
         Implementation of the Generalized End-to-End loss defined in https://arxiv.org/abs/1710.10467 [1]
         Accepts an input of size (N, M, D)
@@ -19,15 +23,15 @@
         super().__init__()
         # pylint: disable=E1102
         self.w = nn.Parameter(torch.tensor(init_w))
         # pylint: disable=E1102
         self.b = nn.Parameter(torch.tensor(init_b))
         self.loss_method = loss_method
 
-        print(" > Initialized Generalized End-to-End loss")
+        logger.info("Initialized Generalized End-to-End loss")
 
         assert self.loss_method in ["softmax", "contrast"]
 
         if self.loss_method == "softmax":
             self.embed_loss = self.embed_loss_softmax
         if self.loss_method == "contrast":
             self.embed_loss = self.embed_loss_contrast
@@ -135,15 +139,15 @@
         super().__init__()
         # pylint: disable=E1102
         self.w = nn.Parameter(torch.tensor(init_w))
         # pylint: disable=E1102
         self.b = nn.Parameter(torch.tensor(init_b))
         self.criterion = torch.nn.CrossEntropyLoss()
 
-        print(" > Initialized Angular Prototypical loss")
+        logger.info("Initialized Angular Prototypical loss")
 
     def forward(self, x, _label=None):
         """
         Calculates the AngleProto loss for an input of dimensions (num_speakers, num_utts_per_speaker, dvec_feats)
         """
 
         assert x.size()[1] >= 2
@@ -173,15 +177,15 @@
 
     def __init__(self, embedding_dim, n_speakers):
         super().__init__()
 
         self.criterion = torch.nn.CrossEntropyLoss()
         self.fc = nn.Linear(embedding_dim, n_speakers)
 
-        print("Initialised Softmax Loss")
+        logger.info("Initialised Softmax Loss")
 
     def forward(self, x, label=None):
         # reshape for compatibility
         x = x.reshape(-1, x.size()[-1])
         label = label.reshape(-1)
 
         x = self.fc(x)
@@ -208,15 +212,15 @@
 
     def __init__(self, embedding_dim, n_speakers, init_w=10.0, init_b=-5.0):
         super().__init__()
 
         self.softmax = SoftmaxLoss(embedding_dim, n_speakers)
         self.angleproto = AngleProtoLoss(init_w, init_b)
 
-        print("Initialised SoftmaxAnglePrototypical Loss")
+        logger.info("Initialised SoftmaxAnglePrototypical Loss")
 
     def forward(self, x, label=None):
         """
         Calculates the SoftmaxAnglePrototypical loss for an input of dimensions (num_speakers, num_utts_per_speaker, dvec_feats)
         """
 
         Lp = self.angleproto(x)
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/models/base_encoder.py` & `coqui_tts-0.23.0/TTS/encoder/models/base_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
+
 import numpy as np
 import torch
 import torchaudio
 from coqpit import Coqpit
 from torch import nn
 
 from TTS.encoder.losses import AngleProtoLoss, GE2ELoss, SoftmaxAngleProtoLoss
 from TTS.utils.generic_utils import set_init_dict
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 class PreEmphasis(nn.Module):
     def __init__(self, coefficient=0.97):
         super().__init__()
         self.coefficient = coefficient
         self.register_buffer("filter", torch.FloatTensor([-self.coefficient, 1.0]).unsqueeze(0).unsqueeze(0))
 
@@ -114,32 +118,32 @@
         use_cuda: bool = False,
         criterion=None,
         cache=False,
     ):
         state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         try:
             self.load_state_dict(state["model"])
-            print(" > Model fully restored. ")
+            logger.info("Model fully restored. ")
         except (KeyError, RuntimeError) as error:
             # If eval raise the error
             if eval:
                 raise error
 
-            print(" > Partial model initialization.")
+            logger.info("Partial model initialization.")
             model_dict = self.state_dict()
             model_dict = set_init_dict(model_dict, state["model"], c)
             self.load_state_dict(model_dict)
             del model_dict
 
         # load the criterion for restore_path
         if criterion is not None and "criterion" in state:
             try:
                 criterion.load_state_dict(state["criterion"])
             except (KeyError, RuntimeError) as error:
-                print(" > Criterion load ignored because of:", error)
+                logger.exception("Criterion load ignored because of: %s", error)
 
         # instance and load the criterion for the encoder classifier in inference time
         if (
             eval
             and criterion is None
             and "criterion" in state
             and getattr(config, "map_classid_to_classname", None) is not None
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/models/lstm.py` & `coqui_tts-0.23.0/TTS/encoder/models/lstm.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/encoder/models/resnet.py` & `coqui_tts-0.23.0/TTS/encoder/models/resnet.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/encoder/utils/generic_utils.py` & `coqui_tts-0.23.0/TTS/encoder/utils/generic_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import glob
+import logging
 import os
 import random
 
 import numpy as np
 from scipy import signal
 
 from TTS.encoder.models.lstm import LSTMSpeakerEncoder
 from TTS.encoder.models.resnet import ResNetSpeakerEncoder
 
+logger = logging.getLogger(__name__)
+
 
 class AugmentWAV(object):
     def __init__(self, ap, augmentation_config):
         self.ap = ap
         self.use_additive_noise = False
 
         if "additive" in augmentation_config.keys():
@@ -34,27 +37,29 @@
                     # ignore not listed directories
                     if noise_dir not in self.additive_noise_types:
                         continue
                     if noise_dir not in self.noise_list:
                         self.noise_list[noise_dir] = []
                     self.noise_list[noise_dir].append(wav_file)
 
-                print(
-                    f" | > Using Additive Noise Augmentation: with {len(additive_files)} audios instances from {self.additive_noise_types}"
+                logger.info(
+                    "Using Additive Noise Augmentation: with %d audios instances from %s",
+                    len(additive_files),
+                    self.additive_noise_types,
                 )
 
         self.use_rir = False
 
         if "rir" in augmentation_config.keys():
             self.rir_config = augmentation_config["rir"]
             if self.rir_config["rir_path"]:
                 self.rir_files = glob.glob(os.path.join(self.rir_config["rir_path"], "**/*.wav"), recursive=True)
                 self.use_rir = True
 
-            print(f" | > Using RIR Noise Augmentation: with {len(self.rir_files)} audios instances")
+            logger.info("Using RIR Noise Augmentation: with %d audios instances", len(self.rir_files))
 
         self.create_augmentation_global_list()
 
     def create_augmentation_global_list(self):
         if self.use_additive_noise:
             self.global_noise_list = self.additive_noise_types
         else:
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/utils/prepare_voxceleb.py` & `coqui_tts-0.23.0/TTS/encoder/utils/prepare_voxceleb.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 # Only support eager mode and TF>=2.0.0
 # pylint: disable=no-member, invalid-name, relative-beyond-top-level
 # pylint: disable=too-many-locals, too-many-statements, too-many-arguments, too-many-instance-attributes
 """ voxceleb 1 & 2 """
 
 import csv
 import hashlib
+import logging
 import os
 import subprocess
 import sys
 import zipfile
 
 import soundfile as sf
-from absl import logging
+
+logger = logging.getLogger(__name__)
 
 SUBSETS = {
     "vox1_dev_wav": [
         "https://thor.robots.ox.ac.uk/~vgg/data/voxceleb/vox1a/vox1_dev_wav_partaa",
         "https://thor.robots.ox.ac.uk/~vgg/data/voxceleb/vox1a/vox1_dev_wav_partab",
         "https://thor.robots.ox.ac.uk/~vgg/data/voxceleb/vox1a/vox1_dev_wav_partac",
         "https://thor.robots.ox.ac.uk/~vgg/data/voxceleb/vox1a/vox1_dev_wav_partad",
@@ -73,22 +75,22 @@
     os.makedirs(directory, exist_ok=True)
 
     try:
         for url in urls:
             zip_filepath = os.path.join(directory, url.split("/")[-1])
             if os.path.exists(zip_filepath):
                 continue
-            logging.info("Downloading %s to %s" % (url, zip_filepath))
+            logger.info("Downloading %s to %s" % (url, zip_filepath))
             subprocess.call(
                 "wget %s --user %s --password %s -O %s" % (url, USER["user"], USER["password"], zip_filepath),
                 shell=True,
             )
 
             statinfo = os.stat(zip_filepath)
-            logging.info("Successfully downloaded %s, size(bytes): %d" % (url, statinfo.st_size))
+            logger.info("Successfully downloaded %s, size(bytes): %d" % (url, statinfo.st_size))
 
         # concatenate all parts into zip files
         if ".zip" not in zip_filepath:
             zip_filepath = "_".join(zip_filepath.split("_")[:-1])
             subprocess.call("cat %s* > %s.zip" % (zip_filepath, zip_filepath), shell=True)
             zip_filepath += ".zip"
         extract_path = zip_filepath.strip(".zip")
@@ -114,49 +116,49 @@
         cmd: command line to be executed.
     Return:
         int, the return code.
     """
     try:
         retcode = subprocess.call(cmd, shell=True)
         if retcode < 0:
-            logging.info(f"Child was terminated by signal {retcode}")
+            logger.info(f"Child was terminated by signal {retcode}")
     except OSError as e:
-        logging.info(f"Execution failed: {e}")
+        logger.info(f"Execution failed: {e}")
         retcode = -999
     return retcode
 
 
 def decode_aac_with_ffmpeg(aac_file, wav_file):
     """Decode a given AAC file into WAV using ffmpeg.
     Args:
         aac_file: file path to input AAC file.
         wav_file: file path to output WAV file.
     Return:
         bool, True if success.
     """
     cmd = f"ffmpeg -i {aac_file} {wav_file}"
-    logging.info(f"Decoding aac file using command line: {cmd}")
+    logger.info(f"Decoding aac file using command line: {cmd}")
     ret = exec_cmd(cmd)
     if ret != 0:
-        logging.error(f"Failed to decode aac file with retcode {ret}")
-        logging.error("Please check your ffmpeg installation.")
+        logger.error(f"Failed to decode aac file with retcode {ret}")
+        logger.error("Please check your ffmpeg installation.")
         return False
     return True
 
 
 def convert_audio_and_make_label(input_dir, subset, output_dir, output_file):
     """Optionally convert AAC to WAV and make speaker labels.
     Args:
         input_dir: the directory which holds the input dataset.
         subset: the name of the specified subset. e.g. vox1_dev_wav
         output_dir: the directory to place the newly generated csv files.
         output_file: the name of the newly generated csv file. e.g. vox1_dev_wav.csv
     """
 
-    logging.info("Preprocessing audio and label for subset %s" % subset)
+    logger.info("Preprocessing audio and label for subset %s" % subset)
     source_dir = os.path.join(input_dir, subset)
 
     files = []
     # Convert all AAC file into WAV format. At the same time, generate the csv
     for root, _, filenames in os.walk(source_dir):
         for filename in filenames:
             name, ext = os.path.splitext(filename)
@@ -186,37 +188,37 @@
     # "wav_filename", "wav_length_ms", "speaker_id", "speaker_name".
     csv_file_path = os.path.join(output_dir, output_file)
     with open(csv_file_path, "w", newline="", encoding="utf-8") as f:
         writer = csv.writer(f, delimiter="\t")
         writer.writerow(["wav_filename", "wav_length_ms", "speaker_id", "speaker_name"])
         for wav_file in files:
             writer.writerow(wav_file)
-    logging.info("Successfully generated csv file {}".format(csv_file_path))
+    logger.info("Successfully generated csv file {}".format(csv_file_path))
 
 
 def processor(directory, subset, force_process):
     """download and process"""
     urls = SUBSETS
     if subset not in urls:
         raise ValueError(subset, "is not in voxceleb")
 
     subset_csv = os.path.join(directory, subset + ".csv")
     if not force_process and os.path.exists(subset_csv):
         return subset_csv
 
-    logging.info("Downloading and process the voxceleb in %s", directory)
-    logging.info("Preparing subset %s", subset)
+    logger.info("Downloading and process the voxceleb in %s", directory)
+    logger.info("Preparing subset %s", subset)
     download_and_extract(directory, subset, urls[subset])
     convert_audio_and_make_label(directory, subset, directory, subset + ".csv")
-    logging.info("Finished downloading and processing")
+    logger.info("Finished downloading and processing")
     return subset_csv
 
 
 if __name__ == "__main__":
-    logging.set_verbosity(logging.INFO)
+    logging.getLogger("TTS").setLevel(logging.INFO)
     if len(sys.argv) != 4:
         print("Usage: python prepare_data.py save_directory user password")
         sys.exit()
 
     DIR, USER["user"], USER["password"] = sys.argv[1], sys.argv[2], sys.argv[3]
     for SUBSET in SUBSETS:
         processor(DIR, SUBSET, False)
```

### Comparing `coqui-tts-0.22.1/TTS/encoder/utils/training.py` & `coqui_tts-0.23.0/TTS/encoder/utils/training.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/encoder/utils/visual.py` & `coqui_tts-0.23.0/TTS/encoder/utils/visual.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/model.py` & `coqui_tts-0.23.0/TTS/model.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/server/README.md` & `coqui_tts-0.23.0/TTS/server/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # :frog: TTS demo server
 Before you use the server, make sure you
-[install](https://github.com/eginhard/coqui-tts/tree/dev#install-tts)) :frog: TTS
+[install](https://github.com/idiap/coqui-ai-TTS/tree/dev#install-tts)) :frog: TTS
 properly and install the additional dependencies with `pip install
 coqui-tts[server]`. Then, you can follow the steps below.
 
 **Note:** If you install :frog:TTS using ```pip```, you can also use the ```tts-server``` end point on the terminal.
 
 Examples runs:
```

### Comparing `coqui-tts-0.22.1/TTS/server/server.py` & `coqui_tts-0.23.0/TTS/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!flask/bin/python
 import argparse
 import io
 import json
+import logging
 import os
 import sys
 from pathlib import Path
 from threading import Lock
 from typing import Union
 from urllib.parse import parse_qs
 
@@ -14,14 +15,17 @@
 except ImportError as e:
     raise ImportError("Server requires requires flask, use `pip install coqui-tts[server]`.") from e
 
 from TTS.config import load_config
 from TTS.utils.manage import ModelManager
 from TTS.utils.synthesizer import Synthesizer
 
+logger = logging.getLogger(__name__)
+logging.getLogger("TTS").setLevel(logging.INFO)
+
 
 def create_argparser():
     def convert_boolean(x):
         return x.lower() in ["true", "1", "yes"]
 
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -196,17 +200,17 @@
     with lock:
         text = request.headers.get("text") or request.values.get("text", "")
         speaker_idx = request.headers.get("speaker-id") or request.values.get("speaker_id", "")
         language_idx = request.headers.get("language-id") or request.values.get("language_id", "")
         style_wav = request.headers.get("style-wav") or request.values.get("style_wav", "")
         style_wav = style_wav_uri_to_dict(style_wav)
 
-        print(f" > Model input: {text}")
-        print(f" > Speaker Idx: {speaker_idx}")
-        print(f" > Language Idx: {language_idx}")
+        logger.info("Model input: %s", text)
+        logger.info("Speaker idx: %s", speaker_idx)
+        logger.info("Language idx: %s", language_idx)
         wavs = synthesizer.tts(text, speaker_name=speaker_idx, language_name=language_idx, style_wav=style_wav)
         out = io.BytesIO()
         synthesizer.save_wav(wavs, out)
     return send_file(out, mimetype="audio/wav")
 
 
 # Basic MaryTTS compatibility layer
@@ -242,15 +246,15 @@
     with lock:
         if request.method == "POST":
             data = parse_qs(request.get_data(as_text=True))
             # NOTE: we ignore param. LOCALE and VOICE for now since we have only one active model
             text = data.get("INPUT_TEXT", [""])[0]
         else:
             text = request.args.get("INPUT_TEXT", "")
-        print(f" > Model input: {text}")
+        logger.info("Model input: %s", text)
         wavs = synthesizer.tts(text)
         out = io.BytesIO()
         synthesizer.save_wav(wavs, out)
     return send_file(out, mimetype="audio/wav")
 
 
 def main():
```

### Comparing `coqui-tts-0.22.1/TTS/server/static/coqui-log-green-TTS.png` & `coqui_tts-0.23.0/TTS/server/static/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/server/templates/details.html` & `coqui_tts-0.23.0/TTS/server/templates/details.html`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/server/templates/index.html` & `coqui_tts-0.23.0/TTS/server/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 padding-top: 56px;
             }
         }
     </style>
 </head>
 
 <body>
-    <a href="https://github.com/eginhard/coqui-tts"><img style="position: absolute; z-index:1000; top: 0; left: 0; border: 0;"
+    <a href="https://github.com/idiap/coqui-ai-TTS"><img style="position: absolute; z-index:1000; top: 0; left: 0; border: 0;"
             src="https://s3.amazonaws.com/github/ribbons/forkme_left_darkblue_121621.png" alt="Fork me on GitHub"></a>
 
     <!-- Navigation -->
     <!--
     <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
       <div class="container">
         <a class="navbar-brand" href="#">Coqui TTS</a>
```

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/__init__.py` & `coqui_tts-0.23.0/TTS/tts/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/align_tts_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/align_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/bark_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/bark_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/delightful_tts_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/delightful_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/fast_pitch_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/fast_pitch_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/fast_speech_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/fast_speech_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/fastspeech2_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/fastspeech2_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/glow_tts_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/glow_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/neuralhmm_tts_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/neuralhmm_tts_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/overflow_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/overflow_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/shared_configs.py` & `coqui_tts-0.23.0/TTS/tts/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/speedy_speech_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/speedy_speech_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/tacotron2_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/tacotron2_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/tacotron_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/tacotron_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/tortoise_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/tortoise_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/vits_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/vits_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/configs/xtts_config.py` & `coqui_tts-0.23.0/TTS/tts/configs/xtts_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/datasets/__init__.py` & `coqui_tts-0.23.0/TTS/tts/datasets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import logging
 import os
 import sys
 from collections import Counter
 from pathlib import Path
 from typing import Callable, Dict, List, Tuple, Union
 
 import numpy as np
 
 from TTS.tts.datasets.dataset import *
 from TTS.tts.datasets.formatters import *
 
+logger = logging.getLogger(__name__)
+
 
 def split_dataset(items, eval_split_max_size=None, eval_split_size=0.01):
     """Split a dataset into train and eval. Consider speaker distribution in multi-speaker training.
 
     Args:
         items (List[List]):
             A list of samples. Each sample is a list of `[audio_path, text, speaker_id]`.
@@ -118,15 +121,15 @@
             formatter = _get_formatter_by_name(formatter_name)
         # load train set
         meta_data_train = formatter(root_path, meta_file_train, ignored_speakers=ignored_speakers)
         assert len(meta_data_train) > 0, f" [!] No training samples found in {root_path}/{meta_file_train}"
 
         meta_data_train = add_extra_keys(meta_data_train, language, dataset_name)
 
-        print(f" | > Found {len(meta_data_train)} files in {Path(root_path).resolve()}")
+        logger.info("Found %d files in %s", len(meta_data_train), Path(root_path).resolve())
         # load evaluation split if set
         if eval_split:
             if meta_file_val:
                 meta_data_eval = formatter(root_path, meta_file_val, ignored_speakers=ignored_speakers)
                 meta_data_eval = add_extra_keys(meta_data_eval, language, dataset_name)
             else:
                 eval_size_per_dataset = eval_split_max_size // len(datasets) if eval_split_max_size else None
@@ -162,20 +165,19 @@
 
 def _get_formatter_by_name(name):
     """Returns the respective preprocessing function."""
     thismodule = sys.modules[__name__]
     return getattr(thismodule, name.lower())
 
 
-def find_unique_chars(data_samples, verbose=True):
+def find_unique_chars(data_samples):
     texts = "".join(item["text"] for item in data_samples)
     chars = set(texts)
     lower_chars = filter(lambda c: c.islower(), chars)
     chars_force_lower = [c.lower() for c in chars]
     chars_force_lower = set(chars_force_lower)
 
-    if verbose:
-        print(f" > Number of unique characters: {len(chars)}")
-        print(f" > Unique characters: {''.join(sorted(chars))}")
-        print(f" > Unique lower characters: {''.join(sorted(lower_chars))}")
-        print(f" > Unique all forced to lower characters: {''.join(sorted(chars_force_lower))}")
+    logger.info("Number of unique characters: %d", len(chars))
+    logger.info("Unique characters: %s", "".join(sorted(chars)))
+    logger.info("Unique lower characters: %s", "".join(sorted(lower_chars)))
+    logger.info("Unique all forced to lower characters: %s", "".join(sorted(chars_force_lower)))
     return chars_force_lower
```

### Comparing `coqui-tts-0.22.1/TTS/tts/datasets/dataset.py` & `coqui_tts-0.23.0/TTS/tts/datasets/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import base64
 import collections
+import logging
 import os
 import random
 from typing import Dict, List, Union
 
 import numpy as np
 import torch
 import torchaudio
 import tqdm
 from torch.utils.data import Dataset
 
 from TTS.tts.utils.data import prepare_data, prepare_stop_target, prepare_tensor
 from TTS.utils.audio import AudioProcessor
 from TTS.utils.audio.numpy_transforms import compute_energy as calculate_energy
 
+logger = logging.getLogger(__name__)
+
 # to prevent too many open files error as suggested here
 # https://github.com/pytorch/pytorch/issues/11201#issuecomment-421146936
 torch.multiprocessing.set_sharing_strategy("file_system")
 
 
 def _parse_sample(item):
     language_name = None
@@ -75,15 +78,14 @@
         phoneme_cache_path: str = None,
         precompute_num_workers: int = 0,
         speaker_id_mapping: Dict = None,
         d_vector_mapping: Dict = None,
         language_id_mapping: Dict = None,
         use_noise_augment: bool = False,
         start_by_longest: bool = False,
-        verbose: bool = False,
     ):
         """Generic 📂 data loader for `tts` models. It is configurable for different outputs and needs.
 
         If you need something different, you can subclass and override.
 
         Args:
             outputs_per_step (int): Number of time frames predicted per step.
@@ -133,16 +135,14 @@
                 embedding layer. Defaults to None.
 
             d_vector_mapping (dict): Mapping of wav files to computed d-vectors. Defaults to None.
 
             use_noise_augment (bool): Enable adding random noise to wav for augmentation. Defaults to False.
 
             start_by_longest (bool): Start by longest sequence. It is especially useful to check OOM. Defaults to False.
-
-            verbose (bool): Print diagnostic information. Defaults to false.
         """
         super().__init__()
         self.batch_group_size = batch_group_size
         self._samples = samples
         self.outputs_per_step = outputs_per_step
         self.compute_linear_spec = compute_linear_spec
         self.return_wav = return_wav
@@ -158,15 +158,14 @@
         self.phoneme_cache_path = phoneme_cache_path
         self.speaker_id_mapping = speaker_id_mapping
         self.d_vector_mapping = d_vector_mapping
         self.language_id_mapping = language_id_mapping
         self.use_noise_augment = use_noise_augment
         self.start_by_longest = start_by_longest
 
-        self.verbose = verbose
         self.rescue_item_idx = 1
         self.pitch_computed = False
         self.tokenizer = tokenizer
 
         if self.tokenizer.use_phonemes:
             self.phoneme_dataset = PhonemeDataset(
                 self.samples, self.tokenizer, phoneme_cache_path, precompute_num_workers=precompute_num_workers
@@ -176,16 +175,15 @@
             self.f0_dataset = F0Dataset(
                 self.samples, self.ap, cache_path=f0_cache_path, precompute_num_workers=precompute_num_workers
             )
         if compute_energy:
             self.energy_dataset = EnergyDataset(
                 self.samples, self.ap, cache_path=energy_cache_path, precompute_num_workers=precompute_num_workers
             )
-        if self.verbose:
-            self.print_logs()
+        self.print_logs()
 
     @property
     def lengths(self):
         lens = []
         for item in self.samples:
             _, wav_file, *_ = _parse_sample(item)
             audio_len = get_audio_size(wav_file)
@@ -210,19 +208,18 @@
         return len(self.samples)
 
     def __getitem__(self, idx):
         return self.load_data(idx)
 
     def print_logs(self, level: int = 0) -> None:
         indent = "\t" * level
-        print("\n")
-        print(f"{indent}> DataLoader initialization")
-        print(f"{indent}| > Tokenizer:")
+        logger.info("%sDataLoader initialization", indent)
+        logger.info("%s| Tokenizer:", indent)
         self.tokenizer.print_logs(level + 1)
-        print(f"{indent}| > Number of instances : {len(self.samples)}")
+        logger.info("%s| Number of instances : %d", indent, len(self.samples))
 
     def load_wav(self, filename):
         waveform = self.ap.load_wav(filename)
         assert waveform.size > 0
         return waveform
 
     def get_phonemes(self, idx, text):
@@ -386,25 +383,23 @@
             samples = self.create_buckets(samples, self.batch_group_size)
 
         # update items to the new sorted items
         audio_lengths = [s["audio_length"] for s in samples]
         text_lengths = [s["text_length"] for s in samples]
         self.samples = samples
 
-        if self.verbose:
-            print(" | > Preprocessing samples")
-            print(" | > Max text length: {}".format(np.max(text_lengths)))
-            print(" | > Min text length: {}".format(np.min(text_lengths)))
-            print(" | > Avg text length: {}".format(np.mean(text_lengths)))
-            print(" | ")
-            print(" | > Max audio length: {}".format(np.max(audio_lengths)))
-            print(" | > Min audio length: {}".format(np.min(audio_lengths)))
-            print(" | > Avg audio length: {}".format(np.mean(audio_lengths)))
-            print(f" | > Num. instances discarded samples: {len(ignore_idx)}")
-            print(" | > Batch group size: {}.".format(self.batch_group_size))
+        logger.info("Preprocessing samples")
+        logger.info("Max text length: {}".format(np.max(text_lengths)))
+        logger.info("Min text length: {}".format(np.min(text_lengths)))
+        logger.info("Avg text length: {}".format(np.mean(text_lengths)))
+        logger.info("Max audio length: {}".format(np.max(audio_lengths)))
+        logger.info("Min audio length: {}".format(np.min(audio_lengths)))
+        logger.info("Avg audio length: {}".format(np.mean(audio_lengths)))
+        logger.info("Num. instances discarded samples: %d", len(ignore_idx))
+        logger.info("Batch group size: {}.".format(self.batch_group_size))
 
     @staticmethod
     def _sort_batch(batch, text_lengths):
         """Sort the batch by the input text length for RNN efficiency.
 
         Args:
             batch (Dict): Batch returned by `__getitem__`.
@@ -639,15 +634,15 @@
         return self.tokenizer.pad_id
 
     def precompute(self, num_workers=1):
         """Precompute phonemes for all samples.
 
         We use pytorch dataloader because we are lazy.
         """
-        print("[*] Pre-computing phonemes...")
+        logger.info("Pre-computing phonemes...")
         with tqdm.tqdm(total=len(self)) as pbar:
             batch_size = num_workers if num_workers > 0 else 1
             dataloder = torch.utils.data.DataLoader(
                 batch_size=batch_size, dataset=self, shuffle=False, num_workers=num_workers, collate_fn=self.collate_fn
             )
             for _ in dataloder:
                 pbar.update(batch_size)
@@ -661,19 +656,18 @@
         ids_torch = torch.LongTensor(len(ids), ids_lens_max).fill_(self.get_pad_id())
         for i, ids_len in enumerate(ids_lens):
             ids_torch[i, :ids_len] = torch.LongTensor(ids[i])
         return {"text": texts, "ph_hat": texts_hat, "token_ids": ids_torch}
 
     def print_logs(self, level: int = 0) -> None:
         indent = "\t" * level
-        print("\n")
-        print(f"{indent}> PhonemeDataset ")
-        print(f"{indent}| > Tokenizer:")
+        logger.info("%sPhonemeDataset", indent)
+        logger.info("%s| Tokenizer:", indent)
         self.tokenizer.print_logs(level + 1)
-        print(f"{indent}| > Number of instances : {len(self.samples)}")
+        logger.info("%s| Number of instances : %d", indent, len(self.samples))
 
 
 class F0Dataset:
     """F0 Dataset for computing F0 from wav files in CPU
 
     Pre-compute F0 values for all the samples at initialization if `cache_path` is not None or already present. It
     also computes the mean and std of F0 values if `normalize_f0` is True.
@@ -697,22 +691,20 @@
     """
 
     def __init__(
         self,
         samples: Union[List[List], List[Dict]],
         ap: "AudioProcessor",
         audio_config=None,  # pylint: disable=unused-argument
-        verbose=False,
         cache_path: str = None,
         precompute_num_workers=0,
         normalize_f0=True,
     ):
         self.samples = samples
         self.ap = ap
-        self.verbose = verbose
         self.cache_path = cache_path
         self.normalize_f0 = normalize_f0
         self.pad_id = 0.0
         self.mean = None
         self.std = None
         if cache_path is not None and not os.path.exists(cache_path):
             os.makedirs(cache_path)
@@ -728,15 +720,15 @@
             f0 = self.normalize(f0)
         return {"audio_unique_name": item["audio_unique_name"], "f0": f0}
 
     def __len__(self):
         return len(self.samples)
 
     def precompute(self, num_workers=0):
-        print("[*] Pre-computing F0s...")
+        logger.info("Pre-computing F0s...")
         with tqdm.tqdm(total=len(self)) as pbar:
             batch_size = num_workers if num_workers > 0 else 1
             # we do not normalize at preproessing
             normalize_f0 = self.normalize_f0
             self.normalize_f0 = False
             dataloder = torch.utils.data.DataLoader(
                 batch_size=batch_size, dataset=self, shuffle=False, num_workers=num_workers, collate_fn=self.collate_fn
@@ -815,17 +807,16 @@
         f0s_torch = torch.LongTensor(len(f0s), f0_lens_max).fill_(self.get_pad_id())
         for i, f0_len in enumerate(f0_lens):
             f0s_torch[i, :f0_len] = torch.LongTensor(f0s[i])
         return {"audio_unique_name": audio_unique_name, "f0": f0s_torch, "f0_lens": f0_lens}
 
     def print_logs(self, level: int = 0) -> None:
         indent = "\t" * level
-        print("\n")
-        print(f"{indent}> F0Dataset ")
-        print(f"{indent}| > Number of instances : {len(self.samples)}")
+        logger.info("%sF0Dataset", indent)
+        logger.info("%s| Number of instances : %d", indent, len(self.samples))
 
 
 class EnergyDataset:
     """Energy Dataset for computing Energy from wav files in CPU
 
     Pre-compute Energy values for all the samples at initialization if `cache_path` is not None or already present. It
     also computes the mean and std of Energy values if `normalize_Energy` is True.
@@ -848,22 +839,20 @@
             Whether to normalize Energy values by mean and std. Defaults to True.
     """
 
     def __init__(
         self,
         samples: Union[List[List], List[Dict]],
         ap: "AudioProcessor",
-        verbose=False,
         cache_path: str = None,
         precompute_num_workers=0,
         normalize_energy=True,
     ):
         self.samples = samples
         self.ap = ap
-        self.verbose = verbose
         self.cache_path = cache_path
         self.normalize_energy = normalize_energy
         self.pad_id = 0.0
         self.mean = None
         self.std = None
         if cache_path is not None and not os.path.exists(cache_path):
             os.makedirs(cache_path)
@@ -879,15 +868,15 @@
             energy = self.normalize(energy)
         return {"audio_unique_name": item["audio_unique_name"], "energy": energy}
 
     def __len__(self):
         return len(self.samples)
 
     def precompute(self, num_workers=0):
-        print("[*] Pre-computing energys...")
+        logger.info("Pre-computing energys...")
         with tqdm.tqdm(total=len(self)) as pbar:
             batch_size = num_workers if num_workers > 0 else 1
             # we do not normalize at preproessing
             normalize_energy = self.normalize_energy
             self.normalize_energy = False
             dataloder = torch.utils.data.DataLoader(
                 batch_size=batch_size, dataset=self, shuffle=False, num_workers=num_workers, collate_fn=self.collate_fn
@@ -967,10 +956,9 @@
         energys_torch = torch.LongTensor(len(energys), energy_lens_max).fill_(self.get_pad_id())
         for i, energy_len in enumerate(energy_lens):
             energys_torch[i, :energy_len] = torch.LongTensor(energys[i])
         return {"audio_unique_name": audio_unique_name, "energy": energys_torch, "energy_lens": energy_lens}
 
     def print_logs(self, level: int = 0) -> None:
         indent = "\t" * level
-        print("\n")
-        print(f"{indent}> energyDataset ")
-        print(f"{indent}| > Number of instances : {len(self.samples)}")
+        logger.info("%senergyDataset")
+        logger.info("%s| Number of instances : %d", indent, len(self.samples))
```

### Comparing `coqui-tts-0.22.1/TTS/tts/datasets/formatters.py` & `coqui_tts-0.23.0/TTS/tts/datasets/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import csv
+import logging
 import os
 import re
 import xml.etree.ElementTree as ET
 from glob import glob
 from pathlib import Path
 from typing import List
 
 from tqdm import tqdm
 
+logger = logging.getLogger(__name__)
+
 ########################
 # DATASETS
 ########################
 
 
 def cml_tts(root_path, meta_file, ignored_speakers=None):
     """Normalizes the CML-TTS meta data file to TTS format
@@ -19,15 +22,15 @@
     filepath = os.path.join(root_path, meta_file)
     # ensure there are 4 columns for every line
     with open(filepath, "r", encoding="utf8") as f:
         lines = f.readlines()
     num_cols = len(lines[0].split("|"))  # take the first row as reference
     for idx, line in enumerate(lines[1:]):
         if len(line.split("|")) != num_cols:
-            print(f" > Missing column in line {idx + 1} -> {line.strip()}")
+            logger.warning("Missing column in line %d -> %s", idx + 1, line.strip())
     # load metadata
     with open(Path(root_path) / meta_file, newline="", encoding="utf-8") as f:
         reader = csv.DictReader(f, delimiter="|")
         metadata = list(reader)
     assert all(x in metadata[0] for x in ["wav_filename", "transcript"])
     client_id = None if "client_id" in metadata[0] else "default"
     emotion_name = None if "emotion_name" in metadata[0] else "neutral"
@@ -46,28 +49,28 @@
                 "audio_file": audio_path,
                 "speaker_name": client_id if client_id is not None else row["client_id"],
                 "emotion_name": emotion_name if emotion_name is not None else row["emotion_name"],
                 "root_path": root_path,
             }
         )
     if not_found_counter > 0:
-        print(f" | > [!] {not_found_counter} files not found")
+        logger.warning("%d files not found", not_found_counter)
     return items
 
 
 def coqui(root_path, meta_file, ignored_speakers=None):
     """Interal dataset formatter."""
     filepath = os.path.join(root_path, meta_file)
     # ensure there are 4 columns for every line
     with open(filepath, "r", encoding="utf8") as f:
         lines = f.readlines()
     num_cols = len(lines[0].split("|"))  # take the first row as reference
     for idx, line in enumerate(lines[1:]):
         if len(line.split("|")) != num_cols:
-            print(f" > Missing column in line {idx + 1} -> {line.strip()}")
+            logger.warning("Missing column in line %d -> %s", idx + 1, line.strip())
     # load metadata
     with open(Path(root_path) / meta_file, newline="", encoding="utf-8") as f:
         reader = csv.DictReader(f, delimiter="|")
         metadata = list(reader)
     assert all(x in metadata[0] for x in ["audio_file", "text"])
     speaker_name = None if "speaker_name" in metadata[0] else "coqui"
     emotion_name = None if "emotion_name" in metadata[0] else "neutral"
@@ -86,15 +89,15 @@
                 "audio_file": audio_path,
                 "speaker_name": speaker_name if speaker_name is not None else row["speaker_name"],
                 "emotion_name": emotion_name if emotion_name is not None else row["emotion_name"],
                 "root_path": root_path,
             }
         )
     if not_found_counter > 0:
-        print(f" | > [!] {not_found_counter} files not found")
+        logger.warning("%d files not found", not_found_counter)
     return items
 
 
 def tweb(root_path, meta_file, **kwargs):  # pylint: disable=unused-argument
     """Normalize TWEB dataset.
     https://www.kaggle.com/bryanpark/the-world-english-bible-speech-dataset
     """
@@ -169,30 +172,30 @@
         if speaker_name_match is None:
             continue
         speaker_name = speaker_name_match.group("speaker_name")
         # ignore speakers
         if isinstance(ignored_speakers, list):
             if speaker_name in ignored_speakers:
                 continue
-        print(" | > {}".format(csv_file))
+        logger.info(csv_file)
         with open(txt_file, "r", encoding="utf-8") as ttf:
             for line in ttf:
                 cols = line.split("|")
                 if not meta_files:
                     wav_file = os.path.join(folder, "wavs", cols[0] + ".wav")
                 else:
                     wav_file = os.path.join(root_path, folder.replace("metadata.csv", ""), "wavs", cols[0] + ".wav")
                 if os.path.isfile(wav_file):
                     text = cols[1].strip()
                     items.append(
                         {"text": text, "audio_file": wav_file, "speaker_name": speaker_name, "root_path": root_path}
                     )
                 else:
                     # M-AI-Labs have some missing samples, so just print the warning
-                    print("> File %s does not exist!" % (wav_file))
+                    logger.warning("File %s does not exist!", wav_file)
     return items
 
 
 def ljspeech(root_path, meta_file, **kwargs):  # pylint: disable=unused-argument
     """Normalizes the LJSpeech meta data file to TTS format
     https://keithito.com/LJ-Speech-Dataset/"""
     txt_file = os.path.join(root_path, meta_file)
@@ -249,15 +252,15 @@
     xml_root = ET.parse(xml_file).getroot()
     items = []
     speaker_name = "sam_accenture"
     for item in xml_root.findall("./fileid"):
         text = item.text
         wav_file = os.path.join(root_path, "vo_voice_quality_transformation", item.get("id") + ".wav")
         if not os.path.exists(wav_file):
-            print(f" [!] {wav_file} in metafile does not exist. Skipping...")
+            logger.warning("%s in metafile does not exist. Skipping...", wav_file)
             continue
         items.append({"text": text, "audio_file": wav_file, "speaker_name": speaker_name, "root_path": root_path})
     return items
 
 
 def ruslan(root_path, meta_file, **kwargs):  # pylint: disable=unused-argument
     """Normalizes the RUSLAN meta data file to TTS format
@@ -370,15 +373,15 @@
             cols = line.split("|")
             wav_file = os.path.join(root_path, "wavs", cols[0].strip() + ".wav")
             if not os.path.exists(wav_file):
                 skipped_files.append(wav_file)
                 continue
             text = cols[1].strip()
             items.append({"text": text, "audio_file": wav_file, "speaker_name": speaker_name, "root_path": root_path})
-    print(f" [!] {len(skipped_files)} files skipped. They don't exist...")
+    logger.warning("%d files skipped. They don't exist...")
     return items
 
 
 # ToDo: add the dataset link when the dataset is released publicly
 def brspeech(root_path, meta_file, ignored_speakers=None):
     """BRSpeech 3.0 beta"""
     txt_file = os.path.join(root_path, meta_file)
@@ -438,15 +441,15 @@
         else:
             wav_file = os.path.join(root_path, wavs_path, speaker_id, file_id + f"_{mic}.{file_ext}")
         if os.path.exists(wav_file):
             items.append(
                 {"text": text, "audio_file": wav_file, "speaker_name": "VCTK_" + speaker_id, "root_path": root_path}
             )
         else:
-            print(f" [!] wav files don't exist - {wav_file}")
+            logger.warning("Wav file doesn't exist - %s", wav_file)
     return items
 
 
 def vctk_old(root_path, meta_files=None, wavs_path="wav48", ignored_speakers=None):
     """homepages.inf.ed.ac.uk/jyamagis/release/VCTK-Corpus.tar.gz"""
     items = []
     meta_files = glob(f"{os.path.join(root_path,'txt')}/**/*.txt", recursive=True)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/align_tts/duration_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/align_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/align_tts/mdn.py` & `coqui_tts-0.23.0/TTS/tts/layers/align_tts/mdn.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/hubert_manager.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/hubert_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # From https://github.com/gitmylo/bark-voice-cloning-HuBERT-quantizer
 
+import logging
 import os.path
 import shutil
 import urllib.request
 
 import huggingface_hub
 
+logger = logging.getLogger(__name__)
+
 
 class HubertManager:
     @staticmethod
     def make_sure_hubert_installed(
         download_url: str = "https://dl.fbaipublicfiles.com/hubert/hubert_base_ls960.pt", model_path: str = ""
     ):
         if not os.path.isfile(model_path):
-            print("Downloading HuBERT base model")
+            logger.info("Downloading HuBERT base model")
             urllib.request.urlretrieve(download_url, model_path)
-            print("Downloaded HuBERT")
+            logger.info("Downloaded HuBERT")
             return model_path
         return None
 
     @staticmethod
     def make_sure_tokenizer_installed(
         model: str = "quantifier_hubert_base_ls960_14.pth",
         repo: str = "GitMylo/bark-voice-cloning",
         model_path: str = "",
     ):
         model_dir = os.path.dirname(model_path)
         if not os.path.isfile(model_path):
-            print("Downloading HuBERT custom tokenizer")
+            logger.info("Downloading HuBERT custom tokenizer")
             huggingface_hub.hf_hub_download(repo, model, local_dir=model_dir, local_dir_use_symlinks=False)
             shutil.move(os.path.join(model_dir, model), model_path)
-            print("Downloaded tokenizer")
+            logger.info("Downloaded tokenizer")
             return model_path
         return None
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/kmeans_hubert.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/kmeans_hubert.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/hubert/tokenizer.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/hubert/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Custom tokenizer model.
 Author: https://www.github.com/gitmylo/
 License: MIT
 """
 
 import json
+import logging
 import os.path
 from zipfile import ZipFile
 
 import numpy
 import torch
 from torch import nn, optim
 
+logger = logging.getLogger(__name__)
+
 
 class HubertTokenizer(nn.Module):
     def __init__(self, hidden_size=1024, input_size=768, output_size=10000, version=0):
         super().__init__()
         next_size = input_size
         if version == 0:
             self.lstm = nn.LSTM(input_size, hidden_size, 2, batch_first=True)
@@ -81,15 +84,15 @@
         y_train_hot = y_train_hot.to("cuda")
 
         # Calculate the loss
         loss = lossfunc(y_pred, y_train_hot)
 
         # Print loss
         if log_loss:
-            print("Loss", loss.item())
+            logger.info("Loss %.3f", loss.item())
 
         # Backward pass
         loss.backward()
 
         # Update the weights
         optimizer.step()
 
@@ -153,18 +156,18 @@
         return json.dumps(data)
 
 
 def auto_train(data_path, save_path="model.pth", load_model: str = None, save_epochs=1):
     data_x, data_y = [], []
 
     if load_model and os.path.isfile(load_model):
-        print("Loading model from", load_model)
+        logger.info("Loading model from %s", load_model)
         model_training = HubertTokenizer.load_from_checkpoint(load_model, "cuda")
     else:
-        print("Creating new model.")
+        logger.info("Creating new model.")
         model_training = HubertTokenizer(version=1).to("cuda")  # Settings for the model to run without lstm
     save_path = os.path.join(data_path, save_path)
     base_save_path = ".".join(save_path.split(".")[:-1])
 
     sem_string = "_semantic.npy"
     feat_string = "_semantic_features.npy"
 
@@ -187,9 +190,9 @@
                     torch.tensor(x).to("cuda"), torch.tensor(y).to("cuda"), j % 50 == 0
                 )  # Print loss every 50 steps
                 j += 1
         save_p = save_path
         save_p_2 = f"{base_save_path}_epoch_{epoch}.pth"
         model_training.save(save_p)
         model_training.save(save_p_2)
-        print(f"Epoch {epoch} completed")
+        logger.info("Epoch %d completed", epoch)
         epoch += 1
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/inference_funcs.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/inference_funcs.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/load_model.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/load_model.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/model.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/model.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/bark/model_fine.py` & `coqui_tts-0.23.0/TTS/tts/layers/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/acoustic_model.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/acoustic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ### credit: https://github.com/dunky11/voicesmith
+import logging
 from typing import Callable, Dict, Tuple
 
 import torch
 import torch.nn.functional as F
 from coqpit import Coqpit
 from torch import nn
 
@@ -16,14 +17,16 @@
 from TTS.tts.layers.delightful_tts.networks import EmbeddingPadded, positional_encoding
 from TTS.tts.layers.delightful_tts.phoneme_prosody_predictor import PhonemeProsodyPredictor
 from TTS.tts.layers.delightful_tts.pitch_adaptor import PitchAdaptor
 from TTS.tts.layers.delightful_tts.variance_predictor import VariancePredictor
 from TTS.tts.layers.generic.aligner import AlignmentNetwork
 from TTS.tts.utils.helpers import generate_path, maximum_path, sequence_mask
 
+logger = logging.getLogger(__name__)
+
 
 class AcousticModel(torch.nn.Module):
     def __init__(
         self,
         args: "ModelArgs",
         tokenizer: "TTSTokenizer" = None,
         speaker_manager: "SpeakerManager" = None,
@@ -213,15 +216,15 @@
     #         self.embedding_dims = self.embedded_speaker_dim
     #     else:
     #         self.embedding_dims = 0
 
     def _init_speaker_embedding(self):
         # pylint: disable=attribute-defined-outside-init
         if self.num_speakers > 0:
-            print(" > initialization of speaker-embedding layers.")
+            logger.info("Initialization of speaker-embedding layers.")
             self.embedded_speaker_dim = self.args.speaker_embedding_channels
             self.emb_g = nn.Embedding(self.num_speakers, self.embedded_speaker_dim)
 
     def _init_d_vector(self):
         # pylint: disable=attribute-defined-outside-init
         if hasattr(self, "emb_g"):
             raise ValueError("[!] Speaker embedding layer already initialized before d_vector settings.")
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/conformer.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conformer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/conv_layers.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/conv_layers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/encoders.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/encoders.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/energy_adaptor.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/energy_adaptor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/kernel_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/kernel_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/networks.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/networks.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/phoneme_prosody_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/pitch_adaptor.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/pitch_adaptor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/delightful_tts/variance_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/delightful_tts/variance_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/feed_forward/decoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/feed_forward/duration_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/feed_forward/encoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/feed_forward/encoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/aligner.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/aligner.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/gated_conv.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/gated_conv.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/normalization.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/normalization.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/pos_encoding.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/pos_encoding.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/res_conv_bn.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/res_conv_bn.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/time_depth_sep_conv.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/time_depth_sep_conv.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/transformer.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/generic/wavenet.py` & `coqui_tts-0.23.0/TTS/tts/layers/generic/wavenet.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/glow_tts/decoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/glow_tts/duration_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/glow_tts/encoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/encoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/glow_tts/glow.py` & `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/glow.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/glow_tts/transformer.py` & `coqui_tts-0.23.0/TTS/tts/layers/glow_tts/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/losses.py` & `coqui_tts-0.23.0/TTS/tts/layers/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 import math
 
 import numpy as np
 import torch
 from coqpit import Coqpit
 from torch import nn
 from torch.nn import functional
 
 from TTS.tts.utils.helpers import sequence_mask
 from TTS.tts.utils.ssim import SSIMLoss as _SSIMLoss
 from TTS.utils.audio.torch_transforms import TorchSTFT
 
+logger = logging.getLogger(__name__)
+
 
 # pylint: disable=abstract-method
 # relates https://github.com/pytorch/pytorch/issues/42305
 class L1LossMasked(nn.Module):
     def __init__(self, seq_len_norm):
         super().__init__()
         self.seq_len_norm = seq_len_norm
@@ -128,19 +131,19 @@
         """
         mask = sequence_mask(sequence_length=length, max_len=y.size(1)).unsqueeze(2)
         y_norm = sample_wise_min_max(y, mask)
         y_hat_norm = sample_wise_min_max(y_hat, mask)
         ssim_loss = self.loss_func((y_norm * mask).unsqueeze(1), (y_hat_norm * mask).unsqueeze(1))
 
         if ssim_loss.item() > 1.0:
-            print(f" > SSIM loss is out-of-range {ssim_loss.item()}, setting it 1.0")
+            logger.info("SSIM loss is out-of-range (%.2f), setting it to 1.0", ssim_loss.item())
             ssim_loss = torch.tensor(1.0, device=ssim_loss.device)
 
         if ssim_loss.item() < 0.0:
-            print(f" > SSIM loss is out-of-range {ssim_loss.item()}, setting it 0.0")
+            logger.info("SSIM loss is out-of-range (%.2f), setting it to 0.0", ssim_loss.item())
             ssim_loss = torch.tensor(0.0, device=ssim_loss.device)
 
         return ssim_loss
 
 
 class AttentionEntropyLoss(nn.Module):
     # pylint: disable=R0201
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/overflow/common_layers.py` & `coqui_tts-0.23.0/TTS/tts/layers/overflow/common_layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import logging
 from typing import List, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 from tqdm.auto import tqdm
 
 from TTS.tts.layers.tacotron.common_layers import Linear
 from TTS.tts.layers.tacotron.tacotron2 import ConvBNBlock
 
+logger = logging.getLogger(__name__)
+
 
 class Encoder(nn.Module):
     r"""Neural HMM Encoder
 
     Same as Tacotron 2 encoder but increases the input length by states per phone
 
     Args:
@@ -209,16 +212,16 @@
 
         Args:
             std (float Tensor): tensor containing the standard deviation to be
         """
         original_tensor = std.clone().detach()
         std = torch.clamp(std, min=self.std_floor)
         if torch.any(original_tensor != std):
-            print(
-                "[*] Standard deviation was floored! The model is preventing overfitting, nothing serious to worry about"
+            logger.info(
+                "Standard deviation was floored! The model is preventing overfitting, nothing serious to worry about"
             )
         return std
 
 
 class OverflowUtils:
     @staticmethod
     def get_data_parameters_for_flat_start(
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/overflow/decoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/overflow/decoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/overflow/neural_hmm.py` & `coqui_tts-0.23.0/TTS/tts/layers/overflow/neural_hmm.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/overflow/plotting_utils.py` & `coqui_tts-0.23.0/TTS/tts/layers/overflow/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/attentions.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/attentions.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/capacitron_layers.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/capacitron_layers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/common_layers.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/common_layers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/gst_layers.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/gst_layers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/tacotron.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # coding: utf-8
 # adapted from https://github.com/r9y9/tacotron_pytorch
 
+import logging
+
 import torch
 from torch import nn
 
 from .attentions import init_attn
 from .common_layers import Prenet
 
+logger = logging.getLogger(__name__)
+
 
 class BatchNormConv1d(nn.Module):
     r"""A wrapper for Conv1d with BatchNorm. It sets the activation
     function between Conv and BatchNorm layers. BatchNorm layer
     is initialized with the TF default values for momentum and eps.
 
     Args:
@@ -476,15 +480,15 @@
             outputs += [output]
             attentions += [attention]
             stop_tokens += [stop_token]
             t += 1
             if t > inputs.shape[1] / 4 and (stop_token > 0.6 or attention[:, -1].item() > 0.6):
                 break
             if t > self.max_decoder_steps:
-                print("   | > Decoder stopped with 'max_decoder_steps")
+                logger.info("Decoder stopped with `max_decoder_steps` %d", self.max_decoder_steps)
                 break
         return self._parse_outputs(outputs, attentions, stop_tokens)
 
 
 class StopNet(nn.Module):
     r"""Stopnet signalling decoder to stop inference.
     Args:
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tacotron/tacotron2.py` & `coqui_tts-0.23.0/TTS/tts/layers/tacotron/tacotron2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+import logging
+
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 from .attentions import init_attn
 from .common_layers import Linear, Prenet
 
+logger = logging.getLogger(__name__)
+
 
 # pylint: disable=no-value-for-parameter
 # pylint: disable=unexpected-keyword-arg
 class ConvBNBlock(nn.Module):
     r"""Convolutions with Batch Normalization and non-linear activation.
 
     Args:
@@ -352,15 +356,15 @@
             outputs += [decoder_output.squeeze(1)]
             stop_tokens += [stop_token]
             alignments += [alignment]
 
             if stop_token > self.stop_threshold and t > inputs.shape[0] // 2:
                 break
             if len(outputs) == self.max_decoder_steps:
-                print(f"   > Decoder stopped with `max_decoder_steps` {self.max_decoder_steps}")
+                logger.info("Decoder stopped with `max_decoder_steps` %d", self.max_decoder_steps)
                 break
 
             memory = self._update_memory(decoder_output)
             t += 1
 
         outputs, stop_tokens, alignments = self._parse_outputs(outputs, stop_tokens, alignments)
 
@@ -385,15 +389,15 @@
             outputs += [decoder_output.squeeze(1)]
             stop_tokens += [stop_token]
             alignments += [alignment]
 
             if stop_token > 0.7:
                 break
             if len(outputs) == self.max_decoder_steps:
-                print("   | > Decoder stopped with 'max_decoder_steps")
+                logger.info("Decoder stopped with `max_decoder_steps` %d", self.max_decoder_steps)
                 break
 
             self.memory_truncated = decoder_output
             t += 1
 
         outputs, stop_tokens, alignments = self._parse_outputs(outputs, stop_tokens, alignments)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/arch_utils.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/arch_utils.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/audio_utils.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/audio_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import logging
 import os
 from glob import glob
 from typing import Dict, List
 
 import librosa
 import numpy as np
 import torch
 import torchaudio
 from scipy.io.wavfile import read
 
 from TTS.utils.audio.torch_transforms import TorchSTFT
 
+logger = logging.getLogger(__name__)
+
 
 def load_wav_to_torch(full_path):
     sampling_rate, data = read(full_path)
     if data.dtype == np.int32:
         norm_fix = 2**31
     elif data.dtype == np.int16:
         norm_fix = 2**15
@@ -24,15 +27,15 @@
     return (torch.FloatTensor(data.astype(np.float32)) / norm_fix, sampling_rate)
 
 
 def check_audio(audio, audiopath: str):
     # Check some assumptions about audio range. This should be automatically fixed in load_wav_to_torch, but might not be in some edge cases, where we should squawk.
     # '2' is arbitrarily chosen since it seems like audio will often "overdrive" the [-1,1] bounds.
     if torch.any(audio > 2) or not torch.any(audio < 0):
-        print(f"Error with {audiopath}. Max={audio.max()} min={audio.min()}")
+        logger.error("Error with %s. Max=%.2f min=%.2f", audiopath, audio.max(), audio.min())
     audio.clip_(-1, 1)
 
 
 def read_audio_file(audiopath: str):
     if audiopath[-4:] == ".wav":
         audio, lsr = load_wav_to_torch(audiopath)
     elif audiopath[-4:] == ".mp3":
@@ -132,15 +135,15 @@
 
 def load_voices(voices: List[str], extra_voice_dirs: List[str] = []):
     latents = []
     clips = []
     for voice in voices:
         if voice == "random":
             if len(voices) > 1:
-                print("Cannot combine a random voice with a non-random voice. Just using a random voice.")
+                logger.warning("Cannot combine a random voice with a non-random voice. Just using a random voice.")
             return None, None
         clip, latent = load_voice(voice, extra_voice_dirs)
         if latent is None:
             assert (
                 len(latents) == 0
             ), "Can only combine raw audio voices or latent voices, not both. Do it yourself if you want this."
             clips.extend(clip)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/autoregressive.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/autoregressive.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/classifier.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/classifier.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/clvp.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/clvp.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/diffusion.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/diffusion_decoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/diffusion_decoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/dpm_solver.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/dpm_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import logging
 import math
 
 import torch
 
+logger = logging.getLogger(__name__)
+
 
 class NoiseScheduleVP:
     def __init__(
         self,
         schedule="discrete",
         betas=None,
         alphas_cumprod=None,
@@ -1167,15 +1170,15 @@
                 x_prev = x_lower
                 lambda_s = ns.marginal_lambda(s)
             h = torch.min(
                 theta * h * torch.float_power(E, -1.0 / order).float(),
                 lambda_0 - lambda_s,
             )
             nfe += order
-        print("adaptive solver nfe", nfe)
+        logger.debug("adaptive solver nfe %d", nfe)
         return x
 
     def add_noise(self, x, t, noise=None):
         """
         Compute the noised input xt = alpha_t * x + sigma_t * noise.
 
         Args:
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/random_latent_generator.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/random_latent_generator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/tokenizer.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/tokenizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/transformer.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/transformer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/utils.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import logging
 import os
 from urllib import request
 
 from tqdm import tqdm
 
+logger = logging.getLogger(__name__)
+
 DEFAULT_MODELS_DIR = os.path.join(os.path.expanduser("~"), ".cache", "tortoise", "models")
 MODELS_DIR = os.environ.get("TORTOISE_MODELS_DIR", DEFAULT_MODELS_DIR)
 MODELS_DIR = "/data/speech_synth/models/"
 MODELS = {
     "autoregressive.pth": "https://huggingface.co/jbetker/tortoise-tts-v2/resolve/main/.models/autoregressive.pth",
     "classifier.pth": "https://huggingface.co/jbetker/tortoise-tts-v2/resolve/main/.models/classifier.pth",
     "clvp2.pth": "https://huggingface.co/jbetker/tortoise-tts-v2/resolve/main/.models/clvp2.pth",
@@ -24,18 +27,18 @@
     os.makedirs(MODELS_DIR, exist_ok=True)
     for model_name, url in MODELS.items():
         if specific_models is not None and model_name not in specific_models:
             continue
         model_path = os.path.join(MODELS_DIR, model_name)
         if os.path.exists(model_path):
             continue
-        print(f"Downloading {model_name} from {url}...")
+        logger.info("Downloading %s from %s...", model_name, url)
         with tqdm(unit="B", unit_scale=True, unit_divisor=1024, miniters=1) as t:
             request.urlretrieve(url, model_path, lambda nb, bs, fs, t=t: t.update(nb * bs - t.n))
-        print("Done.")
+        logger.info("Done.")
 
 
 def get_model_path(model_name, models_dir=MODELS_DIR):
     """
     Get path to given model, download it if it doesn't exist.
     """
     if model_name not in MODELS:
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/vocoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/vocoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/wav2vec_alignment.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/wav2vec_alignment.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/tortoise/xtransformers.py` & `coqui_tts-0.23.0/TTS/tts/layers/tortoise/xtransformers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/vits/discriminator.py` & `coqui_tts-0.23.0/TTS/tts/layers/vits/discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/vits/networks.py` & `coqui_tts-0.23.0/TTS/tts/layers/vits/networks.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/vits/stochastic_duration_predictor.py` & `coqui_tts-0.23.0/TTS/tts/layers/vits/stochastic_duration_predictor.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/vits/transforms.py` & `coqui_tts-0.23.0/TTS/tts/layers/vits/transforms.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/dvae.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/dvae.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import functools
+import logging
 from math import sqrt
 
 import torch
 import torch.distributed as distributed
 import torch.nn as nn
 import torch.nn.functional as F
 import torchaudio
 from einops import rearrange
 
+logger = logging.getLogger(__name__)
+
 
 def default(val, d):
     return val if val is not None else d
 
 
 def eval_decorator(fn):
     def inner(model, *args, **kwargs):
@@ -75,15 +78,15 @@
             ep = self.embed.permute(1, 0)
             ea = self.embed_avg.permute(1, 0)
             rand_embed = torch.randn_like(ep) * mask
             self.embed = (ep * ~mask + rand_embed).permute(1, 0)
             self.embed_avg = (ea * ~mask + rand_embed).permute(1, 0)
             self.cluster_size = self.cluster_size * ~mask.squeeze()
             if torch.any(mask):
-                print(f"Reset {torch.sum(mask)} embedding codes.")
+                logger.info("Reset %d embedding codes.", torch.sum(mask))
                 self.codes = None
                 self.codes_full = False
 
         flatten = input.reshape(-1, self.dim)
         dist = flatten.pow(2).sum(1, keepdim=True) - 2 * flatten @ self.embed + self.embed.pow(2).sum(0, keepdim=True)
         soft_codes = -dist
         _, embed_ind = soft_codes.max(1)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/gpt.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/gpt_inference.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/gpt_inference.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/hifigan_decoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/hifigan_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import logging
+
 import torch
 import torchaudio
 from torch import nn
 from torch.nn import Conv1d, ConvTranspose1d
 from torch.nn import functional as F
 from torch.nn.utils.parametrizations import weight_norm
 from torch.nn.utils.parametrize import remove_parametrizations
 
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 LRELU_SLOPE = 0.1
 
 
 def get_padding(k, d):
     return int((k * d - d) / 2)
 
 
@@ -312,15 +316,15 @@
             Tensor: [B, 1, T]
         """
         c = c.to(self.conv_pre.weight.device)
         c = torch.nn.functional.pad(c, (self.inference_padding, self.inference_padding), "replicate")
         return self.forward(c)
 
     def remove_weight_norm(self):
-        print("Removing weight norm...")
+        logger.info("Removing weight norm...")
         for l in self.ups:
             remove_parametrizations(l, "weight")
         for l in self.resblocks:
             l.remove_weight_norm()
         remove_parametrizations(self.conv_pre, "weight")
         remove_parametrizations(self.conv_post, "weight")
 
@@ -386,26 +390,26 @@
         return out
 
 
 def set_init_dict(model_dict, checkpoint_state, c):
     # Partial initialization: if there is a mismatch with new and old layer, it is skipped.
     for k, v in checkpoint_state.items():
         if k not in model_dict:
-            print(" | > Layer missing in the model definition: {}".format(k))
+            logger.warning("Layer missing in the model definition: %s", k)
     # 1. filter out unnecessary keys
     pretrained_dict = {k: v for k, v in checkpoint_state.items() if k in model_dict}
     # 2. filter out different size layers
     pretrained_dict = {k: v for k, v in pretrained_dict.items() if v.numel() == model_dict[k].numel()}
     # 3. skip reinit layers
     if c.has("reinit_layers") and c.reinit_layers is not None:
         for reinit_layer_name in c.reinit_layers:
             pretrained_dict = {k: v for k, v in pretrained_dict.items() if reinit_layer_name not in k}
     # 4. overwrite entries in the existing state dict
     model_dict.update(pretrained_dict)
-    print(" | > {} / {} layers are restored.".format(len(pretrained_dict), len(model_dict)))
+    logger.info("%d / %d layers are restored.", len(pretrained_dict), len(model_dict))
     return model_dict
 
 
 class PreEmphasis(nn.Module):
     def __init__(self, coefficient=0.97):
         super().__init__()
         self.coefficient = coefficient
@@ -575,32 +579,32 @@
         use_cuda: bool = False,
         criterion=None,
         cache=False,
     ):
         state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         try:
             self.load_state_dict(state["model"])
-            print(" > Model fully restored. ")
+            logger.info("Model fully restored.")
         except (KeyError, RuntimeError) as error:
             # If eval raise the error
             if eval:
                 raise error
 
-            print(" > Partial model initialization.")
+            logger.info("Partial model initialization.")
             model_dict = self.state_dict()
             model_dict = set_init_dict(model_dict, state["model"])
             self.load_state_dict(model_dict)
             del model_dict
 
         # load the criterion for restore_path
         if criterion is not None and "criterion" in state:
             try:
                 criterion.load_state_dict(state["criterion"])
             except (KeyError, RuntimeError) as error:
-                print(" > Criterion load ignored because of:", error)
+                logger.exception("Criterion load ignored because of: %s", error)
 
         if use_cuda:
             self.cuda()
             if criterion is not None:
                 criterion = criterion.cuda()
 
         if eval:
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/latent_encoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/latent_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/perceiver_encoder.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/perceiver_encoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/stream_generator.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/stream_generator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/tokenizer.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,45 @@
+import logging
 import os
 import re
 import textwrap
 from functools import cached_property
 
 import pypinyin
 import torch
 from hangul_romanize import Transliter
 from hangul_romanize.rule import academic
 from num2words import num2words
 from spacy.lang.ar import Arabic
 from spacy.lang.en import English
 from spacy.lang.es import Spanish
+from spacy.lang.hi import Hindi
 from spacy.lang.ja import Japanese
 from spacy.lang.zh import Chinese
 from tokenizers import Tokenizer
 
 from TTS.tts.layers.xtts.zh_num2words import TextNorm as zh_num2words
 
+logger = logging.getLogger(__name__)
+
 
 def get_spacy_lang(lang):
+    """Return Spacy language used for sentence splitting."""
     if lang == "zh":
         return Chinese()
     elif lang == "ja":
         return Japanese()
     elif lang == "ar":
         return Arabic()
     elif lang == "es":
         return Spanish()
+    elif lang == "hi":
+        return Hindi()
     else:
-        # For most languages, Enlish does the job
+        # For most languages, English does the job
         return English()
 
 
 def split_sentence(text, lang, text_split_length=250):
     """Preprocess the input text"""
     text_splits = []
     if text_split_length is not None and len(text) >= text_split_length:
@@ -607,28 +614,31 @@
             "cs": 186,
             "ru": 182,
             "nl": 251,
             "tr": 226,
             "ja": 71,
             "hu": 224,
             "ko": 95,
+            "hi": 150,
         }
 
     @cached_property
     def katsu(self):
         import cutlet
 
         return cutlet.Cutlet()
 
     def check_input_length(self, txt, lang):
         lang = lang.split("-")[0]  # remove the region
         limit = self.char_limits.get(lang, 250)
         if len(txt) > limit:
-            print(
-                f"[!] Warning: The text length exceeds the character limit of {limit} for language '{lang}', this might cause truncated audio."
+            logger.warning(
+                "The text length exceeds the character limit of %d for language '%s', this might cause truncated audio.",
+                limit,
+                lang,
             )
 
     def preprocess_text(self, txt, lang):
         if lang in {"ar", "cs", "de", "en", "es", "fr", "hu", "it", "nl", "pl", "pt", "ru", "tr", "zh", "ko"}:
             txt = multilingual_cleaners(txt, lang)
             if lang == "zh":
                 txt = chinese_transliterate(txt)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/trainer/dataset.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 import random
 import sys
 
 import torch
 import torch.nn.functional as F
 import torch.utils.data
 
 from TTS.tts.models.xtts import load_audio
 
+logger = logging.getLogger(__name__)
+
 torch.set_num_threads(1)
 
 
 def key_samples_by_col(samples, col):
     """Returns a dictionary of samples keyed by language."""
     samples_by_col = {}
     for sample in samples:
@@ -66,21 +69,21 @@
         self.samples = samples
         if not is_eval:
             random.seed(config.training_seed)
             # random.shuffle(self.samples)
             random.shuffle(self.samples)
             # order by language
             self.samples = key_samples_by_col(self.samples, "language")
-            print(" > Sampling by language:", self.samples.keys())
+            logger.info("Sampling by language: %s", self.samples.keys())
         else:
             # for evaluation load and check samples that are corrupted to ensures the reproducibility
             self.check_eval_samples()
 
     def check_eval_samples(self):
-        print(" > Filtering invalid eval samples!!")
+        logger.info("Filtering invalid eval samples!!")
         new_samples = []
         for sample in self.samples:
             try:
                 tseq, _, wav, _, _, _ = self.load_item(sample)
             except:
                 continue
             # Basically, this audio file is nonexistent or too long to be supported by the dataset.
@@ -88,15 +91,15 @@
                 wav is None
                 or (self.max_wav_len is not None and wav.shape[-1] > self.max_wav_len)
                 or (self.max_text_len is not None and tseq.shape[0] > self.max_text_len)
             ):
                 continue
             new_samples.append(sample)
         self.samples = new_samples
-        print(" > Total eval samples after filtering:", len(self.samples))
+        logger.info("Total eval samples after filtering: %d", len(self.samples))
 
     def get_text(self, text, lang):
         tokens = self.tokenizer.encode(text, lang)
         tokens = torch.IntTensor(tokens)
         assert not torch.any(tokens == 1), f"UNK token found in {text} -> {self.tokenizer.decode(tokens)}"
         # The stop token should always be sacred.
         assert not torch.any(tokens == 0), f"Stop token found in {text}"
@@ -146,38 +149,41 @@
             sample = self.samples[lang][index]
             # a unique id for each sampel to deal with fails
             sample_id = lang + "_" + str(index)
 
         # ignore samples that we already know that is not valid ones
         if sample_id in self.failed_samples:
             if self.debug_failures:
-                print(f"Ignoring sample {sample['audio_file']} because it was already ignored before !!")
+                logger.info("Ignoring sample %s because it was already ignored before !!", sample["audio_file"])
             # call get item again to get other sample
             return self[1]
 
         # try to load the sample, if fails added it to the failed samples list
         try:
             tseq, audiopath, wav, cond, cond_len, cond_idxs = self.load_item(sample)
         except:
             if self.debug_failures:
-                print(f"error loading {sample['audio_file']} {sys.exc_info()}")
+                logger.warning("Error loading %s %s", sample["audio_file"], sys.exc_info())
             self.failed_samples.add(sample_id)
             return self[1]
 
         # check if the audio and text size limits and if it out of the limits, added it failed_samples
         if (
             wav is None
             or (self.max_wav_len is not None and wav.shape[-1] > self.max_wav_len)
             or (self.max_text_len is not None and tseq.shape[0] > self.max_text_len)
         ):
             # Basically, this audio file is nonexistent or too long to be supported by the dataset.
             # It's hard to handle this situation properly. Best bet is to return the a random valid token and skew the dataset somewhat as a result.
             if self.debug_failures and wav is not None and tseq is not None:
-                print(
-                    f"error loading {sample['audio_file']}: ranges are out of bounds; {wav.shape[-1]}, {tseq.shape[0]}"
+                logger.warning(
+                    "Error loading %s: ranges are out of bounds: %d, %d",
+                    sample["audio_file"],
+                    wav.shape[-1],
+                    tseq.shape[0],
                 )
             self.failed_samples.add(sample_id)
             return self[1]
 
         res = {
             # 'real_text': text,
             "text": tseq,
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/trainer/gpt_trainer.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/trainer/gpt_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from dataclasses import dataclass, field
 from typing import Dict, List, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torchaudio
 from coqpit import Coqpit
@@ -15,14 +16,16 @@
 from TTS.tts.layers.xtts.dvae import DiscreteVAE
 from TTS.tts.layers.xtts.tokenizer import VoiceBpeTokenizer
 from TTS.tts.layers.xtts.trainer.dataset import XTTSDataset
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.tts.models.xtts import Xtts, XttsArgs, XttsAudioConfig
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class GPTTrainerConfig(XttsConfig):
     lr: float = 5e-06
     training_seed: int = 1
     optimizer_wd_only_on_weights: bool = False
     weighted_loss_attrs: dict = field(default_factory=lambda: {})
@@ -53,15 +56,15 @@
     vocoder: str = ""  # overide vocoder key on the config to avoid json write issues
 
 
 def callback_clearml_load_save(operation_type, model_info):
     # return None means skip the file upload/log, returning model_info will continue with the log/upload
     # you can also change the upload destination file name model_info.upload_filename or check the local file size with Path(model_info.local_model_path).stat().st_size
     assert operation_type in ("load", "save")
-    # print(operation_type, model_info.__dict__)
+    logger.debug("%s %s", operation_type, model_info.__dict__)
 
     if "similarities.pth" in model_info.__dict__["local_model_path"]:
         return None
 
     return model_info
 
 
@@ -87,15 +90,15 @@
             self.xtts.mel_stats = load_fsspec(self.args.mel_norm_file)
 
         # load GPT if available
         if self.args.gpt_checkpoint:
             gpt_checkpoint = torch.load(self.args.gpt_checkpoint, map_location=torch.device("cpu"))
             # deal with coqui Trainer exported model
             if "model" in gpt_checkpoint.keys() and "config" in gpt_checkpoint.keys():
-                print("Coqui Trainer checkpoint detected! Converting it!")
+                logger.info("Coqui Trainer checkpoint detected! Converting it!")
                 gpt_checkpoint = gpt_checkpoint["model"]
                 states_keys = list(gpt_checkpoint.keys())
                 for key in states_keys:
                     if "gpt." in key:
                         new_key = key.replace("gpt.", "")
                         gpt_checkpoint[new_key] = gpt_checkpoint[key]
                         del gpt_checkpoint[key]
@@ -106,15 +109,15 @@
             if (
                 "text_embedding.weight" in gpt_checkpoint
                 and gpt_checkpoint["text_embedding.weight"].shape != self.xtts.gpt.text_embedding.weight.shape
             ):
                 num_new_tokens = (
                     self.xtts.gpt.text_embedding.weight.shape[0] - gpt_checkpoint["text_embedding.weight"].shape[0]
                 )
-                print(f" > Loading checkpoint with {num_new_tokens} additional tokens.")
+                logger.info("Loading checkpoint with %d additional tokens.", num_new_tokens)
 
                 # add new tokens to a linear layer (text_head)
                 emb_g = gpt_checkpoint["text_embedding.weight"]
                 new_row = torch.randn(num_new_tokens, emb_g.shape[1])
                 start_token_row = emb_g[-1, :]
                 emb_g = torch.cat([emb_g, new_row], axis=0)
                 emb_g[-1, :] = start_token_row
@@ -133,15 +136,15 @@
                 start_token_row = text_head_bias[-1]
                 new_bias_entry = torch.zeros(num_new_tokens)
                 text_head_bias = torch.cat([text_head_bias, new_bias_entry], axis=0)
                 text_head_bias[-1] = start_token_row
                 gpt_checkpoint["text_head.bias"] = text_head_bias
 
             self.xtts.gpt.load_state_dict(gpt_checkpoint, strict=True)
-            print(">> GPT weights restored from:", self.args.gpt_checkpoint)
+            logger.info("GPT weights restored from: %s", self.args.gpt_checkpoint)
 
         # Mel spectrogram extractor for conditioning
         if self.args.gpt_use_perceiver_resampler:
             self.torch_mel_spectrogram_style_encoder = TorchMelSpectrogram(
                 filter_length=2048,
                 hop_length=256,
                 win_length=1024,
@@ -179,15 +182,15 @@
             use_transposed_convs=False,
         )
 
         self.dvae.eval()
         if self.args.dvae_checkpoint:
             dvae_checkpoint = torch.load(self.args.dvae_checkpoint, map_location=torch.device("cpu"))
             self.dvae.load_state_dict(dvae_checkpoint, strict=False)
-            print(">> DVAE weights restored from:", self.args.dvae_checkpoint)
+            logger.info("DVAE weights restored from: %s", self.args.dvae_checkpoint)
         else:
             raise RuntimeError(
                 "You need to specify config.model_args.dvae_checkpoint path to be able to train the GPT decoder!!"
             )
 
         # Mel spectrogram extractor for DVAE
         self.torch_mel_spectrogram_dvae = TorchMelSpectrogram(
@@ -225,15 +228,15 @@
     @torch.no_grad()
     def test_run(self, assets) -> Tuple[Dict, Dict]:  # pylint: disable=W0613
         test_audios = {}
         if self.config.test_sentences:
             # init gpt for inference mode
             self.xtts.gpt.init_gpt_for_inference(kv_cache=self.args.kv_cache, use_deepspeed=False)
             self.xtts.gpt.eval()
-            print(" | > Synthesizing test sentences.")
+            logger.info("Synthesizing test sentences.")
             for idx, s_info in enumerate(self.config.test_sentences):
                 wav = self.xtts.synthesize(
                     s_info["text"],
                     self.config,
                     s_info["speaker_wav"],
                     s_info["language"],
                     gpt_cond_len=3,
```

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/xtts_manager.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/xtts_manager.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/layers/xtts/zh_num2words.py` & `coqui_tts-0.23.0/TTS/tts/layers/xtts/zh_num2words.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # Authors:
 #   2019.5 Zhiyang Zhou (https://github.com/Joee1995/chn_text_norm.git)
 #   2019.9 - 2022 Jiayu DU
 
 import argparse
 import csv
+import logging
 import re
 import string
 import sys
 
+logger = logging.getLogger(__name__)
+
 # fmt: off
 # ================================================================================ #
 #                                    basic constant
 # ================================================================================ #
 CHINESE_DIGIS = "零一二三四五六七八九"
 BIG_CHINESE_DIGIS_SIMPLIFIED = "零壹贰叁肆伍陆柒捌玖"
 BIG_CHINESE_DIGIS_TRADITIONAL = "零壹貳參肆伍陸柒捌玖"
@@ -919,97 +922,98 @@
 
     def percentage2chntext(self):
         return "百分之" + num2chn(self.percentage.strip().strip("%"))
 
 
 def normalize_nsw(raw_text):
     text = "^" + raw_text + "$"
+    logger.debug(text)
 
     # 规范化日期
     pattern = re.compile(r"\D+((([089]\d|(19|20)\d{2})年)?(\d{1,2}月(\d{1,2}[日号])?)?)")
     matchers = pattern.findall(text)
     if matchers:
-        # print('date')
+        logger.debug("date")
         for matcher in matchers:
             text = text.replace(matcher[0], Date(date=matcher[0]).date2chntext(), 1)
 
     # 规范化金钱
     pattern = re.compile(r"\D+((\d+(\.\d+)?)[多余几]?" + CURRENCY_UNITS + r"(\d" + CURRENCY_UNITS + r"?)?)")
     matchers = pattern.findall(text)
     if matchers:
-        # print('money')
+        logger.debug("money")
         for matcher in matchers:
             text = text.replace(matcher[0], Money(money=matcher[0]).money2chntext(), 1)
 
     # 规范化固话/手机号码
     # 手机
     # http://www.jihaoba.com/news/show/13680
     # 移动：139、138、137、136、135、134、159、158、157、150、151、152、188、187、182、183、184、178、198
     # 联通：130、131、132、156、155、186、185、176
     # 电信：133、153、189、180、181、177
     pattern = re.compile(r"\D((\+?86 ?)?1([38]\d|5[0-35-9]|7[678]|9[89])\d{8})\D")
     matchers = pattern.findall(text)
     if matchers:
-        # print('telephone')
+        logger.debug("telephone")
         for matcher in matchers:
             text = text.replace(matcher[0], TelePhone(telephone=matcher[0]).telephone2chntext(), 1)
     # 固话
     pattern = re.compile(r"\D((0(10|2[1-3]|[3-9]\d{2})-?)?[1-9]\d{6,7})\D")
     matchers = pattern.findall(text)
     if matchers:
-        # print('fixed telephone')
+        logger.debug("fixed telephone")
         for matcher in matchers:
             text = text.replace(matcher[0], TelePhone(telephone=matcher[0]).telephone2chntext(fixed=True), 1)
 
     # 规范化分数
     pattern = re.compile(r"(\d+/\d+)")
     matchers = pattern.findall(text)
     if matchers:
-        # print('fraction')
+        logger.debug("fraction")
         for matcher in matchers:
             text = text.replace(matcher, Fraction(fraction=matcher).fraction2chntext(), 1)
 
     # 规范化百分数
     text = text.replace("％", "%")
     pattern = re.compile(r"(\d+(\.\d+)?%)")
     matchers = pattern.findall(text)
     if matchers:
-        # print('percentage')
+        logger.debug("percentage")
         for matcher in matchers:
             text = text.replace(matcher[0], Percentage(percentage=matcher[0]).percentage2chntext(), 1)
 
     # 规范化纯数+量词
     pattern = re.compile(r"(\d+(\.\d+)?)[多余几]?" + COM_QUANTIFIERS)
     matchers = pattern.findall(text)
     if matchers:
-        # print('cardinal+quantifier')
+        logger.debug("cardinal+quantifier")
         for matcher in matchers:
             text = text.replace(matcher[0], Cardinal(cardinal=matcher[0]).cardinal2chntext(), 1)
 
     # 规范化数字编号
     pattern = re.compile(r"(\d{4,32})")
     matchers = pattern.findall(text)
     if matchers:
-        # print('digit')
+        logger.debug("digit")
         for matcher in matchers:
             text = text.replace(matcher, Digit(digit=matcher).digit2chntext(), 1)
 
     # 规范化纯数
     pattern = re.compile(r"(\d+(\.\d+)?)")
     matchers = pattern.findall(text)
     if matchers:
-        # print('cardinal')
+        logger.debug("cardinal")
         for matcher in matchers:
             text = text.replace(matcher[0], Cardinal(cardinal=matcher[0]).cardinal2chntext(), 1)
 
     # restore P2P, O2O, B2C, B2B etc
     pattern = re.compile(r"(([a-zA-Z]+)二([a-zA-Z]+))")
     matchers = pattern.findall(text)
     if matchers:
-        # print('particular')
+        logger.debug("particular")
         for matcher in matchers:
             text = text.replace(matcher[0], matcher[1] + "2" + matcher[2], 1)
 
     return text.lstrip("^").rstrip("$")
 
 
 def remove_erhua(text):
@@ -1099,15 +1103,15 @@
         text = normalize_nsw(text)
 
         text = text.translate(PUNCS_TRANSFORM)
 
         if self.check_chars:
             for c in text:
                 if not IN_VALID_CHARS.get(c):
-                    print(f"WARNING: illegal char {c} in: {text}", file=sys.stderr)
+                    logger.warning("Illegal char %s in: %s", c, text)
                     return ""
 
         if self.remove_space:
             text = remove_space(text)
 
         return text
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/__init__.py` & `coqui_tts-0.23.0/TTS/tts/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from typing import Dict, List, Union
 
 from TTS.utils.generic_utils import find_module
 
+logger = logging.getLogger(__name__)
+
 
 def setup_model(config: "Coqpit", samples: Union[List[List], List[Dict]] = None) -> "BaseTTS":
-    print(" > Using model: {}".format(config.model))
+    logger.info("Using model: %s", config.model)
     # fetch the right model implementation.
     if "base_model" in config and config["base_model"] is not None:
         MyModel = find_module("TTS.tts.models", config.base_model.lower())
     else:
         MyModel = find_module("TTS.tts.models", config.model.lower())
     model = MyModel.init_from_config(config=config, samples=samples)
     return model
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/align_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/align_tts.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/models/bark.py` & `coqui_tts-0.23.0/TTS/tts/models/bark.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/models/base_tacotron.py` & `coqui_tts-0.23.0/TTS/tts/models/base_tacotron.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import logging
 from abc import abstractmethod
 from typing import Dict, Tuple
 
 import torch
 from coqpit import Coqpit
 from torch import nn
 
@@ -13,14 +14,16 @@
 from TTS.tts.utils.synthesis import synthesis
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 from TTS.utils.generic_utils import format_aux_input
 from TTS.utils.io import load_fsspec
 from TTS.utils.training import gradual_training_scheduler
 
+logger = logging.getLogger(__name__)
+
 
 class BaseTacotron(BaseTTS):
     """Base class shared by Tacotron and Tacotron2"""
 
     def __init__(
         self,
         config: "TacotronConfig",
@@ -112,15 +115,15 @@
             # set r from config used at training time (for inference)
             self.decoder.set_r(state["config"]["r"])
         else:
             # set r from the new config (for new-models)
             self.decoder.set_r(config.r)
         if eval:
             self.eval()
-            print(f" > Model's reduction rate `r` is set to: {self.decoder.r}")
+            logger.info("Model's reduction rate `r` is set to: %d", self.decoder.r)
             assert not self.training
 
     def get_criterion(self) -> nn.Module:
         """Get the model criterion used in training."""
         return TacotronLoss(self.config)
 
     @staticmethod
@@ -144,15 +147,15 @@
 
         Args:
             assets (dict): A dict of training assets. For `tts` models, it must include `{'audio_processor': ap}`.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         aux_inputs = self._get_test_aux_input()
         for idx, sen in enumerate(test_sentences):
             outputs_dict = synthesis(
                 self,
@@ -298,8 +301,8 @@
         """
         if self.gradual_training:
             r, trainer.config.batch_size = gradual_training_scheduler(trainer.total_steps_done, trainer.config)
             trainer.config.r = r
             self.decoder.set_r(r)
             if trainer.config.bidirectional_decoder:
                 trainer.model.decoder_backward.set_r(r)
-            print(f"\n > Number of output frames: {self.decoder.r}")
+            logger.info("Number of output frames: %d", self.decoder.r)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/base_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/base_tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import random
 from typing import Dict, List, Tuple, Union
 
 import torch
 import torch.distributed as dist
 from coqpit import Coqpit
@@ -14,14 +15,16 @@
 from TTS.tts.datasets.dataset import TTSDataset
 from TTS.tts.utils.data import get_length_balancer_weights
 from TTS.tts.utils.languages import LanguageManager, get_language_balancer_weights
 from TTS.tts.utils.speakers import SpeakerManager, get_speaker_balancer_weights
 from TTS.tts.utils.synthesis import synthesis
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 
+logger = logging.getLogger(__name__)
+
 # pylint: skip-file
 
 
 class BaseTTS(BaseTrainerModel):
     """Base `tts` class. Every new `tts` model must inherit this.
 
     It defines common `tts` specific functions on top of `Model` implementation.
@@ -101,15 +104,15 @@
         # set ultimate speaker embedding size
         if config.use_speaker_embedding or config.use_d_vector_file:
             self.embedded_speaker_dim = (
                 config.d_vector_dim if "d_vector_dim" in config and config.d_vector_dim is not None else 512
             )
         # init speaker embedding layer
         if config.use_speaker_embedding and not config.use_d_vector_file:
-            print(" > Init speaker_embedding layer.")
+            logger.info("Init speaker_embedding layer.")
             self.speaker_embedding = nn.Embedding(self.num_speakers, self.embedded_speaker_dim)
             self.speaker_embedding.weight.data.normal_(0, 0.3)
 
     def get_aux_input(self, **kwargs) -> Dict:
         """Prepare and return `aux_input` used by `forward()`"""
         return {"speaker_id": None, "style_wav": None, "d_vector": None, "language_id": None}
 
@@ -241,28 +244,28 @@
 
     def get_sampler(self, config: Coqpit, dataset: TTSDataset, num_gpus=1):
         weights = None
         data_items = dataset.samples
 
         if getattr(config, "use_language_weighted_sampler", False):
             alpha = getattr(config, "language_weighted_sampler_alpha", 1.0)
-            print(" > Using Language weighted sampler with alpha:", alpha)
+            logger.info("Using Language weighted sampler with alpha: %.2f", alpha)
             weights = get_language_balancer_weights(data_items) * alpha
 
         if getattr(config, "use_speaker_weighted_sampler", False):
             alpha = getattr(config, "speaker_weighted_sampler_alpha", 1.0)
-            print(" > Using Speaker weighted sampler with alpha:", alpha)
+            logger.info("Using Speaker weighted sampler with alpha: %.2f", alpha)
             if weights is not None:
                 weights += get_speaker_balancer_weights(data_items) * alpha
             else:
                 weights = get_speaker_balancer_weights(data_items) * alpha
 
         if getattr(config, "use_length_weighted_sampler", False):
             alpha = getattr(config, "length_weighted_sampler_alpha", 1.0)
-            print(" > Using Length weighted sampler with alpha:", alpha)
+            logger.info("Using Length weighted sampler with alpha: %.2f", alpha)
             if weights is not None:
                 weights += get_length_balancer_weights(data_items) * alpha
             else:
                 weights = get_length_balancer_weights(data_items) * alpha
 
         if weights is not None:
             sampler = WeightedRandomSampler(weights, len(weights))
@@ -326,15 +329,14 @@
                 min_text_len=config.min_text_len,
                 max_text_len=config.max_text_len,
                 min_audio_len=config.min_audio_len,
                 max_audio_len=config.max_audio_len,
                 phoneme_cache_path=config.phoneme_cache_path,
                 precompute_num_workers=config.precompute_num_workers,
                 use_noise_augment=False if is_eval else config.use_noise_augment,
-                verbose=verbose,
                 speaker_id_mapping=speaker_id_mapping,
                 d_vector_mapping=d_vector_mapping if config.use_d_vector_file else None,
                 tokenizer=self.tokenizer,
                 start_by_longest=config.start_by_longest,
                 language_id_mapping=language_id_mapping,
             )
 
@@ -386,15 +388,15 @@
 
         Args:
             assets (dict): A dict of training assets. For `tts` models, it must include `{'audio_processor': ap}`.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         aux_inputs = self._get_test_aux_input()
         for idx, sen in enumerate(test_sentences):
             if isinstance(sen, list):
                 aux_inputs = self.get_aux_input_from_test_sentences(sen)
@@ -425,26 +427,26 @@
             output_path = os.path.join(trainer.output_path, "speakers.pth")
             self.speaker_manager.save_ids_to_file(output_path)
             trainer.config.speakers_file = output_path
             # some models don't have `model_args` set
             if hasattr(trainer.config, "model_args"):
                 trainer.config.model_args.speakers_file = output_path
             trainer.config.save_json(os.path.join(trainer.output_path, "config.json"))
-            print(f" > `speakers.pth` is saved to {output_path}.")
-            print(" > `speakers_file` is updated in the config.json.")
+            logger.info("`speakers.pth` is saved to: %s", output_path)
+            logger.info("`speakers_file` is updated in the config.json.")
 
         if self.language_manager is not None:
             output_path = os.path.join(trainer.output_path, "language_ids.json")
             self.language_manager.save_ids_to_file(output_path)
             trainer.config.language_ids_file = output_path
             if hasattr(trainer.config, "model_args"):
                 trainer.config.model_args.language_ids_file = output_path
             trainer.config.save_json(os.path.join(trainer.output_path, "config.json"))
-            print(f" > `language_ids.json` is saved to {output_path}.")
-            print(" > `language_ids_file` is updated in the config.json.")
+            logger.info("`language_ids.json` is saved to: %s", output_path)
+            logger.info("`language_ids_file` is updated in the config.json.")
 
 
 class BaseTTSE2E(BaseTTS):
     def _set_model_args(self, config: Coqpit):
         self.config = config
         if "Config" in config.__class__.__name__:
             num_chars = (
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/delightful_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/delightful_tts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from dataclasses import dataclass, field
 from itertools import chain
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
@@ -32,14 +33,16 @@
 from TTS.utils.audio.numpy_transforms import mel_to_wav as mel_to_wav_numpy
 from TTS.utils.audio.processor import AudioProcessor
 from TTS.utils.io import load_fsspec
 from TTS.vocoder.layers.losses import MultiScaleSTFTLoss
 from TTS.vocoder.models.hifigan_generator import HifiganGenerator
 from TTS.vocoder.utils.generic_utils import plot_results
 
+logger = logging.getLogger(__name__)
+
 
 def id_to_torch(aux_id, cuda=False):
     if aux_id is not None:
         aux_id = np.asarray(aux_id)
         aux_id = torch.from_numpy(aux_id)
     if cuda:
         return aux_id.cuda()
@@ -158,17 +161,17 @@
     return output
 
 
 def _wav_to_spec(y, n_fft, hop_length, win_length, center=False):
     y = y.squeeze(1)
 
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("min value is %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("max value is %.3f", torch.max(y))
 
     global hann_window  # pylint: disable=global-statement
     dtype_device = str(y.dtype) + "_" + str(y.device)
     wnsize_dtype_device = str(win_length) + "_" + dtype_device
     if wnsize_dtype_device not in hann_window:
         hann_window[wnsize_dtype_device] = torch.hann_window(win_length).to(dtype=y.dtype, device=y.device)
 
@@ -249,17 +252,17 @@
 
     Return Shapes:
         - spec : :math:`[B,C,T_spec]`
     """
     y = y.squeeze(1)
 
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("min value is %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("max value is %.3f", torch.max(y))
 
     global mel_basis, hann_window  # pylint: disable=global-statement
     mel_basis_key = name_mel_basis(y, n_fft, fmax)
     wnsize_dtype_device = str(win_length) + "_" + str(y.dtype) + "_" + str(y.device)
     if mel_basis_key not in mel_basis:
         # pylint: disable=missing-kwoa
         mel = librosa_mel_fn(
@@ -324,23 +327,21 @@
 class ForwardTTSE2eF0Dataset(F0Dataset):
     """Override F0Dataset to avoid slow computing of pitches"""
 
     def __init__(
         self,
         ap,
         samples: Union[List[List], List[Dict]],
-        verbose=False,
         cache_path: str = None,
         precompute_num_workers=0,
         normalize_f0=True,
     ):
         super().__init__(
             samples=samples,
             ap=ap,
-            verbose=verbose,
             cache_path=cache_path,
             precompute_num_workers=precompute_num_workers,
             normalize_f0=normalize_f0,
         )
 
     def _compute_and_save_pitch(self, wav_file, pitch_file=None):
         wav, _ = load_audio(wav_file)
@@ -404,15 +405,15 @@
         raw_text = item["text"]
         wav, _ = load_audio(item["audio_file"])
         wav_filename = os.path.basename(item["audio_file"])
 
         try:
             token_ids = self.get_token_ids(idx, item["text"])
         except:
-            print(idx, item)
+            logger.exception("%s %s", idx, item)
             # pylint: disable=raise-missing-from
             raise OSError
         f0 = None
         if self.compute_f0:
             f0 = self.get_f0(idx)["f0"]
 
         # after phonemization the text length may change
@@ -769,15 +770,15 @@
 
         if self.args.use_d_vector_file:
             self._init_d_vector()
 
     def _init_speaker_embedding(self):
         # pylint: disable=attribute-defined-outside-init
         if self.num_speakers > 0:
-            print(" > initialization of speaker-embedding layers.")
+            logger.info("Initialization of speaker-embedding layers.")
             self.embedded_speaker_dim = self.args.speaker_embedding_channels
             self.args.embedded_speaker_dim = self.args.speaker_embedding_channels
 
     def _init_d_vector(self):
         # pylint: disable=attribute-defined-outside-init
         if hasattr(self, "emb_g"):
             raise ValueError("[!] Speaker embedding layer already initialized before d_vector settings.")
@@ -1287,15 +1288,15 @@
         """Generic test run for `tts` models used by `Trainer`.
 
         You can override this for a different behaviour.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         for idx, s_info in enumerate(test_sentences):
             aux_inputs = self.get_aux_input_from_test_sentences(s_info)
             outputs = self.synthesize(
                 aux_inputs["text"],
@@ -1401,22 +1402,22 @@
         return batch
 
     def get_sampler(self, config: Coqpit, dataset: TTSDataset, num_gpus=1):
         weights = None
         data_items = dataset.samples
         if getattr(config, "use_weighted_sampler", False):
             for attr_name, alpha in config.weighted_sampler_attrs.items():
-                print(f" > Using weighted sampler for attribute '{attr_name}' with alpha '{alpha}'")
+                logger.info("Using weighted sampler for attribute '%s' with alpha %.2f", attr_name, alpha)
                 multi_dict = config.weighted_sampler_multipliers.get(attr_name, None)
-                print(multi_dict)
+                logger.info(multi_dict)
                 weights, attr_names, attr_weights = get_attribute_balancer_weights(
                     attr_name=attr_name, items=data_items, multi_dict=multi_dict
                 )
                 weights = weights * alpha
-                print(f" > Attribute weights for '{attr_names}' \n | > {attr_weights}")
+                logger.info("Attribute weights for '%s' \n | > %s", attr_names, attr_weights)
 
         if weights is not None:
             sampler = WeightedRandomSampler(weights, len(weights))
         else:
             sampler = None
         # sampler for DDP
         if sampler is None:
@@ -1448,15 +1449,14 @@
                 min_audio_len=config.min_audio_len,
                 max_audio_len=config.max_audio_len,
                 phoneme_cache_path=config.phoneme_cache_path,
                 precompute_num_workers=config.precompute_num_workers,
                 compute_f0=config.compute_f0,
                 f0_cache_path=config.f0_cache_path,
                 attn_prior_cache_path=config.attn_prior_cache_path if config.use_attn_priors else None,
-                verbose=verbose,
                 tokenizer=self.tokenizer,
                 start_by_longest=config.start_by_longest,
             )
 
             # wait all the DDP process to be ready
             if num_gpus > 1:
                 dist.barrier()
@@ -1525,15 +1525,15 @@
     def on_epoch_end(self, trainer):  # pylint: disable=unused-argument
         # stop updating mean and var
         # TODO: do the same for F0
         self.energy_scaler.eval()
 
     @staticmethod
     def init_from_config(
-        config: "DelightfulTTSConfig", samples: Union[List[List], List[Dict]] = None, verbose=False
+        config: "DelightfulTTSConfig", samples: Union[List[List], List[Dict]] = None
     ):  # pylint: disable=unused-argument
         """Initiate model from config
 
         Args:
             config (ForwardTTSE2eConfig): Model config.
             samples (Union[List[List], List[Dict]]): Training samples to parse speaker ids for training.
                 Defaults to None.
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/forward_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/forward_tts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from dataclasses import dataclass, field
 from typing import Dict, List, Tuple, Union
 
 import torch
 from coqpit import Coqpit
 from torch import nn
 from torch.cuda.amp.autocast_mode import autocast
@@ -14,14 +15,16 @@
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.tts.utils.helpers import average_over_durations, generate_path, maximum_path, sequence_mask
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_avg_energy, plot_avg_pitch, plot_spectrogram
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class ForwardTTSArgs(Coqpit):
     """ForwardTTS Model arguments.
 
     Args:
 
@@ -299,15 +302,15 @@
         if config.use_d_vector_file:
             self.embedded_speaker_dim = config.d_vector_dim
             if self.args.d_vector_dim != self.args.hidden_channels:
                 # self.proj_g = nn.Conv1d(self.args.d_vector_dim, self.args.hidden_channels, 1)
                 self.proj_g = nn.Linear(in_features=self.args.d_vector_dim, out_features=self.args.hidden_channels)
         # init speaker embedding layer
         if config.use_speaker_embedding and not config.use_d_vector_file:
-            print(" > Init speaker_embedding layer.")
+            logger.info("Init speaker_embedding layer.")
             self.emb_g = nn.Embedding(self.num_speakers, self.args.hidden_channels)
             nn.init.uniform_(self.emb_g.weight, -0.1, 0.1)
 
     @staticmethod
     def generate_attn(dr, x_mask, y_mask=None):
         """Generate an attention mask from the durations.
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/glow_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/glow_tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import math
 from typing import Dict, List, Tuple, Union
 
 import torch
 from coqpit import Coqpit
 from torch import nn
 from torch.cuda.amp.autocast_mode import autocast
@@ -14,14 +15,16 @@
 from TTS.tts.utils.helpers import generate_path, maximum_path, sequence_mask
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.synthesis import synthesis
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 class GlowTTS(BaseTTS):
     """GlowTTS model.
 
     Paper::
         https://arxiv.org/abs/2005.11129
 
@@ -49,15 +52,15 @@
 
         Fully init a model ready for action. All the class attributes and class members
         (e.g Tokenizer, AudioProcessor, etc.). are initialized internally based on config values.
 
         >>> from TTS.tts.configs.glow_tts_config import GlowTTSConfig
         >>> from TTS.tts.models.glow_tts import GlowTTS
         >>> config = GlowTTSConfig()
-        >>> model = GlowTTS.init_from_config(config, verbose=False)
+        >>> model = GlowTTS.init_from_config(config)
     """
 
     def __init__(
         self,
         config: GlowTTSConfig,
         ap: "AudioProcessor" = None,
         tokenizer: "TTSTokenizer" = None,
@@ -123,15 +126,15 @@
             )
             if self.speaker_manager is not None:
                 assert (
                     config.d_vector_dim == self.speaker_manager.embedding_dim
                 ), " [!] d-vector dimension mismatch b/w config and speaker manager."
         # init speaker embedding layer
         if config.use_speaker_embedding and not config.use_d_vector_file:
-            print(" > Init speaker_embedding layer.")
+            logger.info("Init speaker_embedding layer.")
             self.embedded_speaker_dim = self.hidden_channels_enc
             self.emb_g = nn.Embedding(self.num_speakers, self.hidden_channels_enc)
             nn.init.uniform_(self.emb_g.weight, -0.1, 0.1)
         # set conditioning dimensions
         self.c_in_channels = self.embedded_speaker_dim
 
     @staticmethod
@@ -475,21 +478,21 @@
         """Generic test run for `tts` models used by `Trainer`.
 
         You can override this for a different behaviour.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         aux_inputs = self._get_test_aux_input()
         if len(test_sentences) == 0:
-            print(" | [!] No test sentences provided.")
+            logger.warning("No test sentences provided.")
         else:
             for idx, sen in enumerate(test_sentences):
                 outputs = synthesis(
                     self,
                     sen,
                     self.config,
                     "cuda" in str(next(self.parameters()).device),
@@ -536,22 +539,21 @@
         return GlowTTSLoss()
 
     def on_train_step_start(self, trainer):
         """Decide on every training step wheter enable/disable data depended initialization."""
         self.run_data_dep_init = trainer.total_steps_done < self.data_dep_init_steps
 
     @staticmethod
-    def init_from_config(config: "GlowTTSConfig", samples: Union[List[List], List[Dict]] = None, verbose=True):
+    def init_from_config(config: "GlowTTSConfig", samples: Union[List[List], List[Dict]] = None):
         """Initiate model from config
 
         Args:
             config (VitsConfig): Model config.
             samples (Union[List[List], List[Dict]]): Training samples to parse speaker ids for training.
                 Defaults to None.
-            verbose (bool): If True, print init messages. Defaults to True.
         """
         from TTS.utils.audio import AudioProcessor
 
-        ap = AudioProcessor.init_from_config(config, verbose)
+        ap = AudioProcessor.init_from_config(config)
         tokenizer, new_config = TTSTokenizer.init_from_config(config)
         speaker_manager = SpeakerManager.init_from_config(config, samples)
         return GlowTTS(new_config, ap, tokenizer, speaker_manager)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/neuralhmm_tts.py` & `coqui_tts-0.23.0/TTS/tts/models/neuralhmm_tts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from typing import Dict, List, Union
 
 import torch
 from coqpit import Coqpit
 from torch import nn
 from trainer.logging.tensorboard_logger import TensorboardLogger
@@ -15,14 +16,16 @@
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 from TTS.utils.generic_utils import format_aux_input
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 class NeuralhmmTTS(BaseTTS):
     """Neural HMM TTS model.
 
     Paper::
         https://arxiv.org/abs/2108.13320
 
@@ -231,26 +234,25 @@
         return outputs
 
     @staticmethod
     def get_criterion():
         return NLLLoss()
 
     @staticmethod
-    def init_from_config(config: "NeuralhmmTTSConfig", samples: Union[List[List], List[Dict]] = None, verbose=True):
+    def init_from_config(config: "NeuralhmmTTSConfig", samples: Union[List[List], List[Dict]] = None):
         """Initiate model from config
 
         Args:
             config (VitsConfig): Model config.
             samples (Union[List[List], List[Dict]]): Training samples to parse speaker ids for training.
                 Defaults to None.
-            verbose (bool): If True, print init messages. Defaults to True.
         """
         from TTS.utils.audio import AudioProcessor
 
-        ap = AudioProcessor.init_from_config(config, verbose)
+        ap = AudioProcessor.init_from_config(config)
         tokenizer, new_config = TTSTokenizer.init_from_config(config)
         speaker_manager = SpeakerManager.init_from_config(config, samples)
         return NeuralhmmTTS(new_config, ap, tokenizer, speaker_manager)
 
     def load_checkpoint(
         self, config: Coqpit, checkpoint_path: str, eval: bool = False, strict: bool = True, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
@@ -262,41 +264,45 @@
 
     def on_init_start(self, trainer):
         """If the current dataset does not have normalisation statistics and initialisation transition_probability it computes them otherwise loads."""
         if not os.path.isfile(trainer.config.mel_statistics_parameter_path) or trainer.config.force_generate_statistics:
             dataloader = trainer.get_train_dataloader(
                 training_assets=None, samples=trainer.train_samples, verbose=False
             )
-            print(
-                f" | > Data parameters not found for: {trainer.config.mel_statistics_parameter_path}. Computing mel normalization parameters..."
+            logger.info(
+                "Data parameters not found for: %s. Computing mel normalization parameters...",
+                trainer.config.mel_statistics_parameter_path,
             )
             data_mean, data_std, init_transition_prob = OverflowUtils.get_data_parameters_for_flat_start(
                 dataloader, trainer.config.out_channels, trainer.config.state_per_phone
             )
-            print(
-                f" | > Saving data parameters to: {trainer.config.mel_statistics_parameter_path}: value: {data_mean, data_std, init_transition_prob}"
+            logger.info(
+                "Saving data parameters to: %s: value: %s",
+                trainer.config.mel_statistics_parameter_path,
+                (data_mean, data_std, init_transition_prob),
             )
             statistics = {
                 "mean": data_mean.item(),
                 "std": data_std.item(),
                 "init_transition_prob": init_transition_prob.item(),
             }
             torch.save(statistics, trainer.config.mel_statistics_parameter_path)
 
         else:
-            print(
-                f" | > Data parameters found for: {trainer.config.mel_statistics_parameter_path}. Loading mel normalization parameters..."
+            logger.info(
+                "Data parameters found for: %s. Loading mel normalization parameters...",
+                trainer.config.mel_statistics_parameter_path,
             )
             statistics = torch.load(trainer.config.mel_statistics_parameter_path)
             data_mean, data_std, init_transition_prob = (
                 statistics["mean"],
                 statistics["std"],
                 statistics["init_transition_prob"],
             )
-            print(f" | > Data parameters loaded with value: {data_mean, data_std, init_transition_prob}")
+            logger.info("Data parameters loaded with value: %s", (data_mean, data_std, init_transition_prob))
 
         trainer.config.flat_start_params["transition_p"] = (
             init_transition_prob.item() if torch.is_tensor(init_transition_prob) else init_transition_prob
         )
         OverflowUtils.update_flat_start_transition(trainer.model, init_transition_prob)
         trainer.model.update_mean_std(statistics)
 
@@ -314,15 +320,15 @@
             "mel_from_most_probable_state": plot_spectrogram(
                 get_spec_from_most_probable_state(alignments[0], means[0]), fig_size=(12, 3)
             ),
             "mel_target": plot_spectrogram(batch["mel_input"][0], fig_size=(12, 3)),
         }
 
         # sample one item from the batch -1 will give the smalles item
-        print(" | > Synthesising audio from the model...")
+        logger.info("Synthesising audio from the model...")
         inference_output = self.inference(
             batch["text_input"][-1].unsqueeze(0), aux_input={"x_lengths": batch["text_lengths"][-1].unsqueeze(0)}
         )
         figures["synthesised"] = plot_spectrogram(inference_output["model_outputs"][0], fig_size=(12, 3))
 
         states = [p[1] for p in inference_output["input_parameters"][0]]
         transition_probability_synthesising = [p[2].cpu().numpy() for p in inference_output["output_parameters"][0]]
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/overflow.py` & `coqui_tts-0.23.0/TTS/tts/models/overflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from typing import Dict, List, Union
 
 import torch
 from coqpit import Coqpit
 from torch import nn
 from trainer.logging.tensorboard_logger import TensorboardLogger
@@ -16,14 +17,16 @@
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.tts.utils.speakers import SpeakerManager
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 from TTS.utils.generic_utils import format_aux_input
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 
 class Overflow(BaseTTS):
     """OverFlow TTS model.
 
     Paper::
         https://arxiv.org/abs/2211.06892
 
@@ -246,26 +249,25 @@
         return outputs
 
     @staticmethod
     def get_criterion():
         return NLLLoss()
 
     @staticmethod
-    def init_from_config(config: "OverFlowConfig", samples: Union[List[List], List[Dict]] = None, verbose=True):
+    def init_from_config(config: "OverFlowConfig", samples: Union[List[List], List[Dict]] = None):
         """Initiate model from config
 
         Args:
             config (VitsConfig): Model config.
             samples (Union[List[List], List[Dict]]): Training samples to parse speaker ids for training.
                 Defaults to None.
-            verbose (bool): If True, print init messages. Defaults to True.
         """
         from TTS.utils.audio import AudioProcessor
 
-        ap = AudioProcessor.init_from_config(config, verbose)
+        ap = AudioProcessor.init_from_config(config)
         tokenizer, new_config = TTSTokenizer.init_from_config(config)
         speaker_manager = SpeakerManager.init_from_config(config, samples)
         return Overflow(new_config, ap, tokenizer, speaker_manager)
 
     def load_checkpoint(
         self, config: Coqpit, checkpoint_path: str, eval: bool = False, strict: bool = True, cache=False
     ):  # pylint: disable=unused-argument, redefined-builtin
@@ -278,41 +280,45 @@
 
     def on_init_start(self, trainer):
         """If the current dataset does not have normalisation statistics and initialisation transition_probability it computes them otherwise loads."""
         if not os.path.isfile(trainer.config.mel_statistics_parameter_path) or trainer.config.force_generate_statistics:
             dataloader = trainer.get_train_dataloader(
                 training_assets=None, samples=trainer.train_samples, verbose=False
             )
-            print(
-                f" | > Data parameters not found for: {trainer.config.mel_statistics_parameter_path}. Computing mel normalization parameters..."
+            logger.info(
+                "Data parameters not found for: %s. Computing mel normalization parameters...",
+                trainer.config.mel_statistics_parameter_path,
             )
             data_mean, data_std, init_transition_prob = OverflowUtils.get_data_parameters_for_flat_start(
                 dataloader, trainer.config.out_channels, trainer.config.state_per_phone
             )
-            print(
-                f" | > Saving data parameters to: {trainer.config.mel_statistics_parameter_path}: value: {data_mean, data_std, init_transition_prob}"
+            logger.info(
+                "Saving data parameters to: %s: value: %s",
+                trainer.config.mel_statistics_parameter_path,
+                (data_mean, data_std, init_transition_prob),
             )
             statistics = {
                 "mean": data_mean.item(),
                 "std": data_std.item(),
                 "init_transition_prob": init_transition_prob.item(),
             }
             torch.save(statistics, trainer.config.mel_statistics_parameter_path)
 
         else:
-            print(
-                f" | > Data parameters found for: {trainer.config.mel_statistics_parameter_path}. Loading mel normalization parameters..."
+            logger.info(
+                "Data parameters found for: %s. Loading mel normalization parameters...",
+                trainer.config.mel_statistics_parameter_path,
             )
             statistics = torch.load(trainer.config.mel_statistics_parameter_path)
             data_mean, data_std, init_transition_prob = (
                 statistics["mean"],
                 statistics["std"],
                 statistics["init_transition_prob"],
             )
-            print(f" | > Data parameters loaded with value: {data_mean, data_std, init_transition_prob}")
+            logger.info("Data parameters loaded with value: %s", (data_mean, data_std, init_transition_prob))
 
         trainer.config.flat_start_params["transition_p"] = (
             init_transition_prob.item() if torch.is_tensor(init_transition_prob) else init_transition_prob
         )
         OverflowUtils.update_flat_start_transition(trainer.model, init_transition_prob)
         trainer.model.update_mean_std(statistics)
 
@@ -330,15 +336,15 @@
             "mel_from_most_probable_state": plot_spectrogram(
                 get_spec_from_most_probable_state(alignments[0], means[0], self.decoder), fig_size=(12, 3)
             ),
             "mel_target": plot_spectrogram(batch["mel_input"][0], fig_size=(12, 3)),
         }
 
         # sample one item from the batch -1 will give the smalles item
-        print(" | > Synthesising audio from the model...")
+        logger.info("Synthesising audio from the model...")
         inference_output = self.inference(
             batch["text_input"][-1].unsqueeze(0), aux_input={"x_lengths": batch["text_lengths"][-1].unsqueeze(0)}
         )
         figures["synthesised"] = plot_spectrogram(inference_output["model_outputs"][0], fig_size=(12, 3))
 
         states = [p[1] for p in inference_output["input_parameters"][0]]
         transition_probability_synthesising = [p[2].cpu().numpy() for p in inference_output["output_parameters"][0]]
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/tacotron.py` & `coqui_tts-0.23.0/TTS/tts/models/tacotron.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/models/tacotron2.py` & `coqui_tts-0.23.0/TTS/tts/models/tacotron2.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/models/tortoise.py` & `coqui_tts-0.23.0/TTS/tts/models/tortoise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import random
 from contextlib import contextmanager
 from dataclasses import dataclass
 from time import time
 
 import torch
@@ -19,14 +20,16 @@
 from TTS.tts.layers.tortoise.diffusion_decoder import DiffusionTts
 from TTS.tts.layers.tortoise.random_latent_generator import RandomLatentConverter
 from TTS.tts.layers.tortoise.tokenizer import VoiceBpeTokenizer
 from TTS.tts.layers.tortoise.vocoder import VocConf, VocType
 from TTS.tts.layers.tortoise.wav2vec_alignment import Wav2VecAlignment
 from TTS.tts.models.base_tts import BaseTTS
 
+logger = logging.getLogger(__name__)
+
 
 def pad_or_truncate(t, length):
     """
     Utility function for forcing <t> to have the specified sequence length, whether by clipping it or padding it with 0s.
     """
     tp = t[..., :length]
     if t.shape[-1] == length:
@@ -96,15 +99,15 @@
 
     Failing to do this padding will produce speech with a harsh end that sounds like "BLAH" or similar.
     """
     # Strip off the autoregressive stop token and add padding.
     stop_token_indices = (codes == stop_token).nonzero()
     if len(stop_token_indices) == 0:
         if complain:
-            print(
+            logger.warning(
                 "No stop tokens found in one of the generated voice clips. This typically means the spoken audio is "
                 "too long. In some cases, the output will still be good, though. Listen to it and if it is missing words, "
                 "try breaking up your input text."
             )
         return codes
     codes[stop_token_indices] = 83
     stm = stop_token_indices.min().item()
@@ -709,16 +712,15 @@
             samples = []
             num_batches = num_autoregressive_samples // self.autoregressive_batch_size
             stop_mel_token = self.autoregressive.stop_mel_token
             calm_token = (
                 83  # This is the token for coding silence, which is fixed in place with "fix_autoregressive_output"
             )
             self.autoregressive = self.autoregressive.to(self.device)
-            if verbose:
-                print("Generating autoregressive samples..")
+            logger.info("Generating autoregressive samples..")
             with (
                 self.temporary_cuda(self.autoregressive) as autoregressive,
                 torch.autocast(device_type="cuda", dtype=torch.float16, enabled=half),
             ):
                 for b in tqdm(range(num_batches), disable=not verbose):
                     codes = autoregressive.inference_speech(
                         auto_conditioning,
@@ -771,16 +773,15 @@
                         device=text_tokens.device,
                     ),
                     return_latent=True,
                     clip_inputs=False,
                 )
             del auto_conditioning
 
-            if verbose:
-                print("Transforming autoregressive outputs into audio..")
+            logger.info("Transforming autoregressive outputs into audio..")
             wav_candidates = []
             for b in range(best_results.shape[0]):
                 codes = best_results[b].unsqueeze(0)
                 latents = best_latents[b].unsqueeze(0)
 
                 # Find the first occurrence of the "calm" token and trim the codes to that.
                 ctokens = 0
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/vits.py` & `coqui_tts-0.23.0/TTS/tts/models/vits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import math
 import os
 from dataclasses import dataclass, field, replace
 from itertools import chain
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
@@ -34,14 +35,16 @@
 from TTS.tts.utils.text.tokenizer import TTSTokenizer
 from TTS.tts.utils.visual import plot_alignment
 from TTS.utils.io import load_fsspec
 from TTS.utils.samplers import BucketBatchSampler
 from TTS.vocoder.models.hifigan_generator import HifiganGenerator
 from TTS.vocoder.utils.generic_utils import plot_results
 
+logger = logging.getLogger(__name__)
+
 ##############################
 # IO / Feature extraction
 ##############################
 
 # pylint: disable=global-statement
 hann_window = {}
 mel_basis = {}
@@ -100,17 +103,17 @@
 
     Return Shapes:
         - spec : :math:`[B,C,T]`
     """
     y = y.squeeze(1)
 
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("min value is %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("max value is %.3f", torch.max(y))
 
     global hann_window
     dtype_device = str(y.dtype) + "_" + str(y.device)
     wnsize_dtype_device = str(win_length) + "_" + dtype_device
     if wnsize_dtype_device not in hann_window:
         hann_window[wnsize_dtype_device] = torch.hann_window(win_length).to(dtype=y.dtype, device=y.device)
 
@@ -166,17 +169,17 @@
 
     Return Shapes:
         - spec : :math:`[B,C,T]`
     """
     y = y.squeeze(1)
 
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("min value is %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("max value is %.3f", torch.max(y))
 
     global mel_basis, hann_window
     dtype_device = str(y.dtype) + "_" + str(y.device)
     fmax_dtype_device = str(fmax) + "_" + dtype_device
     wnsize_dtype_device = str(win_length) + "_" + dtype_device
     if fmax_dtype_device not in mel_basis:
         mel = librosa_mel_fn(sr=sample_rate, n_fft=n_fft, n_mels=num_mels, fmin=fmin, fmax=fmax)
@@ -760,29 +763,29 @@
                 not self.args.speaker_encoder_model_path or not self.args.speaker_encoder_config_path
             ):
                 raise RuntimeError(
                     " [!] To use the speaker consistency loss (SCL) you need to specify speaker_encoder_model_path and speaker_encoder_config_path !!"
                 )
 
             self.speaker_manager.encoder.eval()
-            print(" > External Speaker Encoder Loaded !!")
+            logger.info("External Speaker Encoder Loaded !!")
 
             if (
                 hasattr(self.speaker_manager.encoder, "audio_config")
                 and self.config.audio.sample_rate != self.speaker_manager.encoder.audio_config["sample_rate"]
             ):
                 self.audio_transform = torchaudio.transforms.Resample(
                     orig_freq=self.config.audio.sample_rate,
                     new_freq=self.speaker_manager.encoder.audio_config["sample_rate"],
                 )
 
     def _init_speaker_embedding(self):
         # pylint: disable=attribute-defined-outside-init
         if self.num_speakers > 0:
-            print(" > initialization of speaker-embedding layers.")
+            logger.info("Initialization of speaker-embedding layers.")
             self.embedded_speaker_dim = self.args.speaker_embedding_channels
             self.emb_g = nn.Embedding(self.num_speakers, self.embedded_speaker_dim)
 
     def _init_d_vector(self):
         # pylint: disable=attribute-defined-outside-init
         if hasattr(self, "emb_g"):
             raise ValueError("[!] Speaker embedding layer already initialized before d_vector settings.")
@@ -794,15 +797,15 @@
         Args:
             config (Coqpit): Model configuration.
         """
         if self.args.language_ids_file is not None:
             self.language_manager = LanguageManager(language_ids_file_path=config.language_ids_file)
 
         if self.args.use_language_embedding and self.language_manager:
-            print(" > initialization of language-embedding layers.")
+            logger.info("Initialization of language-embedding layers.")
             self.num_languages = self.language_manager.num_languages
             self.embedded_language_dim = self.args.embedded_language_dim
             self.emb_l = nn.Embedding(self.num_languages, self.embedded_language_dim)
             torch.nn.init.xavier_uniform_(self.emb_l.weight)
         else:
             self.embedded_language_dim = 0
 
@@ -829,25 +832,25 @@
             before_dict = get_module_weights_sum(self.duration_predictor)
             # Applies weights_reset recursively to every submodule of the duration predictor
             self.duration_predictor.apply(fn=weights_reset)
             after_dict = get_module_weights_sum(self.duration_predictor)
             for key, value in after_dict.items():
                 if value == before_dict[key]:
                     raise RuntimeError(" [!] The weights of Duration Predictor was not reinit check it !")
-            print(" > Duration Predictor was reinit.")
+            logger.info("Duration Predictor was reinit.")
 
         if self.args.reinit_text_encoder:
             before_dict = get_module_weights_sum(self.text_encoder)
             # Applies weights_reset recursively to every submodule of the duration predictor
             self.text_encoder.apply(fn=weights_reset)
             after_dict = get_module_weights_sum(self.text_encoder)
             for key, value in after_dict.items():
                 if value == before_dict[key]:
                     raise RuntimeError(" [!] The weights of Text Encoder was not reinit check it !")
-            print(" > Text Encoder was reinit.")
+            logger.info("Text Encoder was reinit.")
 
     def get_aux_input(self, aux_input: Dict):
         sid, g, lid, _ = self._set_cond_input(aux_input)
         return {"speaker_ids": sid, "style_wav": None, "d_vectors": g, "language_ids": lid}
 
     def _freeze_layers(self):
         if self.args.freeze_encoder:
@@ -1433,15 +1436,15 @@
         """Generic test run for `tts` models used by `Trainer`.
 
         You can override this for a different behaviour.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         for idx, s_info in enumerate(test_sentences):
             aux_inputs = self.get_aux_input_from_test_sentences(s_info)
             wav, alignment, _, _ = synthesis(
                 self,
@@ -1550,22 +1553,22 @@
         return batch
 
     def get_sampler(self, config: Coqpit, dataset: TTSDataset, num_gpus=1, is_eval=False):
         weights = None
         data_items = dataset.samples
         if getattr(config, "use_weighted_sampler", False):
             for attr_name, alpha in config.weighted_sampler_attrs.items():
-                print(f" > Using weighted sampler for attribute '{attr_name}' with alpha '{alpha}'")
+                logger.info("Using weighted sampler for attribute '%s' with alpha %.3f", attr_name, alpha)
                 multi_dict = config.weighted_sampler_multipliers.get(attr_name, None)
-                print(multi_dict)
+                logger.info(multi_dict)
                 weights, attr_names, attr_weights = get_attribute_balancer_weights(
                     attr_name=attr_name, items=data_items, multi_dict=multi_dict
                 )
                 weights = weights * alpha
-                print(f" > Attribute weights for '{attr_names}' \n | > {attr_weights}")
+                logger.info("Attribute weights for '%s' \n | > %s", attr_names, attr_weights)
 
         # input_audio_lenghts = [os.path.getsize(x["audio_file"]) for x in data_items]
 
         if weights is not None:
             w_sampler = WeightedRandomSampler(weights, len(weights))
             batch_sampler = BucketBatchSampler(
                 w_sampler,
@@ -1605,15 +1608,14 @@
                 batch_group_size=0 if is_eval else config.batch_group_size * config.batch_size,
                 min_text_len=config.min_text_len,
                 max_text_len=config.max_text_len,
                 min_audio_len=config.min_audio_len,
                 max_audio_len=config.max_audio_len,
                 phoneme_cache_path=config.phoneme_cache_path,
                 precompute_num_workers=config.precompute_num_workers,
-                verbose=verbose,
                 tokenizer=self.tokenizer,
                 start_by_longest=config.start_by_longest,
             )
 
             # wait all the DDP process to be ready
             if num_gpus > 1:
                 dist.barrier()
@@ -1715,15 +1717,15 @@
         if self.args.encoder_sample_rate is not None and eval:
             # audio resampler is not used in inference time
             self.audio_resampler = None
 
         # handle fine-tuning from a checkpoint with additional speakers
         if hasattr(self, "emb_g") and state["model"]["emb_g.weight"].shape != self.emb_g.weight.shape:
             num_new_speakers = self.emb_g.weight.shape[0] - state["model"]["emb_g.weight"].shape[0]
-            print(f" > Loading checkpoint with {num_new_speakers} additional speakers.")
+            logger.info("Loading checkpoint with %d additional speakers.", num_new_speakers)
             emb_g = state["model"]["emb_g.weight"]
             new_row = torch.randn(num_new_speakers, emb_g.shape[1])
             emb_g = torch.cat([emb_g, new_row], axis=0)
             state["model"]["emb_g.weight"] = emb_g
         # load the model weights
         self.load_state_dict(state["model"], strict=strict)
 
@@ -1772,15 +1774,15 @@
         new_chk = rehash_fairseq_vits_checkpoint(checkpoint_file)
         self.load_state_dict(new_chk, strict=strict)
         if eval:
             self.eval()
             assert not self.training
 
     @staticmethod
-    def init_from_config(config: "VitsConfig", samples: Union[List[List], List[Dict]] = None, verbose=True):
+    def init_from_config(config: "VitsConfig", samples: Union[List[List], List[Dict]] = None):
         """Initiate model from config
 
         Args:
             config (VitsConfig): Model config.
             samples (Union[List[List], List[Dict]]): Training samples to parse speaker ids for training.
                 Defaults to None.
         """
@@ -1795,15 +1797,15 @@
         else:
             encoder_to_vocoder_upsampling_factor = config.audio.sample_rate / config.model_args.encoder_sample_rate
             effective_hop_length = config.audio.hop_length * encoder_to_vocoder_upsampling_factor
             assert (
                 upsample_rate == effective_hop_length
             ), f" [!] Product of upsample rates must be equal to the hop length - {upsample_rate} vs {effective_hop_length}"
 
-        ap = AudioProcessor.init_from_config(config, verbose=verbose)
+        ap = AudioProcessor.init_from_config(config)
         tokenizer, new_config = TTSTokenizer.init_from_config(config)
         speaker_manager = SpeakerManager.init_from_config(config, samples)
         language_manager = LanguageManager.init_from_config(config)
 
         if config.model_args.speaker_encoder_model_path:
             speaker_manager.init_encoder(
                 config.model_args.speaker_encoder_model_path, config.model_args.speaker_encoder_config_path
```

### Comparing `coqui-tts-0.22.1/TTS/tts/models/xtts.py` & `coqui_tts-0.23.0/TTS/tts/models/xtts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from dataclasses import dataclass
 
 import librosa
 import torch
 import torch.nn.functional as F
 import torchaudio
@@ -11,14 +12,16 @@
 from TTS.tts.layers.xtts.hifigan_decoder import HifiDecoder
 from TTS.tts.layers.xtts.stream_generator import init_stream_support
 from TTS.tts.layers.xtts.tokenizer import VoiceBpeTokenizer, split_sentence
 from TTS.tts.layers.xtts.xtts_manager import LanguageManager, SpeakerManager
 from TTS.tts.models.base_tts import BaseTTS
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 init_stream_support()
 
 
 def wav_to_mel_cloning(
     wav,
     mel_norms_file="../experiments/clips_mel_norms.pth",
     mel_norms=None,
@@ -78,15 +81,15 @@
 
     if lsr != sampling_rate:
         audio = torchaudio.functional.resample(audio, lsr, sampling_rate)
 
     # Check some assumptions about audio range. This should be automatically fixed in load_wav_to_torch, but might not be in some edge cases, where we should squawk.
     # '10' is arbitrarily chosen since it seems like audio will often "overdrive" the [-1,1] bounds.
     if torch.any(audio > 10) or not torch.any(audio < 0):
-        print(f"Error with {audiopath}. Max={audio.max()} min={audio.min()}")
+        logger.error("Error with %s. Max=%.2f min=%.2f", audiopath, audio.max(), audio.min())
     # clip audio invalid values
     audio.clip_(-1, 1)
     return audio
 
 
 def pad_or_truncate(t, length):
     """
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/assets/tortoise/tokenizer.json` & `coqui_tts-0.23.0/TTS/tts/utils/assets/tortoise/tokenizer.json`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/data.py` & `coqui_tts-0.23.0/TTS/tts/utils/data.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/fairseq.py` & `coqui_tts-0.23.0/TTS/tts/utils/fairseq.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/helpers.py` & `coqui_tts-0.23.0/TTS/tts/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/languages.py` & `coqui_tts-0.23.0/TTS/tts/utils/languages.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/managers.py` & `coqui_tts-0.23.0/TTS/tts/utils/managers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/measures.py` & `coqui_tts-0.23.0/TTS/tts/utils/measures.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/core.c` & `coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.c`

 * *Files 1% similar despite different names*

```diff
@@ -1110,177 +1110,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":688
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":695
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":702
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":712
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1311,42 +1311,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3244,15 +3244,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_xs, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_t_ys, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3261,29 +3261,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3294,15 +3294,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3311,29 +3311,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3344,15 +3344,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3361,29 +3361,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3394,15 +3394,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3411,29 +3411,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3444,15 +3444,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3461,29 +3461,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3494,89 +3494,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":926
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3584,33 +3584,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":928
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -3618,96 +3618,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":930
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":933
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":934
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":938
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3723,15 +3723,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":939
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3739,53 +3739,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":940
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
@@ -3793,30 +3793,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 942, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":939
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3831,15 +3831,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":944
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3855,15 +3855,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3871,53 +3871,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":946
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":946
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
@@ -3925,30 +3925,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 948, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":945
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3963,15 +3963,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":950
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3987,15 +3987,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4003,53 +4003,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":952
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":952
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":954
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
@@ -4057,30 +4057,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 954, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":951
+    /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4095,176 +4095,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":964
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":976
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":976
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":964
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":964
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":979
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":991
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":991
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":979
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":994
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1001
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1001
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":994
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1008
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1008
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1004
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+/* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1015
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1015
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":1011
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -18201,26 +18201,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":942
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 942, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-2ckg1ga1/lib/python3.9/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-zm95vn3w/lib/python3.9/site-packages/numpy/__init__.pxd":948
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 948, __pyx_L1_error)
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/monotonic_align/core.pyx` & `coqui_tts-0.23.0/TTS/tts/utils/monotonic_align/core.pyx`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/speakers.py` & `coqui_tts-0.23.0/TTS/tts/utils/speakers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import json
+import logging
 import os
 from typing import Any, Dict, List, Union
 
 import fsspec
 import numpy as np
 import torch
 from coqpit import Coqpit
 
 from TTS.config import get_from_config_or_model_args_with_default
 from TTS.tts.utils.managers import EmbeddingManager
 
+logger = logging.getLogger(__name__)
+
 
 class SpeakerManager(EmbeddingManager):
     """Manage the speakers for multi-speaker 🐸TTS models. Load a datafile and parse the information
     in a way that can be queried by speaker or clip.
 
     There are 3 different scenarios considered:
 
@@ -166,15 +169,17 @@
             speaker_manager.set_ids_from_data(data, parse_key="speaker_name")
         if restore_path:
             speakers_file = _set_file_path(restore_path)
             # restoring speaker manager from a previous run.
             if c.use_d_vector_file:
                 # restore speaker manager with the embedding file
                 if not os.path.exists(speakers_file):
-                    print("WARNING: speakers.json was not found in restore_path, trying to use CONFIG.d_vector_file")
+                    logger.warning(
+                        "speakers.json was not found in %s, trying to use CONFIG.d_vector_file", restore_path
+                    )
                     if not os.path.exists(c.d_vector_file):
                         raise RuntimeError(
                             "You must copy the file speakers.json to restore_path, or set a valid file in CONFIG.d_vector_file"
                         )
                     speaker_manager.load_embeddings_from_file(c.d_vector_file)
                 speaker_manager.load_embeddings_from_file(speakers_file)
             elif not c.use_d_vector_file:  # restor speaker manager with speaker ID file.
@@ -189,24 +194,24 @@
         elif c.use_d_vector_file and not c.d_vector_file:
             raise "use_d_vector_file is True, so you need pass a external speaker embedding file."
         elif c.use_speaker_embedding and "speakers_file" in c and c.speakers_file:
             # new speaker manager with speaker IDs file.
             speaker_manager.load_ids_from_file(c.speakers_file)
 
         if speaker_manager.num_speakers > 0:
-            print(
-                " > Speaker manager is loaded with {} speakers: {}".format(
-                    speaker_manager.num_speakers, ", ".join(speaker_manager.name_to_id)
-                )
+            logger.info(
+                "Speaker manager is loaded with %d speakers: %s",
+                speaker_manager.num_speakers,
+                ", ".join(speaker_manager.name_to_id),
             )
 
         # save file if path is defined
         if out_path:
             out_file_path = os.path.join(out_path, "speakers.json")
-            print(f" > Saving `speakers.json` to {out_file_path}.")
+            logger.info("Saving `speakers.json` to %s", out_file_path)
             if c.use_d_vector_file and c.d_vector_file:
                 speaker_manager.save_embeddings_to_file(out_file_path)
             else:
                 speaker_manager.save_ids_to_file(out_file_path)
     return speaker_manager
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/ssim.py` & `coqui_tts-0.23.0/TTS/tts/utils/ssim.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/synthesis.py` & `coqui_tts-0.23.0/TTS/tts/utils/synthesis.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/bangla/phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/bangla/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/belarusian/phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/belarusian/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/characters.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/characters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import logging
 from dataclasses import replace
 from typing import Dict
 
 from TTS.tts.configs.shared_configs import CharactersConfig
 
+logger = logging.getLogger(__name__)
+
 
 def parse_symbols():
     return {
         "pad": _pad,
         "eos": _eos,
         "bos": _bos,
         "characters": _characters,
@@ -301,22 +304,22 @@
         return self._id_to_char[idx]
 
     def print_log(self, level: int = 0):
         """
         Prints the vocabulary in a nice format.
         """
         indent = "\t" * level
-        print(f"{indent}| > Characters: {self._characters}")
-        print(f"{indent}| > Punctuations: {self._punctuations}")
-        print(f"{indent}| > Pad: {self._pad}")
-        print(f"{indent}| > EOS: {self._eos}")
-        print(f"{indent}| > BOS: {self._bos}")
-        print(f"{indent}| > Blank: {self._blank}")
-        print(f"{indent}| > Vocab: {self.vocab}")
-        print(f"{indent}| > Num chars: {self.num_chars}")
+        logger.info("%s| Characters: %s", indent, self._characters)
+        logger.info("%s| Punctuations: %s", indent, self._punctuations)
+        logger.info("%s| Pad: %s", indent, self._pad)
+        logger.info("%s| EOS: %s", indent, self._eos)
+        logger.info("%s| BOS: %s", indent, self._bos)
+        logger.info("%s| Blank: %s", indent, self._blank)
+        logger.info("%s| Vocab: %s", indent, self.vocab)
+        logger.info("%s| Num chars: %d", indent, self.num_chars)
 
     @staticmethod
     def init_from_config(config: "Coqpit"):  # pylint: disable=unused-argument
         """Init your character class from a config.
 
         Implement this method for your subclass.
         """
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/numbers.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/numbers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/chinese_mandarin/pinyinToPhonemes.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/cleaners.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/cmudict.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/cmudict.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/english/abbreviations.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/english/abbreviations.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/english/number_norm.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/english/number_norm.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/english/time_norm.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/english/time_norm.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/french/abbreviations.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/french/abbreviations.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/japanese/phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/japanese/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/korean/ko_dictionary.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/korean/ko_dictionary.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/korean/korean.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/korean/korean.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/korean/phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/korean/phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/__init__.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/bangla_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/base.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import abc
+import logging
 from typing import List, Tuple
 
 from TTS.tts.utils.text.punctuation import Punctuation
 
+logger = logging.getLogger(__name__)
+
 
 class BasePhonemizer(abc.ABC):
     """Base phonemizer class
 
     Phonemization follows the following steps:
         1. Preprocessing:
             - remove empty lines
@@ -132,9 +135,9 @@
             p = self._phonemize(t, separator)
             phonemized.append(p)
         phonemized = self._phonemize_postprocess(phonemized, punctuations)
         return phonemized
 
     def print_logs(self, level: int = 0):
         indent = "\t" * level
-        print(f"{indent}| > phoneme language: {self.language}")
-        print(f"{indent}| > phoneme backend: {self.name()}")
+        logger.info("%s| phoneme language: %s", indent, self.language)
+        logger.info("%s| phoneme backend: %s", indent, self.name())
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/belarusian_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/espeak_wrapper.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/espeak_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Dict, List
 
 from packaging.version import Version
 
 from TTS.tts.utils.text.phonemizers.base import BasePhonemizer
 from TTS.tts.utils.text.punctuation import Punctuation
 
+logger = logging.getLogger(__name__)
+
 
 def is_tool(name):
     from shutil import which
 
     return which(name) is not None
 
 
@@ -49,15 +51,15 @@
     cmd = [
         espeak_lib,
         "-q",
         "-b",
         "1",  # UTF8 text encoding
     ]
     cmd.extend(args)
-    logging.debug("espeakng: executing %s", repr(cmd))
+    logger.debug("espeakng: executing %s", repr(cmd))
 
     with subprocess.Popen(
         cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
     ) as p:
         res = iter(p.stdout.readline, b"")
@@ -185,15 +187,15 @@
         if tie:
             args.append("--tie=%s" % tie)
 
         args.append(text)
         # compute phonemes
         phonemes = ""
         for line in _espeak_exe(self._ESPEAK_LIB, args, sync=True):
-            logging.debug("line: %s", repr(line))
+            logger.debug("line: %s", repr(line))
             ph_decoded = line.decode("utf8").strip()
             # espeak:
             #   version 1.48.15: " p_ɹ_ˈaɪ_ɚ t_ə n_oʊ_v_ˈɛ_m_b_ɚ t_w_ˈɛ_n_t_i t_ˈuː\n"
             # espeak-ng:
             #   "p_ɹ_ˈaɪ_ɚ t_ə n_oʊ_v_ˈɛ_m_b_ɚ t_w_ˈɛ_n_t_i t_ˈuː\n"
 
             # espeak-ng backend can add language flags that need to be removed:
@@ -223,28 +225,28 @@
         for line in _espeak_exe(_DEF_ESPEAK_LIB, args, sync=True):
             line = line.decode("utf8").strip()
             if count > 0:
                 cols = line.split()
                 lang_code = cols[1]
                 lang_name = cols[3]
                 langs[lang_code] = lang_name
-            logging.debug("line: %s", repr(line))
+            logger.debug("line: %s", repr(line))
             count += 1
         return langs
 
     def version(self) -> str:
         """Get the version of the used backend.
 
         Returns:
             str: Version of the used backend.
         """
         args = ["--version"]
         for line in _espeak_exe(self.backend, args, sync=True):
             version = line.decode("utf8").strip().split()[2]
-            logging.debug("line: %s", repr(line))
+            logger.debug("line: %s", repr(line))
             return version
 
     @classmethod
     def is_available(cls):
         """Return true if ESpeak is available else false"""
         return is_tool("espeak") or is_tool("espeak-ng")
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/gruut_wrapper.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/gruut_wrapper.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ja_jp_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/ko_kr_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/multi_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/multi_phonemizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import logging
 from typing import Dict, List
 
 from TTS.tts.utils.text.phonemizers import DEF_LANG_TO_PHONEMIZER, get_phonemizer_by_name
 
+logger = logging.getLogger(__name__)
+
 
 class MultiPhonemizer:
     """🐸TTS multi-phonemizer that operates phonemizers for multiple langugages
 
     Args:
         custom_lang_to_phonemizer (Dict):
             Custom phonemizer mapping if you want to change the defaults. In the format of
@@ -42,16 +45,16 @@
         return self.lang_to_phonemizer[language].phonemize(text, separator)
 
     def supported_languages(self) -> List:
         return list(self.lang_to_phonemizer.keys())
 
     def print_logs(self, level: int = 0):
         indent = "\t" * level
-        print(f"{indent}| > phoneme language: {self.supported_languages()}")
-        print(f"{indent}| > phoneme backend: {self.name()}")
+        logger.info("%s| phoneme language: %s", indent, self.supported_languages())
+        logger.info("%s| phoneme backend: %s", indent, self.name())
 
 
 # if __name__ == "__main__":
 #     texts = {
 #         "tr": "Merhaba, bu Türkçe bit örnek!",
 #         "en-us": "Hello, this is English example!",
 #         "de": "Hallo, das ist ein Deutches Beipiel!",
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/phonemizers/zh_cn_phonemizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/punctuation.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/punctuation.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/text/tokenizer.py` & `coqui_tts-0.23.0/TTS/tts/utils/text/tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
 from typing import Callable, Dict, List, Union
 
 from TTS.tts.utils.text import cleaners
 from TTS.tts.utils.text.characters import Graphemes, IPAPhonemes
 from TTS.tts.utils.text.phonemizers import DEF_LANG_TO_PHONEMIZER, get_phonemizer_by_name
 from TTS.tts.utils.text.phonemizers.multi_phonemizer import MultiPhonemizer
 from TTS.utils.generic_utils import get_import_path, import_class
 
+logger = logging.getLogger(__name__)
+
 
 class TTSTokenizer:
     """🐸TTS tokenizer to convert input characters to token IDs and back.
 
     Token IDs for OOV chars are discarded but those are stored in `self.not_found_characters` for later.
 
     Args:
@@ -69,16 +72,16 @@
             try:
                 idx = self.characters.char_to_id(char)
                 token_ids.append(idx)
             except KeyError:
                 # discard but store not found characters
                 if char not in self.not_found_characters:
                     self.not_found_characters.append(char)
-                    print(text)
-                    print(f" [!] Character {repr(char)} not found in the vocabulary. Discarding it.")
+                    logger.warning(text)
+                    logger.warning("Character %s not found in the vocabulary. Discarding it.", repr(char))
         return token_ids
 
     def decode(self, token_ids: List[int]) -> str:
         """Decodes a sequence of IDs to a string of text."""
         text = ""
         for token_id in token_ids:
             text += self.characters.id_to_char(token_id)
@@ -100,18 +103,21 @@
         1. Text normalizatin
         2. Phonemization (if use_phonemes is True)
         3. Add blank char between characters
         4. Add BOS and EOS characters
         5. Text to token IDs
         """
         # TODO: text cleaner should pick the right routine based on the language
+        logger.debug("Tokenizer input text: %s", text)
         if self.text_cleaner is not None:
             text = self.text_cleaner(text)
+            logger.debug("Cleaned text: %s", text)
         if self.use_phonemes:
             text = self.phonemizer.phonemize(text, separator="", language=language)
+            logger.debug("Phonemes: %s", text)
         text = self.encode(text)
         if self.add_blank:
             text = self.intersperse_blank_char(text, True)
         if self.use_eos_bos:
             text = self.pad_with_bos_eos(text)
         return text
 
@@ -131,24 +137,24 @@
         char_to_use = self.characters.blank_id if use_blank_char else self.characters.pad
         result = [char_to_use] * (len(char_sequence) * 2 + 1)
         result[1::2] = char_sequence
         return result
 
     def print_logs(self, level: int = 0):
         indent = "\t" * level
-        print(f"{indent}| > add_blank: {self.add_blank}")
-        print(f"{indent}| > use_eos_bos: {self.use_eos_bos}")
-        print(f"{indent}| > use_phonemes: {self.use_phonemes}")
+        logger.info("%s| add_blank: %s", indent, self.add_blank)
+        logger.info("%s| use_eos_bos: %s", indent, self.use_eos_bos)
+        logger.info("%s| use_phonemes: %s", indent, self.use_phonemes)
         if self.use_phonemes:
-            print(f"{indent}| > phonemizer:")
+            logger.info("%s| phonemizer:", indent)
             self.phonemizer.print_logs(level + 1)
         if len(self.not_found_characters) > 0:
-            print(f"{indent}| > {len(self.not_found_characters)} not found characters:")
+            logger.info("%s| %d characters not found:", indent, len(self.not_found_characters))
             for char in self.not_found_characters:
-                print(f"{indent}| > {char}")
+                logger.info("%s| %s", indent, char)
 
     @staticmethod
     def init_from_config(config: "Coqpit", characters: "BaseCharacters" = None):
         """Init Tokenizer object from config
 
         Args:
             config (Coqpit): Coqpit model config.
```

### Comparing `coqui-tts-0.22.1/TTS/tts/utils/visual.py` & `coqui_tts-0.23.0/TTS/tts/utils/visual.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/audio/numpy_transforms.py` & `coqui_tts-0.23.0/TTS/utils/audio/numpy_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 from io import BytesIO
 from typing import Tuple
 
 import librosa
 import numpy as np
 import scipy
 import soundfile as sf
 from librosa import magphase, pyin
 
+logger = logging.getLogger(__name__)
+
 # For using kwargs
 # pylint: disable=unused-argument
 
 
 def build_mel_basis(
     *,
     sample_rate: int = None,
@@ -218,15 +221,15 @@
 
 
 def griffin_lim(*, spec: np.ndarray = None, num_iter=60, **kwargs) -> np.ndarray:
     angles = np.exp(2j * np.pi * np.random.rand(*spec.shape))
     S_complex = np.abs(spec).astype(complex)
     y = istft(y=S_complex * angles, **kwargs)
     if not np.isfinite(y).all():
-        print(" [!] Waveform is not finite everywhere. Skipping the GL.")
+        logger.warning("Waveform is not finite everywhere. Skipping the GL.")
         return np.array([0.0])
     for _ in range(num_iter):
         angles = np.exp(1j * np.angle(stft(y=y, **kwargs)))
         y = istft(y=S_complex * angles, **kwargs)
     return y
```

### Comparing `coqui-tts-0.22.1/TTS/utils/audio/processor.py` & `coqui_tts-0.23.0/TTS/utils/audio/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from io import BytesIO
 from typing import Dict, Tuple
 
 import librosa
 import numpy as np
 import scipy.io.wavfile
 import scipy.signal
@@ -22,14 +23,16 @@
     rms_volume_norm,
     spec_to_mel,
     stft,
     trim_silence,
     volume_norm,
 )
 
+logger = logging.getLogger(__name__)
+
 # pylint: disable=too-many-public-methods
 
 
 class AudioProcessor(object):
     """Audio Processor for TTS.
 
     Note:
@@ -128,18 +131,14 @@
             enable/disable RMS volume normalization when loading an audio file. Defaults to False.
 
         db_level (int, optional):
             dB level used for rms normalization. The range is -99 to 0. Defaults to None.
 
         stats_path (str, optional):
             Path to the computed stats file. Defaults to None.
-
-        verbose (bool, optional):
-            enable/disable logging. Defaults to True.
-
     """
 
     def __init__(
         self,
         sample_rate=None,
         resample=False,
         num_mels=None,
@@ -168,15 +167,14 @@
         trim_db=60,
         do_sound_norm=False,
         do_amp_to_db_linear=True,
         do_amp_to_db_mel=True,
         do_rms_norm=False,
         db_level=None,
         stats_path=None,
-        verbose=True,
         **_,
     ):
         # setup class attributed
         self.sample_rate = sample_rate
         self.resample = resample
         self.num_mels = num_mels
         self.log_func = log_func
@@ -224,18 +222,17 @@
             self.hop_length = hop_length
             self.win_length = win_length
         assert min_level_db != 0.0, " [!] min_level_db is 0"
         assert (
             self.win_length <= self.fft_size
         ), f" [!] win_length cannot be larger than fft_size - {self.win_length} vs {self.fft_size}"
         members = vars(self)
-        if verbose:
-            print(" > Setting up Audio Processor...")
-            for key, value in members.items():
-                print(" | > {}:{}".format(key, value))
+        logger.info("Setting up Audio Processor...")
+        for key, value in members.items():
+            logger.info(" | %s: %s", key, value)
         # create spectrogram utils
         self.mel_basis = build_mel_basis(
             sample_rate=self.sample_rate,
             fft_size=self.fft_size,
             num_mels=self.num_mels,
             mel_fmax=self.mel_fmax,
             mel_fmin=self.mel_fmin,
@@ -246,18 +243,18 @@
             self.setup_scaler(mel_mean, mel_std, linear_mean, linear_std)
             self.signal_norm = True
             self.max_norm = None
             self.clip_norm = None
             self.symmetric_norm = None
 
     @staticmethod
-    def init_from_config(config: "Coqpit", verbose=True):
+    def init_from_config(config: "Coqpit"):
         if "audio" in config:
-            return AudioProcessor(verbose=verbose, **config.audio)
-        return AudioProcessor(verbose=verbose, **config)
+            return AudioProcessor(**config.audio)
+        return AudioProcessor(**config)
 
     ### normalization ###
     def normalize(self, S: np.ndarray) -> np.ndarray:
         """Normalize values into `[0, self.max_norm]` or `[-self.max_norm, self.max_norm]`
 
         Args:
             S (np.ndarray): Spectrogram to normalize.
@@ -591,15 +588,15 @@
             x = load_wav(filename=filename, sample_rate=sr, resample=True)
         else:
             x = load_wav(filename=filename, sample_rate=self.sample_rate, resample=self.resample)
         if self.do_trim_silence:
             try:
                 x = self.trim_silence(x)
             except ValueError:
-                print(f" [!] File cannot be trimmed for silence - {filename}")
+                logger.exception("File cannot be trimmed for silence - %s", filename)
         if self.do_sound_norm:
             x = self.sound_norm(x)
         if self.do_rms_norm:
             x = self.rms_volume_norm(x, self.db_level)
         return x
 
     def save_wav(self, wav: np.ndarray, path: str, sr: int = None, pipe_out=None) -> None:
```

### Comparing `coqui-tts-0.22.1/TTS/utils/audio/torch_transforms.py` & `coqui_tts-0.23.0/TTS/utils/audio/torch_transforms.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/callbacks.py` & `coqui_tts-0.23.0/TTS/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/capacitron_optimizer.py` & `coqui_tts-0.23.0/TTS/utils/capacitron_optimizer.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/distribute.py` & `coqui_tts-0.23.0/TTS/utils/distribute.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/download.py` & `coqui_tts-0.23.0/TTS/utils/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import urllib.request
 import zipfile
 from os.path import expanduser
 from typing import Any, Iterable, List, Optional
 
 from torch.utils.model_zoo import tqdm
 
+logger = logging.getLogger(__name__)
+
 
 def stream_url(
     url: str, start_byte: Optional[int] = None, block_size: int = 32 * 1024, progress_bar: bool = True
 ) -> Iterable:
     """Stream url by chunk
 
     Args:
@@ -145,43 +147,43 @@
         to_path (str or None, optional): the root path of the extraced files (directory of from_path)
             (Default: ``None``)
         overwrite (bool, optional): overwrite existing files (Default: ``False``)
 
     Returns:
         list: List of paths to extracted files even if not overwritten.
     """
-
+    logger.info("Extracting archive file...")
     if to_path is None:
         to_path = os.path.dirname(from_path)
 
     try:
         with tarfile.open(from_path, "r") as tar:
-            logging.info("Opened tar file %s.", from_path)
+            logger.info("Opened tar file %s.", from_path)
             files = []
             for file_ in tar:  # type: Any
                 file_path = os.path.join(to_path, file_.name)
                 if file_.isfile():
                     files.append(file_path)
                     if os.path.exists(file_path):
-                        logging.info("%s already extracted.", file_path)
+                        logger.info("%s already extracted.", file_path)
                         if not overwrite:
                             continue
                 tar.extract(file_, to_path)
             return files
     except tarfile.ReadError:
         pass
 
     try:
         with zipfile.ZipFile(from_path, "r") as zfile:
-            logging.info("Opened zip file %s.", from_path)
+            logger.info("Opened zip file %s.", from_path)
             files = zfile.namelist()
             for file_ in files:
                 file_path = os.path.join(to_path, file_)
                 if os.path.exists(file_path):
-                    logging.info("%s already extracted.", file_path)
+                    logger.info("%s already extracted.", file_path)
                     if not overwrite:
                         continue
                 zfile.extract(file_, to_path)
         return files
     except zipfile.BadZipFile:
         pass
 
@@ -197,13 +199,14 @@
         output_path (str): Path of the location you want the dataset folder to be saved to.
     """
     data_path = os.path.join(output_path, dataset_name)
     try:
         import kaggle  # pylint: disable=import-outside-toplevel
 
         kaggle.api.authenticate()
-        print(f"""\nDownloading {dataset_name}...""")
+        logger.info("Downloading %s...", dataset_name)
         kaggle.api.dataset_download_files(dataset_path, path=data_path, unzip=True)
     except OSError:
-        print(
-            f"""[!] in order to download kaggle datasets, you need to have a kaggle api token stored in your {os.path.join(expanduser('~'), '.kaggle/kaggle.json')}"""
+        logger.exception(
+            "In order to download kaggle datasets, you need to have a kaggle api token stored in your %s",
+            os.path.join(expanduser("~"), ".kaggle/kaggle.json"),
         )
```

### Comparing `coqui-tts-0.22.1/TTS/utils/downloaders.py` & `coqui_tts-0.23.0/TTS/utils/downloaders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import logging
 import os
 from typing import Optional
 
 from TTS.utils.download import download_kaggle_dataset, download_url, extract_archive
 
+logger = logging.getLogger(__name__)
+
 
 def download_ljspeech(path: str):
     """Download and extract LJSpeech dataset
 
     Args:
         path (str): path to the directory where the dataset will be stored.
     """
     os.makedirs(path, exist_ok=True)
     url = "https://data.keithito.com/data/speech/LJSpeech-1.1.tar.bz2"
     download_url(url, path)
     basename = os.path.basename(url)
     archive = os.path.join(path, basename)
-    print(" > Extracting archive file...")
     extract_archive(archive)
 
 
 def download_vctk(path: str, use_kaggle: Optional[bool] = False):
     """Download and extract VCTK dataset.
 
     Args:
@@ -31,15 +33,14 @@
         download_kaggle_dataset("mfekadu/english-multispeaker-corpus-for-voice-cloning", "VCTK", path)
     else:
         os.makedirs(path, exist_ok=True)
         url = "https://datashare.ed.ac.uk/bitstream/handle/10283/3443/VCTK-Corpus-0.92.zip"
         download_url(url, path)
         basename = os.path.basename(url)
         archive = os.path.join(path, basename)
-        print(" > Extracting archive file...")
         extract_archive(archive)
 
 
 def download_tweb(path: str):
     """Download and extract Tweb dataset
 
     Args:
@@ -67,42 +68,39 @@
         "libri-tts-test-clean": "http://www.openslr.org/resources/60/test-clean.tar.gz",
         "libri-tts-test-other": "http://www.openslr.org/resources/60/test-other.tar.gz",
     }
 
     os.makedirs(path, exist_ok=True)
     if subset == "all":
         for sub, val in subset_dict.items():
-            print(f" > Downloading {sub}...")
+            logger.info("Downloading %s...", sub)
             download_url(val, path)
             basename = os.path.basename(val)
             archive = os.path.join(path, basename)
-            print(" > Extracting archive file...")
             extract_archive(archive)
-        print(" > All subsets downloaded")
+        logger.info("All subsets downloaded")
     else:
         url = subset_dict[subset]
         download_url(url, path)
         basename = os.path.basename(url)
         archive = os.path.join(path, basename)
-        print(" > Extracting archive file...")
         extract_archive(archive)
 
 
 def download_thorsten_de(path: str):
     """Download and extract Thorsten german male voice dataset.
 
     Args:
         path (str): Path to the directory where the dataset will be stored.
     """
     os.makedirs(path, exist_ok=True)
     url = "https://www.openslr.org/resources/95/thorsten-de_v02.tgz"
     download_url(url, path)
     basename = os.path.basename(url)
     archive = os.path.join(path, basename)
-    print(" > Extracting archive file...")
     extract_archive(archive)
 
 
 def download_mailabs(path: str, language: str = "english"):
     """Download and extract Mailabs dataset.
 
     Args:
@@ -118,9 +116,8 @@
         "spanish": "https://data.solak.de/data/Training/stt_tts/es_ES.tgz",
     }
     os.makedirs(path, exist_ok=True)
     url = language_dict[language]
     download_url(url, path)
     basename = os.path.basename(url)
     archive = os.path.join(path, basename)
-    print(" > Extracting archive file...")
     extract_archive(archive)
```

### Comparing `coqui-tts-0.22.1/TTS/utils/generic_utils.py` & `coqui_tts-0.23.0/TTS/utils/generic_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import importlib
 import logging
 import os
 import re
 import subprocess
 import sys
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
+
+logger = logging.getLogger(__name__)
 
 
 # TODO: This method is duplicated in Trainer but out of date there
 def get_git_branch():
     try:
         out = subprocess.check_output(["git", "branch"]).decode("utf8")
         current = next(line for line in out.split("\n") if line.startswith("*"))
@@ -87,26 +89,26 @@
     return ans.joinpath(appname)
 
 
 def set_init_dict(model_dict, checkpoint_state, c):
     # Partial initialization: if there is a mismatch with new and old layer, it is skipped.
     for k, v in checkpoint_state.items():
         if k not in model_dict:
-            print(" | > Layer missing in the model definition: {}".format(k))
+            logger.warning("Layer missing in the model finition %s", k)
     # 1. filter out unnecessary keys
     pretrained_dict = {k: v for k, v in checkpoint_state.items() if k in model_dict}
     # 2. filter out different size layers
     pretrained_dict = {k: v for k, v in pretrained_dict.items() if v.numel() == model_dict[k].numel()}
     # 3. skip reinit layers
     if c.has("reinit_layers") and c.reinit_layers is not None:
         for reinit_layer_name in c.reinit_layers:
             pretrained_dict = {k: v for k, v in pretrained_dict.items() if reinit_layer_name not in k}
     # 4. overwrite entries in the existing state dict
     model_dict.update(pretrained_dict)
-    print(" | > {} / {} layers are restored.".format(len(pretrained_dict), len(model_dict)))
+    logger.info("%d / %d layers are restored.", len(pretrained_dict), len(model_dict))
     return model_dict
 
 
 def format_aux_input(def_args: Dict, kwargs: Dict) -> Dict:
     """Format kwargs to hande auxilary inputs to models.
 
     Args:
@@ -119,24 +121,51 @@
     kwargs = kwargs.copy()
     for name in def_args:
         if name not in kwargs or kwargs[name] is None:
             kwargs[name] = def_args[name]
     return kwargs
 
 
-def get_timestamp():
+def get_timestamp() -> str:
     return datetime.now().strftime("%y%m%d-%H%M%S")
 
 
-def setup_logger(logger_name, root, phase, level=logging.INFO, screen=False, tofile=False):
+class ConsoleFormatter(logging.Formatter):
+    """Custom formatter that prints logging.INFO messages without the level name.
+
+    Source: https://stackoverflow.com/a/62488520
+    """
+
+    def format(self, record):
+        if record.levelno == logging.INFO:
+            self._style._fmt = "%(message)s"
+        else:
+            self._style._fmt = "%(levelname)s: %(message)s"
+        return super().format(record)
+
+
+def setup_logger(
+    logger_name: str,
+    level: int = logging.INFO,
+    *,
+    formatter: Optional[logging.Formatter] = None,
+    screen: bool = False,
+    tofile: bool = False,
+    log_dir: str = "logs",
+    log_name: str = "log",
+) -> None:
     lg = logging.getLogger(logger_name)
-    formatter = logging.Formatter("%(asctime)s.%(msecs)03d - %(levelname)s: %(message)s", datefmt="%y-%m-%d %H:%M:%S")
+    if formatter is None:
+        formatter = logging.Formatter(
+            "%(asctime)s.%(msecs)03d - %(levelname)-8s - %(name)s: %(message)s", datefmt="%y-%m-%d %H:%M:%S"
+        )
     lg.setLevel(level)
     if tofile:
-        log_file = os.path.join(root, phase + "_{}.log".format(get_timestamp()))
+        Path(log_dir).mkdir(exist_ok=True, parents=True)
+        log_file = Path(log_dir) / f"{log_name}_{get_timestamp()}.log"
         fh = logging.FileHandler(log_file, mode="w")
         fh.setFormatter(formatter)
         lg.addHandler(fh)
     if screen:
         sh = logging.StreamHandler()
         sh.setFormatter(formatter)
         lg.addHandler(sh)
```

### Comparing `coqui-tts-0.22.1/TTS/utils/io.py` & `coqui_tts-0.23.0/TTS/utils/io.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/manage.py` & `coqui_tts-0.23.0/TTS/utils/manage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import os
 import re
 import tarfile
 import zipfile
 from pathlib import Path
 from shutil import copyfile, rmtree
 from typing import Dict, Tuple
@@ -10,14 +11,16 @@
 import fsspec
 import requests
 from tqdm import tqdm
 
 from TTS.config import load_config, read_json_with_comments
 from TTS.utils.generic_utils import get_user_data_dir
 
+logger = logging.getLogger(__name__)
+
 LICENSE_URLS = {
     "cc by-nc-nd 4.0": "https://creativecommons.org/licenses/by-nc-nd/4.0/",
     "mpl": "https://www.mozilla.org/en-US/MPL/2.0/",
     "mpl2": "https://www.mozilla.org/en-US/MPL/2.0/",
     "mpl 2.0": "https://www.mozilla.org/en-US/MPL/2.0/",
     "mit": "https://choosealicense.com/licenses/mit/",
     "apache 2.0": "https://choosealicense.com/licenses/apache-2.0/",
@@ -36,21 +39,19 @@
     Models are downloaded under '.TTS' folder in the user's
     home path.
 
     Args:
         models_file (str): path to .model.json file. Defaults to None.
         output_prefix (str): prefix to `tts` to download models. Defaults to None
         progress_bar (bool): print a progress bar when donwloading a file. Defaults to False.
-        verbose (bool): print info. Defaults to True.
     """
 
-    def __init__(self, models_file=None, output_prefix=None, progress_bar=False, verbose=True):
+    def __init__(self, models_file=None, output_prefix=None, progress_bar=False):
         super().__init__()
         self.progress_bar = progress_bar
-        self.verbose = verbose
         if output_prefix is None:
             self.output_prefix = get_user_data_dir("tts")
         else:
             self.output_prefix = os.path.join(output_prefix, "tts")
         self.models_dict = None
         if models_file is not None:
             self.read_models_file(models_file)
@@ -64,27 +65,24 @@
 
         Args:
             file_path (str): path to .models.json.
         """
         self.models_dict = read_json_with_comments(file_path)
 
     def _list_models(self, model_type, model_count=0):
-        if self.verbose:
-            print("\n Name format: type/language/dataset/model")
+        logger.info("")
+        logger.info("Name format: type/language/dataset/model")
         model_list = []
         for lang in self.models_dict[model_type]:
             for dataset in self.models_dict[model_type][lang]:
                 for model in self.models_dict[model_type][lang][dataset]:
                     model_full_name = f"{model_type}--{lang}--{dataset}--{model}"
-                    output_path = os.path.join(self.output_prefix, model_full_name)
-                    if self.verbose:
-                        if os.path.exists(output_path):
-                            print(f" {model_count}: {model_type}/{lang}/{dataset}/{model} [already downloaded]")
-                        else:
-                            print(f" {model_count}: {model_type}/{lang}/{dataset}/{model}")
+                    output_path = Path(self.output_prefix) / model_full_name
+                    downloaded = " [already downloaded]" if output_path.is_dir() else ""
+                    logger.info(" %2d: %s/%s/%s/%s%s", model_count, model_type, lang, dataset, model, downloaded)
                     model_list.append(f"{model_type}/{lang}/{dataset}/{model}")
                     model_count += 1
         return model_list
 
     def _list_for_model_type(self, model_type):
         models_name_list = []
         model_count = 1
@@ -95,88 +93,81 @@
         models_name_list = []
         model_count = 1
         for model_type in self.models_dict:
             model_list = self._list_models(model_type, model_count)
             models_name_list.extend(model_list)
         return models_name_list
 
+    def log_model_details(self, model_type, lang, dataset, model):
+        logger.info("Model type: %s", model_type)
+        logger.info("Language supported: %s", lang)
+        logger.info("Dataset used: %s", dataset)
+        logger.info("Model name: %s", model)
+        if "description" in self.models_dict[model_type][lang][dataset][model]:
+            logger.info("Description: %s", self.models_dict[model_type][lang][dataset][model]["description"])
+        else:
+            logger.info("Description: coming soon")
+        if "default_vocoder" in self.models_dict[model_type][lang][dataset][model]:
+            logger.info(
+                "Default vocoder: %s",
+                self.models_dict[model_type][lang][dataset][model]["default_vocoder"],
+            )
+
     def model_info_by_idx(self, model_query):
-        """Print the description of the model from .models.json file using model_idx
+        """Print the description of the model from .models.json file using model_query_idx
 
         Args:
-            model_query (str): <model_tye>/<model_idx>
+            model_query (str): <model_tye>/<model_query_idx>
         """
         model_name_list = []
         model_type, model_query_idx = model_query.split("/")
         try:
             model_query_idx = int(model_query_idx)
             if model_query_idx <= 0:
-                print("> model_query_idx should be a positive integer!")
+                logger.error("model_query_idx [%d] should be a positive integer!", model_query_idx)
                 return
-        except:
-            print("> model_query_idx should be an integer!")
+        except (TypeError, ValueError):
+            logger.error("model_query_idx [%s] should be an integer!", model_query_idx)
             return
         model_count = 0
         if model_type in self.models_dict:
             for lang in self.models_dict[model_type]:
                 for dataset in self.models_dict[model_type][lang]:
                     for model in self.models_dict[model_type][lang][dataset]:
                         model_name_list.append(f"{model_type}/{lang}/{dataset}/{model}")
                         model_count += 1
         else:
-            print(f"> model_type {model_type} does not exist in the list.")
+            logger.error("Model type %s does not exist in the list.", model_type)
             return
         if model_query_idx > model_count:
-            print(f"model query idx exceeds the number of available models [{model_count}] ")
+            logger.error("model_query_idx exceeds the number of available models [%d]", model_count)
         else:
             model_type, lang, dataset, model = model_name_list[model_query_idx - 1].split("/")
-            print(f"> model type : {model_type}")
-            print(f"> language supported : {lang}")
-            print(f"> dataset used : {dataset}")
-            print(f"> model name : {model}")
-            if "description" in self.models_dict[model_type][lang][dataset][model]:
-                print(f"> description : {self.models_dict[model_type][lang][dataset][model]['description']}")
-            else:
-                print("> description : coming soon")
-            if "default_vocoder" in self.models_dict[model_type][lang][dataset][model]:
-                print(f"> default_vocoder : {self.models_dict[model_type][lang][dataset][model]['default_vocoder']}")
+            self.log_model_details(model_type, lang, dataset, model)
 
     def model_info_by_full_name(self, model_query_name):
         """Print the description of the model from .models.json file using model_full_name
 
         Args:
             model_query_name (str): Format is <model_type>/<language>/<dataset>/<model_name>
         """
         model_type, lang, dataset, model = model_query_name.split("/")
-        if model_type in self.models_dict:
-            if lang in self.models_dict[model_type]:
-                if dataset in self.models_dict[model_type][lang]:
-                    if model in self.models_dict[model_type][lang][dataset]:
-                        print(f"> model type : {model_type}")
-                        print(f"> language supported : {lang}")
-                        print(f"> dataset used : {dataset}")
-                        print(f"> model name : {model}")
-                        if "description" in self.models_dict[model_type][lang][dataset][model]:
-                            print(
-                                f"> description : {self.models_dict[model_type][lang][dataset][model]['description']}"
-                            )
-                        else:
-                            print("> description : coming soon")
-                        if "default_vocoder" in self.models_dict[model_type][lang][dataset][model]:
-                            print(
-                                f"> default_vocoder : {self.models_dict[model_type][lang][dataset][model]['default_vocoder']}"
-                            )
-                    else:
-                        print(f"> model {model} does not exist for {model_type}/{lang}/{dataset}.")
-                else:
-                    print(f"> dataset {dataset} does not exist for {model_type}/{lang}.")
-            else:
-                print(f"> lang {lang} does not exist for {model_type}.")
-        else:
-            print(f"> model_type {model_type} does not exist in the list.")
+        if model_type not in self.models_dict:
+            logger.error("Model type %s does not exist in the list.", model_type)
+            return
+        if lang not in self.models_dict[model_type]:
+            logger.error("Language %s does not exist for %s.", lang, model_type)
+            return
+        if dataset not in self.models_dict[model_type][lang]:
+            logger.error("Dataset %s does not exist for %s/%s.", dataset, model_type, lang)
+            return
+        if model not in self.models_dict[model_type][lang][dataset]:
+            logger.error("Model %s does not exist for %s/%s/%s.", model, model_type, lang, dataset)
+            return
+        self.log_model_details(model_type, lang, dataset, model)
 
     def list_tts_models(self):
         """Print all `TTS` models and return a list of model names
 
         Format is `language/dataset/model`
         """
         return self._list_for_model_type("tts_models")
@@ -193,42 +184,42 @@
 
         Format is `language/dataset/model`
         """
         return self._list_for_model_type("voice_conversion_models")
 
     def list_langs(self):
         """Print all the available languages"""
-        print(" Name format: type/language")
+        logger.info("Name format: type/language")
         for model_type in self.models_dict:
             for lang in self.models_dict[model_type]:
-                print(f" >: {model_type}/{lang} ")
+                logger.info("  %s/%s", model_type, lang)
 
     def list_datasets(self):
         """Print all the datasets"""
-        print(" Name format: type/language/dataset")
+        logger.info("Name format: type/language/dataset")
         for model_type in self.models_dict:
             for lang in self.models_dict[model_type]:
                 for dataset in self.models_dict[model_type][lang]:
-                    print(f" >: {model_type}/{lang}/{dataset}")
+                    logger.info("  %s/%s/%s", model_type, lang, dataset)
 
     @staticmethod
     def print_model_license(model_item: Dict):
         """Print the license of a model
 
         Args:
             model_item (dict): model item in the models.json
         """
         if "license" in model_item and model_item["license"].strip() != "":
-            print(f" > Model's license - {model_item['license']}")
+            logger.info("Model's license - %s", model_item["license"])
             if model_item["license"].lower() in LICENSE_URLS:
-                print(f" > Check {LICENSE_URLS[model_item['license'].lower()]} for more info.")
+                logger.info("Check %s for more info.", LICENSE_URLS[model_item["license"].lower()])
             else:
-                print(" > Check https://opensource.org/licenses for more info.")
+                logger.info("Check https://opensource.org/licenses for more info.")
         else:
-            print(" > Model's license - No license information available")
+            logger.info("Model's license - No license information available")
 
     def _download_github_model(self, model_item: Dict, output_path: str):
         if isinstance(model_item["github_rls_url"], list):
             self._download_model_files(model_item["github_rls_url"], output_path, self.progress_bar)
         else:
             self._download_zip_file(model_item["github_rls_url"], output_path, self.progress_bar)
 
@@ -332,25 +323,25 @@
     def create_dir_and_download_model(self, model_name, model_item, output_path):
         os.makedirs(output_path, exist_ok=True)
         # handle TOS
         if not self.tos_agreed(model_item, output_path):
             if not self.ask_tos(output_path):
                 os.rmdir(output_path)
                 raise Exception(" [!] You must agree to the terms of service to use this model.")
-        print(f" > Downloading model to {output_path}")
+        logger.info("Downloading model to %s", output_path)
         try:
             if "fairseq" in model_name:
                 self.download_fairseq_model(model_name, output_path)
             elif "github_rls_url" in model_item:
                 self._download_github_model(model_item, output_path)
             elif "hf_url" in model_item:
                 self._download_hf_model(model_item, output_path)
 
         except requests.RequestException as e:
-            print(f" > Failed to download the model file to {output_path}")
+            logger.exception("Failed to download the model file to %s", output_path)
             rmtree(output_path)
             raise e
         self.print_model_license(model_item=model_item)
 
     def check_if_configs_are_equal(self, model_name, model_item, output_path):
         with fsspec.open(self._find_files(output_path)[1], "r", encoding="utf-8") as f:
             config_local = json.load(f)
@@ -360,15 +351,15 @@
                 remote_url = url
                 break
 
         with fsspec.open(remote_url, "r", encoding="utf-8") as f:
             config_remote = json.load(f)
 
         if not config_local == config_remote:
-            print(f" > {model_name} is already downloaded however it has been changed. Redownloading it...")
+            logger.info("%s is already downloaded however it has been changed. Redownloading it...", model_name)
             self.create_dir_and_download_model(model_name, model_item, output_path)
 
     def download_model(self, model_name):
         """Download model files given the full model name.
         Model name is in the format
             'type/language/dataset/model'
             e.g. 'tts_model/en/ljspeech/tacotron'
@@ -386,30 +377,30 @@
         output_path = os.path.join(self.output_prefix, model_full_name)
         if os.path.exists(output_path):
             if md5sum is not None:
                 md5sum_file = os.path.join(output_path, "hash.md5")
                 if os.path.isfile(md5sum_file):
                     with open(md5sum_file, mode="r") as f:
                         if not f.read() == md5sum:
-                            print(f" > {model_name} has been updated, clearing model cache...")
+                            logger.info("%s has been updated, clearing model cache...", model_name)
                             self.create_dir_and_download_model(model_name, model_item, output_path)
                         else:
-                            print(f" > {model_name} is already downloaded.")
+                            logger.info("%s is already downloaded.", model_name)
                 else:
-                    print(f" > {model_name} has been updated, clearing model cache...")
+                    logger.info("%s has been updated, clearing model cache...", model_name)
                     self.create_dir_and_download_model(model_name, model_item, output_path)
             # if the configs are different, redownload it
             # ToDo: we need a better way to handle it
             if "xtts" in model_name:
                 try:
                     self.check_if_configs_are_equal(model_name, model_item, output_path)
                 except:
                     pass
             else:
-                print(f" > {model_name} is already downloaded.")
+                logger.info("%s is already downloaded.", model_name)
         else:
             self.create_dir_and_download_model(model_name, model_item, output_path)
 
         # find downloaded files
         output_model_path = output_path
         output_config_path = None
         if (
@@ -540,15 +531,15 @@
                     if progress_bar:
                         ModelManager.tqdm_progress.update(len(data))
                     file.write(data)
             with zipfile.ZipFile(temp_zip_name) as z:
                 z.extractall(output_folder)
             os.remove(temp_zip_name)  # delete zip after extract
         except zipfile.BadZipFile:
-            print(f" > Error: Bad zip file - {file_url}")
+            logger.exception("Bad zip file - %s", file_url)
             raise zipfile.BadZipFile  # pylint: disable=raise-missing-from
         # move the files to the outer path
         for file_path in z.namelist():
             src_path = os.path.join(output_folder, file_path)
             if os.path.isfile(src_path):
                 dst_path = os.path.join(output_folder, os.path.basename(file_path))
                 if src_path != dst_path:
@@ -576,15 +567,15 @@
                         ModelManager.tqdm_progress.update(len(data))
                     file.write(data)
             with tarfile.open(temp_tar_name) as t:
                 t.extractall(output_folder)
                 tar_names = t.getnames()
             os.remove(temp_tar_name)  # delete tar after extract
         except tarfile.ReadError:
-            print(f" > Error: Bad tar file - {file_url}")
+            logger.exception("Bad tar file - %s", file_url)
             raise tarfile.ReadError  # pylint: disable=raise-missing-from
         # move the files to the outer path
         for file_path in os.listdir(os.path.join(output_folder, tar_names[0])):
             src_path = os.path.join(output_folder, tar_names[0], file_path)
             dst_path = os.path.join(output_folder, os.path.basename(file_path))
             if src_path != dst_path:
                 copyfile(src_path, dst_path)
```

### Comparing `coqui-tts-0.22.1/TTS/utils/radam.py` & `coqui_tts-0.23.0/TTS/utils/radam.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/samplers.py` & `coqui_tts-0.23.0/TTS/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/utils/synthesizer.py` & `coqui_tts-0.23.0/TTS/utils/synthesizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import time
 from typing import List
 
 import numpy as np
 import pysbd
 import torch
@@ -17,14 +18,16 @@
 from TTS.tts.utils.synthesis import synthesis, transfer_voice, trim_silence
 from TTS.utils.audio import AudioProcessor
 from TTS.utils.audio.numpy_transforms import save_wav
 from TTS.vc.models import setup_model as setup_vc_model
 from TTS.vocoder.models import setup_model as setup_vocoder_model
 from TTS.vocoder.utils.generic_utils import interpolate_vocoder_input
 
+logger = logging.getLogger(__name__)
+
 
 class Synthesizer(nn.Module):
     def __init__(
         self,
         tts_checkpoint: str = "",
         tts_config_path: str = "",
         tts_speakers_file: str = "",
@@ -214,15 +217,15 @@
 
         Args:
             model_file (str): path to the model checkpoint.
             model_config (str): path to the model config file.
             use_cuda (bool): enable/disable CUDA use.
         """
         self.vocoder_config = load_config(model_config)
-        self.vocoder_ap = AudioProcessor(verbose=False, **self.vocoder_config.audio)
+        self.vocoder_ap = AudioProcessor(**self.vocoder_config.audio)
         self.vocoder_model = setup_vocoder_model(self.vocoder_config)
         self.vocoder_model.load_checkpoint(self.vocoder_config, model_file, eval=True)
         if use_cuda:
             self.vocoder_model.cuda()
 
     def split_into_sentences(self, text) -> List[str]:
         """Split give text into sentences.
@@ -290,17 +293,17 @@
             raise ValueError(
                 "You need to define either `text` (for sythesis) or a `reference_wav` (for voice conversion) to use the Coqui TTS API."
             )
 
         if text:
             sens = [text]
             if split_sentences:
-                print(" > Text splitted to sentences.")
                 sens = self.split_into_sentences(text)
-            print(sens)
+                logger.info("Text split into sentences.")
+            logger.info("Input: %s", sens)
 
         # handle multi-speaker
         if "voice_dir" in kwargs:
             self.voice_dir = kwargs["voice_dir"]
             kwargs.pop("voice_dir")
         speaker_embedding = None
         speaker_id = None
@@ -416,15 +419,15 @@
                     vocoder_input = self.vocoder_ap.normalize(mel_postnet_spec.T)
                     # compute scale factor for possible sample rate mismatch
                     scale_factor = [
                         1,
                         self.vocoder_config["audio"]["sample_rate"] / self.tts_model.ap.sample_rate,
                     ]
                     if scale_factor[1] != 1:
-                        print(" > interpolating tts model output.")
+                        logger.info("Interpolating TTS model output.")
                         vocoder_input = interpolate_vocoder_input(scale_factor, vocoder_input)
                     else:
                         vocoder_input = torch.tensor(vocoder_input).unsqueeze(0)  # pylint: disable=not-callable
                     # run vocoder model
                     # [1, T, C]
                     waveform = self.vocoder_model.inference(vocoder_input.to(vocoder_device))
                 if torch.is_tensor(waveform) and waveform.device != torch.device("cpu") and not use_gl:
@@ -480,15 +483,15 @@
                 vocoder_input = self.vocoder_ap.normalize(mel_postnet_spec.T)
                 # compute scale factor for possible sample rate mismatch
                 scale_factor = [
                     1,
                     self.vocoder_config["audio"]["sample_rate"] / self.tts_model.ap.sample_rate,
                 ]
                 if scale_factor[1] != 1:
-                    print(" > interpolating tts model output.")
+                    logger.info("Interpolating TTS model output.")
                     vocoder_input = interpolate_vocoder_input(scale_factor, vocoder_input)
                 else:
                     vocoder_input = torch.tensor(vocoder_input).unsqueeze(0)  # pylint: disable=not-callable
                 # run vocoder model
                 # [1, T, C]
                 waveform = self.vocoder_model.inference(vocoder_input.to(vocoder_device))
             if torch.is_tensor(waveform) and waveform.device != torch.device("cpu"):
@@ -496,10 +499,10 @@
             if not use_gl:
                 waveform = waveform.numpy()
             wavs = waveform.squeeze()
 
         # compute stats
         process_time = time.time() - start_time
         audio_time = len(wavs) / self.tts_config.audio["sample_rate"]
-        print(f" > Processing time: {process_time}")
-        print(f" > Real-time factor: {process_time / audio_time}")
+        logger.info("Processing time: %.3f", process_time)
+        logger.info("Real-time factor: %.3f", process_time / audio_time)
         return wavs
```

### Comparing `coqui-tts-0.22.1/TTS/utils/training.py` & `coqui_tts-0.23.0/TTS/utils/training.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import logging
+
 import numpy as np
 import torch
 
+logger = logging.getLogger(__name__)
+
 
 def check_update(model, grad_clip, ignore_stopnet=False, amp_opt_params=None):
     r"""Check model gradient against unexpected jumps and failures"""
     skip_flag = False
     if ignore_stopnet:
         if not amp_opt_params:
             grad_norm = torch.nn.utils.clip_grad_norm_(
@@ -17,19 +21,19 @@
             grad_norm = torch.nn.utils.clip_grad_norm_(model.parameters(), grad_clip)
         else:
             grad_norm = torch.nn.utils.clip_grad_norm_(amp_opt_params, grad_clip)
 
     # compatibility with different torch versions
     if isinstance(grad_norm, float):
         if np.isinf(grad_norm):
-            print(" | > Gradient is INF !!")
+            logger.warning("Gradient is INF !!")
             skip_flag = True
     else:
         if torch.isinf(grad_norm):
-            print(" | > Gradient is INF !!")
+            logger.warning("Gradient is INF !!")
             skip_flag = True
     return grad_norm, skip_flag
 
 
 def gradual_training_scheduler(global_step, config):
     """Setup the gradual training schedule wrt number
     of active GPUs"""
```

### Comparing `coqui-tts-0.22.1/TTS/utils/vad.py` & `coqui_tts-0.23.0/TTS/utils/vad.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import logging
+
 import torch
 import torchaudio
 
+logger = logging.getLogger(__name__)
+
 
 def read_audio(path):
     wav, sr = torchaudio.load(path)
 
     if wav.size(0) > 1:
         wav = wav.mean(dim=0, keepdim=True)
 
@@ -50,16 +54,16 @@
 ):
     # get the VAD model and utils functions
     model, get_speech_timestamps, _, collect_chunks = model_and_utils
 
     # read ground truth wav and resample the audio for the VAD
     try:
         wav, gt_sample_rate = read_audio(audio_path)
-    except:
-        print(f"> ❗ Failed to read {audio_path}")
+    except Exception:
+        logger.exception("Failed to read %s", audio_path)
         return None, False
 
     # if needed, resample the audio for the VAD model
     if gt_sample_rate != vad_sample_rate:
         wav_vad = resample_wav(wav, gt_sample_rate, vad_sample_rate)
     else:
         wav_vad = wav
@@ -76,13 +80,13 @@
     )
 
     # if have speech timestamps else save the wav
     if new_speech_timestamps:
         wav = collect_chunks(new_speech_timestamps, wav)
         is_speech = True
     else:
-        print(f"> The file {audio_path} probably does not have speech please check it !!")
+        logger.warning("The file %s probably does not have speech please check it!", audio_path)
         is_speech = False
 
     # save
     torchaudio.save(out_path, wav[None, :], gt_sample_rate)
     return out_path, is_speech
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `coqui-tts-0.22.1/TTS/vc/configs/freevc_config.py` & `coqui_tts-0.23.0/TTS/vc/configs/freevc_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/configs/shared_configs.py` & `coqui_tts-0.23.0/TTS/vc/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/models/__init__.py` & `coqui_tts-0.23.0/TTS/vc/models/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import importlib
+import logging
 import re
 from typing import Dict, List, Union
 
+logger = logging.getLogger(__name__)
+
 
 def to_camel(text):
     text = text.capitalize()
     return re.sub(r"(?!^)_([a-zA-Z])", lambda m: m.group(1).upper(), text)
 
 
 def setup_model(config: "Coqpit", samples: Union[List[List], List[Dict]] = None) -> "BaseVC":
-    print(" > Using model: {}".format(config.model))
+    logger.info("Using model: %s", config.model)
     # fetch the right model implementation.
     if "model" in config and config["model"].lower() == "freevc":
         MyModel = importlib.import_module("TTS.vc.models.freevc").FreeVC
         model = MyModel.init_from_config(config, samples)
     return model
```

### Comparing `coqui-tts-0.22.1/TTS/vc/models/base_vc.py` & `coqui_tts-0.23.0/TTS/vc/models/base_vc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 import random
 from typing import Dict, List, Tuple, Union
 
 import torch
 import torch.distributed as dist
 from coqpit import Coqpit
@@ -16,14 +17,16 @@
 from TTS.tts.utils.languages import LanguageManager, get_language_balancer_weights
 from TTS.tts.utils.speakers import SpeakerManager, get_speaker_balancer_weights
 from TTS.tts.utils.synthesis import synthesis
 from TTS.tts.utils.visual import plot_alignment, plot_spectrogram
 
 # pylint: skip-file
 
+logger = logging.getLogger(__name__)
+
 
 class BaseVC(BaseTrainerModel):
     """Base `vc` class. Every new `vc` model must inherit this.
 
     It defines common `vc` specific functions on top of `Model` implementation.
     """
 
@@ -89,15 +92,15 @@
         # set ultimate speaker embedding size
         if config.use_speaker_embedding or config.use_d_vector_file:
             self.embedded_speaker_dim = (
                 config.d_vector_dim if "d_vector_dim" in config and config.d_vector_dim is not None else 512
             )
         # init speaker embedding layer
         if config.use_speaker_embedding and not config.use_d_vector_file:
-            print(" > Init speaker_embedding layer.")
+            logger.info("Init speaker_embedding layer.")
             self.speaker_embedding = nn.Embedding(self.num_speakers, self.embedded_speaker_dim)
             self.speaker_embedding.weight.data.normal_(0, 0.3)
 
     def get_aux_input(self, **kwargs) -> Dict:
         """Prepare and return `aux_input` used by `forward()`"""
         return {"speaker_id": None, "style_wav": None, "d_vector": None, "language_id": None}
 
@@ -229,28 +232,28 @@
 
     def get_sampler(self, config: Coqpit, dataset: TTSDataset, num_gpus=1):
         weights = None
         data_items = dataset.samples
 
         if getattr(config, "use_language_weighted_sampler", False):
             alpha = getattr(config, "language_weighted_sampler_alpha", 1.0)
-            print(" > Using Language weighted sampler with alpha:", alpha)
+            logger.info("Using Language weighted sampler with alpha: %.2f", alpha)
             weights = get_language_balancer_weights(data_items) * alpha
 
         if getattr(config, "use_speaker_weighted_sampler", False):
             alpha = getattr(config, "speaker_weighted_sampler_alpha", 1.0)
-            print(" > Using Speaker weighted sampler with alpha:", alpha)
+            logger.info("Using Speaker weighted sampler with alpha: %.2f", alpha)
             if weights is not None:
                 weights += get_speaker_balancer_weights(data_items) * alpha
             else:
                 weights = get_speaker_balancer_weights(data_items) * alpha
 
         if getattr(config, "use_length_weighted_sampler", False):
             alpha = getattr(config, "length_weighted_sampler_alpha", 1.0)
-            print(" > Using Length weighted sampler with alpha:", alpha)
+            logger.info("Using Length weighted sampler with alpha: %.2f", alpha)
             if weights is not None:
                 weights += get_length_balancer_weights(data_items) * alpha
             else:
                 weights = get_length_balancer_weights(data_items) * alpha
 
         if weights is not None:
             sampler = WeightedRandomSampler(weights, len(weights))
@@ -314,15 +317,14 @@
                 min_text_len=config.min_text_len,
                 max_text_len=config.max_text_len,
                 min_audio_len=config.min_audio_len,
                 max_audio_len=config.max_audio_len,
                 phoneme_cache_path=config.phoneme_cache_path,
                 precompute_num_workers=config.precompute_num_workers,
                 use_noise_augment=False if is_eval else config.use_noise_augment,
-                verbose=verbose,
                 speaker_id_mapping=speaker_id_mapping,
                 d_vector_mapping=d_vector_mapping if config.use_d_vector_file else None,
                 tokenizer=None,
                 start_by_longest=config.start_by_longest,
                 language_id_mapping=language_id_mapping,
             )
 
@@ -374,15 +376,15 @@
 
         Args:
             assets (dict): A dict of training assets. For `vc` models, it must include `{'audio_processor': ap}`.
 
         Returns:
             Tuple[Dict, Dict]: Test figures and audios to be projected to Tensorboard.
         """
-        print(" | > Synthesizing test sentences.")
+        logger.info("Synthesizing test sentences.")
         test_audios = {}
         test_figures = {}
         test_sentences = self.config.test_sentences
         aux_inputs = self._get_test_aux_input()
         for idx, sen in enumerate(test_sentences):
             if isinstance(sen, list):
                 aux_inputs = self.get_aux_input_from_test_sentences(sen)
@@ -413,19 +415,19 @@
             output_path = os.path.join(trainer.output_path, "speakers.pth")
             self.speaker_manager.save_ids_to_file(output_path)
             trainer.config.speakers_file = output_path
             # some models don't have `model_args` set
             if hasattr(trainer.config, "model_args"):
                 trainer.config.model_args.speakers_file = output_path
             trainer.config.save_json(os.path.join(trainer.output_path, "config.json"))
-            print(f" > `speakers.pth` is saved to {output_path}.")
-            print(" > `speakers_file` is updated in the config.json.")
+            logger.info("`speakers.pth` is saved to %s", output_path)
+            logger.info("`speakers_file` is updated in the config.json.")
 
         if self.language_manager is not None:
             output_path = os.path.join(trainer.output_path, "language_ids.json")
             self.language_manager.save_ids_to_file(output_path)
             trainer.config.language_ids_file = output_path
             if hasattr(trainer.config, "model_args"):
                 trainer.config.model_args.language_ids_file = output_path
             trainer.config.save_json(os.path.join(trainer.output_path, "config.json"))
-            print(f" > `language_ids.json` is saved to {output_path}.")
-            print(" > `language_ids_file` is updated in the config.json.")
+            logger.info("`language_ids.json` is saved to %s", output_path)
+            logger.info("`language_ids_file` is updated in the config.json.")
```

### Comparing `coqui-tts-0.22.1/TTS/vc/models/freevc.py` & `coqui_tts-0.23.0/TTS/vc/models/freevc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Dict, List, Optional, Tuple, Union
 
 import librosa
 import numpy as np
 import torch
 from coqpit import Coqpit
 from torch import nn
@@ -18,14 +19,16 @@
 from TTS.vc.configs.freevc_config import FreeVCConfig
 from TTS.vc.models.base_vc import BaseVC
 from TTS.vc.modules.freevc.commons import get_padding, init_weights
 from TTS.vc.modules.freevc.mel_processing import mel_spectrogram_torch
 from TTS.vc.modules.freevc.speaker_encoder.speaker_encoder import SpeakerEncoder as SpeakerEncoderEx
 from TTS.vc.modules.freevc.wavlm import get_wavlm
 
+logger = logging.getLogger(__name__)
+
 
 class ResidualCouplingBlock(nn.Module):
     def __init__(self, channels, hidden_channels, kernel_size, dilation_rate, n_layers, n_flows=4, gin_channels=0):
         super().__init__()
         self.channels = channels
         self.hidden_channels = hidden_channels
         self.kernel_size = kernel_size
@@ -148,15 +151,15 @@
         x = F.leaky_relu(x)
         x = self.conv_post(x)
         x = torch.tanh(x)
 
         return x
 
     def remove_weight_norm(self):
-        print("Removing weight norm...")
+        logger.info("Removing weight norm...")
         for l in self.ups:
             remove_parametrizations(l, "weight")
         for l in self.resblocks:
             remove_parametrizations(l, "weight")
 
 
 class DiscriminatorP(torch.nn.Module):
@@ -373,15 +376,15 @@
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     def load_pretrained_speaker_encoder(self):
         """Load pretrained speaker encoder model as mentioned in the paper."""
-        print(" > Loading pretrained speaker encoder model ...")
+        logger.info("Loading pretrained speaker encoder model ...")
         self.enc_spk_ex = SpeakerEncoderEx(
             "https://github.com/coqui-ai/TTS/releases/download/v0.13.0_models/speaker_encoder.pt"
         )
 
     def init_multispeaker(self, config: Coqpit):
         """Initialize multi-speaker modules of a model. A model can be trained either with a speaker embedding layer
         or with external `d_vectors` computed from a speaker encoder model.
@@ -543,15 +546,15 @@
             audio = self.inference(c, mel=mel_tgt.transpose(1, 2))
         audio = audio[0][0].data.cpu().float().numpy()
         return audio
 
     def eval_step(): ...
 
     @staticmethod
-    def init_from_config(config: FreeVCConfig, samples: Union[List[List], List[Dict]] = None, verbose=True):
+    def init_from_config(config: FreeVCConfig, samples: Union[List[List], List[Dict]] = None):
         model = FreeVC(config)
         return model
 
     def load_checkpoint(self, config, checkpoint_path, eval=False, strict=True, cache=False):
         state = load_fsspec(checkpoint_path, map_location=torch.device("cpu"), cache=cache)
         self.load_state_dict(state["model"], strict=strict)
         if eval:
```

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/commons.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/commons.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/mel_processing.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/mel_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import logging
+
 import torch
 import torch.utils.data
 from librosa.filters import mel as librosa_mel_fn
 
+logger = logging.getLogger(__name__)
+
 MAX_WAV_VALUE = 32768.0
 
 
 def dynamic_range_compression_torch(x, C=1, clip_val=1e-5):
     """
     PARAMS
     ------
@@ -35,17 +39,17 @@
 
 mel_basis = {}
 hann_window = {}
 
 
 def spectrogram_torch(y, n_fft, sampling_rate, hop_size, win_size, center=False):
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("Min value is: %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("Max value is: %.3f", torch.max(y))
 
     global hann_window
     dtype_device = str(y.dtype) + "_" + str(y.device)
     wnsize_dtype_device = str(win_size) + "_" + dtype_device
     if wnsize_dtype_device not in hann_window:
         hann_window[wnsize_dtype_device] = torch.hann_window(win_size).to(dtype=y.dtype, device=y.device)
 
@@ -83,17 +87,17 @@
     spec = torch.matmul(mel_basis[fmax_dtype_device], spec)
     spec = spectral_normalize_torch(spec)
     return spec
 
 
 def mel_spectrogram_torch(y, n_fft, num_mels, sampling_rate, hop_size, win_size, fmin, fmax, center=False):
     if torch.min(y) < -1.0:
-        print("min value is ", torch.min(y))
+        logger.info("Min value is: %.3f", torch.min(y))
     if torch.max(y) > 1.0:
-        print("max value is ", torch.max(y))
+        logger.info("Max value is: %.3f", torch.max(y))
 
     global mel_basis, hann_window
     dtype_device = str(y.dtype) + "_" + str(y.device)
     fmax_dtype_device = str(fmax) + "_" + dtype_device
     wnsize_dtype_device = str(win_size) + "_" + dtype_device
     if fmax_dtype_device not in mel_basis:
         mel = librosa_mel_fn(sr=sampling_rate, n_fft=n_fft, n_mels=num_mels, fmin=fmin, fmax=fmax)
```

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/modules.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/modules.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/audio.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/audio.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/hparams.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/hparams.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/speaker_encoder/speaker_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from time import perf_counter as timer
 from typing import List, Union
 
 import numpy as np
 import torch
 from torch import nn
 
@@ -13,17 +14,19 @@
     model_embedding_size,
     model_hidden_size,
     model_num_layers,
     partials_n_frames,
     sampling_rate,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class SpeakerEncoder(nn.Module):
-    def __init__(self, weights_fpath, device: Union[str, torch.device] = None, verbose=True):
+    def __init__(self, weights_fpath, device: Union[str, torch.device] = None):
         """
         :param device: either a torch device or the name of a torch device (e.g. "cpu", "cuda").
         If None, defaults to cuda if it is available on your machine, otherwise the model will
         run on cpu. Outputs are always returned on the cpu, as numpy arrays.
         """
         super().__init__()
 
@@ -46,17 +49,15 @@
         #                     weights_fpath)
 
         start = timer()
         checkpoint = load_fsspec(weights_fpath, map_location="cpu")
 
         self.load_state_dict(checkpoint["model_state"], strict=False)
         self.to(device)
-
-        if verbose:
-            print("Loaded the voice encoder model on %s in %.2f seconds." % (device.type, timer() - start))
+        logger.info("Loaded the voice encoder model on %s in %.2f seconds.", device.type, timer() - start)
 
     def forward(self, mels: torch.FloatTensor):
         """
         Computes the embeddings of a batch of utterance spectrograms.
         :param mels: a batch of mel spectrograms of same duration as a float32 tensor of shape
         (batch_size, n_frames, n_channels)
         :return: the embeddings as a float 32 tensor of shape (batch_size, embedding_size).
```

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/config.json` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/config.json`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/modules.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/modules.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vc/modules/freevc/wavlm/wavlm.py` & `coqui_tts-0.23.0/TTS/vc/modules/freevc/wavlm/wavlm.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/README.md` & `coqui_tts-0.23.0/TTS/vocoder/README.md`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/__init__.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/fullband_melgan_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/fullband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/hifigan_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/hifigan_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/melgan_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/multiband_melgan_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/multiband_melgan_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/parallel_wavegan_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/parallel_wavegan_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/shared_configs.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/shared_configs.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/univnet_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/univnet_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/wavegrad_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/wavegrad_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/configs/wavernn_config.py` & `coqui_tts-0.23.0/TTS/vocoder/configs/wavernn_config.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/datasets/__init__.py` & `coqui_tts-0.23.0/TTS/vocoder/datasets/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,53 +6,50 @@
 from TTS.utils.audio import AudioProcessor
 from TTS.vocoder.datasets.gan_dataset import GANDataset
 from TTS.vocoder.datasets.preprocess import load_wav_data, load_wav_feat_data
 from TTS.vocoder.datasets.wavegrad_dataset import WaveGradDataset
 from TTS.vocoder.datasets.wavernn_dataset import WaveRNNDataset
 
 
-def setup_dataset(config: Coqpit, ap: AudioProcessor, is_eval: bool, data_items: List, verbose: bool) -> Dataset:
+def setup_dataset(config: Coqpit, ap: AudioProcessor, is_eval: bool, data_items: List) -> Dataset:
     if config.model.lower() in "gan":
         dataset = GANDataset(
             ap=ap,
             items=data_items,
             seq_len=config.seq_len,
             hop_len=ap.hop_length,
             pad_short=config.pad_short,
             conv_pad=config.conv_pad,
             return_pairs=config.diff_samples_for_G_and_D if "diff_samples_for_G_and_D" in config else False,
             is_training=not is_eval,
             return_segments=not is_eval,
             use_noise_augment=config.use_noise_augment,
             use_cache=config.use_cache,
-            verbose=verbose,
         )
         dataset.shuffle_mapping()
     elif config.model.lower() == "wavegrad":
         dataset = WaveGradDataset(
             ap=ap,
             items=data_items,
             seq_len=config.seq_len,
             hop_len=ap.hop_length,
             pad_short=config.pad_short,
             conv_pad=config.conv_pad,
             is_training=not is_eval,
             return_segments=True,
             use_noise_augment=False,
             use_cache=config.use_cache,
-            verbose=verbose,
         )
     elif config.model.lower() == "wavernn":
         dataset = WaveRNNDataset(
             ap=ap,
             items=data_items,
             seq_len=config.seq_len,
             hop_len=ap.hop_length,
             pad=config.model_params.pad,
             mode=config.model_params.mode,
             mulaw=config.model_params.mulaw,
             is_training=not is_eval,
-            verbose=verbose,
         )
     else:
         raise ValueError(f" [!] Dataset for model {config.model.lower()} cannot be found.")
     return dataset
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/datasets/gan_dataset.py` & `coqui_tts-0.23.0/TTS/vocoder/datasets/gan_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,28 @@
         pad_short,
         conv_pad=2,
         return_pairs=False,
         is_training=True,
         return_segments=True,
         use_noise_augment=False,
         use_cache=False,
-        verbose=False,
     ):
         super().__init__()
         self.ap = ap
         self.item_list = items
         self.compute_feat = not isinstance(items[0], (tuple, list))
         self.seq_len = seq_len
         self.hop_len = hop_len
         self.pad_short = pad_short
         self.conv_pad = conv_pad
         self.return_pairs = return_pairs
         self.is_training = is_training
         self.return_segments = return_segments
         self.use_cache = use_cache
         self.use_noise_augment = use_noise_augment
-        self.verbose = verbose
 
         assert seq_len % hop_len == 0, " [!] seq_len has to be a multiple of hop_len."
         self.feat_frame_len = seq_len // hop_len + (2 * conv_pad)
 
         # map G and D instances
         self.G_to_D_mappings = list(range(len(self.item_list)))
         self.shuffle_mapping()
@@ -105,15 +103,14 @@
         random.shuffle(self.G_to_D_mappings)
 
     def load_item(self, idx):
         """load (audio, feat) couple"""
         if self.compute_feat:
             # compute features from wav
             wavpath = self.item_list[idx]
-            # print(wavpath)
 
             if self.use_cache and self.cache[idx] is not None:
                 audio, mel = self.cache[idx]
             else:
                 audio = self.ap.load_wav(wavpath)
                 mel = self.ap.melspectrogram(audio)
                 audio, mel = self._pad_short_samples(audio, mel)
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/datasets/preprocess.py` & `coqui_tts-0.23.0/TTS/vocoder/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/datasets/wavegrad_dataset.py` & `coqui_tts-0.23.0/TTS/vocoder/datasets/wavegrad_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,26 @@
         hop_len,
         pad_short,
         conv_pad=2,
         is_training=True,
         return_segments=True,
         use_noise_augment=False,
         use_cache=False,
-        verbose=False,
     ):
         super().__init__()
         self.ap = ap
         self.item_list = items
         self.seq_len = seq_len if return_segments else None
         self.hop_len = hop_len
         self.pad_short = pad_short
         self.conv_pad = conv_pad
         self.is_training = is_training
         self.return_segments = return_segments
         self.use_cache = use_cache
         self.use_noise_augment = use_noise_augment
-        self.verbose = verbose
 
         if return_segments:
             assert seq_len % hop_len == 0, " [!] seq_len has to be a multiple of hop_len."
         self.feat_frame_len = seq_len // hop_len + (2 * conv_pad)
 
         # cache acoustic features
         if use_cache:
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/datasets/wavernn_dataset.py` & `coqui_tts-0.23.0/TTS/vocoder/datasets/wavernn_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+import logging
+
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 
 from TTS.utils.audio.numpy_transforms import mulaw_encode, quantize
 
+logger = logging.getLogger(__name__)
+
 
 class WaveRNNDataset(Dataset):
     """
     WaveRNN Dataset searchs for all the wav files under root path
     and converts them to acoustic features on the fly.
     """
 
-    def __init__(
-        self, ap, items, seq_len, hop_len, pad, mode, mulaw, is_training=True, verbose=False, return_segments=True
-    ):
+    def __init__(self, ap, items, seq_len, hop_len, pad, mode, mulaw, is_training=True, return_segments=True):
         super().__init__()
         self.ap = ap
         self.compute_feat = not isinstance(items[0], (tuple, list))
         self.item_list = items
         self.seq_len = seq_len
         self.hop_len = hop_len
         self.mel_len = seq_len // hop_len
         self.pad = pad
         self.mode = mode
         self.mulaw = mulaw
         self.is_training = is_training
-        self.verbose = verbose
         self.return_segments = return_segments
 
         assert self.seq_len % self.hop_len == 0
 
     def __len__(self):
         return len(self.item_list)
 
@@ -56,15 +57,15 @@
             wavpath = self.item_list[index]
             audio = self.ap.load_wav(wavpath)
             if self.return_segments:
                 min_audio_len = 2 * self.seq_len + (2 * self.pad * self.hop_len)
             else:
                 min_audio_len = audio.shape[0] + (2 * self.pad * self.hop_len)
             if audio.shape[0] < min_audio_len:
-                print(" [!] Instance is too short! : {}".format(wavpath))
+                logger.warning("Instance is too short: %s", wavpath)
                 audio = np.pad(audio, [0, min_audio_len - audio.shape[0] + self.hop_len])
             mel = self.ap.melspectrogram(audio)
 
             if self.mode in ["gauss", "mold"]:
                 x_input = audio
             elif isinstance(self.mode, int):
                 x_input = (
@@ -76,15 +77,15 @@
                 raise RuntimeError("Unknown dataset mode - ", self.mode)
 
         else:
             wavpath, feat_path = self.item_list[index]
             mel = np.load(feat_path.replace("/quant/", "/mel/"))
 
             if mel.shape[-1] < self.mel_len + 2 * self.pad:
-                print(" [!] Instance is too short! : {}".format(wavpath))
+                logger.warning("Instance is too short: %s", wavpath)
                 self.item_list[index] = self.item_list[index + 1]
                 feat_path = self.item_list[index]
                 mel = np.load(feat_path.replace("/quant/", "/mel/"))
             if self.mode in ["gauss", "mold"]:
                 x_input = self.ap.load_wav(wavpath)
             elif isinstance(self.mode, int):
                 x_input = np.load(feat_path.replace("/mel/", "/quant/"))
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/hifigan.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/hifigan.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/losses.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/losses.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/lvc_block.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/lvc_block.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/melgan.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/melgan.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/parallel_wavegan.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/parallel_wavegan.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/pqmf.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/pqmf.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/upsample.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/layers/wavegrad.py` & `coqui_tts-0.23.0/TTS/vocoder/layers/wavegrad.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/__init__.py` & `coqui_tts-0.23.0/TTS/vocoder/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import importlib
+import logging
 import re
 
 from coqpit import Coqpit
 
+logger = logging.getLogger(__name__)
+
 
 def to_camel(text):
     text = text.capitalize()
     return re.sub(r"(?!^)_([a-zA-Z])", lambda m: m.group(1).upper(), text)
 
 
 def setup_model(config: Coqpit):
@@ -23,21 +26,21 @@
         elif config.model.lower() == "wavegrad":
             MyModel = getattr(MyModel, "Wavegrad")
         else:
             try:
                 MyModel = getattr(MyModel, to_camel(config.model))
             except ModuleNotFoundError as e:
                 raise ValueError(f"Model {config.model} not exist!") from e
-    print(" > Vocoder Model: {}".format(config.model))
+    logger.info("Vocoder model: %s", config.model)
     return MyModel.init_from_config(config)
 
 
 def setup_generator(c):
     """TODO: use config object as arguments"""
-    print(" > Generator Model: {}".format(c.generator_model))
+    logger.info("Generator model: %s", c.generator_model)
     MyModel = importlib.import_module("TTS.vocoder.models." + c.generator_model.lower())
     MyModel = getattr(MyModel, to_camel(c.generator_model))
     # this is to preserve the Wavernn class name (instead of Wavernn)
     if c.generator_model.lower() in "hifigan_generator":
         model = MyModel(in_channels=c.audio["num_mels"], out_channels=1, **c.generator_model_params)
     elif c.generator_model.lower() in "melgan_generator":
         model = MyModel(
@@ -92,15 +95,15 @@
     else:
         raise NotImplementedError(f"Model {c.generator_model} not implemented!")
     return model
 
 
 def setup_discriminator(c):
     """TODO: use config objekt as arguments"""
-    print(" > Discriminator Model: {}".format(c.discriminator_model))
+    logger.info("Discriminator model: %s", c.discriminator_model)
     if "parallel_wavegan" in c.discriminator_model:
         MyModel = importlib.import_module("TTS.vocoder.models.parallel_wavegan_discriminator")
     else:
         MyModel = importlib.import_module("TTS.vocoder.models." + c.discriminator_model.lower())
     MyModel = getattr(MyModel, to_camel(c.discriminator_model.lower()))
     if c.discriminator_model in "hifigan_discriminator":
         model = MyModel()
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/base_vocoder.py` & `coqui_tts-0.23.0/TTS/vocoder/models/base_vocoder.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/fullband_melgan_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/fullband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/gan.py` & `coqui_tts-0.23.0/TTS/vocoder/models/gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,15 +345,14 @@
             pad_short=config.pad_short,
             conv_pad=config.conv_pad,
             return_pairs=config.diff_samples_for_G_and_D if "diff_samples_for_G_and_D" in config else False,
             is_training=not is_eval,
             return_segments=not is_eval,
             use_noise_augment=config.use_noise_augment,
             use_cache=config.use_cache,
-            verbose=verbose,
         )
         dataset.shuffle_mapping()
         sampler = DistributedSampler(dataset, shuffle=True) if num_gpus > 1 else None
         loader = DataLoader(
             dataset,
             batch_size=1 if is_eval else config.batch_size,
             shuffle=num_gpus == 0,
@@ -365,10 +364,10 @@
         return loader
 
     def get_criterion(self):
         """Return criterions for the optimizers"""
         return [DiscriminatorLoss(self.config), GeneratorLoss(self.config)]
 
     @staticmethod
-    def init_from_config(config: Coqpit, verbose=True) -> "GAN":
-        ap = AudioProcessor.init_from_config(config, verbose=verbose)
+    def init_from_config(config: Coqpit) -> "GAN":
+        ap = AudioProcessor.init_from_config(config)
         return GAN(config, ap=ap)
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/hifigan_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/hifigan_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/hifigan_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/hifigan_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # adopted from https://github.com/jik876/hifi-gan/blob/master/models.py
+import logging
+
 import torch
 from torch import nn
 from torch.nn import Conv1d, ConvTranspose1d
 from torch.nn import functional as F
 from torch.nn.utils.parametrizations import weight_norm
 from torch.nn.utils.parametrize import remove_parametrizations
 
 from TTS.utils.io import load_fsspec
 
+logger = logging.getLogger(__name__)
+
 LRELU_SLOPE = 0.1
 
 
 def get_padding(k, d):
     return int((k * d - d) / 2)
 
 
@@ -278,15 +282,15 @@
             Tensor: [B, 1, T]
         """
         c = c.to(self.conv_pre.weight.device)
         c = torch.nn.functional.pad(c, (self.inference_padding, self.inference_padding), "replicate")
         return self.forward(c)
 
     def remove_weight_norm(self):
-        print("Removing weight norm...")
+        logger.info("Removing weight norm...")
         for l in self.ups:
             remove_parametrizations(l, "weight")
         for l in self.resblocks:
             l.remove_weight_norm()
         remove_parametrizations(self.conv_pre, "weight")
         remove_parametrizations(self.conv_post, "weight")
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/melgan_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/melgan_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/melgan_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/melgan_multiscale_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/melgan_multiscale_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/multiband_melgan_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/multiband_melgan_generator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/parallel_wavegan_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_discriminator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
 import math
 
 import torch
 from torch import nn
 from torch.nn.utils.parametrize import remove_parametrizations
 
 from TTS.vocoder.layers.parallel_wavegan import ResidualBlock
 
+logger = logging.getLogger(__name__)
+
 
 class ParallelWaveganDiscriminator(nn.Module):
     """PWGAN discriminator as in https://arxiv.org/abs/1910.11480.
     It classifies each audio window real/fake and returns a sequence
     of predictions.
         It is a stack of convolutional blocks with dilation.
     """
@@ -72,15 +75,15 @@
                 torch.nn.utils.parametrizations.weight_norm(m)
 
         self.apply(_apply_weight_norm)
 
     def remove_weight_norm(self):
         def _remove_weight_norm(m):
             try:
-                # print(f"Weight norm is removed from {m}.")
+                logger.info("Weight norm is removed from %s", m)
                 remove_parametrizations(m, "weight")
             except ValueError:  # this module didn't have weight norm
                 return
 
         self.apply(_remove_weight_norm)
 
 
@@ -175,13 +178,13 @@
                 torch.nn.utils.parametrizations.weight_norm(m)
 
         self.apply(_apply_weight_norm)
 
     def remove_weight_norm(self):
         def _remove_weight_norm(m):
             try:
-                print(f"Weight norm is removed from {m}.")
+                logger.info("Weight norm is removed from %s", m)
                 remove_parametrizations(m, "weight")
             except ValueError:  # this module didn't have weight norm
                 return
 
         self.apply(_remove_weight_norm)
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/parallel_wavegan_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/parallel_wavegan_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import logging
 import math
 
 import numpy as np
 import torch
 from torch.nn.utils.parametrize import remove_parametrizations
 
 from TTS.utils.io import load_fsspec
 from TTS.vocoder.layers.parallel_wavegan import ResidualBlock
 from TTS.vocoder.layers.upsample import ConvUpsample
 
+logger = logging.getLogger(__name__)
+
 
 class ParallelWaveganGenerator(torch.nn.Module):
     """PWGAN generator as in https://arxiv.org/pdf/1910.11480.pdf.
     It is similar to WaveNet with no causal convolution.
         It is conditioned on an aux feature (spectrogram) to generate
     an output waveform from an input noise.
     """
@@ -122,26 +125,26 @@
         c = c.to(self.first_conv.weight.device)
         c = torch.nn.functional.pad(c, (self.inference_padding, self.inference_padding), "replicate")
         return self.forward(c)
 
     def remove_weight_norm(self):
         def _remove_weight_norm(m):
             try:
-                # print(f"Weight norm is removed from {m}.")
+                logger.info("Weight norm is removed from %s", m)
                 remove_parametrizations(m, "weight")
             except ValueError:  # this module didn't have weight norm
                 return
 
         self.apply(_remove_weight_norm)
 
     def apply_weight_norm(self):
         def _apply_weight_norm(m):
             if isinstance(m, (torch.nn.Conv1d, torch.nn.Conv2d)):
                 torch.nn.utils.parametrizations.weight_norm(m)
-                # print(f"Weight norm is applied to {m}.")
+                logger.info("Weight norm is applied to %s", m)
 
         self.apply(_apply_weight_norm)
 
     @staticmethod
     def _get_receptive_field_size(layers, stacks, kernel_size, dilation=lambda x: 2**x):
         assert layers % stacks == 0
         layers_per_cycle = layers // stacks
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/random_window_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/random_window_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/univnet_discriminator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/univnet_discriminator.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/univnet_generator.py` & `coqui_tts-0.23.0/TTS/vocoder/models/univnet_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import logging
 from typing import List
 
 import numpy as np
 import torch
 import torch.nn.functional as F
 from torch.nn.utils import parametrize
 
 from TTS.vocoder.layers.lvc_block import LVCBlock
 
+logger = logging.getLogger(__name__)
+
 LRELU_SLOPE = 0.1
 
 
 class UnivnetGenerator(torch.nn.Module):
     def __init__(
         self,
         in_channels: int,
@@ -109,28 +112,28 @@
         return x
 
     def remove_weight_norm(self):
         """Remove weight normalization module from all of the layers."""
 
         def _remove_weight_norm(m):
             try:
-                # print(f"Weight norm is removed from {m}.")
+                logger.info("Weight norm is removed from %s", m)
                 parametrize.remove_parametrizations(m, "weight")
             except ValueError:  # this module didn't have weight norm
                 return
 
         self.apply(_remove_weight_norm)
 
     def apply_weight_norm(self):
         """Apply weight normalization module from all of the layers."""
 
         def _apply_weight_norm(m):
             if isinstance(m, (torch.nn.Conv1d, torch.nn.Conv2d)):
                 torch.nn.utils.parametrizations.weight_norm(m)
-                # print(f"Weight norm is applied to {m}.")
+                logger.info("Weight norm is applied to %s", m)
 
         self.apply(_apply_weight_norm)
 
     @staticmethod
     def _get_receptive_field_size(layers, stacks, kernel_size, dilation=lambda x: 2**x):
         assert layers % stacks == 0
         layers_per_cycle = layers // stacks
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/wavegrad.py` & `coqui_tts-0.23.0/TTS/vocoder/models/wavegrad.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,14 @@
             hop_len=ap.hop_length,
             pad_short=self.config.pad_short,
             conv_pad=self.config.conv_pad,
             is_training=not is_eval,
             return_segments=True,
             use_noise_augment=False,
             use_cache=config.use_cache,
-            verbose=verbose,
         )
         sampler = DistributedSampler(dataset) if num_gpus > 1 else None
         loader = DataLoader(
             dataset,
             batch_size=self.config.batch_size,
             shuffle=num_gpus <= 1,
             drop_last=False,
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/models/wavernn.py` & `coqui_tts-0.23.0/TTS/vocoder/models/wavernn.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,14 @@
             items=samples,
             seq_len=config.seq_len,
             hop_len=ap.hop_length,
             pad=config.model_args.pad,
             mode=config.model_args.mode,
             mulaw=config.model_args.mulaw,
             is_training=not is_eval,
-            verbose=verbose,
         )
         sampler = DistributedSampler(dataset, shuffle=True) if num_gpus > 1 else None
         loader = DataLoader(
             dataset,
             batch_size=1 if is_eval else config.batch_size,
             shuffle=num_gpus == 0,
             collate_fn=dataset.collate,
```

### Comparing `coqui-tts-0.22.1/TTS/vocoder/utils/distribution.py` & `coqui_tts-0.23.0/TTS/vocoder/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/TTS/vocoder/utils/generic_utils.py` & `coqui_tts-0.23.0/TTS/vocoder/utils/generic_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+import logging
 from typing import Dict
 
 import numpy as np
 import torch
 from matplotlib import pyplot as plt
 
 from TTS.tts.utils.visual import plot_spectrogram
 from TTS.utils.audio import AudioProcessor
 
+logger = logging.getLogger(__name__)
+
 
 def interpolate_vocoder_input(scale_factor, spec):
     """Interpolate spectrogram by the scale factor.
     It is mainly used to match the sampling rates of
     the tts and vocoder models.
 
     Args:
         scale_factor (float): scale factor to interpolate the spectrogram
         spec (np.array): spectrogram to be interpolated
 
     Returns:
         torch.tensor: interpolated spectrogram.
     """
-    print(" > before interpolation :", spec.shape)
+    logger.info("Before interpolation: %s", spec.shape)
     spec = torch.tensor(spec).unsqueeze(0).unsqueeze(0)  # pylint: disable=not-callable
     spec = torch.nn.functional.interpolate(
         spec, scale_factor=scale_factor, recompute_scale_factor=True, mode="bilinear", align_corners=False
     ).squeeze(0)
-    print(" > after interpolation :", spec.shape)
+    logger.info("After interpolation: %s", spec.shape)
     return spec
 
 
 def plot_results(y_hat: torch.tensor, y: torch.tensor, ap: AudioProcessor, name_prefix: str = None) -> Dict:
     """Plot the predicted and the real waveform and their spectrograms.
 
     Args:
```

### Comparing `coqui-tts-0.22.1/coqui_tts.egg-info/PKG-INFO` & `coqui_tts-0.23.0/coqui_tts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: coqui-tts
-Version: 0.22.1
+Version: 0.23.0
 Summary: Deep learning for Text to Speech.
-Home-page: https://github.com/eginhard/coqui-tts
+Home-page: https://github.com/idiap/coqui-ai-TTS
 Author: Eren Gölge
 Author-email: egolge@coqui.ai
 Maintainer: Enno Hermann
 Maintainer-email: enno.hermann@gmail.com
 License: MPL-2.0
 Project-URL: Documentation, https://coqui-tts.readthedocs.io
-Project-URL: Tracker, https://github.com/eginhard/coqui-tts/issues
-Project-URL: Repository, https://github.com/eginhard/coqui-tts
-Project-URL: Discussions, https://github.com/eginhard/coqui-tts/discussions
+Project-URL: Tracker, https://github.com/idiap/coqui-ai-TTS/issues
+Project-URL: Repository, https://github.com/idiap/coqui-ai-TTS
+Project-URL: Discussions, https://github.com/idiap/coqui-ai-TTS/discussions
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -86,48 +86,49 @@
 Requires-Dist: flask>=2.0.1; extra == "server"
 Provides-Extra: ja
 Requires-Dist: mecab-python3==1.0.6; extra == "ja"
 Requires-Dist: unidic-lite==1.0.8; extra == "ja"
 Requires-Dist: cutlet; extra == "ja"
 
 
-## 🐸Coqui.ai News
+## 🐸Coqui TTS News
+- 📣 Fork of the [original, unmaintained repository](https://github.com/coqui-ai/TTS). New PyPI package: [coqui-tts](https://pypi.org/project/coqui-tts)
 - 📣 ⓍTTSv2 is here with 16 languages and better performance across the board.
-- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/eginhard/coqui-tts/tree/dev/recipes/ljspeech).
+- 📣 ⓍTTS fine-tuning code is out. Check the [example recipes](https://github.com/idiap/coqui-ai-TTS/tree/dev/recipes/ljspeech).
 - 📣 ⓍTTS can now stream with <200ms latency.
 - 📣 ⓍTTS, our production TTS model that can speak 13 languages, is released [Blog Post](https://coqui.ai/blog/tts/open_xtts), [Demo](https://huggingface.co/spaces/coqui/xtts), [Docs](https://coqui-tts.readthedocs.io/en/dev/models/xtts.html)
 - 📣 [🐶Bark](https://github.com/suno-ai/bark) is now available for inference with unconstrained voice cloning. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/bark.html)
 - 📣 You can use [~1100 Fairseq models](https://github.com/facebookresearch/fairseq/tree/main/examples/mms) with 🐸TTS.
 - 📣 🐸TTS now supports 🐢Tortoise with faster inference. [Docs](https://coqui-tts.readthedocs.io/en/dev/models/tortoise.html)
 
 <div align="center">
 <img src="https://static.scarf.sh/a.png?x-pxid=cf317fe7-2188-4721-bc01-124bb5d5dbb2" />
 
-## <img src="https://raw.githubusercontent.com/eginhard/coqui-tts/main/images/coqui-log-green-TTS.png" height="56"/>
+## <img src="https://raw.githubusercontent.com/idiap/coqui-ai-TTS/main/images/coqui-log-green-TTS.png" height="56"/>
 
 
 **🐸TTS is a library for advanced Text-to-Speech generation.**
 
 🚀 Pretrained models in +1100 languages.
 
 🛠️ Tools for training new models and fine-tuning existing models in any language.
 
 📚 Utilities for dataset analysis and curation.
 ______________________________________________________________________
 
 [![Discord](https://img.shields.io/discord/1037326658807533628?color=%239B59B6&label=chat%20on%20discord)](https://discord.gg/5eXr5seRrv)
 [![License](<https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg>)](https://opensource.org/licenses/MPL-2.0)
-[![PyPI version](https://badge.fury.io/py/TTS.svg)](https://badge.fury.io/py/TTS)
-[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/eginhard/coqui-tts/blob/main/CODE_OF_CONDUCT.md)
-[![Downloads](https://pepy.tech/badge/tts)](https://pepy.tech/project/tts)
+[![PyPI version](https://badge.fury.io/py/coqui-tts.svg)](https://badge.fury.io/py/coqui-tts)
+[![Covenant](https://camo.githubusercontent.com/7d620efaa3eac1c5b060ece5d6aacfcc8b81a74a04d05cd0398689c01c4463bb/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f6e7472696275746f72253230436f76656e616e742d76322e3025323061646f707465642d6666363962342e737667)](https://github.com/idiap/coqui-ai-TTS/blob/main/CODE_OF_CONDUCT.md)
+[![Downloads](https://pepy.tech/badge/coqui-tts)](https://pepy.tech/project/coqui-tts)
 [![DOI](https://zenodo.org/badge/265612440.svg)](https://zenodo.org/badge/latestdoi/265612440)
 
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/tests.yml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/docker.yaml/badge.svg)
-![GithubActions](https://github.com/eginhard/coqui-tts/actions/workflows/style_check.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/tests.yml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/docker.yaml/badge.svg)
+![GithubActions](https://github.com/idiap/coqui-ai-TTS/actions/workflows/style_check.yml/badge.svg)
 [![Docs](<https://readthedocs.org/projects/coqui-tts/badge/?version=latest&style=plastic>)](https://coqui-tts.readthedocs.io/en/latest/)
 
 </div>
 
 ______________________________________________________________________
 
 ## 💬 Where to ask questions
@@ -136,28 +137,28 @@
 | Type                            | Platforms                               |
 | ------------------------------- | --------------------------------------- |
 | 🚨 **Bug Reports**              | [GitHub Issue Tracker]                  |
 | 🎁 **Feature Requests & Ideas** | [GitHub Issue Tracker]                  |
 | 👩‍💻 **Usage Questions**          | [GitHub Discussions]                    |
 | 🗯 **General Discussion**       | [GitHub Discussions] or [Discord]   |
 
-[github issue tracker]: https://github.com/eginhard/coqui-tts/issues
-[github discussions]: https://github.com/eginhard/coqui-tts/discussions
+[github issue tracker]: https://github.com/idiap/coqui-ai-TTS/issues
+[github discussions]: https://github.com/idiap/coqui-ai-TTS/discussions
 [discord]: https://discord.gg/5eXr5seRrv
 [Tutorials and Examples]: https://github.com/coqui-ai/TTS/wiki/TTS-Notebooks-and-Tutorials
 
 
 ## 🔗 Links and Resources
 | Type                            | Links                               |
 | ------------------------------- | --------------------------------------- |
 | 💼 **Documentation**              | [ReadTheDocs](https://coqui-tts.readthedocs.io/en/latest/)
-| 💾 **Installation**               | [TTS/README.md](https://github.com/eginhard/coqui-tts/tree/dev#installation)|
-| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/eginhard/coqui-tts/blob/main/CONTRIBUTING.md)|
+| 💾 **Installation**               | [TTS/README.md](https://github.com/idiap/coqui-ai-TTS/tree/dev#installation)|
+| 👩‍💻 **Contributing**               | [CONTRIBUTING.md](https://github.com/idiap/coqui-ai-TTS/blob/main/CONTRIBUTING.md)|
 | 📌 **Road Map**                   | [Main Development Plans](https://github.com/coqui-ai/TTS/issues/378)
-| 🚀 **Released Models**            | [Standard models](https://github.com/eginhard/coqui-tts/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/eginhard/coqui-tts#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
+| 🚀 **Released Models**            | [Standard models](https://github.com/idiap/coqui-ai-TTS/blob/dev/TTS/.models.json) and [Fairseq models in ~1100 languages](https://github.com/idiap/coqui-ai-TTS#example-text-to-speech-using-fairseq-models-in-1100-languages-)|
 | 📰 **Papers**                    | [TTS Papers](https://github.com/erogol/TTS-papers)|
 
 ## Features
 - High-performance Deep Learning models for Text2Speech tasks.
     - Text2Spec models (Tacotron, Tacotron2, Glow-TTS, SpeedySpeech).
     - Speaker Encoder to compute speaker embeddings efficiently.
     - Vocoder models (MelGAN, Multiband-MelGAN, GAN-TTS, ParallelWaveGAN, WaveGrad, WaveRNN)
@@ -217,26 +218,26 @@
 
 ### Voice Conversion
 - FreeVC: [paper](https://arxiv.org/abs/2210.15418)
 
 You can also help us implement more models.
 
 ## Installation
-🐸TTS is tested on Ubuntu 18.04 with **python >= 3.9, < 3.12.**.
+🐸TTS is tested on Ubuntu 22.04 with **python >= 3.9, < 3.12.**.
 
 If you are only interested in [synthesizing speech](https://coqui-tts.readthedocs.io/en/latest/inference.html) with the released 🐸TTS models, installing from PyPI is the easiest option.
 
 ```bash
 pip install coqui-tts
 ```
 
 If you plan to code or train models, clone 🐸TTS and install it locally.
 
 ```bash
-git clone https://github.com/eginhard/coqui-tts
+git clone https://github.com/idiap/coqui-ai-TTS
 pip install -e .[all,dev,notebooks,server]  # Select the relevant extras
 ```
 
 If you are on Ubuntu (Debian), you can also run following commands for installation.
 
 ```bash
 $ make system-deps  # intended to be used on Ubuntu (Debian). Let us know if you have a different OS.
```

### Comparing `coqui-tts-0.22.1/coqui_tts.egg-info/SOURCES.txt` & `coqui_tts-0.23.0/coqui_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/coqui_tts.egg-info/requires.txt` & `coqui_tts-0.23.0/coqui_tts.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/images/coqui-log-green-TTS.png` & `coqui_tts-0.23.0/images/coqui-log-green-TTS.png`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/images/example_model_output.png` & `coqui_tts-0.23.0/images/example_model_output.png`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/images/model.png` & `coqui_tts-0.23.0/images/model.png`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/pyproject.toml` & `coqui_tts-0.23.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/requirements.txt` & `coqui_tts-0.23.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `coqui-tts-0.22.1/setup.py` & `coqui_tts-0.23.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         name="TTS.tts.utils.monotonic_align.core",
         sources=["TTS/tts/utils/monotonic_align/core.pyx"],
     )
 ]
 setup(
     name="coqui-tts",
     version=version,
-    url="https://github.com/eginhard/coqui-tts",
+    url="https://github.com/idiap/coqui-ai-TTS",
     author="Eren Gölge",
     author_email="egolge@coqui.ai",
     maintainer="Enno Hermann",
     maintainer_email="enno.hermann@gmail.com",
     description="Deep learning for Text to Speech.",
     long_description=README,
     long_description_content_type="text/markdown",
@@ -100,17 +100,17 @@
     package_data={
         "TTS": [
             "VERSION",
         ]
     },
     project_urls={
         "Documentation": "https://coqui-tts.readthedocs.io",
-        "Tracker": "https://github.com/eginhard/coqui-tts/issues",
-        "Repository": "https://github.com/eginhard/coqui-tts",
-        "Discussions": "https://github.com/eginhard/coqui-tts/discussions",
+        "Tracker": "https://github.com/idiap/coqui-ai-TTS/issues",
+        "Repository": "https://github.com/idiap/coqui-ai-TTS",
+        "Discussions": "https://github.com/idiap/coqui-ai-TTS/discussions",
     },
     cmdclass={
         "build_py": build_py,
         "develop": develop,
         # 'build_ext': build_ext
     },
     install_requires=requirements,
```

