# Comparing `tmp/keras-vision-0.1.tar.gz` & `tmp/keras-vision-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-vision-0.1.tar", last modified: Tue Apr  9 17:44:08 2024, max compression
+gzip compressed data, was "keras-vision-0.2.tar", last modified: Fri Apr 19 21:03:49 2024, max compression
```

## Comparing `keras-vision-0.1.tar` & `keras-vision-0.2.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 17:44:08.702409 keras-vision-0.1/
--rw-rw-rw-   0        0        0       57 2024-04-09 17:44:08.700415 keras-vision-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-09 17:44:08.698397 keras-vision-0.1/keras_vision.egg-info/
--rw-rw-rw-   0        0        0       57 2024-04-09 17:44:08.000000 keras-vision-0.1/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-04-09 17:44:08.000000 keras-vision-0.1/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:44:08.000000 keras-vision-0.1/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-09 17:44:08.000000 keras-vision-0.1/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 17:44:08.000000 keras-vision-0.1/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 17:44:08.702409 keras-vision-0.1/setup.cfg
--rw-rw-rw-   0        0        0      168 2024-04-09 17:44:00.000000 keras-vision-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:03:49.459774 keras-vision-0.2/
+-rw-rw-rw-   0        0        0       79 2024-04-19 21:03:49.458765 keras-vision-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 21:03:49.439221 keras-vision-0.2/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-04-19 21:03:49.457247 keras-vision-0.2/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0     7166 2024-04-18 19:33:34.000000 keras-vision-0.2/keras_vision/MobileViT_v1/BaseLayers.py
+-rw-rw-rw-   0        0        0      500 2024-04-18 05:20:36.000000 keras-vision-0.2/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     2428 2024-04-17 12:26:24.000000 keras-vision-0.2/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     8676 2024-04-18 19:30:16.000000 keras-vision-0.2/keras_vision/MobileViT_v1/minimal_example.py
+-rw-rw-rw-   0        0        0     7039 2024-04-19 07:49:27.000000 keras-vision-0.2/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0     8904 2024-04-18 05:47:49.000000 keras-vision-0.2/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     4861 2024-04-17 11:31:19.000000 keras-vision-0.2/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.2/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.2/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 21:03:49.446248 keras-vision-0.2/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0       79 2024-04-19 21:03:49.000000 keras-vision-0.2/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-04-19 21:03:49.000000 keras-vision-0.2/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 21:03:49.000000 keras-vision-0.2/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-19 21:03:49.000000 keras-vision-0.2/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-19 21:03:49.000000 keras-vision-0.2/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 21:03:49.459774 keras-vision-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      168 2024-04-19 21:03:10.000000 keras-vision-0.2/setup.py
```

