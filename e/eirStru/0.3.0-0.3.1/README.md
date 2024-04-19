# Comparing `tmp/eirStru-0.3.0.tar.gz` & `tmp/eirStru-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.3.0.tar", last modified: Fri Apr 19 09:06:14 2024, max compression
+gzip compressed data, was "eirStru-0.3.1.tar", last modified: Fri Apr 19 11:29:36 2024, max compression
```

## Comparing `eirStru-0.3.0.tar` & `eirStru-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.768273 eirStru-0.3.0/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.0/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.0/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 09:06:14.768050 eirStru-0.3.0/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.0/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.767344 eirStru-0.3.0/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.0/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.0/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.0/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    18256 2024-04-18 16:43:10.000000 eirStru-0.3.0/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.0/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.0/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.0/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.0/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.0/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.0/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 09:06:14.767861 eirStru-0.3.0/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-19 09:06:14.000000 eirStru-0.3.0/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-19 09:06:14.768322 eirStru-0.3.0/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-19 09:06:12.000000 eirStru-0.3.0/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 11:29:36.627542 eirStru-0.3.1/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.3.1/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.3.1/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 11:29:36.627280 eirStru-0.3.1/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.3.1/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 11:29:36.626441 eirStru-0.3.1/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.3.1/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.3.1/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.3.1/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18324 2024-04-19 11:29:31.000000 eirStru-0.3.1/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     4341 2024-04-19 09:06:12.000000 eirStru-0.3.1/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     6488 2024-04-19 09:06:12.000000 eirStru-0.3.1/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.3.1/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.3.1/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1389 2024-04-18 23:20:17.000000 eirStru-0.3.1/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.3.1/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-19 11:29:36.627072 eirStru-0.3.1/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2963 2024-04-19 11:29:36.000000 eirStru-0.3.1/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-19 11:29:36.000000 eirStru-0.3.1/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-19 11:29:36.000000 eirStru-0.3.1/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-19 11:29:36.000000 eirStru-0.3.1/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-19 11:29:36.627590 eirStru-0.3.1/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3776 2024-04-19 11:29:31.000000 eirStru-0.3.1/setup.py
```

### Comparing `eirStru-0.3.0/LICENSE` & `eirStru-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/PKG-INFO` & `eirStru-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.0
+Version: 0.3.1
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.0/README.md` & `eirStru-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/aiomysql_helper.py` & `eirStru-0.3.1/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/common.py` & `eirStru-0.3.1/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,16 @@
     order_guid: Optional[str] = None
     task_info: Optional[EirTaskInfo] = None
     carrier_id: Optional[Any] = None  # 船公司
     bill_no: Optional[Any] = None  # 提单号
     booking_no: Optional[Any] = None  # 订舱号
     cyname: Optional[str] = None  # 推荐堆场
 
+    yard_info: Optional[Dict] = {}  # msk 推荐堆场，按箱型
+
     ctntype_id: Optional[str] = ''  # 箱型
     ctn_digit: Optional[int] = 0  # 箱量
     apply_ctntypedigit: Optional[str] = ''  # 需一次性申请的箱型箱量
 
     begin_time: Optional[datetime] = datetime.strptime(datetime.strftime(datetime.now(), '%Y-%m-%d %H:%M:%S'),
                                                        '%Y-%m-%d %H:%M:%S')  # 刷箱开始时间
     end_time: Optional[datetime] = datetime.strptime(
```

### Comparing `eirStru-0.3.0/eirStru/eirjob_intf.py` & `eirStru-0.3.1/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/eirlogin_intf.py` & `eirStru-0.3.1/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/redis_utils.py` & `eirStru-0.3.1/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/utils.py` & `eirStru-0.3.1/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru/wx_push.py` & `eirStru-0.3.1/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.3.0/eirStru.egg-info/PKG-INFO` & `eirStru-0.3.1/eirStru.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.3.0
+Version: 0.3.1
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.3.0/setup.py` & `eirStru-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.0'
+VERSION = '0.3.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

