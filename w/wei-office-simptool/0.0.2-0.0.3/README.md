# Comparing `tmp/wei_office_simptool-0.0.2.tar.gz` & `tmp/wei_office_simptool-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.2.tar", last modified: Fri Apr 19 01:17:59 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.3.tar", last modified: Fri Apr 19 08:34:04 2024, max compression
```

## Comparing `wei_office_simptool-0.0.2.tar` & `wei_office_simptool-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 01:17:59.953099 wei_office_simptool-0.0.2/
--rw-rw-rw-   0        0        0     3439 2024-04-19 01:17:59.951100 wei_office_simptool-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2746 2024-04-18 08:47:44.000000 wei_office_simptool-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 01:17:59.953099 wei_office_simptool-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2579 2024-04-19 01:13:23.000000 wei_office_simptool-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 01:17:59.927444 wei_office_simptool-0.0.2/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.2/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 01:17:59.931444 wei_office_simptool-0.0.2/wei_office_simptool/
--rw-rw-rw-   0        0        0     1667 2024-04-18 08:41:00.000000 wei_office_simptool-0.0.2/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    12869 2024-04-19 01:13:23.000000 wei_office_simptool-0.0.2/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 01:17:59.945100 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     3439 2024-04-19 01:17:59.000000 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-19 01:17:59.000000 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 01:17:59.000000 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-19 01:17:59.000000 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-19 01:17:59.000000 wei_office_simptool-0.0.2/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.402133 wei_office_simptool-0.0.3/
+-rw-rw-rw-   0        0        0     4854 2024-04-19 08:34:04.400127 wei_office_simptool-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4092 2024-04-19 08:30:50.000000 wei_office_simptool-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 08:34:04.402133 wei_office_simptool-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2648 2024-04-19 08:32:20.000000 wei_office_simptool-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.380078 wei_office_simptool-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.383078 wei_office_simptool-0.0.3/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1667 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.3/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    14275 2024-04-19 08:31:03.000000 wei_office_simptool-0.0.3/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:34:04.396078 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     4854 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-19 08:34:04.000000 wei_office_simptool-0.0.3/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.2/setup.py` & `wei_office_simptool-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.2',
+    version='0.0.3',
     author="Ethan Wilkins",  # 作者
     author_email="thisluckyboy@126.com",  # 作者联系方式，可写自己的邮箱地址
-    description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能。",  # 包的简述
+    description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
-    url="https://github.com/phoenixlucky/test",  # 自己项目地址，比如github的项目地址
+    url="https://github.com/phoenixlucky/wei_office_simptool",  # 自己项目地址，比如github的项目地址
     packages=find_packages(),
     install_requires=[
         'pathlib',
         'pandas',
         'pymysql',
         'datetime',
         'openpyxl',
```

### Comparing `wei_office_simptool-0.0.2/tests/__init__.py` & `wei_office_simptool-0.0.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.2/tests/test_utils.py` & `wei_office_simptool-0.0.3/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 @date:2023/12/3
 @time:17:41
 @month:十二月
 @email:thisluckyboy@126.com
 """
 # test_database.py
 import unittest
+
 from wei_office_simptool.utils import Database
 
+
 class TestDatabase(unittest.TestCase):
     def test_connection(self):
         # 在这里编写你的测试代码
         db = Database(host='localhost', port=3306, user='user', password='password', db='test_db')
         db.connect()
         self.assertTrue(db.connection_state == 1)
         db.close()
```

### Comparing `wei_office_simptool-0.0.2/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.3/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.2/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.3/wei_office_simptool/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,31 +23,30 @@
 @ide:PyCharm
 @date:2023/12/3
 @time:17:33
 @month:十二月
 @email:thisluckyboy@126.com
 """
 import base64
-import pathlib
-import pandas as pd
-import pymysql
 import datetime
+import pathlib
 import smtplib
-from email.mime.text import MIMEText
-from email.mime.multipart import MIMEMultipart
-from email.header import Header
 import time
-from functools import wraps
 from contextlib import contextmanager
-import re
+from email.header import Header
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from functools import wraps
+
+import mysql.connector
 import openpyxl
+import pandas as pd
+import pymysql
 from openpyxl import load_workbook
 
-import toml
-
 
 def fn_timer(func):
     @wraps(func)
     def function_timer(*args, **kwargs):
         t0 = time.perf_counter()
         result = func(*args, **kwargs)
         t1 = time.perf_counter()
@@ -163,14 +162,60 @@
             elif operation_mode == "c":
                 self.callsql(sql)
             elif operation_mode == "wm":
                 self.writesqlmany(sql, purchases)
         else:
             return self.to_df(sql)
 
+class MySQLDatabase:
+    def __init__(self, config):
+        self.config = config
+        self.connection = None
+        self.connect()
+
+    def connect(self):
+        try:
+            self.connection = mysql.connector.connect(**self.config)
+            print("Connected to MySQL database")
+        except mysql.connector.Error as err:
+            print(f"Error: {err}")
+
+    def close(self):
+        if self.connection:
+            self.connection.close()
+            print("MySQL connection closed")
+
+    def execute_query(self, query, params=None):
+        cursor = self.connection.cursor()
+        try:
+            if params:
+                cursor.execute(query, params)
+            else:
+                cursor.execute(query)
+            self.connection.commit()
+            print("Query executed successfully")
+        except mysql.connector.Error as err:
+            print(f"Error: {err}")
+        finally:
+            cursor.close()
+
+    def fetch_query(self, query, params=None):
+        cursor = self.connection.cursor()
+        try:
+            if params:
+                cursor.execute(query, params)
+            else:
+                cursor.execute(query)
+            result = cursor.fetchall()
+            return result
+        except mysql.connector.Error as err:
+            print(f"Error: {err}")
+        finally:
+            cursor.close()
+
 class ExcelHandler:
     def __init__(self, file_name):
         self.file_name = file_name
         self.wb = load_workbook(self.file_name)
 
     def excel_write(self, sheet_name, results, start_row, start_col, end_row, end_col):
         try:
```

