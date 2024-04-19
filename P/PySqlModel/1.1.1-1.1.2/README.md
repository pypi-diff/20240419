# Comparing `tmp/PySqlModel-1.1.1.tar.gz` & `tmp/PySqlModel-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySqlModel-1.1.1.tar", last modified: Fri Apr 19 15:12:40 2024, max compression
+gzip compressed data, was "dist\PySqlModel-1.1.2.tar", last modified: Fri Apr 19 15:34:10 2024, max compression
```

## Comparing `PySqlModel-1.1.1.tar` & `PySqlModel-1.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/
--rw-rw-rw-   0        0        0     1524 2024-04-19 14:25:02.000000 PySqlModel-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      388 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel/
--rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.1/PySqlModel/__init__.py
--rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.1/PySqlModel/base.py
--rw-rw-rw-   0        0        0    11502 2024-04-19 15:12:06.000000 PySqlModel-1.1.1/PySqlModel/mysql.py
--rw-rw-rw-   0        0        0    10877 2024-04-19 15:12:06.000000 PySqlModel-1.1.1/PySqlModel/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/
--rw-rw-rw-   0        0        0      388 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/PySqlModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6974 2024-04-19 14:15:02.000000 PySqlModel-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 15:12:40.000000 PySqlModel-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-19 15:12:31.000000 PySqlModel-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/
+-rw-rw-rw-   0        0        0     1524 2024-04-19 14:25:02.000000 PySqlModel-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      388 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel/
+-rw-rw-rw-   0        0        0      123 2024-04-19 13:01:04.000000 PySqlModel-1.1.2/PySqlModel/__init__.py
+-rw-rw-rw-   0        0        0       94 2023-05-09 17:36:37.000000 PySqlModel-1.1.2/PySqlModel/base.py
+-rw-rw-rw-   0        0        0    11492 2024-04-19 15:31:26.000000 PySqlModel-1.1.2/PySqlModel/mysql.py
+-rw-rw-rw-   0        0        0    10867 2024-04-19 15:31:26.000000 PySqlModel-1.1.2/PySqlModel/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/
+-rw-rw-rw-   0        0        0      388 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/PySqlModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6974 2024-04-19 14:15:02.000000 PySqlModel-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:34:10.000000 PySqlModel-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-19 15:34:01.000000 PySqlModel-1.1.2/setup.py
```

### Comparing `PySqlModel-1.1.1/LICENSE` & `PySqlModel-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.1/PySqlModel/mysql.py` & `PySqlModel-1.1.2/PySqlModel/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
         """
         try:
             field_sql = "`,`".join([field.strip(" `'\"") for field in kwargs.keys()])
             create_sql = ",".join(["%s"] * len(kwargs))
 
             # id 字段为null ，默认自增
             self.sql = f"INSERT INTO `{self.table_name}`  (`{field_sql}`) VALUES ({create_sql});"
-            self.args = kwargs.values()
-            rowcount = self.cursor.execute(self.sql, self.args)
+            args = kwargs.values()
+            rowcount = self.cursor.execute(self.sql, args)
             self.connect.commit()
             return rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
 
     def fields(self, *fields):
@@ -255,50 +255,50 @@
             row = self.cursor.fetchone()
             if row:
                 return row[0]
         except Exception as err:
             print(err)
         return 0
 
-    def delete(self) -> int:
+    def update(self, **kwargs) -> int:
         """
-        删除满足条件的数据
+        修改数据
+        :param kwargs: key = value/字段 = 值 条件
         :return 返回受影响的行
         """
         try:
-            self.sql = f"DELETE FROM `{self.table_name}`"
+            if not kwargs: raise ValueError(f"**kwargs")
+
+            update_sql = ", ".join([f"`{field}`=%s" for field in kwargs.keys()])
+            self.sql = f"UPDATE `{self.table_name}` SET {update_sql}"
             if len(self.where_sql) > 0:
-                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+                self.sql += f" WHERE {' AND '.join(self.where_sql)};"
+
+            args = list(kwargs.values())
+            args.extend(self.args)
+            self.args = args
             rowcount = self.cursor.execute(self.sql, self.args)
             self.connect.commit()
             return rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
         finally:
             self.where_sql = []
             self.args = []
 
-    def update(self, **kwargs) -> int:
+    def delete(self) -> int:
         """
-        修改数据
-        :param kwargs: key = value/字段 = 值 条件
+        删除满足条件的数据
         :return 返回受影响的行
         """
         try:
-            if not kwargs: raise ValueError(f"**kwargs")
-
-            update_sql = ", ".join([f"`{field}`=%s" for field in kwargs.keys()])
-            self.sql = f"UPDATE `{self.table_name}` SET {update_sql}"
+            self.sql = f"DELETE FROM `{self.table_name}`"
             if len(self.where_sql) > 0:
-                self.sql += f" WHERE {' AND '.join(self.where_sql)};"
-
-            args = list(kwargs.values())
-            args.extend(self.args)
-            self.args = args
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
             rowcount = self.cursor.execute(self.sql, self.args)
             self.connect.commit()
             return rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
         finally:
```

### Comparing `PySqlModel-1.1.1/PySqlModel/sqlite.py` & `PySqlModel-1.1.2/PySqlModel/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         """
         try:
             field_sql = "`,`".join([field.strip(" `'\"") for field in kwargs.keys()])
             create_sql = ",".join(["?"] * len(kwargs))
 
             # id 字段为null ，默认自增
             self.sql = f"""INSERT INTO `{self.table_name}`  (`{field_sql}`) VALUES ({create_sql});"""
-            self.args = list(kwargs.values())
-            self.cursor.execute(self.sql, self.args)
+            args = list(kwargs.values())
+            self.cursor.execute(self.sql, args)
             self.connect.commit()
             return self.cursor.rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
 
     def fields(self, *fields):
@@ -236,50 +236,50 @@
             row = self.cursor.fetchone()
             if row:
                 return row[0]
         except Exception as err:
             print(err)
         return 0
 
-    def delete(self) -> int:
+    def update(self, **kwargs) -> int:
         """
-        删除满足条件的数据
+        修改数据
+        :param kwargs: 接收一个字典，key == value 条件
         :return: 影响行数
         """
         try:
-            self.sql = f"DELETE FROM `{self.table_name}`"
+            if not kwargs: raise ValueError(f"**kwargs")
+
+            update_sql = ",".join([f"`{field}`=?" for field in kwargs.keys()])
+            self.sql = f"UPDATE `{self.table_name}` SET {update_sql}"
             if len(self.where_sql) > 0:
-                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
+                self.sql += f" WHERE {' AND '.join(self.where_sql)};"
+
+            args = list(kwargs.values())
+            args.extend(self.args)
+            self.args = args
             self.cursor.execute(self.sql, self.args)
             self.connect.commit()
             return self.cursor.rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
         finally:
             self.where_sql = []
             self.args = []
 
-    def update(self, **kwargs) -> int:
+    def delete(self) -> int:
         """
-        修改数据
-        :param kwargs: 接收一个字典，key == value 条件
+        删除满足条件的数据
         :return: 影响行数
         """
         try:
-            if not kwargs: raise ValueError(f"**kwargs")
-
-            update_sql = ",".join([f"`{field}`=?" for field in kwargs.keys()])
-            self.sql = f"UPDATE `{self.table_name}` SET {update_sql}"
+            self.sql = f"DELETE FROM `{self.table_name}`"
             if len(self.where_sql) > 0:
-                self.sql += f" WHERE {' AND '.join(self.where_sql)};"
-
-            args = list(kwargs.values())
-            args.extend(self.args)
-            self.args = args
+                self.sql += f" WHERE {' AND '.join(self.where_sql)}"
             self.cursor.execute(self.sql, self.args)
             self.connect.commit()
             return self.cursor.rowcount
         except Exception as err:
             self.connect.rollback()
             raise err
         finally:
```

### Comparing `PySqlModel-1.1.1/README.md` & `PySqlModel-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PySqlModel-1.1.1/setup.py` & `PySqlModel-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @Author:函封封
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="PySqlModel",
-    version="1.1.1",
+    version="1.1.2",
     author="HanFengFeng",
     author_email="mr_jia_han@qq.com",
     description="简单方便的数据库查询包",
     # 项目主页
     url="https://github.com/NeverStopDreamingWang/pysqlmodel",
     # 你要安装的包，通过 setuptools.find_packages 找到当前目录下有哪些包
     packages=find_packages(),
```

