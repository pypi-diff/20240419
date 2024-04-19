# Comparing `tmp/novita_client-0.5.3.tar.gz` & `tmp/novita_client-0.5.4.tar.gz`

## Comparing `novita_client-0.5.3.tar` & `novita_client-0.5.4.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.3/.python-version
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.3/Makefile
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.3/generate-readme.sh
--rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.3/image.jpg
--rw-r--r--   0        0        0   101219 2020-02-02 00:00:00.000000 novita_client-0.5.3/image1 copy.jpg
--rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 novita_client-0.5.3/image1.jpg
--rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.3/image2.jpg
--rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img-controlnet.png
--rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img-logo.png
--rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.3/img2img.png
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.3/logo.py
--rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.3/outpainting.png
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 novita_client-0.5.3/ow.py
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.3/requirements-dev.lock
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.3/requirements.lock
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 novita_client-0.5.3/shanginn.py
--rw-r--r--   0        0        0   382237 2020-02-02 00:00:00.000000 novita_client-0.5.3/test.mp4
--rw-r--r--   0        0        0   314009 2020-02-02 00:00:00.000000 novita_client-0.5.3/test.png
--rw-r--r--   0        0        0   479432 2020-02-02 00:00:00.000000 novita_client-0.5.3/txt2img-lora-compare.png
--rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.3/txt2img_with_hiresfix.png
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/cleanup.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/controlnet.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/create-tile.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/doodle.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/img2img.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/img2video.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/instantid.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/latent-consistency-txt2img.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/lcm-img2img.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/lcm-vs-txt2img.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/make-photo.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/merge-face.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/mixpose.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/model-search.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/outpainting.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/reimagine.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/remove-background.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/remove-text.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-background.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-object.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/replace-sky.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-hiresfix.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-lora.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/txt2img-with-refiner.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.3/examples/fixtures/qrcode.png
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/exceptions.py
--rw-r--r--   0        0        0    45014 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/novita.py
--rw-r--r--   0        0        0    37956 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/proto.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/serializer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/settings.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.3/src/novita_client/version.py
--rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_basics.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_enhance.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.3/tests/test_model.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.3/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.3/LICENSE
--rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.3/README.md
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 novita_client-0.5.4/.python-version
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 novita_client-0.5.4/Makefile
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 novita_client-0.5.4/generate-readme.sh
+-rw-r--r--   0        0        0    88494 2020-02-02 00:00:00.000000 novita_client-0.5.4/image.jpg
+-rw-r--r--   0        0        0   101219 2020-02-02 00:00:00.000000 novita_client-0.5.4/image1 copy.jpg
+-rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 novita_client-0.5.4/image1.jpg
+-rw-r--r--   0        0        0    97725 2020-02-02 00:00:00.000000 novita_client-0.5.4/image2.jpg
+-rw-r--r--   0        0        0   696352 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img-controlnet.png
+-rw-r--r--   0        0        0   288795 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img-logo.png
+-rw-r--r--   0        0        0   159522 2020-02-02 00:00:00.000000 novita_client-0.5.4/img2img.png
+-rw-r--r--   0        0        0   195126 2020-02-02 00:00:00.000000 novita_client-0.5.4/instantid.png
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 novita_client-0.5.4/logo.py
+-rw-r--r--   0        0        0   583721 2020-02-02 00:00:00.000000 novita_client-0.5.4/outpainting.png
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 novita_client-0.5.4/ow.py
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 novita_client-0.5.4/requirements-dev.lock
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 novita_client-0.5.4/requirements.lock
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 novita_client-0.5.4/shanginn.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 novita_client-0.5.4/susubot.py
+-rw-r--r--   0        0        0   382237 2020-02-02 00:00:00.000000 novita_client-0.5.4/test.mp4
+-rw-r--r--   0        0        0   490142 2020-02-02 00:00:00.000000 novita_client-0.5.4/test.png
+-rw-r--r--   0        0        0  2297297 2020-02-02 00:00:00.000000 novita_client-0.5.4/txt2img-lora-compare.png
+-rw-r--r--   0        0        0   711146 2020-02-02 00:00:00.000000 novita_client-0.5.4/txt2img_with_hiresfix.png
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/cleanup.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/controlnet.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/create-tile.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/doodle.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/img2img.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/img2video.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/instantid.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/latent-consistency-txt2img.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/lcm-img2img.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/lcm-vs-txt2img.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/make-photo.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/merge-face.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/mixpose.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/model-search.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/outpainting.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/reimagine.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/remove-background.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/remove-text.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-background.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-object.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/replace-sky.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-hiresfix.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-lora.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/txt2img-with-refiner.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 novita_client-0.5.4/examples/fixtures/qrcode.png
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/exceptions.py
+-rw-r--r--   0        0        0    45566 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/novita.py
+-rw-r--r--   0        0        0    37956 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/proto.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/serializer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/settings.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 novita_client-0.5.4/src/novita_client/version.py
+-rw-r--r--   0        0        0    12841 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_basics.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_enhance.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 novita_client-0.5.4/tests/test_model.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 novita_client-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 novita_client-0.5.4/LICENSE
+-rw-r--r--   0        0        0    22761 2020-02-02 00:00:00.000000 novita_client-0.5.4/README.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 novita_client-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    24574 2020-02-02 00:00:00.000000 novita_client-0.5.4/PKG-INFO
```

### Comparing `novita_client-0.5.3/generate-readme.sh` & `novita_client-0.5.4/generate-readme.sh`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/image.jpg` & `novita_client-0.5.4/image.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/image1 copy.jpg` & `novita_client-0.5.4/image1 copy.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/image1.jpg` & `novita_client-0.5.4/image1.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/image2.jpg` & `novita_client-0.5.4/image2.jpg`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/img2img-controlnet.png` & `novita_client-0.5.4/img2img-controlnet.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/img2img-logo.png` & `novita_client-0.5.4/img2img-logo.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/img2img.png` & `novita_client-0.5.4/img2img.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/logo.py` & `novita_client-0.5.4/logo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/outpainting.png` & `novita_client-0.5.4/outpainting.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/ow.py` & `novita_client-0.5.4/ow.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/requirements-dev.lock` & `novita_client-0.5.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/shanginn.py` & `novita_client-0.5.4/shanginn.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/test.mp4` & `novita_client-0.5.4/test.mp4`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/txt2img_with_hiresfix.png` & `novita_client-0.5.4/txt2img_with_hiresfix.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/cleanup.py` & `novita_client-0.5.4/examples/cleanup.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/controlnet.py` & `novita_client-0.5.4/examples/controlnet.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/img2img.py` & `novita_client-0.5.4/examples/img2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/latent-consistency-txt2img.py` & `novita_client-0.5.4/examples/latent-consistency-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/lcm-vs-txt2img.py` & `novita_client-0.5.4/examples/lcm-vs-txt2img.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/make-photo.py` & `novita_client-0.5.4/examples/make-photo.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/model-search.py` & `novita_client-0.5.4/examples/model-search.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/txt2img-with-hiresfix.py` & `novita_client-0.5.4/examples/txt2img-with-hiresfix.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/examples/txt2img-with-lora.py` & `novita_client-0.5.4/examples/txt2img-with-refiner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-#!/usr/bin/env python
-# -*- coding: UTF-8 -*-
-
 import os
-from novita_client import NovitaClient, Txt2ImgV3LoRA, Samplers, ProgressResponseStatusCode, ModelType, add_lora_to_prompt, save_image
-from novita_client.utils import base64_to_image, input_image_to_pil
+
+from novita_client import NovitaClient, Txt2ImgV3Refiner, Samplers
+from novita_client.utils import base64_to_image
 from PIL import Image
 
 
 def make_image_grid(images, rows: int, cols: int, resize: int = None):
     """
     Prepares a single grid of images. Useful for visualization purposes.
     """
@@ -22,35 +20,45 @@
     for i, img in enumerate(images):
         grid.paste(img, box=(i % cols * w, i // cols * h))
     return grid
 
 
 client = NovitaClient(os.getenv('NOVITA_API_KEY'), os.getenv('NOVITA_API_URI', None))
 
-res1 = client.txt2img_v3(
-    prompt="a photo of handsome man, close up",
+r1 = client.txt2img_v3(
+    model_name='sd_xl_base_1.0.safetensors',
+    prompt='a astronaut riding a bike on the moon',
+    width=1024,
+    height=1024,
     image_num=1,
-    guidance_scale=7.0,
-    sampler_name=Samplers.DPMPP_M_KARRAS,
-    model_name="dreamshaper_8_93211.safetensors",
-    height=512,
-    width=512,
-    seed=1024,
+    guidance_scale=7.5,
+    sampler_name=Samplers.EULER_A,
 )
-res2 = client.txt2img_v3(
-    prompt="a photo of handsome man, close up",
+
+r2 = client.txt2img_v3(
+    model_name='sd_xl_base_1.0.safetensors',
+    prompt='a astronaut riding a bike on the moon',
+    width=1024,
+    height=1024,
     image_num=1,
-    guidance_scale=7.0,
-    sampler_name=Samplers.DPMPP_M_KARRAS,
-    model_name="dreamshaper_8_93211.safetensors",
-    height=512,
-    width=512,
-    seed=1024,
-    loras=[
-        Txt2ImgV3LoRA(
-           model_name="add_detail_44319",
-           strength=0.9,
-        )
-    ]
+    guidance_scale=7.5,
+    sampler_name=Samplers.EULER_A,
+    refiner=Txt2ImgV3Refiner(
+        switch_at=0.7
+    )
 )
 
-make_image_grid([base64_to_image(res1.images_encoded[0]), base64_to_image(res2.images_encoded[0])], 1, 2, 512).save("./txt2img-lora-compare.png")
+r3 = client.txt2img_v3(
+    model_name='sd_xl_base_1.0.safetensors',
+    prompt='a astronaut riding a bike on the moon',
+    width=1024,
+    height=1024,
+    image_num=1,
+    guidance_scale=7.5,
+    sampler_name=Samplers.EULER_A,
+    refiner=Txt2ImgV3Refiner(
+        switch_at=0.5
+    )
+)
+
+
+make_image_grid([base64_to_image(r1.images_encoded[0]), base64_to_image(r2.images_encoded[0]), base64_to_image(r3.images_encoded[0])], 1, 3, 1024).save("./txt2img-refiner-compare.png")
```

### Comparing `novita_client-0.5.3/examples/fixtures/qrcode.png` & `novita_client-0.5.4/examples/fixtures/qrcode.png`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/src/novita_client/novita.py` & `novita_client-0.5.4/src/novita_client/novita.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,62 +95,62 @@
         if response.status_code != 200:
             logger.error(f"Request failed: {response}")
             raise NovitaResponseError(
                 f"Request failed with status {response.status_code}, {response.content}")
 
         return response.json()
 
-    def txt2img(self, request: Txt2ImgRequest) -> Txt2ImgResponse:
+    def txt2img(self, request: Txt2ImgRequest, enterprise_plan=False) -> Txt2ImgResponse:
         """Asynchronously generate images from request
 
         Args:
             request (Txt2ImgRequest): The request object containing the text and image generation parameters.
 
         Returns:
             Txt2ImgResponse: The response object containing the task ID and status URL.
         """
-        response = self._post('/v2/txt2img', request.to_dict())
+        response = self._post('/v2/txt2img' if not enterprise_plan else '/v2/enterprise/txt2img', request.to_dict())
 
         return Txt2ImgResponse.from_dict(response)
 
-    def progress(self, task_id: str) -> ProgressResponse:
+    def progress(self, task_id: str, enterprise_plan=False) -> ProgressResponse:
         """Get the progress of a task.
 
         Args:
             task_id (str): The ID of the task to get the progress for.
 
         Returns:
             ProgressResponse: The response object containing the progress information for the task.
         """
-        response = self._get('/v2/progress', {
+        response = self._get('/v2/progress' if not enterprise_plan else '/v2/enterprise/progress', {
             'task_id': task_id,
         })
 
         return ProgressResponse.from_dict(response)
 
     def async_task_result(self, task_id: str) -> V3TaskResponse:
         response = self._get('/v3/async/task-result', {
             'task_id': task_id,
         })
         return V3TaskResponse.from_dict(response)
 
-    def img2img(self, request: Img2ImgRequest) -> Img2ImgResponse:
+    def img2img(self, request: Img2ImgRequest, enterprise_plan=False) -> Img2ImgResponse:
         """Asynchronously generate images from request
 
         Args:
             request (Img2ImgRequest): The request object containing the image and image generation parameters.
 
         Returns:
             Img2ImgResponse: The response object containing the task ID and status URL.
         """
-        response = self._post('/v2/img2img', request.to_dict())
+        response = self._post('/v2/img2img' if not enterprise_plan else '/v2/enterprise/img2img', request.to_dict())
 
         return Img2ImgResponse.from_dict(response)
 
-    def wait_for_task(self, task_id, wait_for: int = 300, callback: callable = None) -> ProgressResponse:
+    def wait_for_task(self, task_id, wait_for: int = 300, callback: callable = None, enterprise_plan=False) -> ProgressResponse:
         """Wait for a task to complete
 
         This method waits for a task to complete by periodically checking its progress. If the task is not completed within the specified time, an NovitaTimeoutError is raised.
 
         Args:
             task_id (_type_): The ID of the task to wait for.
             wait_for (int, optional): The maximum time to wait for the task to complete, in seconds. Defaults to 300.
@@ -162,15 +162,15 @@
             ProgressResponse: The response object containing the progress information for the task.
         """
         i = 0
 
         while i < wait_for:
             logger.info(f"Waiting for task {task_id} to complete")
 
-            progress = self.progress(task_id)
+            progress = self.progress(task_id, enterprise_plan=enterprise_plan)
 
             if callback and callable(callback):
                 try:
                     callback(progress)
                 except Exception as e:
                     logger.error(f"Task {task_id} progress callback failed: {e}")
 
@@ -207,75 +207,75 @@
                 return progress
 
             sleep(settings.DEFAULT_POLL_INTERVAL)
             i += 1
         raise NovitaTimeoutError(
             f"Task {task_id} failed to complete in {wait_for} seconds")
 
-    def sync_txt2img(self, request: Txt2ImgRequest, download_images=True, callback: callable = None) -> ProgressResponse:
+    def sync_txt2img(self, request: Txt2ImgRequest, download_images=True, callback: callable = None, enterprise_plan=False) -> ProgressResponse:
         """Synchronously generate images from request, optionally download images
 
         This method generates images synchronously from the given request object. If download_images is set to True, the generated images will be downloaded.
 
         Args:
             request (Txt2ImgRequest): The request object containing the input text and other parameters.
             download_images (bool, optional): Whether to download the generated images. Defaults to True.
 
         Raises:
             NovitaResponseError: If the text to image generation fails.
 
         Returns:
             ProgressResponse: The response object containing the task status and generated images.
         """
-        response = self.txt2img(request)
+        response = self.txt2img(request, enterprise_plan=enterprise_plan)
 
         if response.data is None:
             raise NovitaResponseError(f"Text to Image generation failed with response {response.msg}, code: {response.code}")
 
-        res = self.wait_for_task(response.data.task_id, callback=callback)
+        res = self.wait_for_task(response.data.task_id, callback=callback, enterprise_plan=enterprise_plan)
         if download_images:
             res.download_images()
         return res
 
-    def sync_img2img(self, request: Img2ImgRequest, download_images=True, callback: callable = None) -> ProgressResponse:
+    def sync_img2img(self, request: Img2ImgRequest, download_images=True, callback: callable = None, enterprise_plan=False) -> ProgressResponse:
         """Synchronously generate images from request, optionally download images
 
         Args:
             request (Img2ImgRequest): The request object containing the input image and other parameters.
             download_images (bool, optional): Whether to download the generated images. Defaults to True.
 
         Returns:
             ProgressResponse: The response object containing the task status and generated images.
         """
-        response = self.img2img(request)
+        response = self.img2img(request, enterprise_plan=enterprise_plan)
 
         if response.data is None:
             raise NovitaResponseError(f"Image to Image generation failed with response {response.msg}, code: {response.code}")
 
-        res = self.wait_for_task(response.data.task_id, callback=callback)
+        res = self.wait_for_task(response.data.task_id, callback=callback, enterprise_plan=enterprise_plan)
         if download_images:
             res.download_images()
         return res
 
-    def sync_upscale(self, request: UpscaleRequest, download_images=True, callback: callable = None) -> ProgressResponse:
+    def sync_upscale(self, request: UpscaleRequest, download_images=True, callback: callable = None, enterprise_plan=False) -> ProgressResponse:
         """Syncronously upscale image from request, optionally download images
 
         Args:
             request (UpscaleRequest): _description_
             download_images (bool, optional): _description_. Defaults to True.
 
         Returns:
             ProgressResponse: _description_
         """
-        response = self.upscale(request)
+        response = self.upscale(request, enterprise_plan=enterprise_plan)
 
         if response.data is None:
             raise NovitaResponseError(f"Upscale failed with response {response.msg}, code: {response.code}")
 
-        res = self.wait_for_task(response.data.task_id, callback=callback)
+        res = self.wait_for_task(response.data.task_id, callback=callback, enterprise_plan=enterprise_plan)
         if download_images:
             res.download_images()
         return res
 
     def upscale(self, request: UpscaleRequest) -> UpscaleResponse:
         """Upscale image
```

### Comparing `novita_client-0.5.3/src/novita_client/proto.py` & `novita_client-0.5.4/src/novita_client/proto.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/src/novita_client/utils.py` & `novita_client-0.5.4/src/novita_client/utils.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/tests/test_basics.py` & `novita_client-0.5.4/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/tests/test_enhance.py` & `novita_client-0.5.4/tests/test_enhance.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/tests/test_model.py` & `novita_client-0.5.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/.gitignore` & `novita_client-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/LICENSE` & `novita_client-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/README.md` & `novita_client-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `novita_client-0.5.3/pyproject.toml` & `novita_client-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "novita_client"
-version = "0.5.3"
+version = "0.5.4"
 description = "novita SDK for Python"
 authors = [
     { name = "novita", email = "novitalabs@gmail.com" }
 ]
 
 
 dependencies = [
```

### Comparing `novita_client-0.5.3/PKG-INFO` & `novita_client-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: novita_client
-Version: 0.5.3
+Version: 0.5.4
 Summary: novita SDK for Python
 Project-URL: Homepage, https://github.com/novita/python-sdk
 Project-URL: Bug Tracker, https://discord.gg/nzqq8UScpx
 Author-email: novita <novitalabs@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 novita.ai
```

