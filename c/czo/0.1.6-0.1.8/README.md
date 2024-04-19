# Comparing `tmp/czo-0.1.6.tar.gz` & `tmp/czo-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czo-0.1.6.tar", last modified: Tue Apr  2 05:37:19 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `czo-0.1.6.tar` & `czo-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.767175 czo-0.1.6/
--rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      237 2024-04-02 05:37:19.767175 czo-0.1.6/PKG-INFO
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       83 2024-03-27 06:33:55.000000 czo-0.1.6/README.md
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       38 2024-04-02 05:37:19.767175 czo-0.1.6/setup.cfg
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      394 2024-04-02 05:36:47.000000 czo-0.1.6/setup.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/czo/
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      232 2024-03-31 07:44:26.000000 czo-0.1.6/src/czo/__init__.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     8557 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_date.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    12017 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_faker.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     5943 2024-04-02 05:36:58.000000 czo-0.1.6/src/czo/_path.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)     4781 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/_rand.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.763174 czo-0.1.6/src/czo/data/
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/__init__.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    14519 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_country.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)    16493 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_housing.py
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)   154755 2024-03-27 06:33:55.000000 czo-0.1.6/src/czo/data/_internal_utils.py
-drwxrwxr-x   0 sfwwslm   (1000) sfwwslm   (1000)        0 2024-04-02 05:37:19.767175 czo-0.1.6/src/czo.egg-info/
--rw-r--r--   0 sfwwslm   (1000) sfwwslm   (1000)      237 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/PKG-INFO
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)      368 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/SOURCES.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        1 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/dependency_links.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)       25 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/requires.txt
--rw-rw-r--   0 sfwwslm   (1000) sfwwslm   (1000)        4 2024-04-02 05:37:19.000000 czo-0.1.6/src/czo.egg-info/top_level.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 czo-0.1.8/czo/__init__.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_date.py
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_faker.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_net.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_path.py
+-rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_rand.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/__init__.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_country.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_housing.py
+-rw-r--r--   0        0        0   154755 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_internal_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 czo-0.1.8/czo/utils/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 czo-0.1.8/czo/utils/__meta.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 czo-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 czo-0.1.8/LICENSE
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 czo-0.1.8/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 czo-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 czo-0.1.8/PKG-INFO
```

### Comparing `czo-0.1.6/src/czo/_date.py` & `czo-0.1.8/czo/_date.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,21 +110,21 @@
     def difference_time_two(date1: str, date2: str, reversal: bool = False) -> float:
         """
         计算两个日期之间的时间差（以秒为单位）。
 
         Args:
             date1: 第一个日期，格式为"%Y-%m-%d %H:%M:%S"。
             date2: 第二个日期，格式为"%Y-%m-%d %H:%M:%S"。
-            reversal: 是否将第一个日期作为基准日期，默认为False。
+            reversal: 默认使用 date2 - date1 的方式计算时间差，如果为 True，则使用 date1 - date2 的方式计算时间差。
 
         Returns:
             两个日期之间的时间差，以秒为单位。
 
         Examples:
-            >>> difference_time_two("2022-01-01 12:00:00", "2022-01-01 10:00:00")
+            >>> difference_time_two("2022-01-01 10:00:00", "2022-01-01 12:00:00")
             7200.0
         """
         date1 = datetime.datetime.strptime(date1, "%Y-%m-%d %H:%M:%S")
         date2 = datetime.datetime.strptime(date2, "%Y-%m-%d %H:%M:%S")
         if reversal:
             date1, date2 = date2, date1
         return (date2 - date1).total_seconds()
```

### Comparing `czo-0.1.6/src/czo/_faker.py` & `czo-0.1.8/czo/_faker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import random
 import string
 
+from .utils import Singleton
 
-class Faker:
+
+class Faker(Singleton):
     """伪造常用数据"""
 
     @property
     def __areaCodeDict(self) -> dict:
         """区域文件地址"""
         from .data._internal_utils import dataDict
         return dataDict
```

### Comparing `czo-0.1.6/src/czo/_path.py` & `czo-0.1.8/czo/_path.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.6/src/czo/_rand.py` & `czo-0.1.8/czo/_rand.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,7 +142,14 @@
         """
         生成一个随机的IPv6地址。
 
         Returns:
         - IPv6Address: 返回一个随机生成的IPv6地址对象。
         """
         return ipaddress.IPv6Address(random.randint(0, 2**128-1))
+
+    @staticmethod
+    def mac():
+
+        mac_address = ':'.join(['{:02x}'.format(
+            (uuid.getnode() >> elements) & 0xff) for elements in range(0, 2*6, 2)])
+        return mac_address
```

### Comparing `czo-0.1.6/src/czo/data/_country.py` & `czo-0.1.8/czo/data/_country.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.6/src/czo/data/_housing.py` & `czo-0.1.8/czo/data/_housing.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.6/src/czo/data/_internal_utils.py` & `czo-0.1.8/czo/data/_internal_utils.py`

 * *Files identical despite different names*

