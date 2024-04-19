# Comparing `tmp/xtn-tools-pro-1.0.0.0.0.tar.gz` & `tmp/xtn-tools-pro-1.0.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.0.tar", last modified: Fri Apr 19 08:42:46 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.0.1.tar", last modified: Fri Apr 19 10:18:10 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.0.0.tar` & `xtn-tools-pro-1.0.0.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.0/LICENSE
--rw-rw-rw-   0        0        0      287 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1189 2024-04-19 08:41:52.000000 xtn-tools-pro-1.0.0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0     4003 2024-04-18 07:53:11.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/__init__.py
--rw-rw-rw-   0        0        0     2626 2024-04-18 04:57:03.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/tools.py
--rw-rw-rw-   0        0        0     4877 2024-04-18 05:04:49.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/tools_time.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 08:42:46.000000 xtn-tools-pro-1.0.0.0.0/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.0.1/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1189 2024-04-19 10:18:04.000000 xtn-tools-pro-1.0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5567 2024-04-19 08:42:19.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0     4003 2024-04-18 07:53:11.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/tools.py
+-rw-rw-rw-   0        0        0     1507 2024-04-19 10:16:52.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/tools_flie.py
+-rw-rw-rw-   0        0        0     4867 2024-04-19 10:12:45.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/tools_time.py
+drwxrwxrwx   0        0        0        0 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 10:18:10.000000 xtn-tools-pro-1.0.0.0.1/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.0.0/setup.py` & `xtn-tools-pro-1.0.0.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.0.0",  # 版本
+    version="1.0.0.0.1",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     :param file_path: 文件路径
     :return: 
     """
     result = get_file_md5_32(file_path)
     return result[8:24]
 
 
-
 def get_str_to_json(str_json):
     """
         字符串类型的json格式 转 json
     :param str_json: 字符串json
     :return:
     """
     try:
@@ -97,10 +96,13 @@
     if limit <= 0:
         return 0
     # 根据总条数和limit计算总页数
     total_pages = math.ceil(total / limit)
     return total_pages
 
 
+
+
+
+
 if __name__ == '__main__':
     pass
-
```

### Comparing `xtn-tools-pro-1.0.0.0.0/xtn_tools_pro/tools_time.py` & `xtn-tools-pro-1.0.0.0.1/xtn_tools_pro/tools_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 说明：
-#    程序说明xxxxxxxxxxxxxxxxxxx
+#    时间相关的工具
 # History:
 # Date          Author    Version       Modification
 # --------------------------------------------------------------------------------------------------
 # 2024/4/18    xiatn     V00.01.000    新建
 # --------------------------------------------------------------------------------------------------
 import time, datetime
```

