# Comparing `tmp/common-tools-ai-bnq-0.0.3.tar.gz` & `tmp/common-tools-ai-bnq-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-tools-ai-bnq-0.0.3.tar", last modified: Fri Apr 19 08:07:42 2024, max compression
+gzip compressed data, was "common-tools-ai-bnq-0.0.4.tar", last modified: Fri Apr 19 09:15:34 2024, max compression
```

## Comparing `common-tools-ai-bnq-0.0.3.tar` & `common-tools-ai-bnq-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:07:42.861977 common-tools-ai-bnq-0.0.3/
--rw-rw-rw-   0        0        0      258 2024-04-19 08:07:42.860977 common-tools-ai-bnq-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-03-27 09:01:03.000000 common-tools-ai-bnq-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:07:42.799093 common-tools-ai-bnq-0.0.3/bnq_py_core/
--rw-rw-rw-   0        0        0      122 2024-03-27 09:34:31.000000 common-tools-ai-bnq-0.0.3/bnq_py_core/__init__.py
--rw-rw-rw-   0        0        0     4165 2024-03-27 09:40:51.000000 common-tools-ai-bnq-0.0.3/bnq_py_core/logger_record.py
--rw-rw-rw-   0        0        0     2688 2024-04-19 08:07:26.000000 common-tools-ai-bnq-0.0.3/bnq_py_core/nacos_connect.py
--rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.3/bnq_py_core/read_conf_from_ini.py
--rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.3/bnq_py_core/singleton.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:07:42.821160 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/
--rw-rw-rw-   0        0        0      258 2024-04-19 08:07:42.000000 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2024-04-19 08:07:42.000000 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:07:42.000000 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-19 08:07:42.000000 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-19 08:07:42.000000 common-tools-ai-bnq-0.0.3/common_tools_ai_bnq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:07:42.861977 common-tools-ai-bnq-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      563 2024-04-19 07:55:16.000000 common-tools-ai-bnq-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:07:42.858977 common-tools-ai-bnq-0.0.3/test/
--rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.3/test/__init__.py
--rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.3/test/test_batch_triton.py
--rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.3/test/test_decorator.py
--rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.3/test/test_pymysql.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:15:34.645530 common-tools-ai-bnq-0.0.4/
+-rw-rw-rw-   0        0        0      258 2024-04-19 09:15:34.644598 common-tools-ai-bnq-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-03-27 09:01:03.000000 common-tools-ai-bnq-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 09:15:34.629523 common-tools-ai-bnq-0.0.4/bnq_py_core/
+-rw-rw-rw-   0        0        0      122 2024-03-27 09:34:31.000000 common-tools-ai-bnq-0.0.4/bnq_py_core/__init__.py
+-rw-rw-rw-   0        0        0     4574 2024-04-19 09:14:08.000000 common-tools-ai-bnq-0.0.4/bnq_py_core/logger_record.py
+-rw-rw-rw-   0        0        0     2816 2024-04-19 08:54:44.000000 common-tools-ai-bnq-0.0.4/bnq_py_core/nacos_connect.py
+-rw-rw-rw-   0        0        0     2074 2024-04-19 07:39:44.000000 common-tools-ai-bnq-0.0.4/bnq_py_core/read_conf_from_ini.py
+-rw-rw-rw-   0        0        0      716 2024-03-27 09:35:48.000000 common-tools-ai-bnq-0.0.4/bnq_py_core/singleton.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:15:34.641609 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/
+-rw-rw-rw-   0        0        0      258 2024-04-19 09:15:34.000000 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2024-04-19 09:15:34.000000 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 09:15:34.000000 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-19 09:15:34.000000 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-19 09:15:34.000000 common-tools-ai-bnq-0.0.4/common_tools_ai_bnq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 09:15:34.645530 common-tools-ai-bnq-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      563 2024-04-19 09:15:30.000000 common-tools-ai-bnq-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 09:15:34.643597 common-tools-ai-bnq-0.0.4/test/
+-rw-rw-rw-   0        0        0      122 2024-04-10 03:16:38.000000 common-tools-ai-bnq-0.0.4/test/__init__.py
+-rw-rw-rw-   0        0        0    27286 2024-04-10 03:37:31.000000 common-tools-ai-bnq-0.0.4/test/test_batch_triton.py
+-rw-rw-rw-   0        0        0     3464 2024-04-10 07:43:55.000000 common-tools-ai-bnq-0.0.4/test/test_decorator.py
+-rw-rw-rw-   0        0        0      897 2024-04-16 08:13:06.000000 common-tools-ai-bnq-0.0.4/test/test_pymysql.py
```

### Comparing `common-tools-ai-bnq-0.0.3/bnq_py_core/logger_record.py` & `common-tools-ai-bnq-0.0.4/bnq_py_core/logger_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     """
     __instance = None  # 单例
     __filename = None  # 日志文件名
 
     def __new__(cls, log_dir=None, *args, **kwargs):
         """保证日志模块是单例模式"""
         if not cls.__instance:
-            cls.__instance = super(LoggingRecord, cls).__new__(cls, *args, **kwargs)
+            cls.__instance = super(LoggingRecord, cls).__new__(cls)
         __now_time = int(round(time.time()))
         __time_record = time.strftime("%Y%m%d", time.localtime(__now_time))
         if log_dir:
             cls.__filename = __time_record + "_" + log_dir + ".log"
         else:
-            cls.__filename = __time_record + "_BNQ_DESIGN.log"
+            cls.__filename = __time_record + "_BNQ_AI.log"
         return cls.__instance
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, max_bytes=20 * 1024 * 1024, backup_count=10, log_level=logging.INFO, log_dir=None):
         self.record_info = None
         self.logger = None
-        self.log_record_path = None  # 日志记录路径
+        self.log_record_path = log_dir  # 日志记录路径
+        self.max_bytes = max_bytes  # 日志文件大小
+        self.backup_count = backup_count  # 日志文件备份数量
+        self.level = log_level  # 日志级别
         self.init_log()
 
     def init_log(self):
         """初始化log模块
 
         Returns:
 
@@ -57,27 +59,27 @@
             "formatters": {
                 "default": {
                     "format": '%(asctime)s - %(levelname)s - %(name)s - %(message)s'
                 }
             },
             "handlers": {
                 "file_handler": {
-                    "level": "DEBUG",
+                    "level": self.level,
                     "formatter": "default",
                     "class": "concurrent_log_handler.ConcurrentRotatingFileHandler",
                     "filename": log_filename,
-                    "maxBytes": 20 * 1024 * 1024,
-                    "backupCount": 10,
+                    "maxBytes": self.max_bytes,
+                    "backupCount": self.backup_count,
                     "encoding": "UTF-8"
                 },
             },
             "loggers": {
                 "": {
                     "handlers": ["file_handler"],
-                    "level": logging.INFO
+                    "level": self.level
                 }
             }
         })
         configure(
             context_class=dict,
             logger_factory=stdlib.LoggerFactory(),
             wrapper_class=stdlib.BoundLogger,
@@ -85,16 +87,24 @@
                 stdlib.filter_by_level,
                 stdlib.PositionalArgumentsFormatter(),
                 processors.StackInfoRenderer(),
                 processors.format_exc_info,
                 processors.UnicodeDecoder(),
                 stdlib.render_to_log_kwargs]
         )
-        self.logger = logging.getLogger("BNQ-AI-SPACE-DESIGN")
-        self.logger.level = logging.INFO
+        self.logger = logging.getLogger("BNQ-AI")
+        self.logger.level = self.level
+
+    def debug(self, record_info):
+        """debug级别的日志记录
+
+        :param record_info:
+        :return:
+        """
+        self.logger.debug(record_info)
 
     def info(self, record_info):
         """
 
         Args:
             record_info:
 
@@ -127,16 +137,17 @@
         self.logger.warning(warning_info)
 
     def exception(self, exception_info):
         self.logger.exception(exception_info)
 
 
 if __name__ == "__main__":
-    testLog = LoggingRecord()
+    testLog = LoggingRecord(log_level=logging.DEBUG)
     for i in range(10):
         print(i, 'i')
         print(testLog, "testLog")
+        testLog.debug(i)
         testLog.info("中文测试")
         testLog.error(i)
         testLog.warning(i)
         testLog.exception(i)
-        time.sleep(3)
+        # time.sleep(3)
```

### Comparing `common-tools-ai-bnq-0.0.3/bnq_py_core/read_conf_from_ini.py` & `common-tools-ai-bnq-0.0.4/bnq_py_core/read_conf_from_ini.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.3/bnq_py_core/singleton.py` & `common-tools-ai-bnq-0.0.4/bnq_py_core/singleton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.3/setup.py` & `common-tools-ai-bnq-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Author:Zhang HongTao
 # @File:setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='common-tools-ai-bnq',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         # 依赖项列表
         'structlog==23.1.0',
         'concurrent-log-handler==0.9.22',
         'nacos-sdk-python==0.1.12'
     ],
```

### Comparing `common-tools-ai-bnq-0.0.3/test/test_batch_triton.py` & `common-tools-ai-bnq-0.0.4/test/test_batch_triton.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.3/test/test_decorator.py` & `common-tools-ai-bnq-0.0.4/test/test_decorator.py`

 * *Files identical despite different names*

### Comparing `common-tools-ai-bnq-0.0.3/test/test_pymysql.py` & `common-tools-ai-bnq-0.0.4/test/test_pymysql.py`

 * *Files identical despite different names*

