# Comparing `tmp/dalpha-0.4.4rc0.tar.gz` & `tmp/dalpha-0.4.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.4rc0.tar", max compression
+gzip compressed data, was "dalpha-0.4.4rc1.tar", max compression
```

## Comparing `dalpha-0.4.4rc0.tar` & `dalpha-0.4.4rc1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc0/README.md
--rw-r--r--   0        0        0    27798 2024-04-08 01:16:34.229539 dalpha-0.4.4rc0/dalpha/__init__.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/context.py
--rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/dalpha_openai.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc0/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc0/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/logging/utils.py
--rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc0/dalpha/redis.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc0/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-04-08 01:16:34.229539 dalpha-0.4.4rc0/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc1/README.md
+-rw-r--r--   0        0        0    28316 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/dalpha/__init__.py
+-rw-r--r--   0        0        0      275 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/context.py
+-rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/dalpha_openai.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc1/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc1/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc1/dalpha/redis.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc1/PKG-INFO
```

### Comparing `dalpha-0.4.4rc0/README.md` & `dalpha-0.4.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/__init__.py` & `dalpha-0.4.4rc1/dalpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import requests, json, boto3, io, logging, sys, os, pkg_resources
 import time
 import sentry_sdk
 from requests.adapters import HTTPAdapter, Retry
 
+from dalpha.cobra_cls import Cobra
+
 from dalpha.signal_handler import get_shutdown_requested
 from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, Context
 from dalpha.logging import logger
 from dalpha.logging.events import Event
 
 def __load_config(file_path):
     if not os.path.isfile(file_path):
@@ -291,15 +293,14 @@
                 for message in messages:
                     try:
                         message_dict = json.loads(message.value.decode('utf-8'))
                     except json.JSONDecodeError:
                         # TODO: 현재 로직이면 이 경우 offset skip 됨, 잘못된 동작은 아닌 듯 하나 체크 필요
                         logger.error("유효한 JSON 형식이 아닙니다.")
                         continue
-                    self.evaluates[message.key] = message.offset
                     ret.append(message_dict)
 
             # TODO: filter_valid kafka에도 구현 (receiptHandle은 필요 없으나, 경우에 따라 불필요한 메세지 제거)
 
             if len(ret) == 0:
                 return None
             elif len(ret) == 1:
@@ -412,14 +413,15 @@
                 break
             for message in messages:
                 try:
                     message_dict = json.loads(message.value.decode('utf-8'))
                 except json.JSONDecodeError:
                     logger.error("유효한 JSON 형식이 아닙니다.")
                     continue
+                # TODO(XXX): evaluates key 관리 필요 없다면 제거, commit 할 때 지워주지 않고 있음
                 self.evaluates[message.key] = message.offset
                 ret.append(message_dict['payload'])
 
         if len(ret) == 0:
             return None
         elif len(ret) == 1:
             logger.info(
@@ -478,15 +480,20 @@
         try:
             if mock:
                 logger.info(message = f"validate payload - {output}")
                 return
             if inference_time == None and self.poll_time != None:
                 inference_time = time.time() - self.poll_time
                 self.poll_time = None
-            if self.use_sqs:
+            if self.use_kafka:
+                try:
+                    self.kafka_consumer.commit()
+                except Exception as e:
+                    logger.error(f"error from kafka commit\n{e}")
+            elif self.use_sqs:
                 try: 
                     response = self.sqs.delete_message(
                         QueueUrl = self.queue_url,
                         ReceiptHandle = self.evaluates[evaluate_id]
                     )
                 except Exception as e:
                     logger.error(f"error from sqs.delete_message\n{e}")
@@ -541,15 +548,20 @@
                 })
             except Exception as e:
                 Exception("failed to parse validate_error input : ", e)
             if mock:
                 logger.info(message = f"validate_error payload - {output}")
                 return
 
-            if self.use_sqs:
+            if self.use_kafka:
+                try:
+                    self.kafka_consumer.commit()
+                except Exception as e:
+                    self.kafka_consumer.commit(f"error from kafka.commit\n{e}")
+            elif self.use_sqs:
                 try: 
                     response = self.sqs.delete_message(
                         QueueUrl = self.queue_url,
                         ReceiptHandle = self.evaluates[evaluate_id]
                     )
                 except Exception as e:
                     logger.error(f"error from sqs.delete_message\n{e}")
```

### Comparing `dalpha-0.4.4rc0/dalpha/context.py` & `dalpha-0.4.4rc1/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/dalpha_openai.py` & `dalpha-0.4.4rc1/dalpha/dalpha_openai.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/logging/__init__.py` & `dalpha-0.4.4rc1/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/logging/log_formatter.py` & `dalpha-0.4.4rc1/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/logging/utils.py` & `dalpha-0.4.4rc1/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/dalpha/redis.py` & `dalpha-0.4.4rc1/dalpha/redis.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc0/pyproject.toml` & `dalpha-0.4.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.4rc0"
+version = "0.4.4rc1"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,15 +16,15 @@
 kafka-python = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.4rc0"
+version = "0.4.4rc1"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.4.4rc0/PKG-INFO` & `dalpha-0.4.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.4rc0
+Version: 0.4.4rc1
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

