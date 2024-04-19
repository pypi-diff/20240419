# Comparing `tmp/kimchima-0.4.7.tar.gz` & `tmp/kimchima-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.4.7.tar", max compression
+gzip compressed data, was "kimchima-0.4.8.tar", max compression
```

## Comparing `kimchima-0.4.7.tar` & `kimchima-0.4.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11343 2024-04-17 14:44:32.421839 kimchima-0.4.7/LICENSE
--rw-r--r--   0        0        0      908 2024-04-17 14:44:32.421839 kimchima-0.4.7/README.md
--rw-r--r--   0        0        0     2595 2024-04-17 14:44:32.421839 kimchima-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/__init__.py
--rw-r--r--   0        0        0      684 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/chat_template/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/chat_template/chat_template_factory.py
--rw-r--r--   0        0        0        0 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1566 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0        0 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/models/__init__.py
--rw-r--r--   0        0        0      674 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     2347 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1015 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1598 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3222 2024-04-17 14:44:32.421839 kimchima-0.4.7/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4712 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1838 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3558 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1966 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_chat.py
--rw-r--r--   0        0        0     2290 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_chat_template_factory.py
--rw-r--r--   0        0        0     1818 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     3587 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_downloadr.py
--rw-r--r--   0        0        0     2032 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     2509 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0      702 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/__init__.py
--rw-r--r--   0        0        0     1817 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/chat.py
--rw-r--r--   0        0        0     4024 2024-04-17 14:44:32.425839 kimchima-0.4.7/src/kimchima/utils/downloader.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-19 05:39:42.012785 kimchima-0.4.8/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-19 05:39:42.012785 kimchima-0.4.8/README.md
+-rw-r--r--   0        0        0     2595 2024-04-19 05:39:42.016785 kimchima-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/__init__.py
+-rw-r--r--   0        0        0      684 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/chat_template/__init__.py
+-rw-r--r--   0        0        0     1844 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/chat_template/chat_template_factory.py
+-rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1566 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     2347 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1015 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3222 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4712 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1838 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3558 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1966 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_chat.py
+-rw-r--r--   0        0        0     2290 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_chat_template_factory.py
+-rw-r--r--   0        0        0     1818 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     3587 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_downloadr.py
+-rw-r--r--   0        0        0     2032 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     2509 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0      702 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/__init__.py
+-rw-r--r--   0        0        0     1817 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/chat.py
+-rw-r--r--   0        0        0     4851 2024-04-19 05:39:42.016785 kimchima-0.4.8/src/kimchima/utils/downloader.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 kimchima-0.4.8/PKG-INFO
```

### Comparing `kimchima-0.4.7/LICENSE` & `kimchima-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/README.md` & `kimchima-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/pyproject.toml` & `kimchima-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.4.7"
+version = "0.4.8"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
```

### Comparing `kimchima-0.4.7/src/kimchima/__init__.py` & `kimchima-0.4.8/src/kimchima/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/chat_template/__init__.py` & `kimchima-0.4.8/src/kimchima/chat_template/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/chat_template/chat_template_factory.py` & `kimchima-0.4.8/src/kimchima/chat_template/chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/cmds/auto_cli.py` & `kimchima-0.4.8/src/kimchima/cmds/auto_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.4.8/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pipelines/__init__.py` & `kimchima-0.4.8/src/kimchima/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pipelines/pipelines_factory.py` & `kimchima-0.4.8/src/kimchima/pipelines/pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/__init__.py` & `kimchima-0.4.8/src/kimchima/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/devices.py` & `kimchima-0.4.8/src/kimchima/pkg/devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.4.8/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/logging.py` & `kimchima-0.4.8/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/model_factory.py` & `kimchima-0.4.8/src/kimchima/pkg/model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.4.8/src/kimchima/pkg/quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.4.8/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.4.8/src/kimchima/pkg/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_chat.py` & `kimchima-0.4.8/src/kimchima/tests/test_chat.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_chat_template_factory.py` & `kimchima-0.4.8/src/kimchima/tests/test_chat_template_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_devices.py` & `kimchima-0.4.8/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_downloadr.py` & `kimchima-0.4.8/src/kimchima/tests/test_downloadr.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.4.8/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.4.8/src/kimchima/tests/test_pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.4.8/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/utils/__init__.py` & `kimchima-0.4.8/src/kimchima/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/utils/chat.py` & `kimchima-0.4.8/src/kimchima/utils/chat.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.4.7/src/kimchima/utils/downloader.py` & `kimchima-0.4.8/src/kimchima/utils/downloader.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,27 +18,36 @@
 from kimchima.pkg import logging
 from transformers import (
     pipeline, 
     AutoModel,
     AutoTokenizer,
     AutoModelForCausalLM,
     )
+import shutil
+import os
 
 logger=logging.get_logger(__name__)
 
 
 
 class Downloader:
 
     def __init__(self):
         raise EnvironmentError(
             "Embeddings is designed to be instantiated "
             "using the `Embeddings.from_pretrained(pretrained_model_name_or_path)` method."
         )
-    
+    def _move_files_and_remove_dir(src_folder, dst_folder):
+        for filename in os.listdir(src_folder):
+            dst_file = os.path.join(dst_folder, filename)
+            if os.path.exists(dst_file):
+                os.remove(dst_file)
+            shutil.move(os.path.join(src_folder, filename), dst_folder)
+        shutil.rmtree(src_folder)
+
     @classmethod
     def model_downloader(cls, *args, **kwargs):
         r"""
         Here we will use pipeline from Huggingface to download the model.
         And save the model to the specified folder.
         """
         model_name=kwargs.pop("model_name", None)
@@ -62,17 +71,26 @@
         perform tasks like text generation or translation.
         """
 
         model_name=kwargs.pop("model_name", None)
         if model_name is None:
             raise ValueError("model_name is required")
         folder_name=kwargs.pop("folder_name", None)
-
+        if folder_name is None:
+            folder_name = model_name
         model=AutoModel.from_pretrained(model_name)
-        model.save_pretrained(folder_name if folder_name is not None else model_name)
+        # save_pretrained only saves the model weights, not the configuration
+        model.save_pretrained(folder_name )
+        
+        tokenizer=AutoTokenizer.from_pretrained(model_name)
+        tokenizer.save_pretrained(folder_name + "/tmp1", legacy_format=False)
+        tokenizer.save_pretrained(folder_name + "/tmp2", legacy_format=True)
+
+        for tmp_folder in ["/tmp1", "/tmp2"]:
+            cls._move_files_and_remove_dir(folder_name+ tmp_folder, folder_name)
         logger.info(f"Model {model_name} has been downloaded successfully")
 
     
     @classmethod
     def casual_downloader(cls, *args, **kwargs):
         r"""
         Here we will use AutoModelForCausalLM from Huggingface to download the model
@@ -100,8 +118,9 @@
         if model_name is None:
             raise ValueError("model_name is required")
 
         folder_name=kwargs.pop("folder_name", None)
         
         tokenizer=AutoTokenizer.from_pretrained(model_name)
         tokenizer.save_pretrained(folder_name if folder_name is not None else model_name)
-        logger.info(f"Tokenizer {model_name} has been downloaded successfully")
+        logger.info(f"Tokenizer {model_name} has been downloaded successfully")
+
```

### Comparing `kimchima-0.4.7/PKG-INFO` & `kimchima-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.4.7
+Version: 0.4.8
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

