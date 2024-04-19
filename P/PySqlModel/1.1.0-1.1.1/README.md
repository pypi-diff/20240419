# Comparing `tmp/PySqlModel-1.1.0.tar.gz` & `tmp/PySqlModel-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySqlModel-1.1.0.tar", last modified: Fri Apr 19 14:02:54 2024, max compression
+gzip compressed data, was "dist\PySqlModel-1.1.1.tar", last modified: Fri Apr 19 15:12:40 2024, max compression
```

## Comparing `PySqlModel-1.1.0.tar` & `PySqlModel-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/
--rw-rw-rw-   0        0        0    35823 2024-02-26 15:41:22.000000 PySqlModel-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      388 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel/
--rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.0/PySqlModel/__init__.py
--rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.0/PySqlModel/base.py
--rw-rw-rw-   0        0        0    11570 2024-04-19 14:00:57.000000 PySqlModel-1.1.0/PySqlModel/mysql.py
--rw-rw-rw-   0        0        0    10957 2024-04-19 13:56:54.000000 PySqlModel-1.1.0/PySqlModel/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/
--rw-rw-rw-   0        0        0      388 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2024-02-26 16:37:57.000000 PySqlModel-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-19 13:16:57.000000 PySqlModel-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/
+-rw-rw-rw-   0        0        0     1524 2024-04-19 14:25:02.000000 PySqlModel-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      388 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel/
+-rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.1/PySqlModel/__init__.py
+-rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.1/PySqlModel/base.py
+-rw-rw-rw-   0        0        0    11502 2024-04-19 15:12:06.000000 PySqlModel-1.1.1/PySqlModel/mysql.py
+-rw-rw-rw-   0        0        0    10877 2024-04-19 15:12:06.000000 PySqlModel-1.1.1/PySqlModel/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/
+-rw-rw-rw-   0        0        0      388 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6974 2024-04-19 14:15:02.000000 PySqlModel-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-19 15:12:31.000000 PySqlModel-1.1.1/setup.py
```

### Comparing `PySqlModel-1.1.0/PySqlModel/mysql.py` & `PySqlModel-1.1.1/PySqlModel/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,14 @@
             self.cursor.execute(self.sql, self.args)
             rows = self.cursor.fetchall()
             result_field = self.__extract_field_list()
             return [dict(zip(result_field, row)) for row in rows]
         except Exception as err:
             raise err
         finally:
-            self.field_list = []
             self.where_sql = []
             self.limit_sql = ""
             self.order_sql = ""
             self.args = []
 
     def find(self) -> Union[dict, None]:
         """
@@ -234,15 +233,14 @@
                 result_field = self.__extract_field_list()
                 kwargs = dict(zip(result_field, row))
                 return kwargs
             return None
         except Exception as err:
             raise err
         finally:
-            self.field_list = []
             self.where_sql = []
             self.limit_sql = ""
             self.order_sql = ""
             self.args = []
 
     def count(self) -> int:
         """
```

### Comparing `PySqlModel-1.1.0/PySqlModel/sqlite.py` & `PySqlModel-1.1.1/PySqlModel/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List, Tuple, Union
 
 
 # sqlite操作
 class SQLite():
     # 系统数据库
     __SYSTEM_TABLES = ["sqlite_master", "sqlite_sequence"]
-    
+
     def __init__(self, connect=None, **kwargs):
         """
         DATABASES = {
             "database": "./demo.db"
         }
         """
         if connect is not None and hasattr(connect, "cursor"):
@@ -61,15 +61,15 @@
             self.table_name = table_name.strip(" `'\"")  # 将表名赋值给实例属性
 
             self.field_list = field_dict.keys()  # 获取该表的所有的字段名
 
             table_list = self.show_table()  # 获取数据库里所有的表
             if self.table_name in table_list:  # 判断该表是否已存在
                 return True  # 该表已存在！直接返回
-    
+
             field_list = ["`{key}` {value}".format(key=str(key).strip(" `'\""), value=value) for key, value in field_dict.items()]
             create_field = ",".join(field_list)  # 将所有的字段与字段类型以 “ , ” 拼接
             self.sql = f"""CREATE TABLE `{self.table_name}`(
   {create_field}
 );"""
         try:
             self.cursor.execute(self.sql)
@@ -181,15 +181,14 @@
             self.cursor.execute(self.sql, self.args)
             rows = self.cursor.fetchall()
             result_field = self.__extract_field_list()
             return [dict(zip(result_field, row)) for row in rows]
         except Exception as err:
             raise err
         finally:
-            self.field_list = []
             self.where_sql = []
             self.limit_sql = ""
             self.order_sql = ""
             self.args = []
 
     def find(self) -> Union[dict, None]:
         """
@@ -215,15 +214,14 @@
                 result_field = self.__extract_field_list()
                 kwargs = dict(zip(result_field, row))
                 return kwargs
             return None
         except Exception as err:
             raise err
         finally:
-            self.field_list = []
             self.where_sql = []
             self.limit_sql = ""
             self.order_sql = ""
             self.args = []
 
     def count(self) -> int:
         """
@@ -237,15 +235,15 @@
             self.cursor.execute(self.sql, self.args)
             row = self.cursor.fetchone()
             if row:
                 return row[0]
         except Exception as err:
             print(err)
         return 0
-    
+
     def delete(self) -> int:
         """
         删除满足条件的数据
         :return: 影响行数
         """
         try:
             self.sql = f"DELETE FROM `{self.table_name}`"
```

### Comparing `PySqlModel-1.1.0/setup.py` & `PySqlModel-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @Author:函封封
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="PySqlModel",
-    version="1.1.0",
+    version="1.1.1",
     author="HanFengFeng",
     author_email="mr_jia_han@qq.com",
     description="简单方便的数据库查询包",
     # 项目主页
     url="https://github.com/NeverStopDreamingWang/pysqlmodel",
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
```

