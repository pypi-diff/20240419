# Comparing `tmp/alibabacloud_filedetect-1.0.1.tar.gz` & `tmp/alibabacloud_filedetect-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_filedetect-1.0.1.tar", last modified: Mon Sep 19 11:32:53 2022, max compression
+gzip compressed data, was "dist/alibabacloud_filedetect-1.1.0.tar", last modified: Thu Apr 18 06:36:48 2024, max compression
```

## Comparing `alibabacloud_filedetect-1.0.1.tar` & `alibabacloud_filedetect-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2178 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2178 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      117 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      624 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    11357 2022-09-19 11:03:47.000000 alibabacloud_filedetect-1.0.1/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-19 11:32:53.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/
--rw-r--r--   0 root         (0) root         (0)      576 2022-08-19 06:50:31.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/ERR_CODE.py
--rw-r--r--   0 root         (0) root         (0)     5680 2022-08-21 09:21:13.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/MiniThreadPool.py
--rw-r--r--   0 root         (0) root         (0)    12420 2022-09-08 02:51:06.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/ScanTask.py
--rw-r--r--   0 root         (0) root         (0)      394 2022-08-31 11:15:43.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/IDetectResultCallback.py
--rw-r--r--   0 root         (0) root         (0)     3694 2022-08-31 11:17:09.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/DetectResult.py
--rw-r--r--   0 root         (0) root         (0)     8561 2022-08-31 11:21:21.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/OpenAPIDetector.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-09-19 11:30:43.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/__init__.py
--rw-r--r--   0 root         (0) root         (0)      555 2022-09-08 02:48:12.000000 alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/Config.py
--rw-r--r--   0 root         (0) root         (0)     1148 2022-09-19 11:13:23.000000 alibabacloud_filedetect-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)       43 2022-09-15 11:31:36.000000 alibabacloud_filedetect-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)     2564 2022-09-15 11:40:25.000000 alibabacloud_filedetect-1.0.1/setup.py
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-01 03:25:15.000000 alibabacloud_filedetect-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1252 2022-09-19 11:12:24.000000 alibabacloud_filedetect-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:36:48.000000 alibabacloud_filedetect-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 06:36:48.000000 alibabacloud_filedetect-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-18 06:36:48.000000 alibabacloud_filedetect-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:36:48.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-18 06:36:47.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-18 06:36:47.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-18 06:36:47.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 06:36:47.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      662 2024-04-18 06:36:47.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-09-19 11:03:47.000000 alibabacloud_filedetect-1.1.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 06:36:48.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/
+-rw-r--r--   0 root         (0) root         (0)      647 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/ERR_CODE.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/MiniThreadPool.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/Decompress.py
+-rw-r--r--   0 root         (0) root         (0)    17065 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/ScanTask.py
+-rw-r--r--   0 root         (0) root         (0)      394 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/IDetectResultCallback.py
+-rw-r--r--   0 root         (0) root         (0)     4533 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/DetectResult.py
+-rw-r--r--   0 root         (0) root         (0)    11263 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/OpenAPIDetector.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-18 06:28:56.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      555 2024-04-12 01:46:41.000000 alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/Config.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2022-09-19 11:13:23.000000 alibabacloud_filedetect-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      171 2024-04-18 06:28:04.000000 alibabacloud_filedetect-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)     2564 2024-04-18 06:25:59.000000 alibabacloud_filedetect-1.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-01 03:25:15.000000 alibabacloud_filedetect-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1252 2022-09-19 11:12:24.000000 alibabacloud_filedetect-1.1.0/README.md
```

### Comparing `alibabacloud_filedetect-1.0.1/PKG-INFO` & `alibabacloud_filedetect-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_filedetect
-Version: 1.0.1
+Version: 1.1.0
 Summary: Alibaba Cloud File Detection SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-file-detect-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Keywords: alibabacloud,file_detect_python_sdk
 Platform: any
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/PKG-INFO` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-filedetect
-Version: 1.0.1
+Version: 1.1.0
 Summary: Alibaba Cloud File Detection SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-file-detect-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Keywords: alibabacloud,file_detect_python_sdk
 Platform: any
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect.egg-info/SOURCES.txt` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE
 MANIFEST.in
 README-CN.md
 README.md
 setup.cfg
 setup.py
 alibabacloud_filedetect/Config.py
+alibabacloud_filedetect/Decompress.py
 alibabacloud_filedetect/DetectResult.py
 alibabacloud_filedetect/ERR_CODE.py
 alibabacloud_filedetect/IDetectResultCallback.py
 alibabacloud_filedetect/MiniThreadPool.py
 alibabacloud_filedetect/OpenAPIDetector.py
 alibabacloud_filedetect/ScanTask.py
 alibabacloud_filedetect/__init__.py
```

### Comparing `alibabacloud_filedetect-1.0.1/LICENSE` & `alibabacloud_filedetect-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/ERR_CODE.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/ERR_CODE.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from enum import Enum
 
 class ERR_CODE(Enum):
-
     ERR_INIT = -100 # 需要初始化，或者重复初始化
     ERR_FILE_NOT_FOUND = -99 # 文件未找到
     ERR_DETECT_QUEUE_FULL = -98 # 检测队列满
     ERR_CALL_API = -97  # 调用API错误
     ERR_TIMEOUT = -96  # 超时
     ERR_UPLOAD = -95  # 文件上传失败；用户可重新发起检测，再次尝试
     ERR_ABORT = -94  # 程序退出，样本未得到检测
     ERR_TIMEOUT_QUEUE = -93  # 队列超时，用户发起检测频率过高或超时时间过短
+    ERR_MD5 = -92 # MD5格式不对
+    ERR_URL = -91 # URL格式不对
     ERR_SUCC = 0 # 成功
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/MiniThreadPool.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/MiniThreadPool.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/ScanTask.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/ScanTask.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,99 +30,125 @@
     REQUEST_TOO_FREQUENTLY = 2000 # 请求太频繁，请稍后再试
     HAS_EXCEPTION = -1 # 存在异常
     IS_OK = 0
     IS_BLACK = 1 # 可疑文件
     IS_DETECTING = 3 # 检测中，请等待
     
 
-    def __init__(self, file_path, size, timeout, callback):
-        self.__m_seq = 0
-        self.__m_path = file_path
-        self.__m_size = size
-        self.__m_timeout = timeout
-        self.__m_callback = callback
-        self.__m_result = DetectResult()
-        
-        self.__m_start_time = self.currentTimeMillis()
-        self.__m_last_time = 0
+    def __init__(self):
+        self.__seq = 0
+        self.__path = None
+        self.__size = 0
+        self.__timeout = 0
+        self.__callback = None
+        self.__result = DetectResult()
+        
+        self.__start_time = 0
+        self.__last_time = 0
+
+        self.__taskCallback = None
+        self.__decompress = None
+        self.__islocal = True # 是否为本地文件
+
+    
+    def __currentTimeMillis(self):
+        return int(round(time.time() * 1000))
 
-        self.__m_taskCallback = None
+
+    def initScanFile(self, file_path, size, timeout, callback, decompress):
+        self.__islocal = True
+        self.__path = file_path
+        self.__size = size
+        self.__timeout = timeout
+        self.__callback = callback
+        self.__start_time = self.__currentTimeMillis()
+        self.__decompress = decompress
+
+
+    def initScanUrl(self, url, md5, timeout, callback, decompress):
+        self.__islocal = False
+        self.__path = url
+        self.__result.md5 = md5
+        self.__timeout = timeout
+        self.__callback = callback
+        self.__start_time = self.__currentTimeMillis()
+        self.__decompress = decompress
 
     
     def setSeq(self, seq):
-        self.__m_seq = seq
+        self.__seq = seq
 
 
     def getSeq(self):
-        return self.__m_seq
+        return self.__seq
 
 
     def setTaskCallback(self, callback):
-        self.__m_taskCallback = callback
-        if self.__m_taskCallback is not None:
-            self.__m_taskCallback.onTaskBegin(self)
+        self.__taskCallback = callback
+        if self.__taskCallback is not None:
+            self.__taskCallback.onTaskBegin(self)
         
 
     def run(self):
         from .OpenAPIDetector import OpenAPIDetector
         # 缓存对象
         detector = OpenAPIDetector.get_instance()
 
-        client = detector.m_client
-        client_opt = detector.m_client_opt
+        client = detector.client
+        client_opt = detector.client_opt
 
-        queue = detector.m_queue
-        if detector.m_is_inited is False or client is None or queue is None:
-             self.errorCallback(ERR_CODE.ERR_INIT, None)
+        queue = detector.queue
+        if detector.is_inited is False or client is None or queue is None:
+             self.errorCallback(ERR_CODE.ERR_INIT, self.__path)
              return
         
 
         # 判断是否已超时
         if self.__checkTimeout():
             return
         
         
         # 计算文件md5
-        if self.__m_result.md5 is None:
-            self.__m_result.md5 = self.__calcMd5(self.__m_path)
-            if self.__m_result.md5 is None:
-                self.errorCallback(ERR_CODE.ERR_FILE_NOT_FOUND, None)
+        if self.__result.md5 is None:
+            self.__result.md5 = self.__calcMd5(self.__path)
+            if self.__result.md5 is None:
+                self.errorCallback(ERR_CODE.ERR_FILE_NOT_FOUND, self.__path)
                 return
         
 
         # 如果距离上次查询过短，则需要等待一会
-        if self.currentTimeMillis() - self.__m_last_time < Config.QUERY_RESULT_INTERVAL:
+        if self.__currentTimeMillis() - self.__last_time < Config.QUERY_RESULT_INTERVAL:
             with queue:
                 queue.wait(Config.QUERY_RESULT_INTERVAL/1000.0)
-            if self.currentTimeMillis() - self.__m_last_time < Config.QUERY_RESULT_INTERVAL:
+            if self.__currentTimeMillis() - self.__last_time < Config.QUERY_RESULT_INTERVAL:
                 # 时间不够就放到队列里去
                 queue.addLast(self)
                 return
 
         # 更新时间戳
-        self.__m_last_time = self.currentTimeMillis()
+        self.__last_time = self.__currentTimeMillis()
 
         # 获取扫描结果
         result_info = None
         while True:
-            result_info = self.__getResultByAPI(client, client_opt, self.__m_result.md5)
+            result_info = self.__getResultByAPI(client, client_opt, self.__result.md5)
             if result_info.result != self.REQUEST_TOO_FREQUENTLY:
                 break
             self.__needSleep(Config.REQUEST_TOO_FREQUENTLY_SLEEP_TIME) # 请求太过频繁，需要休眠
             # 判断是否已超时
             if self.__checkTimeout():
                 return
         
         if result_info.result == self.HAS_EXCEPTION:
             return # 出错，退出
         elif result_info.result == self.GET_RESULT_FAIL:
             # 没有结果，则尝试上传文件
             detect_ret = 0
             while True:
-                detect_ret = self.__uploadAndDetectByAPI(client, client_opt, self.__m_path, self.__m_result.md5)
+                detect_ret = self.__uploadAndDetectByAPI(client, client_opt, self.__path, self.__result.md5)
                 if detect_ret != self.REQUEST_TOO_FREQUENTLY:
                     break
                 
                 self.__needSleep(Config.REQUEST_TOO_FREQUENTLY_SLEEP_TIME) # 请求太过频繁，需要休眠
                 if self.__checkTimeout():
                     return
 
@@ -133,50 +159,45 @@
             self.okCallback(True, result_info) # 报黑
         elif result_info.result == self.IS_DETECTING: # 检测中，请等待
             queue.addLast(self)
         else:
             self.okCallback(False, result_info) # 其他结果均为白
 
 
-    def currentTimeMillis(self):
-        return int(round(time.time() * 1000))
-
-
     def errorCallback(self, errCode, errString):
-        self.__m_result.error_code = errCode
-        self.__m_result.error_string = errString
-        self.__m_result.time =  self.currentTimeMillis() - self.__m_start_time
-        if self.__m_taskCallback is not None:
-            self.__m_taskCallback.onTaskEnd(self)
-        if self.__m_callback is not None:
-            self.__m_callback.onScanResult(self.__m_seq, self.__m_path, self.__m_result)
+        self.__result.error_code = errCode
+        self.__result.error_string = errString
+        self.__result.time =  self.__currentTimeMillis() - self.__start_time
+        if self.__taskCallback is not None:
+            self.__taskCallback.onTaskEnd(self)
+        if self.__callback is not None:
+            self.__callback.onScanResult(self.__seq, self.__path, self.__result)
         
 
-
     def okCallback(self, is_black, result_info):
-        self.__m_result.error_code = ERR_CODE.ERR_SUCC
-        self.__m_result.result = DetectResult.RESULT.RES_BLACK if is_black else DetectResult.RESULT.RES_WHITE
-        self.__m_result.time = self.currentTimeMillis() - self.__m_start_time
-        self.__m_result.score = result_info.score
-        self.__m_result.virus_type = result_info.virus_type
-        self.__m_result.ext_info = result_info.ext
-        if self.__m_taskCallback is not None:
-            self.__m_taskCallback.onTaskEnd(self)
-        if self.__m_callback is not None:
-            self.__m_callback.onScanResult(self.__m_seq, self.__m_path, self.__m_result)
+        self.__result.error_code = ERR_CODE.ERR_SUCC
+        self.__result.result = DetectResult.RESULT.RES_BLACK if is_black else DetectResult.RESULT.RES_WHITE
+        self.__result.time = self.__currentTimeMillis() - self.__start_time
+        self.__result.score = result_info.score
+        self.__result.virus_type = result_info.virus_type
+        self.__result.ext_info = result_info.ext
+        if self.__taskCallback is not None:
+            self.__taskCallback.onTaskEnd(self)
+        if self.__callback is not None:
+            self.__callback.onScanResult(self.__seq, self.__path, self.__result)
         
     
     def __checkTimeout(self):
-        curr_time = self.currentTimeMillis()
-        if self.__m_timeout >= 0:
-            if curr_time - self.__m_start_time > self.__m_timeout:
-                if self.__m_result.md5 is None:
-                    self.errorCallback(ERR_CODE.ERR_TIMEOUT_QUEUE, None)
+        curr_time = self.__currentTimeMillis()
+        if self.__timeout >= 0:
+            if curr_time - self.__start_time > self.__timeout:
+                if self.__result.md5 is None:
+                    self.errorCallback(ERR_CODE.ERR_TIMEOUT_QUEUE, self.__path)
                 else:
-                    self.errorCallback(ERR_CODE.ERR_TIMEOUT, None)
+                    self.errorCallback(ERR_CODE.ERR_TIMEOUT, self.__path)
                 return True
 
         return False
 
 
     def __needSleep(self, ms):
         try:
@@ -233,14 +254,15 @@
             hashKeyList = [md5]
             get_file_detect_result_request = sas_20181203_models.GetFileDetectResultRequest(hashKeyList, type=0)
             response = client.get_file_detect_result_with_options(get_file_detect_result_request, client_opt)
             org_result = response.body.result_list[0]
             score = org_result.score if org_result.score is not None else 0
             result = org_result.result if org_result.result is not None else 0
             result_info = self.ResultInfo().init_result(result, score, org_result.virus_type, org_result.ext)
+            self.__getListCompressFileResult(client, client_opt, md5, org_result)
             return result_info
 
         except Exception as error:
             if hasattr(error, "code"):
                 if error.code == "GetResultFail":
                     return self.ResultInfo().init_result(self.GET_RESULT_FAIL)
                 elif error.code == "RequestTooFrequently":
@@ -251,43 +273,122 @@
                     self.errorCallback(ERR_CODE.ERR_CALL_API, self.__getErrorMessage(api_name, error.code, error.message))
                     return self.ResultInfo().init_result(self.HAS_EXCEPTION)
             else:
                 self.errorCallback(ERR_CODE.ERR_CALL_API, self.__getErrorMessage(api_name, "ERR_NETWORK", traceback.format_exc()))
                 return self.ResultInfo().init_result(self.HAS_EXCEPTION)
 
 
+    def __getListCompressFileResult(self, client, client_opt, md5, org_result):
+        if org_result is None or org_result.result is None or org_result.compress is None:
+            return False # 结果值不合法
+        if org_result.result == self.IS_DETECTING:
+            return False # 在检测中
+        if not org_result.compress:
+            return False # 不是压缩包
+        
+        cur_page = 1
+        page_size = 50
+        self.__result.compresslist = []
+        while True:
+            ret_code = self.__getListCompressFileResultByAPI(client, client_opt, md5, cur_page, page_size)
+            if ret_code == self.REQUEST_TOO_FREQUENTLY:
+                self.__needSleep(Config.REQUEST_TOO_FREQUENTLY_SLEEP_TIME) # 请求太过频繁，需要休眠
+                continue
+            elif ret_code == self.HAS_EXCEPTION:
+                break # 报错退出
+            elif ret_code != page_size:
+                break # 查询完成，退出
+            cur_page += 1 # 加载下一页
+        return True
+
+
+    def __getListCompressFileResultByAPI(self, client, client_opt, md5, cur_page, page_size):
+        api_name = "ListCompressFileDetectResult"
+        try:
+            request = sas_20181203_models.ListCompressFileDetectResultRequest(cur_page, md5, page_size)
+            response = client.list_compress_file_detect_result_with_options(request, client_opt)
+            cnt = 0
+            for org_result in response.body.result_list:
+                cnt += 1
+                comp_res = DetectResult.CompressFileDetectResultInfo(org_result.path)
+                if org_result.score is not None:
+                    comp_res.score = org_result.score
+                if org_result.result is not None:
+                    if org_result.result == self.IS_BLACK:
+                        comp_res.result = DetectResult.RESULT.RES_BLACK
+                        vinfo = DetectResult.VirusInfo()
+                        vinfo.virus_type = org_result.virus_type
+                        vinfo.ext_info = org_result.ext
+                        comp_res.setVirusInfo(vinfo)
+                    elif org_result.result == self.IS_OK:
+                        comp_res.result = DetectResult.RESULT.RES_WHITE
+                    self.__result.compresslist.append(comp_res)
+            return cnt
+        except Exception as error:
+            if hasattr(error, "code"):
+                if error.code == "RequestTooFrequently":
+                    return self.REQUEST_TOO_FREQUENTLY
+                elif error.code == "Throttling.User":
+                    return self.REQUEST_TOO_FREQUENTLY
+                else:
+                    comp_res = DetectResult.CompressFileDetectResultInfo(self.__getErrorMessage(api_name, error.code, error.message))
+                    self.__result.compresslist.append(comp_res)
+                    return self.HAS_EXCEPTION
+            else:
+                comp_res = DetectResult.CompressFileDetectResultInfo(self.__getErrorMessage(api_name, "ERR_NETWORK", traceback.format_exc()))
+                self.__result.compresslist.append(comp_res)
+                return self.HAS_EXCEPTION
+
+
     def __uploadAndDetectByAPI(self, client, client_opt, path, md5):
         api_name = ""
         api_callerr = ERR_CODE.ERR_CALL_API
         try:
-            # 获取上传参数
-            api_name = "CreateFileDetectUploadUrl"
-            api_callerr = ERR_CODE.ERR_CALL_API
-            hash_key_context_list_0 = sas_20181203_models.CreateFileDetectUploadUrlRequestHashKeyContextList(
-                hash_key = md5,
-                file_size = self.__m_size
-            )
-            create_file_detect_upload_url_request = sas_20181203_models.CreateFileDetectUploadUrlRequest(type=0, hash_key_context_list=[hash_key_context_list_0])
-            response = client.create_file_detect_upload_url_with_options(create_file_detect_upload_url_request, client_opt)
-            upload_url_response = response.body.upload_url_list[0]
+            if self.__islocal is True:
+                # 获取上传参数
+                api_name = "CreateFileDetectUploadUrl"
+                api_callerr = ERR_CODE.ERR_CALL_API
+                hash_key_context_list_0 = sas_20181203_models.CreateFileDetectUploadUrlRequestHashKeyContextList(
+                    hash_key = md5,
+                    file_size = self.__size
+                )
+                create_file_detect_upload_url_request = sas_20181203_models.CreateFileDetectUploadUrlRequest(type=0, hash_key_context_list=[hash_key_context_list_0])
+                response = client.create_file_detect_upload_url_with_options(create_file_detect_upload_url_request, client_opt)
+                upload_url_response = response.body.upload_url_list[0]
             
-            if not upload_url_response.file_exist:
+            if self.__islocal is True and upload_url_response.file_exist is False:
                 # 上传文件
                 api_name = "UploadFile"
                 api_callerr = ERR_CODE.ERR_UPLOAD
                 upload_file_res = self.__uploadFile(path, upload_url_response.public_url, upload_url_response.context)
                     
             # 发起检测
             api_name = "CreateFileDetect"
             api_callerr = ERR_CODE.ERR_CALL_API
-            create_file_detect_request = sas_20181203_models.CreateFileDetectRequest(
-                type=0,
-                hash_key=md5,
-                oss_key=upload_url_response.context.oss_key
-            )
+            create_file_detect_request = None
+            if self.__islocal is True:
+                create_file_detect_request = sas_20181203_models.CreateFileDetectRequest(
+                    type=0,
+                    hash_key=md5,
+                    oss_key=upload_url_response.context.oss_key
+                )
+            else:
+                create_file_detect_request = sas_20181203_models.CreateFileDetectRequest(
+                    type=0,
+                    hash_key=md5,
+                    download_url=path
+                )
+            if self.__decompress is not None:
+                create_file_detect_request.from_map(
+                    {
+                        "Decompress": self.__decompress.isOpen(),
+                        "DecompressMaxLayer": self.__decompress.getMaxLayer(),
+                        "DecompressMaxFileCount": self.__decompress.getMaxFileCount()
+                    }
+                )
             client.create_file_detect_with_options(create_file_detect_request, client_opt)
 
         except Exception as error:
             if hasattr(error, "code"):
                 if error.code == "RequestTooFrequently":
                     return self.REQUEST_TOO_FREQUENTLY
                 elif error.code == "Throttling.User":
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/DetectResult.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/DetectResult.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         # {"action":"xxx", "error_code":"NetworkError", "error_message":"zzz"}
         self.error_string = None # 扩展错误信息
         
         self.result = self.RESULT.RES_UNKNOWN # 检测结果
         self.score = 0 # 分值，取值范围0-100
         self.virus_type = None # 病毒类型，如“黑客工具”
         self.ext_info = None # 扩展信息为json字符串
+        self.compresslist = None
 
 
     # 检测结果是否完成，True: 可通过getDetectResultInfo查看结果; False: 可通过getErrorInfo获取错误信息
     def isSucc(self):
         return self.error_code == ERR_CODE.ERR_SUCC
 
 
@@ -60,14 +61,15 @@
             vinfo.virus_type = self.virus_type
             vinfo.ext_info = self.ext_info
         info = self.DetectResultInfo(vinfo)
         info.md5 = self.md5
         info.time = self.time
         info.result = self.result
         info.score = self.score
+        info.compresslist = self.compresslist
         return info
 
           
     class ErrorInfo(object):
         def __init__(self):
             self.md5 = None # 样本md5
             self.time = 0 # 用时，单位为毫秒
@@ -91,13 +93,30 @@
 
 
     class DetectResultInfo(object):
         def __init__(self, vinfo=None):
             self.md5 = None # 样本md5
             self.time = 0 # 用时，单位为毫秒
             self.result = DetectResult.RESULT.RES_UNKNOWN # 检测结果
-            self.result = 2
             self.score = 0 # 分值，取值范围0-100
+            compresslist = None # 如果是压缩包，并且开启了压缩包解压参数，则此处会输出压缩包内文件检测结果
             self.__virusinfo = vinfo
-            
+        
+        # 获取病毒信息,如result为RES_BLACK，可通过此接口获取病毒信息
+        def getVirusInfo(self):
+            return self.__virusinfo
+    
+
+    class CompressFileDetectResultInfo(object):
+        def __init__(self, path=None):
+            self.path = path # 压缩文件路径
+            self.result = DetectResult.RESULT.RES_UNKNOWN # 检测结果
+            self.score = 0 # 分值，取值范围0-100
+            self.__virusinfo = None
+        
+        # 获取病毒信息,如result为RES_BLACK，可通过此接口获取病毒信息
         def getVirusInfo(self):
-            return self.__virusinfo 
+            return self.__virusinfo
+
+        def setVirusInfo(self, vinfo):
+            self.__virusinfo = vinfo
+
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/OpenAPIDetector.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/OpenAPIDetector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import os
+import re
 import sys
 import math
 import time
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from collections import deque
 from alibabacloud_sas20181203.client import Client as Sas20181203Client
@@ -12,14 +13,15 @@
 
 from .ERR_CODE import ERR_CODE
 from .Config import Config
 from .MiniThreadPool import BlockingDeque, SyncObject, RejectedExecutionHandler, MiniThreadPoolExecutor
 from .IDetectResultCallback import IDetectResultCallback
 from .DetectResult import DetectResult
 from .ScanTask import ScanTask, TaskCallback
+from .Decompress import Decompress
 
 
 class OpenAPIDetector(TaskCallback):
     _instance_lock = threading.Lock()
     
     # 获取单例检测器
     @classmethod
@@ -39,168 +41,215 @@
 
 
     def __init__(self):
         pass
 
 
     def __init(self):
-        self.m_is_inited = False
-        self.m_client = None
-        self.m_client_opt = None
-        self.m_queue = None
-
-        self.__m_threadpool = None
-        self.__m_counter = 0
-        self.__m_rej_handler = None
+        self.is_inited = False
+        self.client = None
+        self.client_opt = None
+        self.queue = None
+
+        self.__threadpool = None
+        self.__counter = 0
+        self.__rej_handler = None
+        self.__decompress = None
+        self.__alive_task_num = 0
 
         self.sync_obj = SyncObject()
 
     
     """
     检测器初始化
     @param accessKeyId
     @param accessKeySecret
     @return
     """
     def init(self, accessKeyId, accessKeySecret):
-        if self.m_is_inited:
+        if self.is_inited:
             return ERR_CODE.ERR_INIT
         
         config = open_api_models.Config(accessKeyId, accessKeySecret)
         config.endpoint = "tds.aliyuncs.com"
-        self.m_client = Sas20181203Client(config)
-        self.m_client_opt = util_models.RuntimeOptions()
-        self.m_client_opt.connectTimeout = Config.HTTP_CONNECT_TIMEOUT
-        self.m_client_opt.readTimeout = Config.HTTP_READ_TIMEOUT  
+        self.client = Sas20181203Client(config)
+        self.client_opt = util_models.RuntimeOptions()
+        self.client_opt.connectTimeout = Config.HTTP_CONNECT_TIMEOUT
+        self.client_opt.readTimeout = Config.HTTP_READ_TIMEOUT  
 
         class TaskRejectedExecutionHandler(RejectedExecutionHandler):
             def rejectedExecution(self, r, executor):
                 if isinstance(r, ScanTask):
                     r.errorCallback(ERR_CODE.ERR_ABORT, None)
-        self.__m_rej_handler = TaskRejectedExecutionHandler()
+        self.__rej_handler = TaskRejectedExecutionHandler()
         
-        self.m_queue = BlockingDeque()
-        self.__m_threadpool = MiniThreadPoolExecutor(self.m_queue, Config.THREAD_POOL_SIZE)
-        self.__m_threadpool.prestartAllThreads()
-        self.__m_threadpool.setRejectedExecutionHandler(self.__m_rej_handler)
+        self.queue = BlockingDeque()
+        self.__threadpool = MiniThreadPoolExecutor(self.queue, Config.THREAD_POOL_SIZE)
+        self.__threadpool.prestartAllThreads()
+        self.__threadpool.setRejectedExecutionHandler(self.__rej_handler)
         
-        self.__m_counter = 0
-        self.__m_alive_task_num = 0
-        self.m_is_inited = True
+        self.__counter = 0
+        self.__alive_task_num = 0
+        self.is_inited = True
         return ERR_CODE.ERR_SUCC
     
 
     # 检测器反初始化
     def uninit(self):
-        if self.m_is_inited is False:
+        if self.is_inited is False:
             return
         
-        self.m_is_inited = False
-        self.__m_threadpool.shutdown()
+        self.is_inited = False
+        self.__threadpool.shutdown()
 
         with self.sync_obj:
-            self.__m_threadpool = None
-            self.__m_rej_handler = None
-            self.m_queue = None
-            self.m_client = None
-            self.m_client_opt = None
-            self.__m_counter = None
+            self.__threadpool = None
+            self.__rej_handler = None
+            self.queue = None
+            self.client = None
+            self.client_opt = None
+    
+    """
+    初始化解压缩配置参数
+    @param open 是否识别压缩文件并解压
+    @param maxlayer 最大解压层数，open参数为true时生效
+    @param maxfilecount 最大解压文件数，open参数为true时生效
+    """
+    def initDecompress(self, open, maxlayer, maxfilecount):
+        if self.is_inited is False:
+            return ERR_CODE.ERR_INIT
+        self.__decompress = Decompress(open, maxlayer, maxfilecount)
+        return ERR_CODE.ERR_SUCC
 
 
     """
     同步文件检测
     @param file_path 待检测文件路径
     @param timeout 超时时长，单位毫秒， < 0 无限等待
-    @param res 检测结果
-    @throws Exception
-    """    
+    """
     def detectSync(self, file_path, timeout):
+        return self.__internalDetectSync(file_path, None, timeout)
+    
+
+    """
+    同步URL文件检测
+    @param url 待检测文件下载链接URL
+    @param md5 文件md5
+	@param timeout 超时时长，单位毫秒， < 0 无限等待
+	@return res 检测结果
+    """
+    def detectUrlSync(self, url, md5, timeout):
+        return self.__internalDetectSync(url, md5, timeout)
+
+
+    def __internalDetectSync(self, file_path, md5, timeout):
         res = []
         res.append(DetectResult())
         detect_sync_obj = SyncObject()
         class SyncTaskCallback(IDetectResultCallback):
             def onScanResult(self, seq, file_path, callback_res):
                 res[0] = callback_res
                 with detect_sync_obj:
                     detect_sync_obj.notify()
-
-        seq = self.detect(file_path, timeout, SyncTaskCallback())
+        
+        seq = 0
+        if md5 is None:
+            # 本地文件检测
+            seq = self.detect(file_path, timeout, SyncTaskCallback())
+        else:
+            # URL文件检测
+            seq = self.detectUrl(file_path, md5, timeout, SyncTaskCallback())
         if seq > 0:
             try:
                 with detect_sync_obj:
                     detect_sync_obj.wait()
             except Exception as e:
                 pass
         return res[0]
     
 
-    def check_counter(self):
-        if self.__m_counter < 0:
-            self.__m_counter = 1
-        if self.__m_counter > math.pow(2, 31):
-            self.__m_counter = 1
-        return
-
-
     """
     异步文件检测
     @param file_path 待检测文件路径
     @param timeout 超时时长，单位毫秒， < 0 无限等待
-    @param res 检测结果
+    @param callback 检测结果
     @return >0 发起检测成功，检测请求序列号 < 0 错误码，参见ERR_CODE
     """
     def detect(self, file_path, timeout, callback):
-        if not os.path.isfile(file_path):
-            file_size = -1
-        else:
-            file_size = os.path.getsize(file_path)
-        task = ScanTask(file_path, file_size, timeout, callback)
-        if not os.path.isfile(file_path):
-            task.errorCallback(ERR_CODE.ERR_FILE_NOT_FOUND, None)
+        file_size = self.__get_filesize(file_path)
+        task = ScanTask()
+        task.initScanFile(file_path, file_size, timeout, callback, self.__decompress)
+        if file_size < 0:
+            task.errorCallback(ERR_CODE.ERR_FILE_NOT_FOUND, file_path)
             return ERR_CODE.ERR_FILE_NOT_FOUND.value
-        
+        return self.__internalDetect(task)
+
+    
+    """
+    异步URL文件检测
+    @param url 待检测文件下载链接URL
+	@param md5 文件md5
+	@param timeout 超时时长，单位毫秒， < 0 无限等待
+	@param callback 检测结果
+	@return >0 发起检测成功，检测请求序列号 < 0 错误码，参见ERR_CODE
+    """
+    def detectUrl(self, url, md5, timeout, callback):
+        if md5 is not None:
+            # 转小写
+            md5 = md5.lower()
+        task = ScanTask()
+        task.initScanUrl(url, md5, timeout, callback, self.__decompress)
+        if md5 is None or len(md5) != 32 or re.match(r'^[a-f0-9]{32}$', md5) is None:
+            task.errorCallback(ERR_CODE.ERR_MD5, md5)
+            return ERR_CODE.ERR_MD5.value
+        if url is None:
+            task.errorCallback(ERR_CODE.ERR_URL, url)
+            return ERR_CODE.ERR_URL.value
+        # 检查url的合法性
+        if self.__is_valid_url(url) is False:
+            task.errorCallback(ERR_CODE.ERR_URL, "Malformed URL: {}".format(url))
+            return ERR_CODE.ERR_URL.value
+        return self.__internalDetect(task)
+    
+
+    def __internalDetect(self, task):
         seq = 0
         try:
-            if self.m_is_inited:
+            if self.is_inited:
                 with self.sync_obj:
-                    if self.m_is_inited:
-                        self.__m_counter += 1
-                        self.check_counter()
-                        task.setSeq(self.__m_counter)
+                    if self.is_inited:
+                        self.__counter += 1
+                        self.__check_counter()
+                        task.setSeq(self.__counter)
                         if self.getQueueSize() >= Config.QUEUE_SIZE_MAX:
                             raise RuntimeError("Deque full")
                         task.setTaskCallback(self)
-                        self.m_queue.addLast(task)
-                        with self.m_queue:
-                            self.m_queue.notify()
+                        self.queue.addLast(task)
+                        with self.queue:
+                            self.queue.notify()
                         seq = task.getSeq()
-        
         except RuntimeError as e:
             task.errorCallback(ERR_CODE.ERR_DETECT_QUEUE_FULL, None)
             return ERR_CODE.ERR_DETECT_QUEUE_FULL.value
         
         if seq <= 0:
             task.errorCallback(ERR_CODE.ERR_INIT, None)
             return ERR_CODE.ERR_INIT.value
-        
         return seq
 
 
-    def currentTimeMillis(self):
-        return int(round(time.time() * 1000))
-
     """
     @brief 获取检测队列长度
     @return 检测队列长度
     """
     def getQueueSize(self):
-        if self.m_is_inited:
+        if self.is_inited:
             with self.sync_obj:
-                if self.m_is_inited:
-                    return self.__m_alive_task_num
+                if self.is_inited:
+                    return self.__alive_task_num
         return 0
 
     
     """
     @brief 等待队列空间可用（可进行新样本插入）
     @param timeout 超时时长，单位毫秒， < 0 无限等待
     @return ERR_SUCC 成功，队列已有可用空间 ERR_TIMEOUT 失败，队列仍然满
@@ -215,17 +264,17 @@
             
             if timeout >= 0 and all_time >= timeout:
                 break
             
             sleep_unit = 200
             if timeout >= 0 and timeout > all_time and (timeout-all_time<sleep_unit):
                 sleep_unit = timeout - all_time
-            start_time = self.currentTimeMillis()
+            start_time = self.__current_time_millis()
             time.sleep(sleep_unit/1000.0)
-            all_time += self.currentTimeMillis() - start_time
+            all_time += self.__current_time_millis() - start_time
         
         return code
     
 
     """
     @brief 等待队列为空
     @param timeout 超时时长，单位毫秒， < 0 无限等待
@@ -241,25 +290,56 @@
 
             if timeout >=0 and all_time >= timeout:
                 break
 
             sleep_unit = 200
             if timeout >= 0 and timeout > all_time and (timeout-all_time<sleep_unit):
                 sleep_unit = timeout - all_time
-            start_time = self.currentTimeMillis()
+            start_time = self.__current_time_millis()
             time.sleep(sleep_unit/1000.0)
-            all_time += self.currentTimeMillis() - start_time
+            all_time += self.__current_time_millis() - start_time
         return code
-
     
+
     def onTaskEnd(self, task):
-        if self.m_is_inited:
+        if self.is_inited:
             with self.sync_obj:
-                if self.m_is_inited:
-                    self.__m_alive_task_num -= 1
+                if self.is_inited:
+                    self.__alive_task_num -= 1
     
 
     def onTaskBegin(self, task):
-        if self.m_is_inited:
+        if self.is_inited:
             with self.sync_obj:
-                if self.m_is_inited:
-                    self.__m_alive_task_num += 1
+                if self.is_inited:
+                    self.__alive_task_num += 1
+
+
+    def __current_time_millis(self):
+        return int(round(time.time() * 1000))
+
+
+    def __get_filesize(self, path):
+        if not os.path.isfile(path):
+            return -1
+        else:
+            return os.path.getsize(path)
+
+    
+    def __is_valid_url(self, url):
+        try:
+            if sys.version_info[0] == 3:
+                from urllib.parse import urlparse
+            else:
+                from urlparse import urlparse
+            parsed = urlparse(url)
+            return (bool(parsed.scheme) and bool(parsed.netloc))
+        except Exception as e:
+            return False
+
+    
+    def __check_counter(self):
+        if self.__counter < 0:
+            self.__counter = 1
+        if self.__counter > math.pow(2, 31):
+            self.__counter = 1
+        return
```

### Comparing `alibabacloud_filedetect-1.0.1/alibabacloud_filedetect/Config.py` & `alibabacloud_filedetect-1.1.0/alibabacloud_filedetect/Config.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_filedetect-1.0.1/README-CN.md` & `alibabacloud_filedetect-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_filedetect-1.0.1/setup.py` & `alibabacloud_filedetect-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 NAME = "alibabacloud_filedetect"
 DESCRIPTION = "Alibaba Cloud File Detection SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-file-detect-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_sas20181203>=1.1.30",
+    "alibabacloud_sas20181203>=2.28.0",
     "alibabacloud_tea_util>=0.3.5, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
     "requests"
 
 ]
 
 LONG_DESCRIPTION = ''
```

### Comparing `alibabacloud_filedetect-1.0.1/README.md` & `alibabacloud_filedetect-1.1.0/README.md`

 * *Files identical despite different names*

