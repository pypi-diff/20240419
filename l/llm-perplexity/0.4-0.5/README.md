# Comparing `tmp/llm-perplexity-0.4.tar.gz` & `tmp/llm_perplexity-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-perplexity-0.4.tar", last modified: Fri Mar  8 09:53:38 2024, max compression
+gzip compressed data, was "llm_perplexity-0.5.tar", last modified: Fri Apr 19 07:29:45 2024, max compression
```

## Comparing `llm-perplexity-0.4.tar` & `llm_perplexity-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:53:38.574482 llm-perplexity-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-03-08 09:53:29.000000 llm-perplexity-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-08 09:53:38.574482 llm-perplexity-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-08 09:53:29.000000 llm-perplexity-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:53:38.574482 llm-perplexity-0.4/llm_perplexity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-08 09:53:38.000000 llm-perplexity-0.4/llm_perplexity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-03-08 09:53:29.000000 llm-perplexity-0.4/llm_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-08 09:53:29.000000 llm-perplexity-0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:53:38.574482 llm-perplexity-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:29:45.509863 llm_perplexity-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-19 07:29:36.000000 llm_perplexity-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 07:29:45.509863 llm_perplexity-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-19 07:29:36.000000 llm_perplexity-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 07:29:45.509863 llm_perplexity-0.5/llm_perplexity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 07:29:45.000000 llm_perplexity-0.5/llm_perplexity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-04-19 07:29:36.000000 llm_perplexity-0.5/llm_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-19 07:29:36.000000 llm_perplexity-0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 07:29:45.509863 llm_perplexity-0.5/setup.cfg
```

### Comparing `llm-perplexity-0.4/LICENSE` & `llm_perplexity-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-perplexity-0.4/PKG-INFO` & `llm_perplexity-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-perplexity
-Version: 0.4
+Version: 0.5
 Summary: LLM access to pplx-api 3 by Perplexity Labs
 Author: hex
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hex/llm-perplexity
 Project-URL: Changelog, https://github.com/hex/llm-perplexity/releases
 Project-URL: Issues, https://github.com/hex/llm-perplexity/issues
 Project-URL: CI, https://github.com/hex/llm-perplexity/actions
```

### Comparing `llm-perplexity-0.4/README.md` & `llm_perplexity-0.5/README.md`

 * *Files identical despite different names*

### Comparing `llm-perplexity-0.4/llm_perplexity.egg-info/PKG-INFO` & `llm_perplexity-0.5/llm_perplexity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-perplexity
-Version: 0.4
+Version: 0.5
 Summary: LLM access to pplx-api 3 by Perplexity Labs
 Author: hex
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/hex/llm-perplexity
 Project-URL: Changelog, https://github.com/hex/llm-perplexity/releases
 Project-URL: Issues, https://github.com/hex/llm-perplexity/issues
 Project-URL: CI, https://github.com/hex/llm-perplexity/actions
```

### Comparing `llm-perplexity-0.4/llm_perplexity.py` & `llm_perplexity-0.5/llm_perplexity.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     register(Perplexity("sonar-small-chat", default_max_tokens=16384), aliases=("pp-small-chat",))
     register(Perplexity("sonar-small-online", default_max_tokens=12288), aliases=("pp-small-online",))
     register(Perplexity("sonar-medium-chat", default_max_tokens=16384), aliases=("pp-medium-chat",))
     register(Perplexity("sonar-medium-online", default_max_tokens=12288), aliases=("pp-medium-online",))
     register(Perplexity("codellama-70b-instruct", default_max_tokens=16384), aliases=("pp-70b-instruct",))
     register(Perplexity("mistral-7b-instruct", default_max_tokens=16384), aliases=("pp-7b-instruct",))
     register(Perplexity("mixtral-8x7b-instruct", default_max_tokens=16384), aliases=("pp-8x7b-instruct",))
+    register(Perplexity("mixtral-8x22b-instruct", default_max_tokens=16384), aliases=("pp-8x22b-instruct",))
+    register(Perplexity("llama-3-8b-instruct", default_max_tokens=8192))
+    register(Perplexity("llama-3-70b-instruct", default_max_tokens=8192))
+
 
 class PerplexityOptions(llm.Options):
     max_tokens: Optional[int] = Field(
         description="The maximum number of completion tokens returned by the API. The total number of tokens requested in max_tokens plus the number of prompt tokens sent in messages must not exceed the context window token limit of model requested. If left unspecified, then the model will generate tokens until either it reaches its stop token or the end of its context window",
         default=None,
     )
 
@@ -141,8 +145,8 @@
                 for text in stream:
                     yield text.choices[0].delta.content
         else:
            completion = client.chat.completions.create(**kwargs)
            yield completion.choices[0].message.content
 
     def __str__(self):
-        return f"Perplexity: {self.model_id}"
+        return f"Perplexity: {self.model_id}"
```

### Comparing `llm-perplexity-0.4/pyproject.toml` & `llm_perplexity-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-perplexity"
-version = "0.4"
+version = "0.5"
 description = "LLM access to pplx-api 3 by Perplexity Labs"
 readme = "README.md"
 authors = [{name = "hex"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -16,8 +16,8 @@
 [project.urls]
 Homepage = "https://github.com/hex/llm-perplexity"
 Changelog = "https://github.com/hex/llm-perplexity/releases"
 Issues = "https://github.com/hex/llm-perplexity/issues"
 CI = "https://github.com/hex/llm-perplexity/actions"
 
 [project.entry-points.llm]
-perplexity = "llm_perplexity"
+perplexity = "llm_perplexity"
```

