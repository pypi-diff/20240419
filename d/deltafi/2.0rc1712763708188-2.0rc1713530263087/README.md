# Comparing `tmp/deltafi-2.0rc1712763708188.tar.gz` & `tmp/deltafi-2.0rc1713530263087.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltafi-2.0rc1712763708188.tar", max compression
+gzip compressed data, was "deltafi-2.0rc1713530263087.tar", max compression
```

## Comparing `deltafi-2.0rc1712763708188.tar` & `deltafi-2.0rc1713530263087.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      189 2023-08-18 18:44:06.655768 deltafi-2.0rc1712763708188/README.md
--rw-r--r--   0        0        0      709 2023-09-12 19:43:28.655326 deltafi-2.0rc1712763708188/deltafi/__init__.py
--rw-r--r--   0        0        0     5323 2024-04-10 15:22:52.625810 deltafi-2.0rc1712763708188/deltafi/action.py
--rw-r--r--   0        0        0     2847 2023-10-25 16:46:16.158339 deltafi-2.0rc1712763708188/deltafi/actioneventqueue.py
--rw-r--r--   0        0        0      865 2024-04-10 15:22:52.626810 deltafi-2.0rc1712763708188/deltafi/actiontype.py
--rw-r--r--   0        0        0    11301 2024-04-10 15:22:52.627810 deltafi-2.0rc1712763708188/deltafi/domain.py
--rw-r--r--   0        0        0      943 2024-04-10 15:22:52.628810 deltafi-2.0rc1712763708188/deltafi/exception.py
--rw-r--r--   0        0        0     1090 2023-11-15 20:50:55.275227 deltafi-2.0rc1712763708188/deltafi/genericmodel.py
--rw-r--r--   0        0        0     1656 2024-04-10 15:22:52.630810 deltafi-2.0rc1712763708188/deltafi/input.py
--rw-r--r--   0        0        0     2136 2023-08-18 18:44:06.656768 deltafi-2.0rc1712763708188/deltafi/logger.py
--rw-r--r--   0        0        0      967 2023-08-18 18:44:06.656768 deltafi-2.0rc1712763708188/deltafi/metric.py
--rw-r--r--   0        0        0    12294 2024-04-10 15:22:52.631810 deltafi-2.0rc1712763708188/deltafi/plugin.py
--rw-r--r--   0        0        0     8177 2024-04-10 15:22:52.633810 deltafi-2.0rc1712763708188/deltafi/result.py
--rw-r--r--   0        0        0     2740 2023-09-05 12:02:08.690603 deltafi-2.0rc1712763708188/deltafi/storage.py
--rw-r--r--   0        0        0      709 2023-09-12 19:43:28.657326 deltafi-2.0rc1712763708188/deltafi/test_kit/__init__.py
--rw-r--r--   0        0        0     1378 2023-09-12 19:43:28.662326 deltafi-2.0rc1712763708188/deltafi/test_kit/assertions.py
--rw-r--r--   0        0        0     1581 2023-09-12 19:43:28.662326 deltafi-2.0rc1712763708188/deltafi/test_kit/compare_helpers.py
--rw-r--r--   0        0        0      833 2023-08-18 18:44:06.657768 deltafi-2.0rc1712763708188/deltafi/test_kit/constants.py
--rw-r--r--   0        0        0     2090 2024-01-29 15:59:31.393845 deltafi-2.0rc1712763708188/deltafi/test_kit/domain.py
--rw-r--r--   0        0        0     1899 2024-01-29 15:59:31.394845 deltafi-2.0rc1712763708188/deltafi/test_kit/egress.py
--rw-r--r--   0        0        0     2587 2024-01-29 15:59:31.394845 deltafi-2.0rc1712763708188/deltafi/test_kit/enrich.py
--rw-r--r--   0        0        0    14602 2024-04-10 15:22:52.633810 deltafi-2.0rc1712763708188/deltafi/test_kit/framework.py
--rw-r--r--   0        0        0     4085 2024-04-10 15:22:52.634811 deltafi-2.0rc1712763708188/deltafi/test_kit/transform.py
--rw-r--r--   0        0        0     1933 2024-01-29 15:59:31.395845 deltafi-2.0rc1712763708188/deltafi/test_kit/validate.py
--rw-r--r--   0        0        0     1310 2024-04-10 15:42:11.789872 deltafi-2.0rc1712763708188/pyproject.toml
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1712763708188/PKG-INFO
+-rw-r--r--   0        0        0      189 2023-04-10 13:32:51.621370 deltafi-2.0rc1713530263087/README.md
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:19.408525 deltafi-2.0rc1713530263087/deltafi/__init__.py
+-rw-r--r--   0        0        0     5323 2024-04-19 12:26:50.356820 deltafi-2.0rc1713530263087/deltafi/action.py
+-rw-r--r--   0        0        0     2847 2023-10-25 14:03:47.782289 deltafi-2.0rc1713530263087/deltafi/actioneventqueue.py
+-rw-r--r--   0        0        0      865 2024-04-19 12:26:50.356820 deltafi-2.0rc1713530263087/deltafi/actiontype.py
+-rw-r--r--   0        0        0    11301 2024-04-19 12:26:50.356820 deltafi-2.0rc1713530263087/deltafi/domain.py
+-rw-r--r--   0        0        0      943 2024-04-19 12:26:50.356820 deltafi-2.0rc1713530263087/deltafi/exception.py
+-rw-r--r--   0        0        0     1090 2023-11-15 22:01:12.726378 deltafi-2.0rc1713530263087/deltafi/genericmodel.py
+-rw-r--r--   0        0        0     1656 2024-04-19 12:26:50.356820 deltafi-2.0rc1713530263087/deltafi/input.py
+-rw-r--r--   0        0        0     2136 2023-04-10 13:32:51.623371 deltafi-2.0rc1713530263087/deltafi/logger.py
+-rw-r--r--   0        0        0      967 2023-04-10 13:32:51.623371 deltafi-2.0rc1713530263087/deltafi/metric.py
+-rw-r--r--   0        0        0    12294 2024-04-19 12:26:50.357821 deltafi-2.0rc1713530263087/deltafi/plugin.py
+-rw-r--r--   0        0        0     8177 2024-04-19 12:26:50.357821 deltafi-2.0rc1713530263087/deltafi/result.py
+-rw-r--r--   0        0        0     2740 2023-05-19 17:18:33.056792 deltafi-2.0rc1713530263087/deltafi/storage.py
+-rw-r--r--   0        0        0      709 2023-10-18 22:01:19.414525 deltafi-2.0rc1713530263087/deltafi/test_kit/__init__.py
+-rw-r--r--   0        0        0     1378 2023-10-18 22:01:19.414525 deltafi-2.0rc1713530263087/deltafi/test_kit/assertions.py
+-rw-r--r--   0        0        0     1581 2023-10-18 22:01:19.414525 deltafi-2.0rc1713530263087/deltafi/test_kit/compare_helpers.py
+-rw-r--r--   0        0        0      833 2023-10-18 22:01:19.414525 deltafi-2.0rc1713530263087/deltafi/test_kit/constants.py
+-rw-r--r--   0        0        0     2090 2024-01-29 15:43:38.761375 deltafi-2.0rc1713530263087/deltafi/test_kit/domain.py
+-rw-r--r--   0        0        0     1899 2024-01-29 15:43:38.761375 deltafi-2.0rc1713530263087/deltafi/test_kit/egress.py
+-rw-r--r--   0        0        0     2587 2024-01-29 15:43:38.761375 deltafi-2.0rc1713530263087/deltafi/test_kit/enrich.py
+-rw-r--r--   0        0        0    14602 2024-04-19 12:26:50.358821 deltafi-2.0rc1713530263087/deltafi/test_kit/framework.py
+-rw-r--r--   0        0        0     4085 2024-04-19 12:26:50.358821 deltafi-2.0rc1713530263087/deltafi/test_kit/transform.py
+-rw-r--r--   0        0        0     1933 2024-01-29 15:43:38.763375 deltafi-2.0rc1713530263087/deltafi/test_kit/validate.py
+-rw-r--r--   0        0        0     1310 2024-04-19 12:38:08.410106 deltafi-2.0rc1713530263087/pyproject.toml
+-rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 deltafi-2.0rc1713530263087/PKG-INFO
```

### Comparing `deltafi-2.0rc1712763708188/deltafi/__init__.py` & `deltafi-2.0rc1713530263087/deltafi/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/action.py` & `deltafi-2.0rc1713530263087/deltafi/action.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/actioneventqueue.py` & `deltafi-2.0rc1713530263087/deltafi/actioneventqueue.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/actiontype.py` & `deltafi-2.0rc1713530263087/deltafi/actiontype.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/domain.py` & `deltafi-2.0rc1713530263087/deltafi/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/exception.py` & `deltafi-2.0rc1713530263087/deltafi/exception.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/genericmodel.py` & `deltafi-2.0rc1713530263087/deltafi/genericmodel.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/input.py` & `deltafi-2.0rc1713530263087/deltafi/input.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/logger.py` & `deltafi-2.0rc1713530263087/deltafi/logger.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/metric.py` & `deltafi-2.0rc1713530263087/deltafi/metric.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/plugin.py` & `deltafi-2.0rc1713530263087/deltafi/plugin.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/result.py` & `deltafi-2.0rc1713530263087/deltafi/result.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/storage.py` & `deltafi-2.0rc1713530263087/deltafi/storage.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/__init__.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/__init__.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/assertions.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/assertions.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/compare_helpers.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/compare_helpers.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/constants.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/constants.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/domain.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/domain.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/egress.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/egress.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/enrich.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/enrich.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/framework.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/framework.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/transform.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/transform.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/deltafi/test_kit/validate.py` & `deltafi-2.0rc1713530263087/deltafi/test_kit/validate.py`

 * *Files identical despite different names*

### Comparing `deltafi-2.0rc1712763708188/pyproject.toml` & `deltafi-2.0rc1713530263087/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltafi"
-version = "2.0rc1712763708188"
+version = "2.0rc1713530263087"
 description = "SDK for DeltaFi plugins and actions"
 authors = ["DeltaFi <deltafi@systolic.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 keywords = ["deltafi"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `deltafi-2.0rc1712763708188/PKG-INFO` & `deltafi-2.0rc1713530263087/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltafi
-Version: 2.0rc1712763708188
+Version: 2.0rc1713530263087
 Summary: SDK for DeltaFi plugins and actions
 License: Apache License, Version 2.0
 Keywords: deltafi
 Author: DeltaFi
 Author-email: deltafi@systolic.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

