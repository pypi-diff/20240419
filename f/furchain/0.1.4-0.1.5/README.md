# Comparing `tmp/furchain-0.1.4.tar.gz` & `tmp/furchain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furchain-0.1.4.tar", max compression
+gzip compressed data, was "furchain-0.1.5.tar", max compression
```

## Comparing `furchain-0.1.4.tar` & `furchain-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     3207 2024-04-14 09:13:42.783499 furchain-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.783499 furchain-0.1.4/furchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.783499 furchain-0.1.4/furchain/audio/__init__.py
--rw-r--r--   0        0        0       59 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/__init__.py
--rw-r--r--   0        0        0      751 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/gpt_sovits_vc.py
--rw-r--r--   0        0        0     3282 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/rvc.py
--rw-r--r--   0        0        0     1047 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/conversion/sovits.py
--rw-r--r--   0        0        0     3943 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/schema.py
--rw-r--r--   0        0        0       34 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/speech/__init__.py
--rw-r--r--   0        0        0     3716 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/speech/gpt_sovits.py
--rw-r--r--   0        0        0       27 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/transcriptions/__init__.py
--rw-r--r--   0        0        0    10530 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/transcriptions/funasr.py
--rw-r--r--   0        0        0      230 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/__init__.py
--rw-r--r--   0        0        0     3141 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_editor.py
--rw-r--r--   0        0        0     3872 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_iterator.py
--rw-r--r--   0        0        0     3097 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/audio_separator.py
--rw-r--r--   0        0        0     2491 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/convert.py
--rw-r--r--   0        0        0      897 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/get_format.py
--rw-r--r--   0        0        0     3557 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/microphone.py
--rw-r--r--   0        0        0     2136 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/audio/utils/play.py
--rw-r--r--   0        0        0     2009 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/config.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/captions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/generation/__init__.py
--rw-r--r--   0        0        0      881 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/generation/stable_diffusion_webui.py
--rw-r--r--   0        0        0      127 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/image/schema.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/__init__.py
--rw-r--r--   0        0        0     6710 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/actions.py
--rw-r--r--   0        0        0     1647 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/schema.py
--rw-r--r--   0        0        0     3171 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/interaction/tools.py
--rw-r--r--   0        0        0     2796 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/logger.py
--rw-r--r--   0        0        0      101 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/__init__.py
--rw-r--r--   0        0        0     2314 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/callbacks.py
--rw-r--r--   0        0        0    14081 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_format.py
--rw-r--r--   0        0        0     7241 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_message_history.py
--rw-r--r--   0        0        0     6789 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/chat_prompt_templates.py
--rw-r--r--   0        0        0      615 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/grammars.py
--rw-r--r--   0        0        0     4297 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/llama_cpp_client.py
--rw-r--r--   0        0        0     2779 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/output_parsers.py
--rw-r--r--   0        0        0    53992 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/text/schema.py
--rw-r--r--   0        0        0        0 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/__init__.py
--rw-r--r--   0        0        0     3208 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/broadcaster.py
--rw-r--r--   0        0        0     1998 2024-04-14 09:13:42.787500 furchain-0.1.4/furchain/utils/iterator.py
--rw-r--r--   0        0        0     1029 2024-04-14 09:13:42.787500 furchain-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 furchain-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3207 2024-04-19 13:10:15.247239 furchain-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/conversion/__init__.py
+-rw-r--r--   0        0        0      751 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/conversion/gpt_sovits_vc.py
+-rw-r--r--   0        0        0     3282 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/conversion/rvc.py
+-rw-r--r--   0        0        0     1047 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/conversion/sovits.py
+-rw-r--r--   0        0        0     3943 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/schema.py
+-rw-r--r--   0        0        0       34 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/speech/__init__.py
+-rw-r--r--   0        0        0     3716 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/speech/gpt_sovits.py
+-rw-r--r--   0        0        0       27 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/transcriptions/__init__.py
+-rw-r--r--   0        0        0    10530 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/transcriptions/funasr.py
+-rw-r--r--   0        0        0      230 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/__init__.py
+-rw-r--r--   0        0        0     3141 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/audio_editor.py
+-rw-r--r--   0        0        0     3872 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/audio_iterator.py
+-rw-r--r--   0        0        0     3097 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/audio_separator.py
+-rw-r--r--   0        0        0     2491 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/convert.py
+-rw-r--r--   0        0        0      897 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/get_format.py
+-rw-r--r--   0        0        0     3557 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/microphone.py
+-rw-r--r--   0        0        0     2136 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/audio/utils/play.py
+-rw-r--r--   0        0        0     2009 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/config.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.247239 furchain-0.1.5/furchain/image/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/image/captions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/image/generation/__init__.py
+-rw-r--r--   0        0        0      881 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/image/generation/stable_diffusion_webui.py
+-rw-r--r--   0        0        0      127 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/image/schema.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/interaction/__init__.py
+-rw-r--r--   0        0        0     6710 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/interaction/actions.py
+-rw-r--r--   0        0        0     1647 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/interaction/schema.py
+-rw-r--r--   0        0        0     3171 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/interaction/tools.py
+-rw-r--r--   0        0        0     2796 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/logger.py
+-rw-r--r--   0        0        0      101 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/__init__.py
+-rw-r--r--   0        0        0     2314 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/callbacks.py
+-rw-r--r--   0        0        0    15900 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/chat_format.py
+-rw-r--r--   0        0        0     7241 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/chat_message_history.py
+-rw-r--r--   0        0        0     6789 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/chat_prompt_templates.py
+-rw-r--r--   0        0        0      615 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/grammars.py
+-rw-r--r--   0        0        0     4297 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/llama_cpp_client.py
+-rw-r--r--   0        0        0     2779 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/output_parsers.py
+-rw-r--r--   0        0        0    53992 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/text/schema.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/utils/__init__.py
+-rw-r--r--   0        0        0     3208 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/utils/broadcaster.py
+-rw-r--r--   0        0        0     1998 2024-04-19 13:10:15.251239 furchain-0.1.5/furchain/utils/iterator.py
+-rw-r--r--   0        0        0     1092 2024-04-19 13:10:15.251239 furchain-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 furchain-0.1.5/PKG-INFO
```

### Comparing `furchain-0.1.4/README.md` & `furchain-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/conversion/gpt_sovits_vc.py` & `furchain-0.1.5/furchain/audio/conversion/gpt_sovits_vc.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/conversion/rvc.py` & `furchain-0.1.5/furchain/audio/conversion/rvc.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/conversion/sovits.py` & `furchain-0.1.5/furchain/audio/conversion/sovits.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/schema.py` & `furchain-0.1.5/furchain/audio/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/speech/gpt_sovits.py` & `furchain-0.1.5/furchain/audio/speech/gpt_sovits.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/transcriptions/funasr.py` & `furchain-0.1.5/furchain/audio/transcriptions/funasr.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/audio_editor.py` & `furchain-0.1.5/furchain/audio/utils/audio_editor.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/audio_iterator.py` & `furchain-0.1.5/furchain/audio/utils/audio_iterator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/audio_separator.py` & `furchain-0.1.5/furchain/audio/utils/audio_separator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/convert.py` & `furchain-0.1.5/furchain/audio/utils/convert.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/get_format.py` & `furchain-0.1.5/furchain/audio/utils/get_format.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/microphone.py` & `furchain-0.1.5/furchain/audio/utils/microphone.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/audio/utils/play.py` & `furchain-0.1.5/furchain/audio/utils/play.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/config.py` & `furchain-0.1.5/furchain/config.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/image/generation/stable_diffusion_webui.py` & `furchain-0.1.5/furchain/image/generation/stable_diffusion_webui.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/interaction/actions.py` & `furchain-0.1.5/furchain/interaction/actions.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/interaction/schema.py` & `furchain-0.1.5/furchain/interaction/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/interaction/tools.py` & `furchain-0.1.5/furchain/interaction/tools.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/logger.py` & `furchain-0.1.5/furchain/logger.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/callbacks.py` & `furchain-0.1.5/furchain/text/callbacks.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/chat_format.py` & `furchain-0.1.5/furchain/text/chat_format.py`

 * *Files 10% similar despite different names*

```diff
@@ -348,14 +348,60 @@
                 prompt += self._human_prefix + i.content + self._sep
             elif isinstance(i, AIMessage):
                 prompt += self._ai_prefix + i.content + self._sep
         prompt += self._ai_prefix  # + response_prefix
         return prompt
 
 
+class Llama3ChatFormatParser(ChatFormatParser):
+    """
+    Chat format parser for the Llama3 format.
+
+    Attributes:
+        _system_prefix (str): Prefix for system messages.
+        _human_prefix (str): Prefix for user messages.
+        _ai_prefix (str): Prefix for assistant messages.
+        _sep (str): Separator string.
+        stop (list): List of stop words or phrases.
+
+    Methods:
+        parse(chat_prompt_value: ChatPromptValue): Parses a chat prompt value in the Llama3 format.
+    """
+    _system_prefix = "<|start_header_id|>system<|end_header_id|>\n\n"
+    _human_prefix = "<|start_header_id|>user<|end_header_id|>\n\n"
+    _ai_prefix = "<|start_header_id|>assistant<|end_header_id|>\n\n"
+    _sep = "<|eot_id|>"
+    stop = ["<|end_of_text|>", _sep]
+
+    @classmethod
+    def parse(cls, chat_prompt_value: ChatPromptValue) -> str:
+        """
+        Parses a chat prompt value in the Llama3 format.
+
+        Args:
+            chat_prompt_value (ChatPromptValue): The chat prompt value to parse.
+
+        Returns:
+            str: The parsed chat prompt value.
+        """
+        messages = chat_prompt_value.messages
+        prompt = "<|begin_of_text|>"
+        system_message = ''
+        if len(messages) > 0 and isinstance(messages[0], SystemMessage):
+            system_message = cls._system_prefix + messages[0].content
+            messages = messages[1:]
+        prompt += system_message + cls._sep
+        for idx, i in enumerate(messages):
+            if isinstance(i, HumanMessage):
+                prompt += cls._human_prefix + i.content + cls._sep
+            elif isinstance(i, AIMessage):
+                prompt += cls._ai_prefix + i.content + cls._sep
+        prompt += cls._ai_prefix
+        return prompt
+
 class ChatFormat(enum.Enum):
     """
     Enum for chat formats.
 
     Attributes:
         Alpaca (str): Alpaca chat format.
         ExtendedAlpaca (str): Extended Alpaca chat format.
@@ -372,14 +418,15 @@
     Alpaca = 'Alpaca'
     ExtendedAlpaca = 'ExtendedAlpaca'
     LimaRPExtendedAlpaca = 'LimaRPExtendedAlpaca'
     ChatML = 'ChatML'
     Llama2 = 'Llama2'
     Vicuna = 'Vicuna'
     Qwen = 'Qwen'
+    Llama3 = 'Llama3'
 
     @property
     def parser(self) -> ChatFormatParser:
         """
         Returns the appropriate chat format parser for the chat format.
 
         Returns:
@@ -388,14 +435,15 @@
         return {
             ChatFormat.Alpaca: AlpacaChatFormatParser,
             ChatFormat.ExtendedAlpaca: ExtendedAlpacaChatFormatParser,
             ChatFormat.LimaRPExtendedAlpaca: LimaRPExtendedAlpacaChatFormatParser,
             ChatFormat.ChatML: ChatMLChatFormatParser,
             ChatFormat.Llama2: Llama2ChatFormatParser,
             ChatFormat.Vicuna: VicunaChatFormatParser,
-            ChatFormat.Qwen: QwenChatFormatParser
+            ChatFormat.Qwen: QwenChatFormatParser,
+            ChatFormat.Llama3: Llama3ChatFormatParser
         }[self]()
 
 
 __all__ = [
     "ChatFormat"
 ]
```

### Comparing `furchain-0.1.4/furchain/text/chat_message_history.py` & `furchain-0.1.5/furchain/text/chat_message_history.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/chat_prompt_templates.py` & `furchain-0.1.5/furchain/text/chat_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/grammars.py` & `furchain-0.1.5/furchain/text/grammars.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/llama_cpp_client.py` & `furchain-0.1.5/furchain/text/llama_cpp_client.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/output_parsers.py` & `furchain-0.1.5/furchain/text/output_parsers.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/text/schema.py` & `furchain-0.1.5/furchain/text/schema.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/utils/broadcaster.py` & `furchain-0.1.5/furchain/utils/broadcaster.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/furchain/utils/iterator.py` & `furchain-0.1.5/furchain/utils/iterator.py`

 * *Files identical despite different names*

### Comparing `furchain-0.1.4/pyproject.toml` & `furchain-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furchain"
-version = "0.1.4"
+version = "0.1.5"
 description = "FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline."
 authors = ["markyfsun <mark@furchain.xyz>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 websocket-client = "^1.7.0"
@@ -22,12 +22,14 @@
 pymongo = "^4.6.1"
 llama-cpp-python = "^0.2.52"
 python-dotenv = "^1.0.1"
 pyaudio = "^0.2.14"
 websockets = "^12.0"
 webuiapi = "^0.9.9"
 emoji = "^2.10.1"
+azure-cognitiveservices-speech = "^1.37.0"
+librosa = "^0.10.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `furchain-0.1.4/PKG-INFO` & `furchain-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: furchain
-Version: 0.1.4
+Version: 0.1.5
 Summary: FurChain is an innovative toolkit for creating and interacting with digital personas, complete with voice cloning and role-playing capabilities. It offers a suite of tools for real-time voice manipulation, chatbot creation, and text-based RPG adventures, all while being open-source and operable offline.
 Author: markyfsun
 Author-email: mark@furchain.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: azure-cognitiveservices-speech (>=1.37.0,<2.0.0)
 Requires-Dist: emoji (>=2.10.1,<3.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: langchain (>=0.1.4,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.16,<0.0.17)
 Requires-Dist: langchain-core (>=0.1.16,<0.2.0)
+Requires-Dist: librosa (>=0.10.1,<0.11.0)
 Requires-Dist: llama-cpp-python (>=0.2.52,<0.3.0)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: pyaudio (>=0.2.14,<0.3.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pymongo (>=4.6.1,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
```

