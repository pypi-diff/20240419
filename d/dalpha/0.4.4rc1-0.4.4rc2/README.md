# Comparing `tmp/dalpha-0.4.4rc1.tar.gz` & `tmp/dalpha-0.4.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.4rc1.tar", max compression
+gzip compressed data, was "dalpha-0.4.4rc2.tar", max compression
```

## Comparing `dalpha-0.4.4rc1.tar` & `dalpha-0.4.4rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc1/README.md
--rw-r--r--   0        0        0    28316 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/dalpha/__init__.py
--rw-r--r--   0        0        0      275 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/context.py
--rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/dalpha_openai.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc1/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc1/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/logging/utils.py
--rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc1/dalpha/redis.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc1/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-04-19 05:24:16.908496 dalpha-0.4.4rc1/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc2/README.md
+-rw-r--r--   0        0        0    28316 2024-04-19 05:24:16.908496 dalpha-0.4.4rc2/dalpha/__init__.py
+-rw-r--r--   0        0        0      566 2024-04-19 07:52:17.137159 dalpha-0.4.4rc2/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/context.py
+-rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/dalpha_openai.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc2/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc2/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc2/dalpha/redis.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc2/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-04-19 07:52:17.137159 dalpha-0.4.4rc2/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc2/PKG-INFO
```

### Comparing `dalpha-0.4.4rc1/README.md` & `dalpha-0.4.4rc2/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/__init__.py` & `dalpha-0.4.4rc2/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/context.py` & `dalpha-0.4.4rc2/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/dalpha_openai.py` & `dalpha-0.4.4rc2/dalpha/dalpha_openai.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/logging/__init__.py` & `dalpha-0.4.4rc2/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/logging/log_formatter.py` & `dalpha-0.4.4rc2/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/logging/utils.py` & `dalpha-0.4.4rc2/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/dalpha/redis.py` & `dalpha-0.4.4rc2/dalpha/redis.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc1/pyproject.toml` & `dalpha-0.4.4rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.4rc1"
+version = "0.4.4rc2"
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
-version = "0.4.4rc1"
+version = "0.4.4rc2"
 authors = [
   { name="Beomseok", email="beomseok.lee@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dalpha-0.4.4rc1/PKG-INFO` & `dalpha-0.4.4rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.4rc1
+Version: 0.4.4rc2
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

