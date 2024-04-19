# Comparing `tmp/substrate-120240416.0.7.tar.gz` & `tmp/substrate-120240416.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-120240416.0.7.tar", max compression
+gzip compressed data, was "substrate-120240416.0.8.tar", max compression
```

## Comparing `substrate-120240416.0.7.tar` & `substrate-120240416.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.7/LICENSE
--rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.7/README.md
--rw-r--r--   0        0        0     2023 2024-04-16 21:57:20.560242 substrate-120240416.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.7/substrate/.keep
--rw-r--r--   0        0        0       17 2024-04-16 21:25:37.772233 substrate-120240416.0.7/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2010 2024-04-16 21:54:10.814592 substrate-120240416.0.7/substrate/__init__.py
--rw-r--r--   0        0        0     6011 2024-04-16 21:56:15.032839 substrate-120240416.0.7/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.7/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-04-16 21:23:27.826516 substrate-120240416.0.7/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-04-16 21:23:27.826379 substrate-120240416.0.7/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-04-16 21:23:27.826967 substrate-120240416.0.7/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-04-16 21:23:27.827571 substrate-120240416.0.7/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-04-16 21:23:27.827722 substrate-120240416.0.7/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-04-16 21:23:27.827901 substrate-120240416.0.7/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-04-16 21:23:27.827319 substrate-120240416.0.7/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-04-16 21:23:27.826777 substrate-120240416.0.7/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2186 2024-04-16 21:25:37.773256 substrate-120240416.0.7/substrate/core/corenode.py
--rw-r--r--   0        0        0     1227 2024-04-16 21:23:27.827149 substrate-120240416.0.7/substrate/core/future_directive.py
--rw-r--r--   0        0        0      894 2024-04-16 21:23:27.825332 substrate-120240416.0.7/substrate/core/id_generator.py
--rw-r--r--   0        0        0    38450 2024-04-16 21:25:37.773637 substrate-120240416.0.7/substrate/core/models.py
--rw-r--r--   0        0        0     2332 2024-04-16 21:23:27.825185 substrate-120240416.0.7/substrate/core/sb.py
--rw-r--r--   0        0        0    32587 2024-04-16 21:25:37.774019 substrate-120240416.0.7/substrate/dataclass_models.py
--rw-r--r--   0        0        0    43578 2024-04-16 21:25:37.774619 substrate-120240416.0.7/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    40555 2024-04-16 21:25:37.774957 substrate-120240416.0.7/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.7/substrate/py.typed
--rw-r--r--   0        0        0     1490 2024-04-16 20:07:00.739577 substrate-120240416.0.7/substrate/substrate.py
--rw-r--r--   0        0        0     1034 2024-04-16 21:25:37.775283 substrate-120240416.0.7/substrate/substrate_response.py
--rw-r--r--   0        0        0    35749 2024-04-16 21:25:37.775828 substrate-120240416.0.7/substrate/typeddict_models.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240416.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-120240416.0.8/LICENSE
+-rw-r--r--   0        0        0       45 2024-03-19 21:55:57.200047 substrate-120240416.0.8/README.md
+-rw-r--r--   0        0        0     2023 2024-04-19 01:13:10.555871 substrate-120240416.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-120240416.0.8/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-04-19 01:11:41.000000 substrate-120240416.0.8/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2010 2024-04-19 01:11:42.000000 substrate-120240416.0.8/substrate/__init__.py
+-rw-r--r--   0        0        0     6011 2024-04-19 01:10:51.026536 substrate-120240416.0.8/substrate/_client.py
+-rw-r--r--   0        0        0       30 2024-03-13 14:46:31.829473 substrate-120240416.0.8/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-04-19 01:11:58.982501 substrate-120240416.0.8/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-19 01:11:58.982373 substrate-120240416.0.8/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-04-19 01:11:58.982766 substrate-120240416.0.8/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-04-19 01:11:58.983463 substrate-120240416.0.8/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-19 01:11:58.983609 substrate-120240416.0.8/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-04-19 01:11:58.983753 substrate-120240416.0.8/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-04-19 01:11:58.983077 substrate-120240416.0.8/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-04-19 01:11:58.982639 substrate-120240416.0.8/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2138 2024-04-19 01:11:58.981556 substrate-120240416.0.8/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1227 2024-04-19 01:11:58.982867 substrate-120240416.0.8/substrate/core/future_directive.py
+-rw-r--r--   0        0        0      894 2024-04-19 01:11:58.981394 substrate-120240416.0.8/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    38416 2024-04-19 01:11:58.982121 substrate-120240416.0.8/substrate/core/models.py
+-rw-r--r--   0        0        0     2332 2024-04-19 01:11:58.981258 substrate-120240416.0.8/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-120240416.0.8/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    43544 2024-04-19 01:11:40.000000 substrate-120240416.0.8/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    41746 2024-04-19 01:11:41.000000 substrate-120240416.0.8/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-120240416.0.8/substrate/py.typed
+-rw-r--r--   0        0        0     1490 2024-04-16 20:07:00.739577 substrate-120240416.0.8/substrate/substrate.py
+-rw-r--r--   0        0        0     1034 2024-04-16 21:25:37.775283 substrate-120240416.0.8/substrate/substrate_response.py
+-rw-r--r--   0        0        0    34066 2024-04-19 01:11:39.000000 substrate-120240416.0.8/substrate/typeddict_models.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 substrate-120240416.0.8/PKG-INFO
```

### Comparing `substrate-120240416.0.7/LICENSE` & `substrate-120240416.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/pyproject.toml` & `substrate-120240416.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "120240416.0.7"
+version = "120240416.0.8"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-120240416.0.7/substrate/__init__.py` & `substrate-120240416.0.8/substrate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 ꩜ Substrate Python SDK
 
-20240416.20240416
+20240416.20240418
 """
 
 from .nodes import (
     CLIP,
     XTTSV2,
     JinaV2,
     BigLaMa,
```

### Comparing `substrate-120240416.0.7/substrate/_client.py` & `substrate-120240416.0.8/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/base_future.py` & `substrate-120240416.0.8/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/client/find_futures_client.py` & `substrate-120240416.0.8/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/client/future.py` & `substrate-120240416.0.8/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/client/graph.py` & `substrate-120240416.0.8/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/coregraph.py` & `substrate-120240416.0.8/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/corenode.py` & `substrate-120240416.0.8/substrate/core/corenode.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from .id_generator import IDGenerator
 from .client.future import TracedFuture
 from .future_directive import TraceDirective
 from .client.find_futures_client import find_futures_client
 
 
 class CoreNode:
-    def __init__(self, **attr):
+    def __init__(self, hide: bool = True, **attr):
         self.node = self.__class__.__name__
         self.args = attr
         generator_instance = IDGenerator.get_instance(self.__class__.__name__)
         self.id = generator_instance.get_next_id()
         self._global_output_keys = None
-        self._should_output_globally: bool = False
+        self._should_output_globally: bool = not hide
         self.SG = nx.DiGraph()
         if attr:
             self.args = BaseFuture.replace_futures_with_placeholder(attr)
         else:
             self.args = {}
         self.SG.add_node(self, **self.args)
         self.futures_from_args: List[BaseFuture] = find_futures_client(attr)
@@ -41,17 +41,14 @@
             "node": self.node,
             "args": self.args,
             **({"_should_output_globally": self._should_output_globally} if self._should_output_globally else {}),
             **({"_global_output_keys": self._global_output_keys} if self._global_output_keys else {}),
         }
 
     def subscribe(self, keys: Optional[List[str]] = None):
-        """
-        Subscribe to the output of this node.
-        """
         self._should_output_globally = True
         if keys:
             self._global_output_keys = keys
         return self
 
     @property
     def future(self) -> TracedFuture:
```

### Comparing `substrate-120240416.0.7/substrate/core/future_directive.py` & `substrate-120240416.0.8/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/id_generator.py` & `substrate-120240416.0.8/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/core/models.py` & `substrate-120240416.0.8/substrate/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
 
 class GenerateTextOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    text: Optional[str] = None
+    text: str
     """
     Text response.
     """
 
 
 class GenerateJSONIn(BaseModel):
     class Config:
@@ -89,15 +89,15 @@
     """
 
 
 class GenerateJSONOut(BaseModel):
     class Config:
         extra = Extra.allow
 
-    json_object: Optional[Dict[str, Any]] = None
+    json_object: Dict[str, Any]
     """
     JSON response.
     """
 
 
 class MultiGenerateTextIn(BaseModel):
     class Config:
```

### Comparing `substrate-120240416.0.7/substrate/core/sb.py` & `substrate-120240416.0.8/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/dataclass_models.py` & `substrate-120240416.0.8/substrate/dataclass_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateTextOut:
-    text: Optional[str] = None
+    text: str
     """
     Text response.
     """
 
 
 @dataclass
 class GenerateJSONIn:
@@ -78,15 +78,15 @@
     """
     Selected node.
     """
 
 
 @dataclass
 class GenerateJSONOut:
-    json_object: Optional[Dict[str, Any]] = None
+    json_object: Dict[str, Any]
     """
     JSON response.
     """
 
 
 @dataclass
 class MultiGenerateTextIn:
```

### Comparing `substrate-120240416.0.7/substrate/future_dataclass_models.py` & `substrate-120240416.0.8/substrate/future_dataclass_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 @dataclass
 class FutureGenerateTextOut:
     """
     (Future reference)
     """
 
-    text: Optional[str] = None
+    text: str
     """
     (Future reference)
     Text response.
     """
 
 
 @dataclass
@@ -111,15 +111,15 @@
 
 @dataclass
 class FutureGenerateJSONOut:
     """
     (Future reference)
     """
 
-    json_object: Optional[Dict[str, Any]] = None
+    json_object: Dict[str, Any]
     """
     (Future reference)
     JSON response.
     """
 
 
 @dataclass
```

### Comparing `substrate-120240416.0.7/substrate/nodes.py` & `substrate-120240416.0.8/substrate/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 ꩜ Substrate
 @GENERATED FILE
-20240416.20240416
+20240416.20240418
 """
 from typing import Type
 
-from .core.corenode import CoreNode
-from .dataclass_models import (
+from .core.models import (
     CLIPOut,
     JinaV2Out,
     XTTSV2Out,
     BigLaMaOut,
     DISISNetOut,
     FillMaskOut,
     EmbedTextOut,
@@ -44,14 +43,15 @@
     GenerativeEditImageOut,
     MultiGenerativeEditImageOut,
     StableDiffusionXLInpaintOut,
     StableDiffusionXLIPAdapterOut,
     StableDiffusionXLLightningOut,
     StableDiffusionXLControlNetOut,
 )
+from .core.corenode import CoreNode
 from .typeddict_models import (
     CLIPIn,
     JinaV2In,
     XTTSV2In,
     BigLaMaIn,
     DISISNetIn,
     FillMaskIn,
@@ -137,57 +137,57 @@
 class GenerateText(CoreNode):
     """
     Generate text using a language model.
 
     https://substrate.run/library#GenerateText
     """
 
-    def __init__(self, args: GenerateTextIn):
+    def __init__(self, args: GenerateTextIn, hide: bool = False):
         """
         Input arguments: `prompt`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.text` (optional)
+        Output fields: `future.text`
 
         https://substrate.run/library#GenerateText
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerateText"
 
     @property
     def out_type(self) -> Type[GenerateTextOut]:
         return GenerateTextOut
 
     @property
     def future(self) -> FutureGenerateTextOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.text` (optional)
+        Output fields: `future.text`
 
         https://substrate.run/library#GenerateText
         """
         return super().future  # type: ignore
 
 
 class MultiGenerateText(CoreNode):
     """
     Generate multiple text choices using a language model.
 
     https://substrate.run/library#MultiGenerateText
     """
 
-    def __init__(self, args: MultiGenerateTextIn):
+    def __init__(self, args: MultiGenerateTextIn, hide: bool = False):
         """
         Input arguments: `prompt` (optional), `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateText
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiGenerateText"
 
     @property
     def out_type(self) -> Type[MultiGenerateTextOut]:
         return MultiGenerateTextOut
 
     @property
@@ -205,57 +205,57 @@
 class GenerateJSON(CoreNode):
     """
     Generate JSON using a language model.
 
     https://substrate.run/library#GenerateJSON
     """
 
-    def __init__(self, args: GenerateJSONIn):
+    def __init__(self, args: GenerateJSONIn, hide: bool = False):
         """
         Input arguments: `prompt`, `json_schema`, `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
-        Output fields: `future.json_object` (optional)
+        Output fields: `future.json_object`
 
         https://substrate.run/library#GenerateJSON
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerateJSON"
 
     @property
     def out_type(self) -> Type[GenerateJSONOut]:
         return GenerateJSONOut
 
     @property
     def future(self) -> FutureGenerateJSONOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        Output fields: `future.json_object` (optional)
+        Output fields: `future.json_object`
 
         https://substrate.run/library#GenerateJSON
         """
         return super().future  # type: ignore
 
 
 class MultiGenerateJSON(CoreNode):
     """
     Generate multiple JSON choices using a language model.
 
     https://substrate.run/library#MultiGenerateJSON
     """
 
-    def __init__(self, args: MultiGenerateJSONIn):
+    def __init__(self, args: MultiGenerateJSONIn, hide: bool = False):
         """
         Input arguments: `prompt` (optional), `json_schema`, `batch_prompts` (optional), `num_choices` (optional), `temperature` (optional), `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateJSON
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiGenerateJSON"
 
     @property
     def out_type(self) -> Type[MultiGenerateJSONOut]:
         return MultiGenerateJSONOut
 
     @property
@@ -273,23 +273,23 @@
 class GenerateTextVision(CoreNode):
     """
     Generate text with image input.
 
     https://substrate.run/library#GenerateTextVision
     """
 
-    def __init__(self, args: GenerateTextVisionIn):
+    def __init__(self, args: GenerateTextVisionIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_uris`, `max_tokens` (optional), `node` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#GenerateTextVision
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerateTextVision"
 
     @property
     def out_type(self) -> Type[GenerateTextVisionOut]:
         return GenerateTextVisionOut
 
     @property
@@ -307,23 +307,23 @@
 class Mistral7BInstruct(CoreNode):
     """
     Generate text using [Mistral 7B Instruct](https://mistral.ai/news/announcing-mistral-7b).
 
     https://substrate.run/library#Mistral7BInstruct
     """
 
-    def __init__(self, args: Mistral7BInstructIn):
+    def __init__(self, args: Mistral7BInstructIn, hide: bool = False):
         """
         Input arguments: `prompt` (optional), `num_choices` (optional), `json_schema` (optional), `batch_prompts` (optional), `temperature` (optional), `max_tokens` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#Mistral7BInstruct
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "Mistral7BInstruct"
 
     @property
     def out_type(self) -> Type[Mistral7BInstructOut]:
         return Mistral7BInstructOut
 
     @property
@@ -341,23 +341,23 @@
 class Firellava13B(CoreNode):
     """
     Generate text with image input using [FireLLaVA 13B](https://fireworks.ai/blog/firellava-the-first-commercially-permissive-oss-llava-model).
 
     https://substrate.run/library#Firellava13B
     """
 
-    def __init__(self, args: Firellava13BIn):
+    def __init__(self, args: Firellava13BIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_uris`, `max_tokens` (optional)
 
         Output fields: `future.text`
 
         https://substrate.run/library#Firellava13B
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "Firellava13B"
 
     @property
     def out_type(self) -> Type[Firellava13BOut]:
         return Firellava13BOut
 
     @property
@@ -375,23 +375,23 @@
 class GenerateImage(CoreNode):
     """
     Generate an image.
 
     https://substrate.run/library#GenerateImage
     """
 
-    def __init__(self, args: GenerateImageIn):
+    def __init__(self, args: GenerateImageIn, hide: bool = False):
         """
         Input arguments: `prompt`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerateImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerateImage"
 
     @property
     def out_type(self) -> Type[GenerateImageOut]:
         return GenerateImageOut
 
     @property
@@ -409,23 +409,23 @@
 class MultiGenerateImage(CoreNode):
     """
     Generate multiple images.
 
     https://substrate.run/library#MultiGenerateImage
     """
 
-    def __init__(self, args: MultiGenerateImageIn):
+    def __init__(self, args: MultiGenerateImageIn, hide: bool = False):
         """
         Input arguments: `prompt`, `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerateImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiGenerateImage"
 
     @property
     def out_type(self) -> Type[MultiGenerateImageOut]:
         return MultiGenerateImageOut
 
     @property
@@ -443,23 +443,23 @@
 class GenerativeEditImage(CoreNode):
     """
     Edit an image using image generation.
 
     https://substrate.run/library#GenerativeEditImage
     """
 
-    def __init__(self, args: GenerativeEditImageIn):
+    def __init__(self, args: GenerativeEditImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#GenerativeEditImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerativeEditImage"
 
     @property
     def out_type(self) -> Type[GenerativeEditImageOut]:
         return GenerativeEditImageOut
 
     @property
@@ -477,23 +477,23 @@
 class MultiGenerativeEditImage(CoreNode):
     """
     Edit multiple images using image generation.
 
     https://substrate.run/library#MultiGenerativeEditImage
     """
 
-    def __init__(self, args: MultiGenerativeEditImageIn):
+    def __init__(self, args: MultiGenerativeEditImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `store` (optional), `node` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#MultiGenerativeEditImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiGenerativeEditImage"
 
     @property
     def out_type(self) -> Type[MultiGenerativeEditImageOut]:
         return MultiGenerativeEditImageOut
 
     @property
@@ -511,23 +511,23 @@
 class StableDiffusionXL(CoreNode):
     """
     Generate an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952).
 
     https://substrate.run/library#StableDiffusionXL
     """
 
-    def __init__(self, args: StableDiffusionXLIn):
+    def __init__(self, args: StableDiffusionXLIn, hide: bool = False):
         """
         Input arguments: `prompt`, `negative_prompt` (optional), `steps` (optional), `num_images`, `store` (optional), `height` (optional), `width` (optional), `seeds` (optional), `guidance_scale` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXL
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "StableDiffusionXL"
 
     @property
     def out_type(self) -> Type[StableDiffusionXLOut]:
         return StableDiffusionXLOut
 
     @property
@@ -545,23 +545,23 @@
 class StableDiffusionXLLightning(CoreNode):
     """
     Generate an image using [Stable Diffusion XL Lightning](https://arxiv.org/abs/2402.13929).
 
     https://substrate.run/library#StableDiffusionXLLightning
     """
 
-    def __init__(self, args: StableDiffusionXLLightningIn):
+    def __init__(self, args: StableDiffusionXLLightningIn, hide: bool = False):
         """
         Input arguments: `prompt`, `negative_prompt` (optional), `num_images` (optional), `store` (optional), `height` (optional), `width` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLLightning
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "StableDiffusionXLLightning"
 
     @property
     def out_type(self) -> Type[StableDiffusionXLLightningOut]:
         return StableDiffusionXLLightningOut
 
     @property
@@ -579,23 +579,23 @@
 class StableDiffusionXLInpaint(CoreNode):
     """
     Edit an image using [Stable Diffusion XL](https://arxiv.org/abs/2307.01952). Supports inpainting (edit part of the image with a mask) and image-to-image (edit the full image).
 
     https://substrate.run/library#StableDiffusionXLInpaint
     """
 
-    def __init__(self, args: StableDiffusionXLInpaintIn):
+    def __init__(self, args: StableDiffusionXLInpaintIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `prompt`, `mask_image_uri` (optional), `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `strength` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLInpaint
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "StableDiffusionXLInpaint"
 
     @property
     def out_type(self) -> Type[StableDiffusionXLInpaintOut]:
         return StableDiffusionXLInpaintOut
 
     @property
@@ -613,23 +613,23 @@
 class StableDiffusionXLControlNet(CoreNode):
     """
     Generate an image with generation structured by an input image, using Stable Diffusion XL with [ControlNet](https://arxiv.org/abs/2302.05543).
 
     https://substrate.run/library#StableDiffusionXLControlNet
     """
 
-    def __init__(self, args: StableDiffusionXLControlNetIn):
+    def __init__(self, args: StableDiffusionXLControlNetIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `control_method`, `prompt`, `num_images`, `output_resolution` (optional), `negative_prompt` (optional), `store` (optional), `conditioning_scale` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLControlNet
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "StableDiffusionXLControlNet"
 
     @property
     def out_type(self) -> Type[StableDiffusionXLControlNetOut]:
         return StableDiffusionXLControlNetOut
 
     @property
@@ -647,23 +647,23 @@
 class StableDiffusionXLIPAdapter(CoreNode):
     """
     Generate an image with an image prompt, using Stable Diffusion XL with [IP-Adapter](https://arxiv.org/abs/2308.06721).
 
     https://substrate.run/library#StableDiffusionXLIPAdapter
     """
 
-    def __init__(self, args: StableDiffusionXLIPAdapterIn):
+    def __init__(self, args: StableDiffusionXLIPAdapterIn, hide: bool = False):
         """
         Input arguments: `prompt`, `image_prompt_uri` (optional), `num_images`, `ip_adapter_scale` (optional), `negative_prompt` (optional), `store` (optional), `width` (optional), `height` (optional), `seeds` (optional)
 
         Output fields: `future.outputs`
 
         https://substrate.run/library#StableDiffusionXLIPAdapter
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "StableDiffusionXLIPAdapter"
 
     @property
     def out_type(self) -> Type[StableDiffusionXLIPAdapterOut]:
         return StableDiffusionXLIPAdapterOut
 
     @property
@@ -681,23 +681,23 @@
 class TranscribeMedia(CoreNode):
     """
     Transcribe speech in an audio or video file.
 
     https://substrate.run/library#TranscribeMedia
     """
 
-    def __init__(self, args: TranscribeMediaIn):
+    def __init__(self, args: TranscribeMediaIn, hide: bool = False):
         """
         Input arguments: `audio_uri`, `prompt` (optional), `language` (optional), `segment` (optional), `align` (optional), `diarize` (optional), `suggest_chapters` (optional)
 
         Output fields: `future.text`, `future.segments` (optional), `future.chapters` (optional)
 
         https://substrate.run/library#TranscribeMedia
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "TranscribeMedia"
 
     @property
     def out_type(self) -> Type[TranscribeMediaOut]:
         return TranscribeMediaOut
 
     @property
@@ -715,23 +715,23 @@
 class GenerateSpeech(CoreNode):
     """
     Generate speech from text.
 
     https://substrate.run/library#GenerateSpeech
     """
 
-    def __init__(self, args: GenerateSpeechIn):
+    def __init__(self, args: GenerateSpeechIn, hide: bool = False):
         """
         Input arguments: `text`, `store` (optional), `node` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#GenerateSpeech
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "GenerateSpeech"
 
     @property
     def out_type(self) -> Type[GenerateSpeechOut]:
         return GenerateSpeechOut
 
     @property
@@ -749,23 +749,23 @@
 class XTTSV2(CoreNode):
     """
     Generate speech from text using [XTTS v2](https://docs.coqui.ai/en/latest/models/xtts.html).
 
     https://substrate.run/library#XTTSV2
     """
 
-    def __init__(self, args: XTTSV2In):
+    def __init__(self, args: XTTSV2In, hide: bool = False):
         """
         Input arguments: `text`, `audio_uri` (optional), `language` (optional), `store` (optional)
 
         Output fields: `future.audio_uri`
 
         https://substrate.run/library#XTTSV2
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "XTTSV2"
 
     @property
     def out_type(self) -> Type[XTTSV2Out]:
         return XTTSV2Out
 
     @property
@@ -783,23 +783,23 @@
 class RemoveBackground(CoreNode):
     """
     Remove the background from an image, with the option to return the foreground as a mask.
 
     https://substrate.run/library#RemoveBackground
     """
 
-    def __init__(self, args: RemoveBackgroundIn):
+    def __init__(self, args: RemoveBackgroundIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `return_mask` (optional), `background_color` (optional), `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RemoveBackground
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "RemoveBackground"
 
     @property
     def out_type(self) -> Type[RemoveBackgroundOut]:
         return RemoveBackgroundOut
 
     @property
@@ -817,23 +817,23 @@
 class FillMask(CoreNode):
     """
     Fill (inpaint) part of an image, e.g. to 'remove' an object.
 
     https://substrate.run/library#FillMask
     """
 
-    def __init__(self, args: FillMaskIn):
+    def __init__(self, args: FillMaskIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `mask_image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#FillMask
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "FillMask"
 
     @property
     def out_type(self) -> Type[FillMaskOut]:
         return FillMaskOut
 
     @property
@@ -851,23 +851,23 @@
 class UpscaleImage(CoreNode):
     """
     Upscale an image.
 
     https://substrate.run/library#UpscaleImage
     """
 
-    def __init__(self, args: UpscaleImageIn):
+    def __init__(self, args: UpscaleImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional), `node` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#UpscaleImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "UpscaleImage"
 
     @property
     def out_type(self) -> Type[UpscaleImageOut]:
         return UpscaleImageOut
 
     @property
@@ -885,23 +885,23 @@
 class SegmentUnderPoint(CoreNode):
     """
     Segment an image under a point and return the segment.
 
     https://substrate.run/library#SegmentUnderPoint
     """
 
-    def __init__(self, args: SegmentUnderPointIn):
+    def __init__(self, args: SegmentUnderPointIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `point`, `store` (optional), `node` (optional)
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentUnderPoint
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "SegmentUnderPoint"
 
     @property
     def out_type(self) -> Type[SegmentUnderPointOut]:
         return SegmentUnderPointOut
 
     @property
@@ -919,23 +919,23 @@
 class DISISNet(CoreNode):
     """
     Segment image foreground using [DIS IS-Net](https://github.com/xuebinqin/DIS).
 
     https://substrate.run/library#DISISNet
     """
 
-    def __init__(self, args: DISISNetIn):
+    def __init__(self, args: DISISNetIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#DISISNet
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "DISISNet"
 
     @property
     def out_type(self) -> Type[DISISNetOut]:
         return DISISNetOut
 
     @property
@@ -953,23 +953,23 @@
 class BigLaMa(CoreNode):
     """
     Inpaint a mask using [LaMa](https://github.com/advimman/lama).
 
     https://substrate.run/library#BigLaMa
     """
 
-    def __init__(self, args: BigLaMaIn):
+    def __init__(self, args: BigLaMaIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `mask_image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#BigLaMa
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "BigLaMa"
 
     @property
     def out_type(self) -> Type[BigLaMaOut]:
         return BigLaMaOut
 
     @property
@@ -987,23 +987,23 @@
 class RealESRGAN(CoreNode):
     """
     Upscale an image using [RealESRGAN](https://github.com/xinntao/Real-ESRGAN).
 
     https://substrate.run/library#RealESRGAN
     """
 
-    def __init__(self, args: RealESRGANIn):
+    def __init__(self, args: RealESRGANIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional)
 
         Output fields: `future.image_uri`
 
         https://substrate.run/library#RealESRGAN
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "RealESRGAN"
 
     @property
     def out_type(self) -> Type[RealESRGANOut]:
         return RealESRGANOut
 
     @property
@@ -1021,23 +1021,23 @@
 class SegmentAnything(CoreNode):
     """
     Segment an image using [SegmentAnything](https://github.com/facebookresearch/segment-anything).
 
     https://substrate.run/library#SegmentAnything
     """
 
-    def __init__(self, args: SegmentAnythingIn):
+    def __init__(self, args: SegmentAnythingIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `point_prompts` (optional), `box_prompts` (optional), `store` (optional)
 
         Output fields: `future.mask_image_uri`
 
         https://substrate.run/library#SegmentAnything
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "SegmentAnything"
 
     @property
     def out_type(self) -> Type[SegmentAnythingOut]:
         return SegmentAnythingOut
 
     @property
@@ -1055,23 +1055,23 @@
 class EmbedText(CoreNode):
     """
     Generate embedding for a text document.
 
     https://substrate.run/library#EmbedText
     """
 
-    def __init__(self, args: EmbedTextIn):
+    def __init__(self, args: EmbedTextIn, hide: bool = False):
         """
         Input arguments: `text`, `store` (optional), `metadata` (optional), `embedded_metadata_keys` (optional), `doc_id` (optional), `node` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedText
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "EmbedText"
 
     @property
     def out_type(self) -> Type[EmbedTextOut]:
         return EmbedTextOut
 
     @property
@@ -1089,23 +1089,23 @@
 class MultiEmbedText(CoreNode):
     """
     Generate embeddings for multiple text documents.
 
     https://substrate.run/library#MultiEmbedText
     """
 
-    def __init__(self, args: MultiEmbedTextIn):
+    def __init__(self, args: MultiEmbedTextIn, hide: bool = False):
         """
         Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional), `node` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedText
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiEmbedText"
 
     @property
     def out_type(self) -> Type[MultiEmbedTextOut]:
         return MultiEmbedTextOut
 
     @property
@@ -1123,23 +1123,23 @@
 class EmbedImage(CoreNode):
     """
     Generate embedding for an image.
 
     https://substrate.run/library#EmbedImage
     """
 
-    def __init__(self, args: EmbedImageIn):
+    def __init__(self, args: EmbedImageIn, hide: bool = False):
         """
         Input arguments: `image_uri`, `store` (optional), `doc_id` (optional), `node` (optional)
 
         Output fields: `future.embedding`
 
         https://substrate.run/library#EmbedImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "EmbedImage"
 
     @property
     def out_type(self) -> Type[EmbedImageOut]:
         return EmbedImageOut
 
     @property
@@ -1157,23 +1157,23 @@
 class MultiEmbedImage(CoreNode):
     """
     Generate embeddings for multiple images.
 
     https://substrate.run/library#MultiEmbedImage
     """
 
-    def __init__(self, args: MultiEmbedImageIn):
+    def __init__(self, args: MultiEmbedImageIn, hide: bool = False):
         """
         Input arguments: `items`, `store` (optional), `node` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#MultiEmbedImage
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "MultiEmbedImage"
 
     @property
     def out_type(self) -> Type[MultiEmbedImageOut]:
         return MultiEmbedImageOut
 
     @property
@@ -1191,23 +1191,23 @@
 class JinaV2(CoreNode):
     """
     Generate embeddings for multiple text documents using [Jina Embeddings 2](https://arxiv.org/abs/2310.19923).
 
     https://substrate.run/library#JinaV2
     """
 
-    def __init__(self, args: JinaV2In):
+    def __init__(self, args: JinaV2In, hide: bool = False):
         """
         Input arguments: `items`, `store` (optional), `embedded_metadata_keys` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#JinaV2
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "JinaV2"
 
     @property
     def out_type(self) -> Type[JinaV2Out]:
         return JinaV2Out
 
     @property
@@ -1225,23 +1225,23 @@
 class CLIP(CoreNode):
     """
     Generate embeddings for text or images using [CLIP](https://openai.com/research/clip).
 
     https://substrate.run/library#CLIP
     """
 
-    def __init__(self, args: CLIPIn):
+    def __init__(self, args: CLIPIn, hide: bool = False):
         """
         Input arguments: `items`, `store` (optional)
 
         Output fields: `future.embeddings`
 
         https://substrate.run/library#CLIP
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "CLIP"
 
     @property
     def out_type(self) -> Type[CLIPOut]:
         return CLIPOut
 
     @property
@@ -1259,23 +1259,23 @@
 class CreateVectorStore(CoreNode):
     """
     Create a vector store for storing and querying embeddings.
 
     https://substrate.run/library#CreateVectorStore
     """
 
-    def __init__(self, args: CreateVectorStoreIn):
+    def __init__(self, args: CreateVectorStoreIn, hide: bool = False):
         """
         Input arguments: `name`, `model`, `m` (optional), `ef_construction` (optional), `metric` (optional)
 
         Output fields: `future.name`, `future.model`, `future.m`, `future.ef_construction`, `future.metric`
 
         https://substrate.run/library#CreateVectorStore
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "CreateVectorStore"
 
     @property
     def out_type(self) -> Type[CreateVectorStoreOut]:
         return CreateVectorStoreOut
 
     @property
@@ -1293,23 +1293,23 @@
 class ListVectorStores(CoreNode):
     """
     List all vector stores.
 
     https://substrate.run/library#ListVectorStores
     """
 
-    def __init__(self, args: ListVectorStoresIn):
+    def __init__(self, args: ListVectorStoresIn, hide: bool = False):
         """
         Input arguments:
 
         Output fields: `future.stores` (optional)
 
         https://substrate.run/library#ListVectorStores
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "ListVectorStores"
 
     @property
     def out_type(self) -> Type[ListVectorStoresOut]:
         return ListVectorStoresOut
 
     @property
@@ -1327,23 +1327,23 @@
 class DeleteVectorStore(CoreNode):
     """
     Delete a vector store.
 
     https://substrate.run/library#DeleteVectorStore
     """
 
-    def __init__(self, args: DeleteVectorStoreIn):
+    def __init__(self, args: DeleteVectorStoreIn, hide: bool = False):
         """
         Input arguments: `name`, `model`
 
         Output fields: `future.name`, `future.model`
 
         https://substrate.run/library#DeleteVectorStore
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "DeleteVectorStore"
 
     @property
     def out_type(self) -> Type[DeleteVectorStoreOut]:
         return DeleteVectorStoreOut
 
     @property
@@ -1361,23 +1361,23 @@
 class QueryVectorStore(CoreNode):
     """
     Query a vector store for similar vectors.
 
     https://substrate.run/library#QueryVectorStore
     """
 
-    def __init__(self, args: QueryVectorStoreIn):
+    def __init__(self, args: QueryVectorStoreIn, hide: bool = False):
         """
         Input arguments: `name`, `model`, `query_strings` (optional), `query_image_uris` (optional), `query_vectors` (optional), `query_ids` (optional), `top_k` (optional), `ef_search` (optional), `include_values` (optional), `include_metadata` (optional), `filters` (optional), `metric` (optional)
 
         Output fields: `future.results`, `future.name` (optional), `future.model` (optional), `future.metric` (optional)
 
         https://substrate.run/library#QueryVectorStore
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "QueryVectorStore"
 
     @property
     def out_type(self) -> Type[QueryVectorStoreOut]:
         return QueryVectorStoreOut
 
     @property
@@ -1395,23 +1395,23 @@
 class FetchVectors(CoreNode):
     """
     Fetch vectors from a vector store.
 
     https://substrate.run/library#FetchVectors
     """
 
-    def __init__(self, args: FetchVectorsIn):
+    def __init__(self, args: FetchVectorsIn, hide: bool = False):
         """
         Input arguments: `name`, `model`, `ids`
 
         Output fields: `future.vectors`
 
         https://substrate.run/library#FetchVectors
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "FetchVectors"
 
     @property
     def out_type(self) -> Type[FetchVectorsOut]:
         return FetchVectorsOut
 
     @property
@@ -1429,23 +1429,23 @@
 class UpdateVectors(CoreNode):
     """
     Update vectors in a vector store.
 
     https://substrate.run/library#UpdateVectors
     """
 
-    def __init__(self, args: UpdateVectorsIn):
+    def __init__(self, args: UpdateVectorsIn, hide: bool = False):
         """
         Input arguments: `name`, `model`, `vectors`
 
         Output fields: `future.count`
 
         https://substrate.run/library#UpdateVectors
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "UpdateVectors"
 
     @property
     def out_type(self) -> Type[UpdateVectorsOut]:
         return UpdateVectorsOut
 
     @property
@@ -1463,23 +1463,23 @@
 class DeleteVectors(CoreNode):
     """
     Delete vectors in a vector store.
 
     https://substrate.run/library#DeleteVectors
     """
 
-    def __init__(self, args: DeleteVectorsIn):
+    def __init__(self, args: DeleteVectorsIn, hide: bool = False):
         """
         Input arguments: `name`, `model`, `ids`
 
         Output fields: `future.count`
 
         https://substrate.run/library#DeleteVectors
         """
-        super().__init__(**args)
+        super().__init__(hide=hide, **args)
         self.node = "DeleteVectors"
 
     @property
     def out_type(self) -> Type[DeleteVectorsOut]:
         return DeleteVectorsOut
 
     @property
```

### Comparing `substrate-120240416.0.7/substrate/substrate.py` & `substrate-120240416.0.8/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/substrate/substrate_response.py` & `substrate-120240416.0.8/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-120240416.0.7/PKG-INFO` & `substrate-120240416.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 120240416.0.7
+Version: 120240416.0.8
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

