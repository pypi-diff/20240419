# Comparing `tmp/qstd_logger_json_formatter-0.1.0.tar.gz` & `tmp/qstd_logger_json_formatter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_logger_json_formatter-0.1.0.tar", last modified: Sun Apr  7 17:36:51 2024, max compression
+gzip compressed data, was "qstd_logger_json_formatter-0.1.1.tar", last modified: Fri Apr 19 15:13:28 2024, max compression
```

## Comparing `qstd_logger_json_formatter-0.1.0.tar` & `qstd_logger_json_formatter-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:36:51.498674 qstd_logger_json_formatter-0.1.0/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_logger_json_formatter-0.1.0/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-07 17:36:51.498674 qstd_logger_json_formatter-0.1.0/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      744 2024-03-31 10:24:13.000000 qstd_logger_json_formatter-0.1.0/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:36:51.498674 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3191 2024-03-31 10:22:25.000000 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-07 17:36:51.498674 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-07 17:36:51.000000 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      275 2024-04-07 17:36:51.000000 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-07 17:36:51.000000 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       27 2024-04-07 17:36:51.000000 qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-07 17:36:51.498674 qstd_logger_json_formatter-0.1.0/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      624 2024-03-31 10:28:15.000000 qstd_logger_json_formatter-0.1.0/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_logger_json_formatter-0.1.1/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      744 2024-03-31 10:24:13.000000 qstd_logger_json_formatter-0.1.1/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     3226 2024-04-19 15:00:03.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1106 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      275 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       27 2024-04-19 15:13:28.000000 qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-04-19 15:13:28.417043 qstd_logger_json_formatter-0.1.1/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      624 2024-04-19 15:11:57.000000 qstd_logger_json_formatter-0.1.1/setup.py
```

### Comparing `qstd_logger_json_formatter-0.1.0/LICENSE` & `qstd_logger_json_formatter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_logger_json_formatter-0.1.0/PKG-INFO` & `qstd_logger_json_formatter-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd_logger_json_formatter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Logging json formatter
 Home-page: https://github.com/QuisEgoSum/qstd-logger-json-formatter
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: logging json formatter
 Requires-Python: >=3.7
```

### Comparing `qstd_logger_json_formatter-0.1.0/README.md` & `qstd_logger_json_formatter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter/__init__.py` & `qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def format(self, record: LogRecord) -> str:
         root_name = record.name.split('.')[0]
         if root_name in self.PARSE_PAYLOAD_ROOT_LOGGER:
             record.message = record.msg
             if not record.args:
                 record.payload = None
-            elif len(record.args) == 1:
+            elif isinstance(record.args, tuple) and len(record.args) == 1:
                 record.payload = record.args[0]
             else:
                 record.payload = record.args
         else:
             record.message = record.getMessage()
             record.payload = None
         record.asctime = self.formatTime(record, self.datefmt)
```

### Comparing `qstd_logger_json_formatter-0.1.0/qstd_logger_json_formatter.egg-info/PKG-INFO` & `qstd_logger_json_formatter-0.1.1/qstd_logger_json_formatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qstd-logger-json-formatter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Logging json formatter
 Home-page: https://github.com/QuisEgoSum/qstd-logger-json-formatter
 Author: QuisEgoSum
 Author-email: subbotin.evdokim@gmail.com
 License: MIT
 Keywords: logging json formatter
 Requires-Python: >=3.7
```

### Comparing `qstd_logger_json_formatter-0.1.0/setup.py` & `qstd_logger_json_formatter-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_logger_json_formatter',
-    version='0.1.0',
+    version='0.1.1',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Logging json formatter',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-logger-json-formatter',
     packages=find_packages(exclude=['tmp', 'example']),
```

