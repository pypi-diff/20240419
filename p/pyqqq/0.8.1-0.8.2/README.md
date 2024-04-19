# Comparing `tmp/pyqqq-0.8.1.tar.gz` & `tmp/pyqqq-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.8.1.tar", max compression
+gzip compressed data, was "pyqqq-0.8.2.tar", max compression
```

## Comparing `pyqqq-0.8.1.tar` & `pyqqq-0.8.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-28 03:41:58.980653 pyqqq-0.8.1/README.md
--rw-r--r--   0        0        0      770 2024-04-16 07:22:34.979272 pyqqq-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-16 07:09:31.610419 pyqqq-0.8.1/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302843 pyqqq-0.8.1/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 03:59:24.168676 pyqqq-0.8.1/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-12 08:13:19.751599 pyqqq-0.8.1/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-28 03:41:58.983583 pyqqq-0.8.1/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24284 2024-04-16 07:09:31.610652 pyqqq-0.8.1/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 03:41:58.983800 pyqqq-0.8.1/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302986 pyqqq-0.8.1/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 02:04:49.386336 pyqqq-0.8.1/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-28 03:41:58.984873 pyqqq-0.8.1/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-07 02:05:26.670417 pyqqq-0.8.1/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24453 2024-04-16 07:09:31.611164 pyqqq-0.8.1/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-22 01:44:28.626559 pyqqq-0.8.1/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-16 02:21:33.322054 pyqqq-0.8.1/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670533 pyqqq-0.8.1/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6677 2024-04-16 07:14:50.116239 pyqqq-0.8.1/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-12 08:13:19.753178 pyqqq-0.8.1/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-12 08:13:19.753716 pyqqq-0.8.1/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-12 08:13:19.754108 pyqqq-0.8.1/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-22 01:44:28.626857 pyqqq-0.8.1/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 08:13:19.754190 pyqqq-0.8.1/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 07:09:31.611654 pyqqq-0.8.1/pyqqq/executors/hook.py
--rw-r--r--   0        0        0   462038 2024-04-16 05:47:11.692471 pyqqq-0.8.1/pyqqq/test.ipynb
--rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670737 pyqqq-0.8.1/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-12 08:13:19.754605 pyqqq-0.8.1/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-16 07:09:31.611787 pyqqq-0.8.1/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:49:01.142004 pyqqq-0.8.1/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-22 01:44:28.626942 pyqqq-0.8.1/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-03-04 03:59:43.304644 pyqqq-0.8.1/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-28 03:41:58.986410 pyqqq-0.8.1/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 02:18:36.457903 pyqqq-0.8.1/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 07:09:31.611989 pyqqq-0.8.1/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-03-04 03:59:43.304764 pyqqq-0.8.1/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-27 01:29:00.427186 pyqqq-0.8.2/README.md
+-rw-r--r--   0        0        0      770 2024-04-19 14:22:12.063041 pyqqq-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-04-19 02:11:04.495312 pyqqq-0.8.2/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681470 pyqqq-0.8.2/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-06 00:30:01.958621 pyqqq-0.8.2/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-15 23:38:31.904216 pyqqq-0.8.2/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-27 01:29:00.428888 pyqqq-0.8.2/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-19 02:11:04.495645 pyqqq-0.8.2/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-27 03:32:53.313827 pyqqq-0.8.2/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:16:13.681703 pyqqq-0.8.2/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-03 06:40:50.199892 pyqqq-0.8.2/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-27 01:29:00.429820 pyqqq-0.8.2/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-06 00:30:01.960145 pyqqq-0.8.2/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24453 2024-04-19 02:11:04.496012 pyqqq-0.8.2/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-13 01:10:46.718207 pyqqq-0.8.2/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-15 23:38:31.905431 pyqqq-0.8.2/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:32.374681 pyqqq-0.8.2/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6677 2024-04-19 02:11:04.496254 pyqqq-0.8.2/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-15 23:38:31.905682 pyqqq-0.8.2/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-15 23:38:31.905855 pyqqq-0.8.2/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-15 23:38:31.906033 pyqqq-0.8.2/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-12 13:30:35.556769 pyqqq-0.8.2/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:38:31.906083 pyqqq-0.8.2/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-19 02:11:04.496835 pyqqq-0.8.2/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-03-06 03:23:38.166158 pyqqq-0.8.2/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-15 23:38:31.906445 pyqqq-0.8.2/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-15 23:38:31.906508 pyqqq-0.8.2/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 21:29:24.457837 pyqqq-0.8.2/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 13:30:35.556892 pyqqq-0.8.2/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-28 02:16:13.684707 pyqqq-0.8.2/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-27 01:29:00.430437 pyqqq-0.8.2/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-02 21:29:24.458374 pyqqq-0.8.2/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-19 02:11:04.497052 pyqqq-0.8.2/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-02-28 02:16:13.684870 pyqqq-0.8.2/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.2/PKG-INFO
```

### Comparing `pyqqq-0.8.1/README.md` & `pyqqq-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyproject.toml` & `pyqqq-0.8.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.8.1"
+version = "0.8.2"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tinydb = "^4.8.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
 websockets = "^12.0"
-pandas = "^1.5.3"
+pandas = "^2.0.3"
 cssutils = "^2.10.2"
 cachetools = "^5.3.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
 sphinx = "^7.2.6"
 myst-parser = "^2.0.0"
```

### Comparing `pyqqq-0.8.1/pyqqq/__init__.py` & `pyqqq-0.8.2/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.8.2/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.8.2/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.8.2/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.8.2/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.8.2/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.8.2/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.8.2/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.8.2/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.8.2/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/data/domestic.py` & `pyqqq-0.8.2/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/data/minutes.py` & `pyqqq-0.8.2/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/data/realtime.py` & `pyqqq-0.8.2/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/data/ticks.py` & `pyqqq-0.8.2/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/datatypes.py` & `pyqqq-0.8.2/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/executors/hook.py` & `pyqqq-0.8.2/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/array.py` & `pyqqq-0.8.2/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/compute.py` & `pyqqq-0.8.2/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/display.py` & `pyqqq-0.8.2/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/kvstore.py` & `pyqqq-0.8.2/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/limiter.py` & `pyqqq-0.8.2/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/logger.py` & `pyqqq-0.8.2/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/market_schedule.py` & `pyqqq-0.8.2/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/mock_api.py` & `pyqqq-0.8.2/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/pyqqq/utils/retry.py` & `pyqqq-0.8.2/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.1/PKG-INFO` & `pyqqq-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.8.1
+Version: 0.8.2
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: cssutils (>=2.10.2,<3.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
```

