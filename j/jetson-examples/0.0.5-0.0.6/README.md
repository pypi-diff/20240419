# Comparing `tmp/jetson_examples-0.0.5.tar.gz` & `tmp/jetson_examples-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.0.5.tar", last modified: Wed Apr 17 12:06:27 2024, max compression
+gzip compressed data, was "jetson_examples-0.0.6.tar", last modified: Fri Apr 19 02:38:42 2024, max compression
```

## Comparing `jetson_examples-0.0.5.tar` & `jetson_examples-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1066 2024-04-16 06:52:15.000000 jetson_examples-0.0.5/LICENSE
--rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/PKG-INFO
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     3332 2024-04-17 04:12:01.000000 jetson_examples-0.0.5/README.md
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/jetson_examples.egg-info/
--rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      878 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)        1 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       58 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       27 2024-04-17 12:06:27.000000 jetson_examples-0.0.5/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1081 2024-04-17 12:05:45.000000 jetson_examples-0.0.5/pyproject.toml
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       22 2024-04-17 12:05:53.000000 jetson_examples-0.0.5/reComputer/__init__.py
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1821 2024-04-17 12:03:58.000000 jetson_examples-0.0.5/reComputer/main.py
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      134 2024-04-16 09:51:17.000000 jetson_examples-0.0.5/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      127 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/check.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/hello-world/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       87 2024-04-17 03:08:32.000000 jetson_examples-0.0.5/reComputer/scripts/hello-world/readme.md
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      280 2024-04-17 11:37:51.000000 jetson_examples-0.0.5/reComputer/scripts/hello-world/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/live-llava/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)    10137 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/live-llava/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      148 2024-04-16 09:49:26.000000 jetson_examples-0.0.5/reComputer/scripts/llava/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava-v1.5-7b/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      147 2024-04-16 09:50:12.000000 jetson_examples-0.0.5/reComputer/scripts/llava-v1.5-7b/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/llava-v1.6-vicuna-7b/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      165 2024-04-16 09:50:51.000000 jetson_examples-0.0.5/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.304756 jetson_examples-0.0.5/reComputer/scripts/nanodb/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      247 2024-04-16 10:00:31.000000 jetson_examples-0.0.5/reComputer/scripts/nanodb/readme.md
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1875 2024-04-16 09:45:34.000000 jetson_examples-0.0.5/reComputer/scripts/nanodb/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/nanoowl/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      161 2024-04-16 09:53:17.000000 jetson_examples-0.0.5/reComputer/scripts/nanoowl/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     2066 2024-04-17 11:48:07.000000 jetson_examples-0.0.5/reComputer/scripts/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/stable-diffusion-webui/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       57 2024-04-16 09:52:42.000000 jetson_examples-0.0.5/reComputer/scripts/stable-diffusion-webui/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/text-generation-webui/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      304 2024-04-16 09:52:01.000000 jetson_examples-0.0.5/reComputer/scripts/text-generation-webui/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      900 2024-04-17 12:02:17.000000 jetson_examples-0.0.5/reComputer/scripts/update.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/reComputer/scripts/whisper/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       43 2024-04-16 09:53:47.000000 jetson_examples-0.0.5/reComputer/scripts/whisper/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       38 2024-04-17 12:06:27.308756 jetson_examples-0.0.5/setup.cfg
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1066 2024-04-16 06:52:15.000000 jetson_examples-0.0.6/LICENSE
+-rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/PKG-INFO
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     3332 2024-04-19 02:35:25.000000 jetson_examples-0.0.6/README.md
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/jetson_examples.egg-info/
+-rw-r--r--   0 seeed     (1000) seeed     (1000)     3982 2024-04-19 02:38:42.000000 jetson_examples-0.0.6/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      944 2024-04-19 02:38:42.000000 jetson_examples-0.0.6/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)        1 2024-04-19 02:38:42.000000 jetson_examples-0.0.6/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       58 2024-04-19 02:38:42.000000 jetson_examples-0.0.6/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       27 2024-04-19 02:38:42.000000 jetson_examples-0.0.6/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1081 2024-04-19 02:38:11.000000 jetson_examples-0.0.6/pyproject.toml
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.350550 jetson_examples-0.0.6/reComputer/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       22 2024-04-19 02:38:16.000000 jetson_examples-0.0.6/reComputer/__init__.py
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1821 2024-04-17 12:03:58.000000 jetson_examples-0.0.6/reComputer/main.py
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.350550 jetson_examples-0.0.6/reComputer/scripts/
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.350550 jetson_examples-0.0.6/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      134 2024-04-16 09:51:17.000000 jetson_examples-0.0.6/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      127 2024-04-16 09:45:34.000000 jetson_examples-0.0.6/reComputer/scripts/check.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.350550 jetson_examples-0.0.6/reComputer/scripts/hello-world/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       87 2024-04-17 03:08:32.000000 jetson_examples-0.0.6/reComputer/scripts/hello-world/readme.md
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      280 2024-04-17 11:37:51.000000 jetson_examples-0.0.6/reComputer/scripts/hello-world/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/live-llava/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)    10137 2024-04-16 09:45:34.000000 jetson_examples-0.0.6/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/llama3/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      226 2024-04-19 02:35:03.000000 jetson_examples-0.0.6/reComputer/scripts/llama3/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/llava/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      148 2024-04-16 09:49:26.000000 jetson_examples-0.0.6/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      147 2024-04-16 09:50:12.000000 jetson_examples-0.0.6/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      165 2024-04-16 09:50:51.000000 jetson_examples-0.0.6/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/nanodb/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      247 2024-04-16 10:00:31.000000 jetson_examples-0.0.6/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     1875 2024-04-16 09:45:34.000000 jetson_examples-0.0.6/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      161 2024-04-16 09:53:17.000000 jetson_examples-0.0.6/reComputer/scripts/nanoowl/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/ollama/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      143 2024-04-19 02:27:31.000000 jetson_examples-0.0.6/reComputer/scripts/ollama/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)     2066 2024-04-17 11:48:07.000000 jetson_examples-0.0.6/reComputer/scripts/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       57 2024-04-16 09:52:42.000000 jetson_examples-0.0.6/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      304 2024-04-16 09:52:01.000000 jetson_examples-0.0.6/reComputer/scripts/text-generation-webui/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)      900 2024-04-17 12:02:17.000000 jetson_examples-0.0.6/reComputer/scripts/update.sh
+drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/reComputer/scripts/whisper/
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       43 2024-04-16 09:53:47.000000 jetson_examples-0.0.6/reComputer/scripts/whisper/run.sh
+-rw-rw-r--   0 seeed     (1000) seeed     (1000)       38 2024-04-19 02:38:42.354550 jetson_examples-0.0.6/setup.cfg
```

### Comparing `jetson_examples-0.0.5/LICENSE` & `jetson_examples-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/PKG-INFO` & `jetson_examples-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.5
+Version: 0.0.6
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jetson_examples-0.0.5/README.md` & `jetson_examples-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.0.6/jetson_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.5
+Version: 0.0.6
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jetson_examples-0.0.5/jetson_examples.egg-info/SOURCES.txt` & `jetson_examples-0.0.6/jetson_examples.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 reComputer/scripts/check.sh
 reComputer/scripts/run.sh
 reComputer/scripts/update.sh
 reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
 reComputer/scripts/hello-world/readme.md
 reComputer/scripts/hello-world/run.sh
 reComputer/scripts/live-llava/run.sh
+reComputer/scripts/llama3/run.sh
 reComputer/scripts/llava/run.sh
 reComputer/scripts/llava-v1.5-7b/run.sh
 reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
 reComputer/scripts/nanodb/readme.md
 reComputer/scripts/nanodb/run.sh
 reComputer/scripts/nanoowl/run.sh
+reComputer/scripts/ollama/run.sh
 reComputer/scripts/stable-diffusion-webui/run.sh
 reComputer/scripts/text-generation-webui/run.sh
 reComputer/scripts/whisper/run.sh
```

### Comparing `jetson_examples-0.0.5/pyproject.toml` & `jetson_examples-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson_examples-0.0.5/reComputer/main.py` & `jetson_examples-0.0.6/reComputer/main.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/reComputer/scripts/live-llava/run.sh` & `jetson_examples-0.0.6/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/reComputer/scripts/nanodb/run.sh` & `jetson_examples-0.0.6/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/reComputer/scripts/run.sh` & `jetson_examples-0.0.6/reComputer/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.5/reComputer/scripts/update.sh` & `jetson_examples-0.0.6/reComputer/scripts/update.sh`

 * *Files identical despite different names*

