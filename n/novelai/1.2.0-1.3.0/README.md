# Comparing `tmp/novelai-1.2.0.tar.gz` & `tmp/novelai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelai-1.2.0.tar", last modified: Sun Mar 24 21:10:58 2024, max compression
+gzip compressed data, was "novelai-1.3.0.tar", last modified: Thu Apr 18 23:22:09 2024, max compression
```

## Comparing `novelai-1.2.0.tar` & `novelai-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.730530 novelai-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.722530 novelai-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.726530 novelai-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-24 21:10:53.000000 novelai-1.2.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-24 21:10:53.000000 novelai-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-03-24 21:10:53.000000 novelai-1.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.726530 novelai-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-24 21:10:53.000000 novelai-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-24 21:10:53.000000 novelai-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    47373 2024-03-24 21:10:58.730530 novelai-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-03-24 21:10:53.000000 novelai-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.722530 novelai-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.726530 novelai-1.2.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-24 21:10:53.000000 novelai-1.2.0/docs/assets/novelai-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.726530 novelai-1.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-24 21:10:53.000000 novelai-1.2.0/docs/examples/concurrent_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-24 21:10:53.000000 novelai-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 21:10:58.730530 novelai-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.722530 novelai-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.726530 novelai-1.2.0/src/novelai/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.730530 novelai-1.2.0/src/novelai/types/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/types/hostinstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-24 21:10:53.000000 novelai-1.2.0/src/novelai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.730530 novelai-1.2.0/src/novelai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47373 2024-03-24 21:10:58.000000 novelai-1.2.0/src/novelai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-24 21:10:58.000000 novelai-1.2.0/src/novelai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 21:10:58.000000 novelai-1.2.0/src/novelai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-24 21:10:58.000000 novelai-1.2.0/src/novelai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 21:10:58.000000 novelai-1.2.0/src/novelai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.730530 novelai-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 21:10:58.730530 novelai-1.2.0/tests/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/images/inpaint_left.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    23198 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/images/portrait.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/test_calculate_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/test_generate_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/test_get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-24 21:10:53.000000 novelai-1.2.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 23:22:04.000000 novelai-1.3.0/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-18 23:22:04.000000 novelai-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-18 23:22:04.000000 novelai-1.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 23:22:04.000000 novelai-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-18 23:22:04.000000 novelai-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47148 2024-04-18 23:22:09.325173 novelai-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-18 23:22:04.000000 novelai-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-18 23:22:04.000000 novelai-1.3.0/docs/assets/novelai-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-18 23:22:04.000000 novelai-1.3.0/docs/examples/concurrent_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-18 23:22:04.000000 novelai-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 23:22:09.325173 novelai-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.321173 novelai-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/src/novelai/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/src/novelai/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/types/hostinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-18 23:22:04.000000 novelai-1.3.0/src/novelai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/src/novelai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47148 2024-04-18 23:22:09.000000 novelai-1.3.0/src/novelai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-18 23:22:09.000000 novelai-1.3.0/src/novelai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 23:22:09.000000 novelai-1.3.0/src/novelai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-18 23:22:09.000000 novelai-1.3.0/src/novelai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 23:22:09.000000 novelai-1.3.0/src/novelai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 23:22:09.325173 novelai-1.3.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/images/inpaint_left.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    23198 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/images/portrait.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/test_calculate_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/test_generate_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/test_get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-18 23:22:04.000000 novelai-1.3.0/tests/test_init.py
```

### Comparing `novelai-1.2.0/.github/workflows/pypi-publish.yml` & `novelai-1.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/.gitignore` & `novelai-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/LICENSE` & `novelai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/PKG-INFO` & `novelai-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelai
-Version: 1.2.0
+Version: 1.3.0
 Summary: 🎨 A lightweight async Python API for NovelAI image generation
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,22 +720,14 @@
 
 Install/update with pip:
 
 ```sh
 pip install -U novelai
 ```
 
-Note that this package requires Python **3.12** or higher. For lower versions, install the legacy version instead:
-
-```sh
-pip install -U novelai-legacy
-```
-
-Legacy branch has the same features as master branch on user side, the only difference is code compatibility.
-
 ## Usage
 
 ### Initialization
 
 Import required packages and initialize a client with your NovelAI account credentials.
 
 ```python
@@ -847,31 +839,31 @@
         image.save(path="output images", verbose=True)
 
 asyncio.run(main())
 ```
 
 ### Vibe Transfer
 
-Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
+Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image_multiple` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
 
 ```python
 import base64
 from novelai import Metadata, Resolution
 
 async def main():
     with open("tests/images/portrait.jpg", "rb") as f:
         base_image = base64.b64encode(f.read()).decode("utf-8")
 
     metadata = Metadata(
         prompt="1girl",
         negative_prompt="bad anatomy",
         res_preset=Resolution.NORMAL_PORTRAIT,
-        reference_image=base_image,
-        reference_infomation_extracted=1,
-        reference_strength=0.6,
+        reference_image_multiple=[base_image],
+        reference_information_extracted_multiple=[1],
+        reference_strength_multiple=[0.6],
     )
 
     output = await client.generate_image(metadata, verbose=True)
 
     for image in output:
         image.save(path="output images", verbose=True)
```

### Comparing `novelai-1.2.0/README.md` & `novelai-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,22 +37,14 @@
 
 Install/update with pip:
 
 ```sh
 pip install -U novelai
 ```
 
-Note that this package requires Python **3.12** or higher. For lower versions, install the legacy version instead:
-
-```sh
-pip install -U novelai-legacy
-```
-
-Legacy branch has the same features as master branch on user side, the only difference is code compatibility.
-
 ## Usage
 
 ### Initialization
 
 Import required packages and initialize a client with your NovelAI account credentials.
 
 ```python
@@ -164,31 +156,31 @@
         image.save(path="output images", verbose=True)
 
 asyncio.run(main())
 ```
 
 ### Vibe Transfer
 
-Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
+Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image_multiple` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
 
 ```python
 import base64
 from novelai import Metadata, Resolution
 
 async def main():
     with open("tests/images/portrait.jpg", "rb") as f:
         base_image = base64.b64encode(f.read()).decode("utf-8")
 
     metadata = Metadata(
         prompt="1girl",
         negative_prompt="bad anatomy",
         res_preset=Resolution.NORMAL_PORTRAIT,
-        reference_image=base_image,
-        reference_infomation_extracted=1,
-        reference_strength=0.6,
+        reference_image_multiple=[base_image],
+        reference_information_extracted_multiple=[1],
+        reference_strength_multiple=[0.6],
     )
 
     output = await client.generate_image(metadata, verbose=True)
 
     for image in output:
         image.save(path="output images", verbose=True)
```

### Comparing `novelai-1.2.0/docs/assets/novelai-logo.svg` & `novelai-1.3.0/docs/assets/novelai-logo.svg`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/docs/examples/concurrent_generation.py` & `novelai-1.3.0/docs/examples/concurrent_generation.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/pyproject.toml` & `novelai-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/__main__.py` & `novelai-1.3.0/src/novelai/__main__.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/client.py` & `novelai-1.3.0/src/novelai/client.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/constant.py` & `novelai-1.3.0/src/novelai/constant.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/exceptions.py` & `novelai-1.3.0/src/novelai/exceptions.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/types/image.py` & `novelai-1.3.0/src/novelai/types/image.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai/types/metadata.py` & `novelai-1.3.0/src/novelai/types/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -99,20 +99,22 @@
     add_original_image: `bool`, optional
         Refer to https://docs.novelai.net/image/inpaint.html#overlay-original-image
     mask: `str`, optional
         Base64-encoded black and white image to use as a mask for inpainting
         White is the area to inpaint and black is the rest
 
     | Vibe Transfer
-    reference_image: `str`, optional
-        Base64-encoded image to use as a base image for Vibe Transfer
-    reference_infomation_extracted: `float`, optional
-        Range: 0-1, refer to https://docs.novelai.net/.image/vibetransfer.html#information-extracted
-    reference_strength: `float`, optional
-        Range: 0-1, refer to https://docs.novelai.net/.image/vibetransfer.html#reference-strength
+    reference_image_multiple: `list[str]`, optional
+        List of base64-encoded images to use as base images for Vibe Transfer
+    reference_information_extracted_multiple: `list[float]`, optional
+        List of floats from range 0-1, should be the same length as `reference_image_multiple` and follow the same order
+        Refer to https://docs.novelai.net/.image/vibetransfer.html#information-extracted
+    reference_strength_multiple: `list[float]`, optional
+        List of floats from range 0-1, should be the same length as `reference_image_multiple` and follow the same order
+        Refer to https://docs.novelai.net/.image/vibetransfer.html#reference-strength
         The strength AI uses to emulate visual cues, such as stylistic aspects, colors etc., from the given input image
 
     | Misc
     params_version: `int`, optional
         Defaults to 1
     legacy: `bool`, optional
         Defaults to False
@@ -163,27 +165,74 @@
     controlnet_model: Controlnet | None = None
 
     # Inpaint
     add_original_image: bool = True
     mask: str | None = None
 
     # Vibe Transfer
-    reference_image: str | None = None
-    reference_infomation_extracted: float = Field(
-        default=1, ge=0.01, le=1, multiple_of=0.01
-    )
-    reference_strength: float = Field(default=0.6, ge=0.01, le=1, multiple_of=0.01)
+    reference_image_multiple: list[str] = []
+    reference_information_extracted_multiple: list[
+        Annotated[float, Field(default=1, ge=0.01, le=1, multiple_of=0.01)]
+    ] = []
+    reference_strength_multiple: list[
+        Annotated[float, Field(default=0.6, ge=0.01, le=1, multiple_of=0.01)]
+    ] = []
 
     # Misc
     params_version: Literal[1] = 1
     legacy: bool = False
     legacy_v3_extend: bool = False
 
     @model_validator(mode="after")
     def n_samples_validator(self) -> "Metadata":
+        """
+        Validate the following:
+
+        - If length of `reference_information_extracted_multiple` and `reference_strength_multiple` matches `reference_image_multiple`.
+            If not, fill the missing values with default or truncate the extra values.
+        - If value of `n_samples` exceeds the maximum allowed value based on resolution.
+        """
+
+        if self.reference_image_multiple:
+            if len(self.reference_information_extracted_multiple) > len(
+                self.reference_image_multiple
+            ):
+                self.reference_information_extracted_multiple = (
+                    self.reference_information_extracted_multiple[
+                        : len(self.reference_image_multiple)
+                    ]
+                )
+            elif len(self.reference_information_extracted_multiple) < len(
+                self.reference_image_multiple
+            ):
+                self.reference_information_extracted_multiple += [
+                    1
+                    for _ in range(
+                        len(self.reference_image_multiple)
+                        - len(self.reference_information_extracted_multiple)
+                    )
+                ]
+
+            if len(self.reference_strength_multiple) > len(
+                self.reference_image_multiple
+            ):
+                self.reference_strength_multiple = self.reference_strength_multiple[
+                    : len(self.reference_image_multiple)
+                ]
+            elif len(self.reference_strength_multiple) < len(
+                self.reference_image_multiple
+            ):
+                self.reference_strength_multiple += [
+                    0.6
+                    for _ in range(
+                        len(self.reference_image_multiple)
+                        - len(self.reference_strength_multiple)
+                    )
+                ]
+
         max_n_samples = self.get_max_n_samples()
         if self.n_samples > max_n_samples:
             raise ValueError(
                 f"Max value of n_samples is {max_n_samples} under current resolution ({self.width}x{self.height}). Got {self.n_samples}."
             )
         return self
```

### Comparing `novelai-1.2.0/src/novelai/utils.py` & `novelai-1.3.0/src/novelai/utils.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/src/novelai.egg-info/PKG-INFO` & `novelai-1.3.0/src/novelai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelai
-Version: 1.2.0
+Version: 1.3.0
 Summary: 🎨 A lightweight async Python API for NovelAI image generation
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,22 +720,14 @@
 
 Install/update with pip:
 
 ```sh
 pip install -U novelai
 ```
 
-Note that this package requires Python **3.12** or higher. For lower versions, install the legacy version instead:
-
-```sh
-pip install -U novelai-legacy
-```
-
-Legacy branch has the same features as master branch on user side, the only difference is code compatibility.
-
 ## Usage
 
 ### Initialization
 
 Import required packages and initialize a client with your NovelAI account credentials.
 
 ```python
@@ -847,31 +839,31 @@
         image.save(path="output images", verbose=True)
 
 asyncio.run(main())
 ```
 
 ### Vibe Transfer
 
-Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
+Vibe transfer doesn't have its own action type. Instead, it is achieved by adding a `reference_image_multiple` parameter in Metadata. The reference image needs to be converted into Base64-encoded format. This can be achieved using `base64` module.
 
 ```python
 import base64
 from novelai import Metadata, Resolution
 
 async def main():
     with open("tests/images/portrait.jpg", "rb") as f:
         base_image = base64.b64encode(f.read()).decode("utf-8")
 
     metadata = Metadata(
         prompt="1girl",
         negative_prompt="bad anatomy",
         res_preset=Resolution.NORMAL_PORTRAIT,
-        reference_image=base_image,
-        reference_infomation_extracted=1,
-        reference_strength=0.6,
+        reference_image_multiple=[base_image],
+        reference_information_extracted_multiple=[1],
+        reference_strength_multiple=[0.6],
     )
 
     output = await client.generate_image(metadata, verbose=True)
 
     for image in output:
         image.save(path="output images", verbose=True)
```

### Comparing `novelai-1.2.0/src/novelai.egg-info/SOURCES.txt` & `novelai-1.3.0/src/novelai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/tests/images/inpaint_left.jpg` & `novelai-1.3.0/tests/images/inpaint_left.jpg`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/tests/images/portrait.jpg` & `novelai-1.3.0/tests/images/portrait.jpg`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/tests/test_calculate_cost.py` & `novelai-1.3.0/tests/test_calculate_cost.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/tests/test_generate_image.py` & `novelai-1.3.0/tests/test_generate_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import base64
 import asyncio
 import unittest
 from unittest.mock import AsyncMock, MagicMock
 
 from httpx import AsyncClient
 
-from novelai import NAIClient, Metadata, Host, Model, Action, Resolution
+from novelai import NAIClient, Metadata, Host, Model, Action
 from novelai.exceptions import (
     APIError,
     AuthError,
     ConcurrentError,
     TimeoutError,
     NovelAIError,
 )
@@ -32,15 +32,15 @@
 
     @unittest.skipIf(
         not (os.getenv("USERNAME") and os.getenv("PASSWORD")),
         "Skipped due to missing environment variables",
     )
     async def test_generate(self):
         await self.naiclient.init()
-        metadata = Metadata(prompt="1girl")
+        metadata = Metadata(prompt="1girl", width=320, height=320)
 
         try:
             output = await self.naiclient.generate_image(metadata, host=Host.WEB)
             self.assertTrue(len(output) > 0)
             for image in output:
                 image.save(filename="generate.png", verbose=True)
                 self.assertTrue(image.filename == "generate.png")
@@ -54,15 +54,16 @@
         "Skipped due to missing environment variables",
     )
     async def test_img2img(self):
         await self.naiclient.init()
         metadata = Metadata(
             prompt="1girl",
             action=Action.IMG2IMG,
-            res_preset=Resolution.NORMAL_PORTRAIT,
+            width=320,
+            height=320,
             image=base_image,
             strength=0.45,
             noise=0.1,
         )
 
         try:
             output = await self.naiclient.generate_image(metadata, host=Host.WEB)
@@ -80,15 +81,16 @@
     )
     async def test_inpaint(self):
         await self.naiclient.init()
         metadata = Metadata(
             prompt="1girl",
             model=Model.V3INP,
             action=Action.INPAINT,
-            res_preset=Resolution.NORMAL_PORTRAIT,
+            width=320,
+            height=320,
             image=base_image,
             mask=mask,
         )
 
         try:
             output = await self.naiclient.generate_image(metadata, host=Host.WEB)
             self.assertTrue(len(output) > 0)
@@ -104,18 +106,19 @@
         "Skipped due to missing environment variables",
     )
     async def test_vibe_transfer(self):
         await self.naiclient.init()
         metadata = Metadata(
             prompt="1girl",
             action=Action.GENERATE,
-            res_preset=Resolution.NORMAL_PORTRAIT,
-            reference_image=base_image,
-            reference_infomation_extracted=1,
-            reference_strength=0.6,
+            width=320,
+            height=320,
+            reference_image_multiple=[base_image],
+            reference_information_extracted_multiple=[1],
+            reference_strength_multiple=[0.6],
         )
 
         try:
             output = await self.naiclient.generate_image(metadata, host=Host.WEB)
             self.assertTrue(len(output) > 0)
             for image in output:
                 image.save(filename="vibe_transfer.png", verbose=True)
```

### Comparing `novelai-1.2.0/tests/test_get_access_token.py` & `novelai-1.3.0/tests/test_get_access_token.py`

 * *Files identical despite different names*

### Comparing `novelai-1.2.0/tests/test_init.py` & `novelai-1.3.0/tests/test_init.py`

 * *Files identical despite different names*

