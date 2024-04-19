# Comparing `tmp/all_in_one_chay-2.4.7.tar.gz` & `tmp/all_in_one_chay-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_in_one_chay-2.4.7.tar", last modified: Tue Apr 16 15:21:28 2024, max compression
+gzip compressed data, was "all_in_one_chay-2.4.8.tar", last modified: Fri Apr 19 15:55:50 2024, max compression
```

## Comparing `all_in_one_chay-2.4.7.tar` & `all_in_one_chay-2.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/
--rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.7/LICENSE
--rw-rw-rw-   0        0        0     4906 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     4269 2024-04-16 15:17:42.000000 all_in_one_chay-2.4.7/README.md
--rw-rw-rw-   0        0        0      622 2024-04-16 15:01:00.000000 all_in_one_chay-2.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-04-16 15:00:52.000000 all_in_one_chay-2.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.931221 all_in_one_chay-2.4.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.931221 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/
--rw-rw-rw-   0        0        0     9572 2024-04-16 15:12:54.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/Allinone.py
--rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/
--rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/book.py
--rw-rw-rw-   0        0        0    11629 2024-04-16 15:07:24.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/calculator.py
--rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
--rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/math_cal_py.py
--rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/student_py.py
--rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/tuxing_cal.py
--rw-rw-rw-   0        0        0     2804 2024-04-16 15:08:27.000000 all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/xiaogongju.py
-drwxrwxrwx   0        0        0        0 2024-04-16 15:21:28.946850 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/
--rw-rw-rw-   0        0        0     4906 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-16 15:21:28.000000 all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/
+-rw-rw-rw-   0        0        0     1091 2024-03-09 13:46:48.000000 all_in_one_chay-2.4.8/LICENSE
+-rw-rw-rw-   0        0        0     5213 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4546 2024-04-19 15:50:47.000000 all_in_one_chay-2.4.8/README.md
+-rw-rw-rw-   0        0        0      642 2024-04-19 15:53:14.000000 all_in_one_chay-2.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-19 15:55:01.000000 all_in_one_chay-2.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/
+-rw-rw-rw-   0        0        0     9739 2024-04-19 15:41:59.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/Allinone.py
+-rw-rw-rw-   0        0        0        0 2024-02-23 09:19:09.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.704378 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/
+-rw-rw-rw-   0        0        0     9185 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/book.py
+-rw-rw-rw-   0        0        0    12741 2024-04-19 15:49:01.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/calculator.py
+-rw-rw-rw-   0        0        0      876 2024-04-16 15:07:32.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py
+-rw-rw-rw-   0        0        0     1711 2024-04-16 15:12:03.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/math_cal_py.py
+-rw-rw-rw-   0        0        0     1381 2024-02-09 06:24:29.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/student_py.py
+-rw-rw-rw-   0        0        0     6949 2024-04-16 15:08:18.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/tuxing_cal.py
+-rw-rw-rw-   0        0        0     2804 2024-04-16 15:08:27.000000 all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/xiaogongju.py
+drwxrwxrwx   0        0        0        0 2024-04-19 15:55:50.720021 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/
+-rw-rw-rw-   0        0        0     5213 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-19 15:55:50.000000 all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/top_level.txt
```

### Comparing `all_in_one_chay-2.4.7/LICENSE` & `all_in_one_chay-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/PKG-INFO` & `all_in_one_chay-2.4.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,121 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.7
+Version: 2.4.8
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7
-Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# All-in-one
-多功能一体机
+# All-in-one Including
+多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:04
+    # @TIME:2024/4/19 23:41
     # @FILE:Allinone.py
-    # @version:2.4.7
+    # @version:2.4.8
     # @Software:Visual Studio Code
 
 FUNCTIONS
     allinone(fuwu, mode, *args)
         :param fuwu 需要服务的功能
         :param mode 部分功能需要的模式（详见Github中All-in-one2.4.0分支的Wiki页）
         :param *args 可变参数，表示需要传入的参数，建议用元组或列表类型，具体所需类型见README.MD
         :return: 0：正常，1：不正常，其他返回值表示功能的结果
 
-        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整-、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件
+        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件）
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\allinone.py
 
 
 Help on module calculator:
 
 NAME
     calculator
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:07
+    # @TIME:2024/4/19 23:42
     # @FILE:calculator.py
     # @Software:Visual Studio Code
 
 FUNCTIONS
-    FtemporCtemp(mode: str, FtemporCtemp: float)
+    FtemporCtemp(mode: str, FtemporCtemp: float) -> float
 
-    duihuan(mode: int, money: float)
+    duihuan(mode: int, money: float) -> float
 
-    fab(x: int)
+    fab(x: int) -> int
 
-    fanzhuanzifuchuan(s: str)
+    factorization(num: int) -> list[int]
 
-    isfab(x: int)
+    fanzhuanzifuchuan(s: str) -> str
 
-    isfabhuiwenshu(x: int)
+    isfab(x: int) -> bool
 
-    isfabhuiwenzhishu(x: int)
+    isfabhuiwenshu(x: int) -> bool
 
-    isfabparam(x: int)
+    isfabhuiwenzhishu(x: int) -> bool
+
+    isfabparam(x: int) -> bool
 
     isfabwanquanpingfangshu(num: int) -> bool
 
-    ishuiwenshu(d: int)
+    ishuiwenshu(d: int) -> bool
 
-    ishuiwenzhishu(d: int)
+    ishuiwenzhishu(d: int) -> bool
 
-    isleapyear(x)
+    isleapyear(x) -> bool
 
-    isparam(d: int)
+    isparam(d: int) -> bool
 
-    istribonacci(n: int)
+    istribonacci(n: int) -> bool
 
-    istribonaccihuiwenshu(n: int)
+    istribonaccihuiwenshu(n: int) -> bool
 
-    istribonaccihuiwenshuparam(n: int)
+    istribonaccihuiwenshuparam(n: int) -> bool
 
-    istribonacciparam(n: int)
+    istribonacciparam(n: int) -> bool
 
     istribonacciwanquanpingfangshu(num: int) -> bool
 
     iswanquanpingfangshu(num: int) -> bool
 
     jinzhizhuanhuan(a: int, b: int, c: str) -> str
 
-    tribonacci(n: int)
+    mima(num: int, n: int) -> int
+
+    tribonacci(n: int) -> int
 
     wanquanpingfangshu(num: int) -> int
 
-    yiyuanerci(float1: float, float2: float, float3: float)
+    yiyuanerci(float1: float, float2: float, float3: float) -> tuple
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\calculator.py
 
 
+
 Help on module erfenchazhao_py:
 
 NAME
     erfenchazhao_py
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
```

### Comparing `all_in_one_chay-2.4.7/README.md` & `all_in_one_chay-2.4.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,105 @@
-# All-in-one
-多功能一体机
+# All-in-one Including
+多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:04
+    # @TIME:2024/4/19 23:41
     # @FILE:Allinone.py
-    # @version:2.4.7
+    # @version:2.4.8
     # @Software:Visual Studio Code
 
 FUNCTIONS
     allinone(fuwu, mode, *args)
         :param fuwu 需要服务的功能
         :param mode 部分功能需要的模式（详见Github中All-in-one2.4.0分支的Wiki页）
         :param *args 可变参数，表示需要传入的参数，建议用元组或列表类型，具体所需类型见README.MD
         :return: 0：正常，1：不正常，其他返回值表示功能的结果
 
-        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整-、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件
+        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件）
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\allinone.py
 
 
 Help on module calculator:
 
 NAME
     calculator
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:07
+    # @TIME:2024/4/19 23:42
     # @FILE:calculator.py
     # @Software:Visual Studio Code
 
 FUNCTIONS
-    FtemporCtemp(mode: str, FtemporCtemp: float)
+    FtemporCtemp(mode: str, FtemporCtemp: float) -> float
 
-    duihuan(mode: int, money: float)
+    duihuan(mode: int, money: float) -> float
 
-    fab(x: int)
+    fab(x: int) -> int
 
-    fanzhuanzifuchuan(s: str)
+    factorization(num: int) -> list[int]
 
-    isfab(x: int)
+    fanzhuanzifuchuan(s: str) -> str
 
-    isfabhuiwenshu(x: int)
+    isfab(x: int) -> bool
 
-    isfabhuiwenzhishu(x: int)
+    isfabhuiwenshu(x: int) -> bool
 
-    isfabparam(x: int)
+    isfabhuiwenzhishu(x: int) -> bool
+
+    isfabparam(x: int) -> bool
 
     isfabwanquanpingfangshu(num: int) -> bool
 
-    ishuiwenshu(d: int)
+    ishuiwenshu(d: int) -> bool
 
-    ishuiwenzhishu(d: int)
+    ishuiwenzhishu(d: int) -> bool
 
-    isleapyear(x)
+    isleapyear(x) -> bool
 
-    isparam(d: int)
+    isparam(d: int) -> bool
 
-    istribonacci(n: int)
+    istribonacci(n: int) -> bool
 
-    istribonaccihuiwenshu(n: int)
+    istribonaccihuiwenshu(n: int) -> bool
 
-    istribonaccihuiwenshuparam(n: int)
+    istribonaccihuiwenshuparam(n: int) -> bool
 
-    istribonacciparam(n: int)
+    istribonacciparam(n: int) -> bool
 
     istribonacciwanquanpingfangshu(num: int) -> bool
 
     iswanquanpingfangshu(num: int) -> bool
 
     jinzhizhuanhuan(a: int, b: int, c: str) -> str
 
-    tribonacci(n: int)
+    mima(num: int, n: int) -> int
+
+    tribonacci(n: int) -> int
 
     wanquanpingfangshu(num: int) -> int
 
-    yiyuanerci(float1: float, float2: float, float3: float)
+    yiyuanerci(float1: float, float2: float, float3: float) -> tuple
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\calculator.py
 
 
+
 Help on module erfenchazhao_py:
 
 NAME
     erfenchazhao_py
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
```

### Comparing `all_in_one_chay-2.4.7/pyproject.toml` & `all_in_one_chay-2.4.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "All-in-one-chay"
-version = "2.4.7"
+version = "2.4.8"
 authors = [
   { name="chay", email="lichenyi_2020@qq.com" },
 ]
 description = "多功能一体机（All-in-one）"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7"
-Issues = "https://github.com/lichenyichay/All-in-one/issues"
+Homepage = "https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8"
+Issues = "https://github.com/lichenyichay/All-in-one-Including/issues"
```

### Comparing `all_in_one_chay-2.4.7/setup.py` & `all_in_one_chay-2.4.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding:UTF-8
 import setuptools
 
 setuptools.setup(
     name="All-in-one-chay",
-    version="2.4.7",
+    version="2.4.8",
     author="Chay",
     author_email="lichenyi_2020@qq.com",
-    url="https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7",
+    url="https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8",
     description="All-in-one",
     long_description="多功能一体机",
     python_requires=">=3.5",
     # packages=setuptools.find_packages("src"),
     packages_dir={"": "src"},
     packages_data={"": ["*.txt", "*.info", "*.properties"], "": ["data/*.*"]},
     exclude=["*.test", "*.test.*", "test.*", "test"],
```

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/Allinone.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/Allinone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:UTF-8 -*-
 # @Author:Chay
-# @TIME:2024/4/16 23:04
+# @TIME:2024/4/19 23:41
 # @FILE:Allinone.py
-# @version:2.4.7
+# @version:2.4.8
 # @Software:Visual Studio Code
 import math,random
 import module.book as book
 import module.calculator as calculator
 import module.erfenchazhao_py  as erfenchazhao_py
 import module.math_cal_py as math_cal
 import module.student_py as student_py
@@ -73,14 +73,18 @@
         return calculator.isfabwanquanpingfangshu(args[0])
     elif fuwu=="判断泰波那契序列完全平方数":
         return calculator.istribonacciwanquanpingfangshu(args[0])
     elif fuwu == "进制转换":
         return calculator.jinzhizhuanhuan(args[0],args[1],args[2])
     elif fuwu=="math库计算器":
         return math_cal.math_cal(mode,args[0],args[1])
+    elif fuwu == "分解因式":
+        return calculator.factorization(args[0])
+    elif fuwu == "提取密码":
+        return calculator.mima(args[0],args[1])
     elif fuwu == "图形计算器":
         while True:
             huida = args[0]
             try:
                 args2=[]
                 for i in range(1,len(args)):
                     args2.append(args[i])
```

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/book.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/book.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/calculator.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding:UTF-8 -*-
 # @Author:Chay
-# @TIME:2024/4/16 23:07
+# @TIME:2024/4/19 23:42
 # @FILE:calculator.py
 # @Software:Visual Studio Code
-import math
+import math,itertools,random
 '''
 函数名：FtemporCtemp
 调用形式：a = FtemporCtemp(mode,FtemporCtemp)
 :param mode 模式 ℃to℉（摄氏度转为华氏度）/℉to℃（华氏度转为摄氏度） 模式不在选择范围内会抛出异常
 :return 转换后的温度（不带单位）
 作用：华氏度与摄氏度转换
 '''
-def FtemporCtemp(mode:str,FtemporCtemp:float):
+def FtemporCtemp(mode:str,FtemporCtemp:float) -> float:
     if mode == "℃to℉":
         return FtemporCtemp*9/5+32
     elif mode == "℉to℃":
         return (FtemporCtemp-32)*5/9
     else:
         raise TypeError("TypeError:模式错误！")
 
@@ -23,15 +23,15 @@
 函数名：duihuan
 调用形式：a = duihuan(mode,money)
 :param mode 模式 1~16 对应不同的货币转换，汇率也不同 模式不在选择范围内会抛出异常
 :param money 要兑换的金额（以模式箭头前的货币单位作为1单位量）
 :return 转换后的货币数量
 作用：货币交换
 '''
-def duihuan(mode:int,money:float):
+def duihuan(mode:int,money:float) -> float:
     if mode == 1:
         return 0.14 * money #CNY to USD
     elif mode == 2:
         return 20.71 * money #CNY to JPY
     elif mode == 3:
         return 7.2 * money #USD to CNY
     elif mode == 4:
@@ -68,29 +68,29 @@
 :param float1 系数1 类型：float
 :param float2 系数2 类型：float
 :param float3 系数3 类型：float
 :return x1 实数根1 类型：float
 :return x2 实数根2 类型：float
 作用：求解一元二次方程
 '''
-def yiyuanerci(float1:float,float2:float,float3:float):
+def yiyuanerci(float1:float,float2:float,float3:float) -> tuple:
     dlt = float2 ** 2 - 4 * float1 * float3
     x1 = (-float2 + math.sqrt(dlt)) / 2 / float1
     x2 = (-float2 - math.sqrt(dlt)) / 2 / float1
-    return f"x1 = {x1},x2 = {x2}"
+    return (x1,x2)
 
 '''
 函数名：fanzhuanzifuchuan
 调用形式：a = fanzhuanzifuchuan(s)
 :param s 需要反转的字符串 类型：str
 :return s1 翻转后的字符串 类型：str
 作用：反转字符串
 '''
 
-def fanzhuanzifuchuan(s:str):
+def fanzhuanzifuchuan(s:str) -> str:
     s=str(s)
     s1=""
     for i in range(len(s)-1,-1,-1):
         j=0
         s1 += s[i]
         j+=1
     return s1
@@ -98,44 +98,44 @@
 '''
 函数名：isparam
 调用形式：a = isparam(d)
 :param d  类型：int
 :return x 是否为质数 类型：bool(True or False)
 作用：判断质数
 '''
-def isparam(d:int):
+def isparam(d:int) -> bool:
     if d <= 1:
         return False
     for i in range(2,math.sqrt(d)+1):
         if d%i==0:
             return False
     return True
 
 '''
 函数名：ishuiwenshu
 调用形式：a = ishuiwenshu(s)
 :param d  类型：int
 :return x 是否为回文数 类型：bool(True or False)
 作用：判断回文数
 '''
-def ishuiwenshu(d:int):
+def ishuiwenshu(d:int) -> bool:
     d1=int(fanzhuanzifuchuan(str(d)))
     if d1==d:
         return True
     else:
         return False
 
 '''
 函数名：ishuiwenzhishu
 调用形式：a = ishuiwenzhishu(d)
 :param d  类型：int
 :return x 是否为回文质数 类型：bool(True or False)
 作用：判断回文质数
 '''
-def ishuiwenzhishu(d:int):
+def ishuiwenzhishu(d:int) -> bool:
     d1=int(fanzhuanzifuchuan(str(d)))
     if d1==d:
         if isparam(d):
             return True
         else:
             return False
     else:
@@ -144,30 +144,30 @@
 '''
 函数名：fab
 调用形式：a = fab(d)
 :param x  类型：int
 :return a[x-1] 斐波那契数列的第x位
 作用：求斐波那契数列的第x位
 '''
-def fab(x:int):
+def fab(x:int) -> int:
     a=[1,1]
     for i in range(2,x):
         a.append(a[i-1]+a[i-2])
     for i in range(x):
         print(a[i]," ")
     return a[x-1]
 
 '''
 函数名：isfab
 调用形式：a = isfab(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否为斐波那契数列中的一个数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数
 '''
-def isfab(x:int):
+def isfab(x:int) -> bool:
     a=[1,1]
     for i in range(2,int(math.sqrt(x+2))):
         a.append(a[i-1]+a[i-2])
     if x not in a:
         return False
     else:
         return True
@@ -175,54 +175,54 @@
 '''
 函数名：isfabparam
 调用形式：a = isfabparam(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契质数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个质数
 '''
-def isfabparam(x:int):
+def isfabparam(x:int) -> bool:
     if isfab(x) and isparam(x):
         return True
     else:
         return False
 
 '''
 函数名：isfabhuiwenshu
 调用形式：a = isfabhuiwenshu(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契回文数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个回文数
 '''
-def isfabhuiwenshu(x:int):
+def isfabhuiwenshu(x:int) -> bool:
     if isfab(x) and ishuiwenshu(x):
         return True
     else:
         return False
 
 '''
 函数名：isfabhuiwenzhishu
 调用形式：a = isfabhuiwenzhishu(d)
 :param d  类型：int(0<d<=12586269025)
 :return x 是否是斐波那契回文质数 类型：bool(True or False)
 作用：是否为斐波那契数列中的一个数且为一个回文质数
 '''
-def isfabhuiwenzhishu(x:int):
+def isfabhuiwenzhishu(x:int) -> bool:
     if isfab(x) and ishuiwenzhishu(x):
         return True
     else:
         return False
 
 '''
 函数名：isleapyear
 调用形式：a = isleapyear(d)
 :param d  类型：int
 :return x 对应年份是否是闰年 类型：bool(True or False)
 作用：判断闰年
 '''   
-def isleapyear(x):
+def isleapyear(x) -> bool:
     if x%4==0:
         if x%100==0:
             if x%400==0:
                 return True
             else:
                 return False
         else:
@@ -235,15 +235,15 @@
 T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
 函数名：tribonacci
 调用形式：a = tribonacci(d)
 :param x  类型：int
 :return a[x-1] 泰波那契序列的第x位
 作用：求泰波那契序列的第x位
 '''
-def tribonacci(n:int):
+def tribonacci(n:int) -> int:
     d=[0,1,1]
     if n<=2:
         return d[n]
     else:
         for i in range(3,n+1):
             d.append(d[i-3]+d[i-2]+d[i-1])
         return d[n]
@@ -253,15 +253,15 @@
 T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
 函数名：istribonacci
 调用形式：a = istribonacci(d)
 :param x  类型：int
 :return x 是否属于泰波那契序列中的一个数（True or False）
 作用：判断是否属于泰波那契序列中的一个数
 '''
-def istribonacci(n:int):
+def istribonacci(n:int) -> bool:
     a=[0,1,1]
     if n>=10000:
         for i in range(3,int(math.sqrt(n+3))):
             a.append(a[i-1]+a[i-2]+a[i-3])
     elif n>=1389537:
         for i in range(3,int(math.sqrt(int(math.sqrt(n+3))))):
             a.append(a[i-1]+a[i-2]+a[i-3])
@@ -278,45 +278,45 @@
 T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
 函数名：istribonaccihuiwenshu
 调用形式：a = istribonaccihuiwenshu(d)
 :param x  类型：int
 :return x 是否是泰波那契序列回文数（True or False）
 作用：判断泰波那契序列回文数
 '''
-def istribonaccihuiwenshu(n:int):
+def istribonaccihuiwenshu(n:int) -> bool:
     if istribonacci(n) and ishuiwenshu(n):
         return True
     else:
         return False
 
 '''
 泰波那契序列 Tn 定义如下： 
 T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
 函数名：istribonaccihuiwenshuparam
 调用形式：a = istribonaccihuiwenshuparam(d)
 :param x  类型：int
 :return x 是否是泰波那契序列回文质数（True or False）
 作用：判断泰波那契序列回文质数
 '''
-def istribonaccihuiwenshuparam(n:int):
+def istribonaccihuiwenshuparam(n:int) -> bool:
     if isfabhuiwenshu(n) and isparam(n):
         return True
     else:
         return False
 
 '''
 泰波那契序列 Tn 定义如下： 
 T0 = 0, T1 = 1, T2 = 1, 且在 n >= 0 的条件下 Tn+3 = Tn + Tn+1 + Tn+2
 函数名：istribonacciparam
 调用形式：a = istribonacciparam(d)
 :param x  类型：int
 :return x 是否是泰波那契序列质数（True or False）
 作用：判断泰波那契序列质数
 '''
-def istribonacciparam(n:int):
+def istribonacciparam(n:int) -> bool:
     if istribonacci(n) and isparam(n):
         return True
     else:
         return False
 
 '''
 函数名：iswanquanpingfangshu
@@ -367,14 +367,15 @@
 '''
 函数名：jinzhizhuanhuan
 调用形式：a =  jinzhizhuanhuan(a,b,c)
 :param a c的进制数 (2<=a<=36)
 :param b 结果的进制数 (2<=a<=36)
 :param c 需转换的数 无需前缀且需符合a进制规则
 :return z 结果
+作用：进行进制转换
 '''
 def jinzhizhuanhuan(a:int,b:int,c:str) -> str:
     if a == b:
         return c
     elif a == 10  and b != 10:
         num = int(c)  
         result = ""  
@@ -397,8 +398,45 @@
             else:
                 base = ord(c[i])-ord('0')
             ans += tmp*base
             tmp *= a
         return str(ans)
 
     else:
-        return jinzhizhuanhuan(10,b,jinzhizhuanhuan(a,10,c))
+        return jinzhizhuanhuan(10,b,jinzhizhuanhuan(a,10,c))
+    
+'''
+函数名：factorization
+调用形式：a = facforization(num)
+:param num 需因式分解的自然数
+:return factor 因式分解的结果
+作用：对一个数进行因式分解
+'''
+def factorization(num:int) -> list[int]:
+    factor = []
+    while num > 1:
+        for i in range(num - 1):
+            k = i + 2
+            if num % k == 0:
+                factor.append(k)
+                num = int(num / k)
+                break
+    return factor
+
+'''
+函数名：mima
+调用形式：a = mima(num)
+:param num 提取密码的数字
+:param n 密码位数
+:return z 结果
+作用：对一个数提取密码
+'''
+def mima(num:int,n:int) -> int:
+    factor = factorization(num)
+    y = []
+    if n <= len(str(max(factor))):
+        for i in itertools.combinations(factor,n):
+            y.append(int(''.join('%d'%o for o in i)))
+        return random.choice(y)
+    else:
+        return 0
+
```

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/erfenchazhao_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/math_cal_py.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/math_cal_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/student_py.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/student_py.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/tuxing_cal.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/tuxing_cal.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All-in-one_chayLichenyi/module/xiaogongju.py` & `all_in_one_chay-2.4.8/src/All-in-one_chayLichenyi/module/xiaogongju.py`

 * *Files identical despite different names*

### Comparing `all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/PKG-INFO` & `all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,121 @@
 Metadata-Version: 2.1
 Name: All-in-one-chay
-Version: 2.4.7
+Version: 2.4.8
 Summary: 多功能一体机（All-in-one）
-Home-page: https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7
+Home-page: https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
 Author: Chay
 Author-email: chay <lichenyi_2020@qq.com>
-Project-URL: Homepage, https://github.com/lichenyichay/All-in-one/releases/tag/v2.4.7
-Project-URL: Issues, https://github.com/lichenyichay/All-in-one/issues
+Project-URL: Homepage, https://github.com/lichenyichay/All-in-one-Including/releases/tag/v2.4.8
+Project-URL: Issues, https://github.com/lichenyichay/All-in-one-Including/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# All-in-one
-多功能一体机
+# All-in-one Including
+多功能一体机库版本，现已更新至2.4.8版本
 说明如下：
 ```python
 Help on module Allinone:
 
 NAME
     Allinone
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:04
+    # @TIME:2024/4/19 23:41
     # @FILE:Allinone.py
-    # @version:2.4.7
+    # @version:2.4.8
     # @Software:Visual Studio Code
 
 FUNCTIONS
     allinone(fuwu, mode, *args)
         :param fuwu 需要服务的功能
         :param mode 部分功能需要的模式（详见Github中All-in-one2.4.0分支的Wiki页）
         :param *args 可变参数，表示需要传入的参数，建议用元组或列表类型，具体所需类型见README.MD
         :return: 0：正常，1：不正常，其他返回值表示功能的结果
 
-        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整-、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件
+        功能（按代码顺序排序，不分先后）：大小写互换、抽取随机数、求最小公倍数、求最大公倍数、图形计算器、小学学生信息管理系统、二分查找、求余、向下取整、向上取整、多个数求和、多个数求差、多个数求积、判断闰年、判断是否为质数、整数、小数计算（加减乘除）、分数计算（加减乘除）......（具体见Github All-in-one2.4.0分支Readme.md文件）
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\allinone.py
 
 
 Help on module calculator:
 
 NAME
     calculator
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
     # @Author:Chay
-    # @TIME:2024/4/16 23:07
+    # @TIME:2024/4/19 23:42
     # @FILE:calculator.py
     # @Software:Visual Studio Code
 
 FUNCTIONS
-    FtemporCtemp(mode: str, FtemporCtemp: float)
+    FtemporCtemp(mode: str, FtemporCtemp: float) -> float
 
-    duihuan(mode: int, money: float)
+    duihuan(mode: int, money: float) -> float
 
-    fab(x: int)
+    fab(x: int) -> int
 
-    fanzhuanzifuchuan(s: str)
+    factorization(num: int) -> list[int]
 
-    isfab(x: int)
+    fanzhuanzifuchuan(s: str) -> str
 
-    isfabhuiwenshu(x: int)
+    isfab(x: int) -> bool
 
-    isfabhuiwenzhishu(x: int)
+    isfabhuiwenshu(x: int) -> bool
 
-    isfabparam(x: int)
+    isfabhuiwenzhishu(x: int) -> bool
+
+    isfabparam(x: int) -> bool
 
     isfabwanquanpingfangshu(num: int) -> bool
 
-    ishuiwenshu(d: int)
+    ishuiwenshu(d: int) -> bool
 
-    ishuiwenzhishu(d: int)
+    ishuiwenzhishu(d: int) -> bool
 
-    isleapyear(x)
+    isleapyear(x) -> bool
 
-    isparam(d: int)
+    isparam(d: int) -> bool
 
-    istribonacci(n: int)
+    istribonacci(n: int) -> bool
 
-    istribonaccihuiwenshu(n: int)
+    istribonaccihuiwenshu(n: int) -> bool
 
-    istribonaccihuiwenshuparam(n: int)
+    istribonaccihuiwenshuparam(n: int) -> bool
 
-    istribonacciparam(n: int)
+    istribonacciparam(n: int) -> bool
 
     istribonacciwanquanpingfangshu(num: int) -> bool
 
     iswanquanpingfangshu(num: int) -> bool
 
     jinzhizhuanhuan(a: int, b: int, c: str) -> str
 
-    tribonacci(n: int)
+    mima(num: int, n: int) -> int
+
+    tribonacci(n: int) -> int
 
     wanquanpingfangshu(num: int) -> int
 
-    yiyuanerci(float1: float, float2: float, float3: float)
+    yiyuanerci(float1: float, float2: float, float3: float) -> tuple
 
 FILE
     d:\chay\project\all-in-one\src\all-in-one_chaylichenyi\module\calculator.py
 
 
+
 Help on module erfenchazhao_py:
 
 NAME
     erfenchazhao_py
 
 DESCRIPTION
     # -*- coding:UTF-8 -*-
```

### Comparing `all_in_one_chay-2.4.7/src/All_in_one_chay.egg-info/SOURCES.txt` & `all_in_one_chay-2.4.8/src/All_in_one_chay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

