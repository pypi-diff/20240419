# Comparing `tmp/vision_agent-0.1.3.tar.gz` & `tmp/vision_agent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.1.3.tar", max compression
+gzip compressed data, was "vision_agent-0.1.4.tar", max compression
```

## Comparing `vision_agent-0.1.3.tar` & `vision_agent-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-04-17 21:55:12.665652 vision_agent-0.1.3/LICENSE
--rw-r--r--   0        0        0     5035 2024-04-17 21:55:12.665652 vision_agent-0.1.3/README.md
--rw-r--r--   0        0        0     2219 2024-04-17 21:55:13.241650 vision_agent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    22019 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0       46 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/data/__init__.py
--rw-r--r--   0        0        0     5128 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/data/data.py
--rw-r--r--   0        0        0       75 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/emb/__init__.py
--rw-r--r--   0        0        0     1375 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/emb/emb.py
--rw-r--r--   0        0        0        0 2024-04-17 21:55:12.677652 vision_agent-0.1.3/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     4786 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5016 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-17 21:55:12.685652 vision_agent-0.1.3/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10045 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      269 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    25410 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-17 21:55:12.689652 vision_agent-0.1.3/vision_agent/type_defs.py
--rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 vision_agent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-19 15:24:22.698770 vision_agent-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5035 2024-04-19 15:24:22.698770 vision_agent-0.1.4/README.md
+-rw-r--r--   0        0        0     2219 2024-04-19 15:24:23.438772 vision_agent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    22735 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0       46 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/data/__init__.py
+-rw-r--r--   0        0        0     5128 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/data/data.py
+-rw-r--r--   0        0        0       75 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/emb/__init__.py
+-rw-r--r--   0        0        0     1375 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/emb/emb.py
+-rw-r--r--   0        0        0        0 2024-04-19 15:24:22.710770 vision_agent-0.1.4/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     4805 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10045 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      280 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    29148 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-19 15:24:22.722770 vision_agent-0.1.4/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     6233 1970-01-01 00:00:00.000000 vision_agent-0.1.4/PKG-INFO
```

### Comparing `vision_agent-0.1.3/LICENSE` & `vision_agent-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/README.md` & `vision_agent-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/pyproject.toml` & `vision_agent-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.1.3"
+version = "0.1.4"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.1.3/vision_agent/agent/agent.py` & `vision_agent-0.1.4/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/agent/easytool.py` & `vision_agent-0.1.4/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.1.4/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/agent/reflexion.py` & `vision_agent-0.1.4/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.1.4/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/agent/vision_agent.py` & `vision_agent-0.1.4/vision_agent/agent/vision_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,14 +361,15 @@
     image_to_data: Dict[str, Dict] = {}
     for tool_result in all_tool_results:
         # only handle bbox/mask tools or frame extraction
         if tool_result["tool_name"] not in [
             "grounding_sam_",
             "grounding_dino_",
             "extract_frames_",
+            "dinov_",
         ]:
             continue
 
         if tool_result["tool_name"] == "extract_frames_":
             image_to_data = _handle_extract_frames(image_to_data, tool_result)
         else:
             image_to_data = _handle_viz_tools(image_to_data, tool_result)
@@ -440,44 +441,57 @@
         if verbose:
             _LOGGER.setLevel(logging.INFO)
 
     def __call__(
         self,
         input: Union[List[Dict[str, str]], str],
         image: Optional[Union[str, Path]] = None,
+        reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> str:
         """Invoke the vision agent.
 
         Parameters:
             input: a prompt that describe the task or a conversation in the format of
                 [{"role": "user", "content": "describe your task here..."}].
             image: the input image referenced in the prompt parameter.
 
         Returns:
             The result of the vision agent in text.
         """
         if isinstance(input, str):
             input = [{"role": "user", "content": input}]
-        return self.chat(input, image=image, visualize_output=visualize_output)
+        return self.chat(
+            input,
+            image=image,
+            visualize_output=visualize_output,
+            reference_data=reference_data,
+        )
 
     def log_progress(self, description: str) -> None:
         _LOGGER.info(description)
         if self.report_progress_callback:
             self.report_progress_callback(description)
 
     def chat_with_workflow(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
+        reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> Tuple[str, List[Dict]]:
         question = chat[0]["content"]
         if image:
             question += f" Image name: {image}"
+        if reference_data:
+            if not ("image" in reference_data and "mask" in reference_data):
+                raise ValueError(
+                    f"Reference data must contain 'image' and 'mask'. but got {reference_data}"
+                )
+            question += f" Reference image: {reference_data['image']}, Reference mask: {reference_data['mask']}"
 
         reflections = ""
         final_answer = ""
         all_tool_results: List[Dict] = []
 
         for _ in range(self.max_retries):
             task_list = self.create_tasks(
@@ -551,18 +565,22 @@
 
         return final_answer, all_tool_results
 
     def chat(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
+        reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> str:
         answer, _ = self.chat_with_workflow(
-            chat, image=image, visualize_output=visualize_output
+            chat,
+            image=image,
+            visualize_output=visualize_output,
+            reference_data=reference_data,
         )
         return answer
 
     def retrieval(
         self,
         model: Union[LLM, LMM, Agent],
         question: str,
```

### Comparing `vision_agent-0.1.3/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.1.4/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/data/data.py` & `vision_agent-0.1.4/vision_agent/data/data.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/emb/emb.py` & `vision_agent-0.1.4/vision_agent/emb/emb.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.1.4/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/image_utils.py` & `vision_agent-0.1.4/vision_agent/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
         The image with the bounding boxes overlayed
     """
     if isinstance(image, (str, Path)):
         image = Image.open(image)
     elif isinstance(image, np.ndarray):
         image = Image.fromarray(image)
 
-    color = {label: COLORS[i % len(COLORS)] for i, label in enumerate(bboxes["labels"])}
+    color = {
+        label: COLORS[i % len(COLORS)] for i, label in enumerate(set(bboxes["labels"]))
+    }
 
     width, height = image.size
     fontsize = max(12, int(min(width, height) / 40))
     draw = ImageDraw.Draw(image)
     font = ImageFont.truetype(
         str(resources.files("vision_agent.fonts").joinpath("default_font_ch_en.ttf")),
         fontsize,
```

### Comparing `vision_agent-0.1.3/vision_agent/llm/llm.py` & `vision_agent-0.1.4/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/lmm/lmm.py` & `vision_agent-0.1.4/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/tools/prompts.py` & `vision_agent-0.1.4/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/tools/tools.py` & `vision_agent-0.1.4/vision_agent/tools/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -368,14 +368,112 @@
                 for mask in data["masks"]
             ]
         ret_pred["labels"] = data["labels"]
         ret_pred["scores"] = data["scores"]
         return ret_pred
 
 
+class DINOv(Tool):
+    r"""DINOv is a tool that can detect and segment similar objects with the given input masks.
+
+    Example
+    -------
+        >>> import vision_agent as va
+        >>> t = va.tools.DINOv()
+        >>> t(prompt=[{"mask":"balloon_mask.jpg", "image": "balloon.jpg"}], image="balloon.jpg"])
+        [{'scores': [0.512, 0.212],
+        'masks': [array([[0, 0, 0, ..., 0, 0, 0],
+           ...,
+           [0, 0, 0, ..., 0, 0, 0]], dtype=uint8)},
+        array([[0, 0, 0, ..., 0, 0, 0],
+           ...,
+           [1, 1, 1, ..., 1, 1, 1]], dtype=uint8)]}]
+    """
+
+    name = "dinov_"
+    description = "'dinov_' is a tool that can detect and segment similar objects given a reference segmentation mask."
+    usage = {
+        "required_parameters": [
+            {"name": "prompt", "type": "List[Dict[str, str]]"},
+            {"name": "image", "type": "str"},
+        ],
+        "examples": [
+            {
+                "scenario": "Can you find all the balloons in this image that is similar to the provided masked area? Image name: input.jpg Reference image: balloon.jpg Reference mask: balloon_mask.jpg",
+                "parameters": {
+                    "prompt": [
+                        {"mask": "balloon_mask.jpg", "image": "balloon.jpg"},
+                    ],
+                    "image": "input.jpg",
+                },
+            },
+            {
+                "scenario": "Detect all the objects in this image that are similar to the provided mask. Image name: original.jpg Reference image: mask.png Reference mask: background.png",
+                "parameters": {
+                    "prompt": [
+                        {"mask": "mask.png", "image": "background.png"},
+                    ],
+                    "image": "original.jpg",
+                },
+            },
+        ],
+    }
+
+    def __call__(
+        self, prompt: List[Dict[str, str]], image: Union[str, ImageType]
+    ) -> Dict:
+        """Invoke the DINOv model.
+
+        Parameters:
+            prompt: a list of visual prompts in the form of {'mask': 'MASK_FILE_PATH', 'image': 'IMAGE_FILE_PATH'}.
+            image: the input image to segment.
+
+        Returns:
+            A dictionary of the below keys: 'scores', 'masks' and 'mask_shape', which stores a list of detected segmentation masks and its scores.
+        """
+        image_b64 = convert_to_b64(image)
+        for p in prompt:
+            p["mask"] = convert_to_b64(p["mask"])
+            p["image"] = convert_to_b64(p["image"])
+        request_data = {
+            "prompt": prompt,
+            "image": image_b64,
+            "tool": "dinov",
+        }
+        data: Dict[str, Any] = _send_inference_request(request_data, "dinov")
+        if "bboxes" in data:
+            data["bboxes"] = [
+                normalize_bbox(box, data["mask_shape"]) for box in data["bboxes"]
+            ]
+        if "masks" in data:
+            data["masks"] = [
+                rle_decode(mask_rle=mask, shape=data["mask_shape"])
+                for mask in data["masks"]
+            ]
+        data["labels"] = ["visual prompt" for _ in range(len(data["masks"]))]
+        return data
+
+
+class AgentDINOv(DINOv):
+    def __call__(
+        self,
+        prompt: List[Dict[str, str]],
+        image: Union[str, ImageType],
+    ) -> Dict:
+        rets = super().__call__(prompt, image)
+        mask_files = []
+        for mask in rets["masks"]:
+            with tempfile.NamedTemporaryFile(suffix=".png", delete=False) as tmp:
+                file_name = Path(tmp.name).with_suffix(".mask.png")
+                Image.fromarray(mask * 255).save(file_name)
+                mask_files.append(str(file_name))
+        rets["masks"] = mask_files
+        return rets
+
+
 class AgentGroundingSAM(GroundingSAM):
     r"""AgentGroundingSAM is the same as GroundingSAM but it saves the masks as files
     returns the file name. This makes it easier for agents to use.
     """
 
     def __call__(
         self,
@@ -648,14 +746,15 @@
     for i, c in enumerate(
         [
             NoOp,
             CLIP,
             ImageCaption,
             GroundingDINO,
             AgentGroundingSAM,
+            AgentDINOv,
             ExtractFrames,
             Crop,
             BboxArea,
             SegArea,
             BboxIoU,
             SegIoU,
             BoxDistance,
```

### Comparing `vision_agent-0.1.3/vision_agent/tools/video.py` & `vision_agent-0.1.4/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/vision_agent/type_defs.py` & `vision_agent-0.1.4/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.1.3/PKG-INFO` & `vision_agent-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.1.3
+Version: 0.1.4
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

