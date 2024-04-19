# Comparing `tmp/tetos-0.1.0.tar.gz` & `tmp/tetos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetos-0.1.0.tar", last modified: Thu Apr 18 02:13:21 2024, max compression
+gzip compressed data, was "tetos-0.1.1.tar", last modified: Fri Apr 19 08:51:29 2024, max compression
```

## Comparing `tetos-0.1.0.tar` & `tetos-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      551 2024-04-18 02:13:13.089049 tetos-0.1.0/LICENSE
--rw-r--r--   0        0        0     2209 2024-04-18 02:13:13.089049 tetos-0.1.0/README.md
--rw-r--r--   0        0        0     1377 2024-04-18 02:13:21.709096 tetos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/__init__.py
--rw-r--r--   0        0        0      928 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/__main__.py
--rw-r--r--   0        0        0     3839 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/azure.py
--rw-r--r--   0        0        0     5195 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/baidu.py
--rw-r--r--   0        0        0     3048 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/base.py
--rw-r--r--   0        0        0    20883 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/consts.py
--rw-r--r--   0        0        0     2473 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/edge.py
--rw-r--r--   0        0        0     4891 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/google.py
--rw-r--r--   0        0        0     2770 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/openai.py
--rw-r--r--   0        0        0     8844 2024-04-18 02:13:13.089049 tetos-0.1.0/src/tetos/volc.py
--rw-r--r--   0        0        0     1934 2024-04-18 02:13:13.089049 tetos-0.1.0/tests/test_speakers.py
--rw-r--r--   0        0        0     3269 1970-01-01 00:00:00.000000 tetos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      551 2024-04-19 08:51:26.404123 tetos-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2469 2024-04-19 08:51:26.404123 tetos-0.1.1/README.md
+-rw-r--r--   0        0        0     1377 2024-04-19 08:51:29.376090 tetos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/__init__.py
+-rw-r--r--   0        0        0      928 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/__main__.py
+-rw-r--r--   0        0        0     3777 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/azure.py
+-rw-r--r--   0        0        0     5210 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/baidu.py
+-rw-r--r--   0        0        0     3048 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/base.py
+-rw-r--r--   0        0        0    20883 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/consts.py
+-rw-r--r--   0        0        0     2473 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/edge.py
+-rw-r--r--   0        0        0     4891 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/google.py
+-rw-r--r--   0        0        0     2770 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/openai.py
+-rw-r--r--   0        0        0     9002 2024-04-19 08:51:26.408123 tetos-0.1.1/src/tetos/volc.py
+-rw-r--r--   0        0        0     1934 2024-04-19 08:51:26.408123 tetos-0.1.1/tests/test_speakers.py
+-rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 tetos-0.1.1/PKG-INFO
```

### Comparing `tetos-0.1.0/LICENSE` & `tetos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/README.md` & `tetos-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   - `api_key`: OpenAI API key
 
 - [Azure TTS](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/text-to-speech)
 
   Required parameters(Please refer to the documentation to get the secrets):
 
   - `speech_key`: Azure Speech service key
-  - `service_region`: Azure Speech service region
+  - `speech_region`: Azure Speech service region
 
 - [Google TTS](https://cloud.google.com/text-to-speech?hl=zh-CN)
 
   Requirements:
 
   - [Enable the Text-to-Speech API in the Google Cloud Console](https://console.developers.google.com/apis/api/texttospeech.googleapis.com/overview?project=586547753837)
   - Environment variables `GOOGLE_APPLICATION_CREDENTIALS` pointing to the service account key file
@@ -34,16 +34,18 @@
   - `secret_key`: Volcengine access secret key. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `app_key`: Volcengine app key
 
 - [Baidu TTS](https://ai.baidu.com/tech/speech/tts)
 
   Required parameters:
 
-  - `app_id`: Baidu app ID, [Get it at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
-  - `api_key`: Baidu API
+  - `api_key`: Baidu API key
+  - `secret_key`: Baidu secret key
+
+  [Get both at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
 
 
 ## Installation
 
 Requires Python 3.8 or higher.
 
 ```bash
@@ -54,14 +56,23 @@
 
 ```
 tetos PROVIDER [PROVIDER_OPTIONS] TEXT [--output FILE]
 ```
 
 Please run `tetos --help` for available providers and options.
 
+Examples
+
+```
+tetos google "Hello, world!"
+tetos azure "Hello, world!" --output output.mp3   # save to another file
+tetos edge --lang zh-CN "你好，世界！"  # specify language
+tetos openai --voice echo "Hello, world!"  # specify voice
+```
+
 ## API Usage
 
 Use Azure TTS as an example:
 
 ```python
 from tetos.azure import AzureSpeaker
```

### Comparing `tetos-0.1.0/pyproject.toml` & `tetos-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Repository = "https://github.com/frostming/tetos"
```

### Comparing `tetos-0.1.0/src/tetos/__main__.py` & `tetos-0.1.1/src/tetos/__main__.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/azure.py` & `tetos-0.1.1/src/tetos/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 from __future__ import annotations
 
 import os
+from dataclasses import dataclass
 from pathlib import Path
 
 import anyio.to_thread
 import azure.cognitiveservices.speech as speechsdk
 import click
 
 from .base import Speaker, SynthesizeError, common_options
 from .consts import AZURE_SUPPORTED_VOICES
 
 
+@dataclass
 class AzureSpeaker(Speaker):
     """Azure TTS speaker.
 
     Args:
         speech_key (str): The Azure Speech key.
         speech_region (str): The Azure Speech region.
         voice (str, optional): The voice to use.
     """
 
-    def __init__(
-        self, speech_key: str, speech_region: str, *, voice: str | None = None
-    ) -> None:
-        self.voice = voice
-        self.speech_key = speech_key
-        self.speech_region = speech_region
-        self._set_proxy()
+    speech_key: str
+    speech_region: str
+    voice: str | None = None
 
-    def _set_proxy(self) -> None:
+    def _set_proxy(self, speech_config: speechsdk.SpeechConfig) -> None:
         from urllib.parse import urlparse
 
         for env in ("http_proxy", "https_proxy", "all_proxy"):
             # Try both lowercase and uppercase versions of the environment variable
             url = os.getenv(env, os.getenv(env.upper(), ""))
             if not url:
                 continue
             parsed_url = urlparse(url)
-            self.speech_config.set_proxy(
+            speech_config.set_proxy(
                 parsed_url.hostname,
                 parsed_url.port,
                 parsed_url.username,
                 parsed_url.password,
             )
             break
 
     def get_speech_config(self, lang: str) -> str:
         config = speechsdk.SpeechConfig(
             subscription=self.speech_key, region=self.speech_region
         )
+        self._set_proxy(config)
         config.set_speech_synthesis_output_format(
             speechsdk.SpeechSynthesisOutputFormat.Audio16Khz32KBitRateMonoMp3
         )
         if self.voice:
             voice = self.voice
         else:
             voice = next(
```

### Comparing `tetos-0.1.0/src/tetos/baidu.py` & `tetos-0.1.1/src/tetos/baidu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 import json
 import logging
 import platform
 import time
+from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, ClassVar, cast
 from urllib.parse import quote_plus
 
 import anyio
 import click
 import httpx
 import mutagen.mp3
-from attr import dataclass, field
 
 from .base import Speaker, SynthesizeError, common_options
 from .consts import BAIDU_SUPPORTED_VOICES
 
 logger = logging.getLogger(__name__)
 
 TOKEN_URL = "https://aip.baidubce.com/oauth/2.0/token"
@@ -41,15 +41,15 @@
 
     api_key: str
     secret_key: str
     voice: str | None = None
     speed: int = 5
     pitch: int = 5
     volume: int = 5
-    _token: dict[str, Any] = field(factory=dict, init=False)
+    _token: dict[str, Any] = field(default_factory=dict, init=False)
 
     TOKEN_FILE: ClassVar[Path] = Path.home() / ".tetos" / "baidu_token.json"
 
     def __post_init__(self) -> None:
         if self.TOKEN_FILE.exists():
             with self.TOKEN_FILE.open() as f:
                 self._token = json.load(f)
```

### Comparing `tetos-0.1.0/src/tetos/base.py` & `tetos-0.1.1/src/tetos/base.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/consts.py` & `tetos-0.1.1/src/tetos/consts.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/edge.py` & `tetos-0.1.1/src/tetos/edge.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/google.py` & `tetos-0.1.1/src/tetos/google.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/openai.py` & `tetos-0.1.1/src/tetos/openai.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/src/tetos/volc.py` & `tetos-0.1.1/src/tetos/volc.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 from .base import Speaker, SynthesizeError, common_options
 from .consts import VOLC_SUPPORTED_VOICES
 
 logger = logging.getLogger(__name__)
 
 
 class VolcSignAuth(Auth):
-    SERVICE_NAME = "sami"
-    REGION = "cn-north-1"
     ALGORITHM = "HMAC-SHA256"
 
     requires_request_body = True
 
-    def __init__(self, access_key: str, secret_key: str) -> None:
+    def __init__(
+        self, access_key: str, secret_key: str, service: str, region: str
+    ) -> None:
         self.access_key = access_key
         self.secret_key = secret_key
+        self.service = service
+        self.region = region
 
     @staticmethod
     def hmac_sha256(key: bytes, content: str) -> bytes:
         return hmac.new(key, content.encode("utf-8"), hashlib.sha256).digest()
 
     def auth_flow(self, request: Request) -> Generator[Request, Response, None]:
         x_content_sha256 = hashlib.sha256(request.content).hexdigest()
@@ -51,15 +53,15 @@
                 "",
                 signed_headers,
                 x_content_sha256,
             ]
         )
 
         canonical_request_hash = hashlib.sha256(canonical_request.encode()).hexdigest()
-        credential_scope = f"{x_date[:8]}/{self.REGION}/{self.SERVICE_NAME}/request"
+        credential_scope = f"{x_date[:8]}/{self.region}/{self.service}/request"
         string_to_sign = "\n".join(
             [
                 self.ALGORITHM,
                 x_date,
                 credential_scope,
                 canonical_request_hash,
             ]
@@ -91,14 +93,16 @@
             Available values: [8000,16000,22050,24000,32000,44100,48000],
             Defaults to 24000.
         speech_rate (int, optional): The speech rate. It should be in range [-50,100].
             100 means 2x speed and -50 means half speed. Defaults to 0.
         pitch_rate (int, optional): The pitch rate. It should be in range [-12,12]. Defaults to 0.
     """
 
+    SERVICE_NAME = "sami"
+    REGION = "cn-north-1"
     AUTH_VERSION = "volc-auth-v1"
     API_HOST = "open.volcengineapi.com"
     VERSION = "2021-07-27"
     TOKEN_FILE = Path.home() / ".tetos" / "volc_token.json"
     SAMI_API_URL = "https://sami.bytedance.com/api/v1/invoke"
 
     def __init__(
@@ -139,15 +143,17 @@
             "expiration": 3600 * 24,  # expire in 1 day
         }
         resp = await self.client.post(
             f"https://{self.API_HOST}/",
             params={"Action": "GetToken", "Version": self.VERSION},
             json=data,
             headers={"Host": self.API_HOST},
-            auth=VolcSignAuth(self.access_key, self.secret_key),
+            auth=VolcSignAuth(
+                self.access_key, self.secret_key, self.SERVICE_NAME, self.REGION
+            ),
         )
         if resp.is_error:
             logger.error("Failed to get token: %s", resp.text)
             raise SynthesizeError("Failed to get token")
         token = resp.json()
         self.TOKEN_FILE.parent.mkdir(parents=True, exist_ok=True)
         with self.TOKEN_FILE.open("w") as f:
```

### Comparing `tetos-0.1.0/tests/test_speakers.py` & `tetos-0.1.1/tests/test_speakers.py`

 * *Files identical despite different names*

### Comparing `tetos-0.1.0/PKG-INFO` & `tetos-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetos
-Version: 0.1.0
+Version: 0.1.1
 Summary: Unified interface for multiple Text-to-Speech (TTS) providers
 Keywords: tts,text-to-speech,speech,audio,ai,nlp
 Author-Email: Frost Ming <me@frostming.com>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,15 +40,15 @@
   - `api_key`: OpenAI API key
 
 - [Azure TTS](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/text-to-speech)
 
   Required parameters(Please refer to the documentation to get the secrets):
 
   - `speech_key`: Azure Speech service key
-  - `service_region`: Azure Speech service region
+  - `speech_region`: Azure Speech service region
 
 - [Google TTS](https://cloud.google.com/text-to-speech?hl=zh-CN)
 
   Requirements:
 
   - [Enable the Text-to-Speech API in the Google Cloud Console](https://console.developers.google.com/apis/api/texttospeech.googleapis.com/overview?project=586547753837)
   - Environment variables `GOOGLE_APPLICATION_CREDENTIALS` pointing to the service account key file
@@ -61,16 +61,18 @@
   - `secret_key`: Volcengine access secret key. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `app_key`: Volcengine app key
 
 - [Baidu TTS](https://ai.baidu.com/tech/speech/tts)
 
   Required parameters:
 
-  - `app_id`: Baidu app ID, [Get it at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
-  - `api_key`: Baidu API
+  - `api_key`: Baidu API key
+  - `secret_key`: Baidu secret key
+
+  [Get both at the console](https://console.bce.baidu.com/ai/#/ai/speech/app/list)
 
 
 ## Installation
 
 Requires Python 3.8 or higher.
 
 ```bash
@@ -81,14 +83,23 @@
 
 ```
 tetos PROVIDER [PROVIDER_OPTIONS] TEXT [--output FILE]
 ```
 
 Please run `tetos --help` for available providers and options.
 
+Examples
+
+```
+tetos google "Hello, world!"
+tetos azure "Hello, world!" --output output.mp3   # save to another file
+tetos edge --lang zh-CN "你好，世界！"  # specify language
+tetos openai --voice echo "Hello, world!"  # specify voice
+```
+
 ## API Usage
 
 Use Azure TTS as an example:
 
 ```python
 from tetos.azure import AzureSpeaker
```

