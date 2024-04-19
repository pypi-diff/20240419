# Comparing `tmp/aporacle-0.0.136.tar.gz` & `tmp/aporacle-0.0.137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.136.tar", max compression
+gzip compressed data, was "aporacle-0.0.137.tar", max compression
```

## Comparing `aporacle-0.0.136.tar` & `aporacle-0.0.137.tar`

### file list

```diff
@@ -1,26 +1,21 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.136/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.136/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.136/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.136/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.136/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.136/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.136/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.136/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.136/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-25 05:26:42.304279 aporacle-0.0.136/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.136/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.136/aporacle/data/db/crud.py
--rw-r--r--   0        0        0    10174 2024-03-22 09:49:57.935682 aporacle-0.0.136/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.136/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.136/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.136/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:16.424282 aporacle-0.0.136/aporacle/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:56.392617 aporacle-0.0.136/aporacle/ml/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:09:40.520484 aporacle-0.0.136/aporacle/ml/train/__init__.py
--rw-r--r--   0        0        0        0 2024-03-10 10:41:27.060572 aporacle-0.0.136/aporacle/ml/train/base/__init__.py
--rw-r--r--   0        0        0     4327 2024-03-25 03:23:22.081532 aporacle-0.0.136/aporacle/ml/train/base/training_runner.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.136/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.136/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.136/aporacle/shared_setup.py
--rw-r--r--   0        0        0      447 2024-04-19 05:22:52.676114 aporacle-0.0.136/pyproject.toml
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 aporacle-0.0.136/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.137/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.137/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.137/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.137/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.137/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.137/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.137/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.137/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.137/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1459 2024-03-25 05:26:42.304279 aporacle-0.0.137/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.137/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.137/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0    10174 2024-03-22 09:49:57.935682 aporacle-0.0.137/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.137/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.137/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.137/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.137/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.137/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.137/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-04-19 05:34:07.279268 aporacle-0.0.137/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.137/PKG-INFO
```

### Comparing `aporacle-0.0.136/aporacle/broadcast/__init__.py` & `aporacle-0.0.137/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/conf/__init__.py` & `aporacle-0.0.137/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.137/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/data/asset/__init__.py` & `aporacle-0.0.137/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/data/combination.py` & `aporacle-0.0.137/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/data/db/crud.py` & `aporacle-0.0.137/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/data/gcp/__init__.py` & `aporacle-0.0.137/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/data/symbols/__init__.py` & `aporacle-0.0.137/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/execution/executables.py` & `aporacle-0.0.137/aporacle/execution/executables.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/network/network_base.py` & `aporacle-0.0.137/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/aporacle/shared_setup.py` & `aporacle-0.0.137/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.136/PKG-INFO` & `aporacle-0.0.137/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.136
+Version: 0.0.137
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
 Requires-Dist: komoutils (>=0.0.224,<0.0.225)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
-Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
 Description-Content-Type: text/markdown
```

