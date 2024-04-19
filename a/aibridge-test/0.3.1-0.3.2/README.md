# Comparing `tmp/aibridge_test-0.3.1.tar.gz` & `tmp/aibridge_test-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aibridge_test-0.3.1.tar", last modified: Thu Apr 18 05:46:05 2024, max compression
+gzip compressed data, was "aibridge_test-0.3.2.tar", last modified: Thu Apr 18 05:54:17 2024, max compression
```

## Comparing `aibridge_test-0.3.1.tar` & `aibridge_test-0.3.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:05.167972 aibridge_test-0.3.1/
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.238952 aibridge_test-0.3.1/AIBridge/
--rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.1/AIBridge/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.440948 aibridge_test-0.3.1/AIBridge/ai_services/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/ai_services/__init__.py
--rw-rw-rw-   0        0        0     9311 2024-04-11 09:50:53.000000 aibridge_test-0.3.1/AIBridge/ai_services/ai21labs_text.py
--rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/ai_services/ai_abstraction.py
--rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/ai_services/ai_services_response.py
--rw-rw-rw-   0        0        0    13501 2024-04-11 09:51:01.000000 aibridge_test-0.3.1/AIBridge/ai_services/anthropic_ai.py
--rw-rw-rw-   0        0        0    12216 2024-04-11 09:51:03.000000 aibridge_test-0.3.1/AIBridge/ai_services/cohere_llm.py
--rw-rw-rw-   0        0        0    14370 2024-04-18 05:44:22.000000 aibridge_test-0.3.1/AIBridge/ai_services/geminin_services.py
--rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/ai_services/image_optimisaton.py
--rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.1/AIBridge/ai_services/openai_images.py
--rw-rw-rw-   0        0        0    11817 2024-04-11 09:46:41.000000 aibridge_test-0.3.1/AIBridge/ai_services/openai_services.py
--rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.1/AIBridge/ai_services/palm_chat.py
--rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.3.1/AIBridge/ai_services/palm_text.py
--rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.1/AIBridge/ai_services/process_mq.py
--rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/ai_services/stable_diffusion_image.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.473981 aibridge_test-0.3.1/AIBridge/constant/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/constant/__init__.py
--rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.1/AIBridge/constant/common.py
--rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.1/AIBridge/constant/constant.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.524947 aibridge_test-0.3.1/AIBridge/database/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/__init__.py
--rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/db_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.549948 aibridge_test-0.3.1/AIBridge/database/models/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/models/__init__.py
--rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/models/ai_response.py
--rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/models/prompts.py
--rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/models/variables.py
--rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/no_sql_service.py
--rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/session.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/sql_service.py
--rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/database/table_oprations.py
--rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.1/AIBridge/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.594950 aibridge_test-0.3.1/AIBridge/output_validation/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/output_validation/__init__.py
--rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/output_validation/active_validator.py
--rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.1/AIBridge/output_validation/convertors.py
--rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.1/AIBridge/output_validation/validations.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.677947 aibridge_test-0.3.1/AIBridge/prompts/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/prompts/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/prompts/prompt_completion.py
--rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/prompts/prompts_save.py
--rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/prompts/prompts_varibales.py
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.724951 aibridge_test-0.3.1/AIBridge/queue_integration/
--rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/queue_integration/__init__.py
--rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/queue_integration/assign_queue.py
--rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/queue_integration/message_queue.py
--rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/AIBridge/queue_integration/queue_model.py
--rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.1/AIBridge/queue_integration/response_class.py
--rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.1/AIBridge/setconfig.py
--rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    21534 2024-04-18 05:46:04.959947 aibridge_test-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 05:46:04.957947 aibridge_test-0.3.1/aibridge_test.egg-info/
--rw-rw-rw-   0        0        0    21534 2024-04-18 05:46:03.000000 aibridge_test-0.3.1/aibridge_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2024-04-18 05:46:04.000000 aibridge_test-0.3.1/aibridge_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 05:46:03.000000 aibridge_test-0.3.1/aibridge_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      228 2024-04-18 05:46:03.000000 aibridge_test-0.3.1/aibridge_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-18 05:46:03.000000 aibridge_test-0.3.1/aibridge_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 05:46:05.168948 aibridge_test-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2863 2024-04-18 05:45:03.000000 aibridge_test-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:17.041612 aibridge_test-0.3.2/
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.400612 aibridge_test-0.3.2/AIBridge/
+-rw-rw-rw-   0        0        0     1575 2024-04-04 08:38:44.000000 aibridge_test-0.3.2/AIBridge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.631605 aibridge_test-0.3.2/AIBridge/ai_services/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/ai_services/__init__.py
+-rw-rw-rw-   0        0        0     9311 2024-04-11 09:50:53.000000 aibridge_test-0.3.2/AIBridge/ai_services/ai21labs_text.py
+-rw-rw-rw-   0        0        0      495 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/ai_services/ai_abstraction.py
+-rw-rw-rw-   0        0        0      978 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/ai_services/ai_services_response.py
+-rw-rw-rw-   0        0        0    13501 2024-04-11 09:51:01.000000 aibridge_test-0.3.2/AIBridge/ai_services/anthropic_ai.py
+-rw-rw-rw-   0        0        0    12216 2024-04-11 09:51:03.000000 aibridge_test-0.3.2/AIBridge/ai_services/cohere_llm.py
+-rw-rw-rw-   0        0        0    14383 2024-04-18 05:51:32.000000 aibridge_test-0.3.2/AIBridge/ai_services/geminin_services.py
+-rw-rw-rw-   0        0        0     3580 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/ai_services/image_optimisaton.py
+-rw-rw-rw-   0        0        0     7514 2024-01-22 04:54:52.000000 aibridge_test-0.3.2/AIBridge/ai_services/openai_images.py
+-rw-rw-rw-   0        0        0    11817 2024-04-11 09:46:41.000000 aibridge_test-0.3.2/AIBridge/ai_services/openai_services.py
+-rw-rw-rw-   0        0        0     2947 2024-04-01 10:21:53.000000 aibridge_test-0.3.2/AIBridge/ai_services/palm_chat.py
+-rw-rw-rw-   0        0        0     9196 2024-04-02 05:11:27.000000 aibridge_test-0.3.2/AIBridge/ai_services/palm_text.py
+-rw-rw-rw-   0        0        0     2024 2024-04-04 04:17:16.000000 aibridge_test-0.3.2/AIBridge/ai_services/process_mq.py
+-rw-rw-rw-   0        0        0    10350 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/ai_services/stable_diffusion_image.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.658607 aibridge_test-0.3.2/AIBridge/constant/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/constant/__init__.py
+-rw-rw-rw-   0        0        0     7755 2024-04-16 09:20:57.000000 aibridge_test-0.3.2/AIBridge/constant/common.py
+-rw-rw-rw-   0        0        0      914 2024-04-05 09:37:33.000000 aibridge_test-0.3.2/AIBridge/constant/constant.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.732611 aibridge_test-0.3.2/AIBridge/database/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/__init__.py
+-rw-rw-rw-   0        0        0      965 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/db_layer.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.766607 aibridge_test-0.3.2/AIBridge/database/models/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/models/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/models/ai_response.py
+-rw-rw-rw-   0        0        0      424 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/models/prompts.py
+-rw-rw-rw-   0        0        0      364 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/models/variables.py
+-rw-rw-rw-   0        0        0     3949 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/no_sql_service.py
+-rw-rw-rw-   0        0        0      751 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/session.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/sql_service.py
+-rw-rw-rw-   0        0        0      433 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/database/table_oprations.py
+-rw-rw-rw-   0        0        0     1161 2024-04-04 03:54:10.000000 aibridge_test-0.3.2/AIBridge/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.796611 aibridge_test-0.3.2/AIBridge/output_validation/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/output_validation/__init__.py
+-rw-rw-rw-   0        0        0      401 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/output_validation/active_validator.py
+-rw-rw-rw-   0        0        0     1613 2024-04-04 09:51:39.000000 aibridge_test-0.3.2/AIBridge/output_validation/convertors.py
+-rw-rw-rw-   0        0        0     5866 2024-04-04 10:12:50.000000 aibridge_test-0.3.2/AIBridge/output_validation/validations.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.844612 aibridge_test-0.3.2/AIBridge/prompts/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/prompts/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/prompts/prompt_completion.py
+-rw-rw-rw-   0        0        0     3896 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/prompts/prompts_save.py
+-rw-rw-rw-   0        0        0     2733 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/prompts/prompts_varibales.py
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:16.900609 aibridge_test-0.3.2/AIBridge/queue_integration/
+-rw-rw-rw-   0        0        0        0 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/queue_integration/__init__.py
+-rw-rw-rw-   0        0        0      417 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/queue_integration/assign_queue.py
+-rw-rw-rw-   0        0        0      852 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/queue_integration/message_queue.py
+-rw-rw-rw-   0        0        0     4254 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/AIBridge/queue_integration/queue_model.py
+-rw-rw-rw-   0        0        0     6965 2024-04-04 04:16:23.000000 aibridge_test-0.3.2/AIBridge/queue_integration/response_class.py
+-rw-rw-rw-   0        0        0     2945 2024-04-16 09:21:15.000000 aibridge_test-0.3.2/AIBridge/setconfig.py
+-rw-rw-rw-   0        0        0    10436 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    21534 2024-04-18 05:54:17.024624 aibridge_test-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    20438 2024-01-16 04:27:43.000000 aibridge_test-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 05:54:17.015607 aibridge_test-0.3.2/aibridge_test.egg-info/
+-rw-rw-rw-   0        0        0    21534 2024-04-18 05:54:16.000000 aibridge_test-0.3.2/aibridge_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-04-18 05:54:16.000000 aibridge_test-0.3.2/aibridge_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 05:54:16.000000 aibridge_test-0.3.2/aibridge_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      228 2024-04-18 05:54:16.000000 aibridge_test-0.3.2/aibridge_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-18 05:54:16.000000 aibridge_test-0.3.2/aibridge_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 05:54:17.041612 aibridge_test-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2863 2024-04-18 05:52:21.000000 aibridge_test-0.3.2/setup.py
```

### Comparing `aibridge_test-0.3.1/AIBridge/__init__.py` & `aibridge_test-0.3.2/AIBridge/__init__.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/ai21labs_text.py` & `aibridge_test-0.3.2/AIBridge/ai_services/ai21labs_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/ai_services_response.py` & `aibridge_test-0.3.2/AIBridge/ai_services/ai_services_response.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/anthropic_ai.py` & `aibridge_test-0.3.2/AIBridge/ai_services/anthropic_ai.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/cohere_llm.py` & `aibridge_test-0.3.2/AIBridge/ai_services/cohere_llm.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/geminin_services.py` & `aibridge_test-0.3.2/AIBridge/ai_services/geminin_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                     if response.candidates[0].content.parts[0].text:
                         content = response.candidates[0].content.parts[0].text
                     else:
                         content = response.candidates[0].content.parts[0].function_call
                         content = json.dumps(type(content).to_dict(content))
                         content = json.loads(content)
                         content = content["args"]
-                    output_tokens += exe_model.count_tokens(str(content))
+                    output_tokens += exe_model.count_tokens(str(content)).total_tokens
                     if output_format:
                         try:
                             if _formatter == "csv":
                                 content = FromJson.json_to_csv(content)
                             elif _formatter == "xml":
                                 content = FromJson.json_to_xml(content)
                         except AIBridgeException as e:
```

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/image_optimisaton.py` & `aibridge_test-0.3.2/AIBridge/ai_services/image_optimisaton.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/openai_images.py` & `aibridge_test-0.3.2/AIBridge/ai_services/openai_images.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/openai_services.py` & `aibridge_test-0.3.2/AIBridge/ai_services/openai_services.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/palm_chat.py` & `aibridge_test-0.3.2/AIBridge/ai_services/palm_chat.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/palm_text.py` & `aibridge_test-0.3.2/AIBridge/ai_services/palm_text.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/process_mq.py` & `aibridge_test-0.3.2/AIBridge/ai_services/process_mq.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/ai_services/stable_diffusion_image.py` & `aibridge_test-0.3.2/AIBridge/ai_services/stable_diffusion_image.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/constant/common.py` & `aibridge_test-0.3.2/AIBridge/constant/common.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/constant/constant.py` & `aibridge_test-0.3.2/AIBridge/constant/constant.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/database/db_layer.py` & `aibridge_test-0.3.2/AIBridge/database/db_layer.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/database/no_sql_service.py` & `aibridge_test-0.3.2/AIBridge/database/no_sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/database/session.py` & `aibridge_test-0.3.2/AIBridge/database/session.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/database/sql_service.py` & `aibridge_test-0.3.2/AIBridge/database/sql_service.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/exceptions.py` & `aibridge_test-0.3.2/AIBridge/exceptions.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/output_validation/convertors.py` & `aibridge_test-0.3.2/AIBridge/output_validation/convertors.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/output_validation/validations.py` & `aibridge_test-0.3.2/AIBridge/output_validation/validations.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/prompts/prompt_completion.py` & `aibridge_test-0.3.2/AIBridge/prompts/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/prompts/prompts_save.py` & `aibridge_test-0.3.2/AIBridge/prompts/prompts_save.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/prompts/prompts_varibales.py` & `aibridge_test-0.3.2/AIBridge/prompts/prompts_varibales.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/queue_integration/message_queue.py` & `aibridge_test-0.3.2/AIBridge/queue_integration/message_queue.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/queue_integration/queue_model.py` & `aibridge_test-0.3.2/AIBridge/queue_integration/queue_model.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/queue_integration/response_class.py` & `aibridge_test-0.3.2/AIBridge/queue_integration/response_class.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/AIBridge/setconfig.py` & `aibridge_test-0.3.2/AIBridge/setconfig.py`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/LICENSE` & `aibridge_test-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/PKG-INFO` & `aibridge_test-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.1
+Version: 0.3.2
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.1/README.md` & `aibridge_test-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/aibridge_test.egg-info/PKG-INFO` & `aibridge_test-0.3.2/aibridge_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aibridge_test
-Version: 0.3.1
+Version: 0.3.2
 Summary: Bridge for LLM"s
 Home-page: https://github.com/me/myproject
 Author: Ashish Tilekar
 Author-email: ashish.tilekar@opsfuse.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aibridge_test-0.3.1/aibridge_test.egg-info/SOURCES.txt` & `aibridge_test-0.3.2/aibridge_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aibridge_test-0.3.1/setup.py` & `aibridge_test-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "aibridge_test"
 DESCRIPTION = 'Bridge for LLM"s'
 URL = "https://github.com/me/myproject"
 EMAIL = "ashish.tilekar@opsfuse.com"
 AUTHOR = "Ashish Tilekar"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.3.1"
+VERSION = "0.3.2"
 REQUIRED = [
     "openai<=1.7.1",
     "SQLAlchemy>=2.0.19",
     "redis>=4.6.0",
     "PyYAML>=6.0.1",
     "Jinja2>=3.1.2",
     "pymongo>=4.4.1",
```
