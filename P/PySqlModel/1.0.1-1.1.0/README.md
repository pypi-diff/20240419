# Comparing `tmp/PySqlModel-1.0.1.tar.gz` & `tmp/PySqlModel-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySqlModel-1.0.1.tar", last modified: Mon Feb 26 17:06:48 2024, max compression
+gzip compressed data, was "dist\PySqlModel-1.1.0.tar", last modified: Fri Apr 19 14:02:54 2024, max compression
```

## Comparing `PySqlModel-1.0.1.tar` & `PySqlModel-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-02-26 15:41:22.000000 PySqlModel-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      242 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel/
--rw-rw-rw-   0        0        0       95 2023-05-09 17:36:37.000000 PySqlModel-1.0.1/PySqlModel/__init__.py
--rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.0.1/PySqlModel/base.py
--rw-rw-rw-   0        0        0    14810 2024-02-26 15:45:55.000000 PySqlModel-1.0.1/PySqlModel/mysql.py
--rw-rw-rw-   0        0        0    11418 2024-02-26 15:45:55.000000 PySqlModel-1.0.1/PySqlModel/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/
--rw-rw-rw-   0        0        0      242 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/PySqlModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2024-02-26 16:37:57.000000 PySqlModel-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-02-26 17:06:48.000000 PySqlModel-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-02-26 16:56:17.000000 PySqlModel-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-02-26 15:41:22.000000 PySqlModel-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      388 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel/
+-rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.0/PySqlModel/__init__.py
+-rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.0/PySqlModel/base.py
+-rw-rw-rw-   0        0        0    11570 2024-04-19 14:00:57.000000 PySqlModel-1.1.0/PySqlModel/mysql.py
+-rw-rw-rw-   0        0        0    10957 2024-04-19 13:56:54.000000 PySqlModel-1.1.0/PySqlModel/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/
+-rw-rw-rw-   0        0        0      388 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/PySqlModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2024-02-26 16:37:57.000000 PySqlModel-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 14:02:54.000000 PySqlModel-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-19 13:16:57.000000 PySqlModel-1.1.0/setup.py
```

### Comparing `PySqlModel-1.0.1/LICENSE` & `PySqlModel-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.0.1/PySqlModel/sqlite.py` & `PySqlModel-1.1.0/PySqlModel/sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,334 +1,323 @@
 """
 @Project:PgSqlModel
 @File:sqlite.py
 @Author:函封封
 """
-import time
-import sqlite3
+import math
+from typing import List, Tuple, Union
 
 
 # sqlite操作
 class SQLite():
-    def __init__(self, **kwargs):
+    # 系统数据库
+    __SYSTEM_TABLES = ["sqlite_master", "sqlite_sequence"]
+    
+    def __init__(self, connect=None, **kwargs):
         """
         DATABASES = {
             "database": "./demo.db"
         }
         """
-        self.sqlite_con = sqlite3.connect(**kwargs)
-        self.sqlite = self.sqlite_con.cursor()  # 创建游标对象
+        if connect is not None and hasattr(connect, "cursor"):
+            self.connect = connect
+        else:
+            import sqlite3
+            self.connect = sqlite3.connect(**kwargs)
+        self.cursor = self.connect.cursor()  # 创建游标对象
         self.table_name = None  # 表名
         self.field_list = []  # 表字段
-        self.condition_sql = ""  # 条件语句
-        self.args = []
+        self.where_sql = []  # 条件语句
+        self.limit_sql = ""  # 分页
+        self.order_sql = ""  # 排序
+        self.sql = ""  # 执行 sql
+        self.args = []  # 条件参数
 
-    def show_table(self):
+    def show_table(self, show_system: bool = False) -> List[str]:
         """
-        show_tables()方法：查询当前数据库中所有表
+        查询当前数据库中所有表
         :return: 返回一个列表
         """
-        sql = "select name from sqlite_master where type='table' and name not in ('sqlite_master','sqlite_sequence')"
-        self.sqlite.execute(sql)
-        data_list = self.sqlite.fetchall()
-        table_list = [data[0] for data in data_list]
+        sql = "select name from sqlite_master where type='table'"
+        self.cursor.execute(sql)
+        rows = self.cursor.fetchall()
+        table_list = []
+        for row in rows:
+            tb_name = row[0]
+            if show_system is False and tb_name in self.__SYSTEM_TABLES:
+                continue
+            table_list.append(tb_name)
         return table_list  # 返回当前数据库内所有的表
 
-    def table(self, table_name: str):
-        """
-        设置操作表
-        :param table_name: 表名
-        :return: self
-        """
-
-        self.table_name = table_name  # 表名
-        sql = f"PRAGMA table_info(`{table_name}`);"
-        self.sqlite.execute(sql)
-        field_list = self.sqlite.fetchall()
-
-        self.field_list = []
-        for field in field_list:
-            self.field_list.append(field[1])
-        return self
-
-    def create_table(self, table_name: str, field_dict: dict):
+    def create_table(self, table_name: str, field_dict: dict, native_sql: str = None) -> bool:
         """
-        create_table() 创建表，已存在直接返回，不存在则创建
+        创建表，已存在直接返回，不存在则创建
         :param table_name: 表名
         :param field_dict: 表字段列表
         :return: 连接成功：返回 True
         """
-        self.table_name = table_name  # 将表名赋值给实例属性
-
-        self.field_list = field_dict.keys()  # 获取该表的所有的字段名
+        if native_sql is not None:
+            self.sql = native_sql
+        else:
+            self.table_name = table_name.strip(" `'\"")  # 将表名赋值给实例属性
 
-        table_list = self.show_table()  # 获取数据库里所有的表
-        if self.table_name in table_list:  # 判断该表是否已存在
-            return True  # 该表已存在！直接返回
+            self.field_list = field_dict.keys()  # 获取该表的所有的字段名
 
-        field_list = [f"`{key}` {value}" for key, value in field_dict.items()]
-        create_field = ",".join(field_list)  # 将所有的字段与字段类型以 “ , ” 拼接
-        sql = f"""create table `{self.table_name}`(
+            table_list = self.show_table()  # 获取数据库里所有的表
+            if self.table_name in table_list:  # 判断该表是否已存在
+                return True  # 该表已存在！直接返回
+    
+            field_list = ["`{key}` {value}".format(key=str(key).strip(" `'\""), value=value) for key, value in field_dict.items()]
+            create_field = ",".join(field_list)  # 将所有的字段与字段类型以 “ , ” 拼接
+            self.sql = f"""CREATE TABLE `{self.table_name}`(
   {create_field}
-  );"""
-        self.sqlite.execute(sql)
-        self.sqlite_con.commit()
-        return True
+);"""
+        try:
+            self.cursor.execute(self.sql)
+            self.connect.commit()
+            return True
+        except Exception as err:
+            self.connect.rollback()
+            raise err
+
+    def table(self, table_name: str):
+        """
+        设置操作表
+        :param table_name: 表名
+        :return: self
+        """
+        self.table_name = table_name.strip(" `'\"")  # 表名
+        return self
 
-    def create(self, **kwargs):
+    def create(self, **kwargs) -> int:
         """
-        create() 添加一行数据
+        添加一条数据
         :param kwargs: 接收一个字典，key = value 字段 = 值
         :return: 添加成功：返回 True 添加失败：返回 Flase
         """
         try:
-            field_sql = "`,`".join(kwargs.keys())
+            field_sql = "`,`".join([field.strip(" `'\"") for field in kwargs.keys()])
             create_sql = ",".join(["?"] * len(kwargs))
 
             # id 字段为null ，默认自增
-            sql = f"""insert into `{self.table_name}`  (`{field_sql}`) values ({create_sql});"""
-            self.sqlite.execute(sql, tuple(kwargs.values()))
-            self.sqlite_con.commit()
-            return self.sqlite.rowcount
+            self.sql = f"""INSERT INTO `{self.table_name}`  (`{field_sql}`) VALUES ({create_sql});"""
+            self.args = list(kwargs.values())
+            self.cursor.execute(self.sql, self.args)
+            self.connect.commit()
+            return self.cursor.rowcount
         except Exception as err:
-            self.sqlite_con.rollback()
+            self.connect.rollback()
             raise err
 
-    def where(self, sql: str = None, *args):
+    def fields(self, *fields):
+        """
+        查询字段
+        :param fields: 字段
+        :return: self
+        """
+        self.field_list = fields
+        return self
+
+    def where(self, sql: str, *args):
         """
         条件函数
         :param native_sql: 原生sql语句
         :param kwargs: key = value/字段 = 值 条件
         :return: self
         """
-        self.condition_sql = sql
-        self.args = tuple(args)
+        self.where_sql.append(sql)
+        self.args.extend(args)
+        return self
+
+    def order_by(self, *orders):
+        order_fields = []
+        for order in orders:
+            order = str(order).strip(" `'\"")
+            if not order:
+                continue
+
+            if order[0] == "-":
+                order_sql = order[1:]
+                sequence = "DESC"
+            else:
+                order_sql = order
+                sequence = "ASC"
+            order_fields.append(f"`{order_sql}` {sequence}")
+        if len(order_fields) > 0:
+            self.order_sql = f" ORDER BY {', '.join(order_fields)}"
+        else:
+            self.order_sql = ""
         return self
 
-    def delete(self):
+    # 设置分页数据，返回总数据量，总页数
+    def page(self, page: int, pagesize: int) -> Tuple[int, int]:
+        if not isinstance(page, int):
+            page = int(page)
+        if not isinstance(pagesize, int):
+            pagesize = int(pagesize)
+        self.limit_sql = " LIMIT {size} OFFSET {offset}".format(
+            size=pagesize,
+            offset=(page - 1) * pagesize,
+        )
+        total = self.count()
+        return total, math.ceil(total / pagesize)
+
+    def select(self) -> List[dict]:
         """
-        删除满足条件的数据
-        :return: 影响行数
+        查询数据库，返回全部数据
+        :return: list[dict] 返回查询到的所有行
         """
-        sql = f"delete from `{self.table_name}` where {self.condition_sql};"
-
         try:
-            self.sqlite.execute(sql, self.args)
-            self.sqlite_con.commit()
-            return self.sqlite.rowcount
+            if len(self.field_list) == 0:
+                self.field_list = self.__get_fields()
+
+            fields_str = ", ".join(self.field_list)
+            self.sql = f"SELECT {fields_str} FROM `{self.table_name}`"
+            if len(self.where_sql) > 0:
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+            if self.order_sql:
+                self.sql += self.order_sql
+            if self.limit_sql:
+                self.sql += self.limit_sql
+            self.cursor.execute(self.sql, self.args)
+            rows = self.cursor.fetchall()
+            result_field = self.__extract_field_list()
+            return [dict(zip(result_field, row)) for row in rows]
         except Exception as err:
-            self.sqlite_con.rollback()
             raise err
         finally:
-            self.condition_sql = ""
+            self.field_list = []
+            self.where_sql = []
+            self.limit_sql = ""
+            self.order_sql = ""
             self.args = []
 
-    def update(self, **kwargs):
+    def find(self) -> Union[dict, None]:
         """
-        update() 修改数据
-        :param kwargs: 接收一个字典，key == value 条件
-        :return: 影响行数
+        查询数据库，返回第一条数据
+        :return dict
         """
-        if not kwargs: raise ValueError(f"**kwargs")
-
-        update_sql = ",".join([f"`{field}`=?" for field in kwargs.keys()])
-        sql = f"update `{self.table_name}` set {update_sql} where {self.condition_sql};"
-        args = list(kwargs.values())
-        args.extend(self.args)
-
         try:
-            self.sqlite.execute(sql, args)
-            self.sqlite_con.commit()
-            return self.sqlite.rowcount
+            if len(self.field_list) == 0:
+                self.field_list = self.__get_fields()
+
+            fields_str = ", ".join(self.field_list)
+            self.sql = f"SELECT {fields_str} FROM `{self.table_name}`"
+            if len(self.where_sql) > 0:
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+            if self.order_sql:
+                self.sql += self.order_sql
+            if self.limit_sql:
+                self.sql += self.limit_sql
+
+            self.cursor.execute(self.sql, self.args)
+            row = self.cursor.fetchone()
+            if row:
+                result_field = self.__extract_field_list()
+                kwargs = dict(zip(result_field, row))
+                return kwargs
+            return None
         except Exception as err:
-            self.sqlite_con.rollback()
             raise err
-        else:
-
-            return True
+        finally:
+            self.field_list = []
+            self.where_sql = []
+            self.limit_sql = ""
+            self.order_sql = ""
+            self.args = []
 
-    def __extract_field_list(self, *args):
+    def count(self) -> int:
         """
-        解析字段列表，获取字段名称
-        :param field_list: list 接受字段列表
-        :return list 返回字段列表
+        查询条数
+        :return 返回查询条数
         """
-        result_field = []
-        for field in args:
-            field = field.strip()
-            if field == "*":
-                result_field.extend(self.field_list)
-            elif field.find(" as ") != -1:
-                field = field.split(" as ")[-1]
-                field = field.strip()
-
-            result_field.append(field)
-        return result_field
-
-    def select(self, *fields):
+        try:
+            self.sql = f"SELECT COUNT(*) FROM `{self.table_name}`"
+            if len(self.where_sql) > 0:
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+            self.cursor.execute(self.sql, self.args)
+            row = self.cursor.fetchone()
+            if row:
+                return row[0]
+        except Exception as err:
+            print(err)
+        return 0
+    
+    def delete(self) -> int:
         """
-        查询数据库，返回全部数据
-        :param fields: list[field_name] 查询结果字段
-        :return: list[dict] 返回查询到的所有行
+        删除满足条件的数据
+        :return: 影响行数
         """
-        # 结果字段
-        if len(fields) == 0:
-            result_field = self.field_list
-            select_field = ",".join(result_field)
-        else:
-            result_field = self.__extract_field_list(*fields)
-            select_field = ",".join(fields)
-
-        if self.condition_sql:
-            sql = f"select {select_field} from `{self.table_name}` where {self.condition_sql};"
-        else:
-            sql = f"select {select_field} from `{self.table_name}`;"
-
         try:
-            self.sqlite.execute(sql)
-            data = self.sqlite.fetchall()
-            result = self.result(result_field, data)
-            return result
+            self.sql = f"DELETE FROM `{self.table_name}`"
+            if len(self.where_sql) > 0:
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+            self.cursor.execute(self.sql, self.args)
+            self.connect.commit()
+            return self.cursor.rowcount
         except Exception as err:
+            self.connect.rollback()
             raise err
         finally:
-            self.condition_sql = ""
+            self.where_sql = []
             self.args = []
 
-    def find(self, *fields):
+    def update(self, **kwargs) -> int:
         """
-        查询数据库，返回第一条数据
-        :param fields: list[field_name] 查询结果字段
-        :return dict
+        修改数据
+        :param kwargs: 接收一个字典，key == value 条件
+        :return: 影响行数
         """
-        # 结果字段
-        if len(fields) == 0:
-            result_field = self.field_list
-            select_field = ",".join(result_field)
-        else:
-            result_field = self.__extract_field_list(*fields)
-            select_field = ",".join(fields)
-
-        if self.condition_sql:
-            sql = f"select {select_field} from `{self.table_name}` where {self.condition_sql};"
-        else:
-            sql = f"select {select_field} from `{self.table_name}`;"
-
         try:
-            self.sqlite.execute(sql, self.args)
-            data = self.sqlite.fetchone()
-            result = self.result(result_field, data)
-            return result
+            if not kwargs: raise ValueError(f"**kwargs")
+
+            update_sql = ",".join([f"`{field}`=?" for field in kwargs.keys()])
+            self.sql = f"UPDATE `{self.table_name}` SET {update_sql}"
+            if len(self.where_sql) > 0:
+                self.sql += f" WHERE {' AND '.join(self.where_sql)};"
+
+            args = list(kwargs.values())
+            args.extend(self.args)
+            self.args = args
+            self.cursor.execute(self.sql, self.args)
+            self.connect.commit()
+            return self.cursor.rowcount
         except Exception as err:
+            self.connect.rollback()
             raise err
         finally:
-            self.condition_sql = ""
+            self.where_sql = []
             self.args = []
 
-    def execute_native_sql(self, native_sql: str):
-        """
-        执行原生sql，支持多条语句
-        :param native_sql: str 接受原生sql
-        :return list[list[dict]] 返回字段列表
-        """
-        native_sql_list = native_sql.split(";")
-        idx = 1
-        result = []
-        for sql in native_sql_list:
-            sql = sql.lower().strip()
-            if not sql: continue  # 跳过空值
-            data = {
-                "name": f"结果{idx}",
-                "abstract": {
-                    "name": sql,
-                    "info": "OK"
-                },
-            }
-            if sql.startswith("use"):
-                start_time = time.time()
-                self.sqlite.execute(sql)
-                end_time = time.time()
-                data["abstract"] = {
-                    "name": sql,
-                    "info": "OK",
-                    "select_time": end_time - start_time,
-                }
-            elif sql.startswith("select"):
-                start_time = time.time()
-                self.sqlite.execute(sql)
-                end_time = time.time()
-                tmp_data = self.sqlite.fetchall()
-                result_field = self.__extract_sql(sql)
-                tmp_data = self.result(result_field, tmp_data)
-                data["result"] = tmp_data
-                data["abstract"] = {
-                    "name": sql,
-                    "info": "OK",
-                    "select_time": end_time - start_time,
-                }
-            elif sql.startswith("show"):
-                start_time = time.time()
-                self.sqlite.execute(sql)
-                end_time = time.time()
-                tmp_data = self.sqlite.fetchall()
-                tmp_data = [i[0] for i in tmp_data]
-                data["result"] = tmp_data
-                data["abstract"] = {
-                    "name": sql,
-                    "info": "OK",
-                    "select_time": end_time - start_time,
-                }
-            else:
-                start_time = time.time()
-                tmp_data = self.sqlite.execute(sql)
-                self.sqlite_con.commit()
-                end_time = time.time()
-                data["abstract"] = {
-                    "name": sql,
-                    "info": f"影响行数：{tmp_data}",
-                    "select_time": end_time - start_time,
-                }
-            result.append(data)
-            idx += 1
-        return result
+    def __get_fields(self) -> list:
+        if self.table_name is None:
+            return []
+
+        self.sql = f"PRAGMA table_info(`{self.table_name}`);"
+        self.cursor.execute(self.sql)
+        field_list = [field[1] for field in self.cursor.fetchall()]
+        return field_list
 
-    def __extract_sql(self, native_sql: str):
+    def __extract_field_list(self) -> list:
         """
-        解析原生sql，获取字段列表
-        :param native_sql: str 接受原生sql
+        解析字段列表，获取字段名称
         :return list 返回字段列表
         """
-        temp_field = str(native_sql).strip().lower()
-        temp_field = temp_field.lstrip("select")
-        end_idx = temp_field.find("from")
-        if end_idx == -1:
-            raise ValueError(f"{native_sql} 中不存在 from")
-
-        temp_field = temp_field[:end_idx]
-        temp_field = temp_field.strip()
-
-        return self.__extract_field_list(temp_field.split(","))
-
-    def result(self, result_field, data):
-        """
-        result() 组织结果数据
-        :param result_field: 接受一个列表，数据为表字段，组织数据使用
-        :param data: sql查询结果，为嵌套元组
-        :return: 列表嵌套字典类型
-        """
-        if data is None:
-            return data
-        if len(data) == 0:
-            return []
-        elif isinstance(data[0], tuple):
-            result = []
-            for i in data:
-                temp = {}
-                for k, j in enumerate(result_field):
-                    temp[j] = i[k]
-                result.append(temp)
-        else:
-            result = {}
-            for k, j in enumerate(result_field):
-                result[j] = data[k]
-        # 返回查询集
-        return result
+        result_field = []
+        for field in self.field_list:
+            if field == "*":
+                result_field.extend(self.__get_fields())
+            elif str(field).lower().find(" as ") != -1:
+                field = field.split(" as ")[-1]
+
+            field = field.strip(" `'\"")
+            if not field:
+                continue
+            result_field.append(field)
+        return result_field
+
+    def close(self):
+        self.cursor.close()
+        self.connect.close()
+
+    def __del__(self):
+        self.close()
```

### Comparing `PySqlModel-1.0.1/setup.py` & `PySqlModel-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 @Author:函封封
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="PySqlModel",
-    version="1.0.1",
+    version="1.1.0",
     author="HanFengFeng",
     author_email="mr_jia_han@qq.com",
     description="简单方便的数据库查询包",
     # 项目主页
     url="https://github.com/NeverStopDreamingWang/pysqlmodel",
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
     install_requires=[
         "pymysql",
         "sqlite3"
-    ]
+    ],
+    project_urls={
+        "github": "https://github.com/NeverStopDreamingWang/pysqlmodel",
+        "gitee": "https://gitee.com/NeverStopDreamingWang/pysqlmodel",
+    }
 )
 
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
```

