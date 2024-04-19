# Comparing `tmp/gd_excelexporter-2.1.5.tar.gz` & `tmp/gd_excelexporter-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gd_excelexporter-2.1.5.tar", max compression
+gzip compressed data, was "gd_excelexporter-3.0.0a1.tar", max compression
```

## Comparing `gd_excelexporter-2.1.5.tar` & `gd_excelexporter-3.0.0a1.tar`

### file list

```diff
@@ -1,33 +1,53 @@
--rw-r--r--   0        0        0     1069 2023-10-18 15:10:32.882454 gd_excelexporter-2.1.5/LICENSE
--rw-r--r--   0        0        0    10174 2023-10-18 15:10:32.882454 gd_excelexporter-2.1.5/README.md
--rw-r--r--   0        0        0     1441 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/pyproject.toml
--rw-r--r--   0        0        0       35 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/babel/__init__.py
--rw-r--r--   0        0        0     3338 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/babel/csharp.py
--rw-r--r--   0        0        0     8496 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/babel/godot.py
--rw-r--r--   0        0        0     4237 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/babel/json.py
--rw-r--r--   0        0        0     4063 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/cli.py
--rw-r--r--   0        0        0     1378 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/config.py
--rw-r--r--   0        0        0     9635 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/engine.py
--rw-r--r--   0        0        0     4561 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/generator.py
--rw-r--r--   0        0        0      341 2023-10-18 15:10:32.906454 gd_excelexporter-2.1.5/src/excelexporter/generators/__init__.py
--rw-r--r--   0        0        0     1965 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds1/__init__.py
--rw-r--r--   0        0        0      624 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds1/data_template.gd
--rw-r--r--   0        0        0      144 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds1/setting_template.gd
--rw-r--r--   0        0        0     1966 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds2/__init__.py
--rw-r--r--   0        0        0      624 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds2/data_template.gd
--rw-r--r--   0        0        0      144 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/gds2/setting_template.gd
--rw-r--r--   0        0        0     1993 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/json/__init__.py
--rw-r--r--   0        0        0     1986 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/json2/__init__.py
--rw-r--r--   0        0        0     2734 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/generators/resource/__init__.py
--rw-r--r--   0        0        0      513 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/logger.py
--rw-r--r--   0        0        0     1335 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/sheetdata.py
--rw-r--r--   0        0        0      200 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/babel.cfg
--rw-r--r--   0        0        0       16 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/gen_all.bat
--rw-r--r--   0        0        0       16 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/gen_pot.bat
--rw-r--r--   0        0        0      144 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/reg/删除右键导出.reg
--rw-r--r--   0        0        0      266 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/reg/删除右键导出所有.reg
--rw-r--r--   0        0        0      178 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/reg/添加右键导出.reg
--rw-r--r--   0        0        0      354 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/reg/添加右键导出所有.reg
--rw-r--r--   0        0        0    18035 2023-10-18 15:10:32.910454 gd_excelexporter-2.1.5/src/excelexporter/template/sample/示例.xlsx
--rw-r--r--   0        0        0    10974 1970-01-01 00:00:00.000000 gd_excelexporter-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-19 01:40:07.975489 gd_excelexporter-3.0.0a1/LICENSE
+-rw-r--r--   0        0        0    11006 2024-04-19 01:40:07.975489 gd_excelexporter-3.0.0a1/README.md
+-rw-r--r--   0        0        0     2696 2024-04-19 01:40:27.891445 gd_excelexporter-3.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/__init__.py
+-rw-r--r--   0        0        0     3338 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/csharp.py
+-rw-r--r--   0        0        0     8496 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/godot.py
+-rw-r--r--   0        0        0     4237 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/json.py
+-rw-r--r--   0        0        0     4427 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/cli.py
+-rw-r--r--   0        0        0     2286 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/config.py
+-rw-r--r--   0        0        0      136 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/engine.py
+-rw-r--r--   0        0        0     1578 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/generator.py
+-rw-r--r--   0        0        0     1078 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/models.py
+-rw-r--r--   0        0        0     2421 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/type_define.py
+-rw-r--r--   0        0        0      136 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/__init__.py
+-rw-r--r--   0        0        0     1042 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlrd_engine.py
+-rw-r--r--   0        0        0     2107 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/engines/xlwings_engine.py
+-rw-r--r--   0        0        0      547 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/exceptions.py
+-rw-r--r--   0        0        0      433 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/__init__.py
+-rw-r--r--   0        0        0     2233 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/data_template.gd
+-rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/setting_template.gd
+-rw-r--r--   0        0        0     2234 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/data_template.gd
+-rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/setting_template.gd
+-rw-r--r--   0        0        0     2280 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json1/__init__.py
+-rw-r--r--   0        0        0     2295 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json2/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/resource/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/logger.py
+-rw-r--r--   0        0        0      278 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/babel.cfg
+-rw-r--r--   0        0        0       16 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/gen_all.bat
+-rw-r--r--   0        0        0       16 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/gen_pot.bat
+-rw-r--r--   0        0        0      144 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/删除右键导出.reg
+-rw-r--r--   0        0        0      266 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/删除右键导出所有.reg
+-rw-r--r--   0        0        0      178 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/添加右键导出.reg
+-rw-r--r--   0        0        0      354 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/reg/添加右键导出所有.reg
+-rw-r--r--   0        0        0    16102 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/template/sample/示例.xlsx
+-rw-r--r--   0        0        0      700 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/__init__.py
+-rw-r--r--   0        0        0      370 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array.py
+-rw-r--r--   0        0        0      448 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array_bool.py
+-rw-r--r--   0        0        0      374 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/array_str.py
+-rw-r--r--   0        0        0      591 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/bool.py
+-rw-r--r--   0        0        0      371 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/dict.py
+-rw-r--r--   0        0        0      307 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/float.py
+-rw-r--r--   0        0        0      351 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/function.py
+-rw-r--r--   0        0        0      310 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/int.py
+-rw-r--r--   0        0        0      346 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/string.py
+-rw-r--r--   0        0        0      443 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_array_str.py
+-rw-r--r--   0        0        0      489 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_dict.py
+-rw-r--r--   0        0        0      460 2024-04-19 01:40:07.999489 gd_excelexporter-3.0.0a1/src/gd_excelexporter/type_defines/tr_string.py
+-rw-r--r--   0        0        0    11970 1970-01-01 00:00:00.000000 gd_excelexporter-3.0.0a1/PKG-INFO
```

### Comparing `gd_excelexporter-2.1.5/LICENSE` & `gd_excelexporter-3.0.0a1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 kaluluosi111
+Copyright (c) 2023 CaroLose
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gd_excelexporter-2.1.5/README.md` & `gd_excelexporter-3.0.0a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# GDExcelExporter 2.1
+# GD-ExcelExporter
+
+[![Build](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/build.yml/badge.svg)](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/build.yml)
+![Code Coverage](https://img.shields.io/badge/Code%20Coverage-92%25-success?style=flat)
+[![Test](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/test.yml/badge.svg)](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/test.yml)
 
 [English](README.en.md)
 
 GDExcelExpoter 是为Godot设计的Excel表格导出数据资源的工具。
 它内置了好几种数据表导出和读取方案（导出器），支持Godot3.x、Godot4.x。
 
 下面我们用`ee`代指`GDExcelExporter`。
 
 [在线文档](https://kaluluosi.github.io/GDExcelExporter/)
 
 ## 更新日志
 
-2.1版本
-
-> **Warning** 
-> 2.0 开始导出格式已经不兼容1.0，如果你的项目里已经大量使用1.0导出的数据表，可能会导致你要修改代码的地方非常多。
-
-1. 重构导出器
-2. 通过`entry_points`支持导出器插件，现在可以开发自己的导出器插件
-3. 多语言支持，集成了pybabel多语言方案，直接支持配置表、gd脚本、tscn、tres整个godot项目的多语言文本提取。以后出一个文档单独讲解。
-4. 单元测试用例补充
-5. ~~悲报：因为pyinstaller不支持 `entry_points` 因此2.1版本之后不提供独立`exe`了。~~ 2.1.4开始重新提供'ee.exe'
+**3.0版本**
+1. 重构框架，类型转换器、导出器、引擎全部面向接口编程，而且都`entry_points`插件化，以后可以自己写插件自定义。
+2. 默认采用xlrd读取excel，以此支持linux、macos、windows全平台的导出，而且速度更快。用户仍然可以选择用xlwings作为excel读取库（由xlrd其实已经不需要了）。
+3. 修改多语言字段类型，原本是`#`开头，比如`#string`，现在改为`tr_string`。
+4. 包改名为`gd_excelexporter`，因为之前包名`gd-excelexporter`和`src\excelexporter`不一致，整出很多麻烦，现在统一了。因此你需要卸载原来的`gd-excelexporter`包，重新安装这个包。
+5. 其他的没有任何改变，兼容原来的`settings`项目目录。但是安全起见建议重新`ee init`一个目录，然后将`data`下的表迁移过去重新导出。
 
 ## 为什么需要这个工具？
 
 Unreal引擎中有一个工具叫做DataTable，它的作用是充当一个小型的数据库给游戏设计人员编辑配置数值数据。
 
 打个比方，我们游戏中有道具系统，而道具整个对象一旦属性字段建模好，那么就可以通过配置这些属性定义出各种各样的道具。
 
@@ -42,34 +42,31 @@
 1. 就不用手写json
 2. 也不用嵌入sqlite
 3. 由于数据是以项目的文件资源存在，因此也是版本管理工具友好的
 4. 也因为数据是文件资源，因此热更新友好
 5. 你不需要学习别的工具去编辑维护数据，会用excel就可以，你可以用上你excel中所有的技巧去编辑数据
 
 
-## 快速开始
+## 快速上手
 
 ### 系统要求
 Python:^3.8.1
 
 Platform: Windows(xlwings只支持Windows)
 
 Godot版本:^3.4
 
 ### 安装
 通过pip （建议）
 ```
-pip install gd-excelexporter
+pip install gd-gd_excelexporter
 ```
 
 或者直接去右边release里下载已经打包好的可执行文件（ee.exe，你需要将这个exe加到环境变量）。
 
-> **Note** 
-> 2.1.4 版本开始exe的打包问题已经解决，后续版本会继续提供`ee.exe`命令行程序。
-
 ### 创建配置表项目
 
 打开你的Godot游戏项目，项目根目录下右键打开命令行（此处打开powershell）
 ![图 1](docs/images/b0e636c8ece81e8d9a81f663e91db7872e8cbd06f97dbd6edae64f15c3d1173b.gif)  
 ![图 2](docs/images/939a62bfbaec7d9c2e7d2c75715d3ab53624cb1ecd4006ce7ae3163fbda721fc.gif)  
 ![图 3](docs/images/69e876afa54e19f5c9fbd50cc274a1a583a9e4233fa0afcfd6407a6ea683b21f.png)  
 ![图 4](docs/images/7658090be99a6b34b8ca397a76eb4a7462adcd5de98fa21f27e944c024123a95.png)  
@@ -248,7 +245,13 @@
 由于每次导表都要到`settings`目录下操作太麻烦了，因此特地开发一个`Godot插件`，让我们可以直接在`Godot编辑器`中点击一个按钮进行导表。
 
 [Godot插件-GDExcelExporter-Plugin](https://github.com/kaluluosi/GDEexcelExporer-Plugin)
 
 ## 最后
 希望这个工具能够给一些独立游戏人或者业余自娱自乐的人一些帮助。
 如果你用上了我的工具，有什么问题最好直接提issue。
+
+如果你在你的独立游戏项目中使用了我的工具，希望你能够在游戏结尾员工名单或者开源证书页面中特别鸣谢加上我的名字，让我也占个光，谢谢。
+
+## 联系方式
+
+![Snipaste_2024-04-19_06-50-25](/assets/Snipaste_2024-04-19_06-50-25_icwxbsqi8.png)
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/babel/csharp.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/csharp.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/babel/godot.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/godot.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/babel/json.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/babel/json.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/cli.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,132 @@
 import shutil
 import click
 import logging
 import os
 import pkg_resources
+import gd_excelexporter
+
+from gd_excelexporter.core.generator import Generator
+from gd_excelexporter.core.engine import Engine
 
 # from babel import *  # noqa
 from babel.messages.frontend import CommandLineInterface
-from excelexporter.config import Configuration
-from excelexporter.engine import Engine, discover_generator
+from gd_excelexporter.config import Configuration
+
 
 logger = logging.getLogger(__name__)
 
 
 @click.group
-def main():
+def cli():
     """
     ===============================
-    Excel表导出工具
+
+    Godot Excel表导出工具
+
+    联系
+    mail: kaluluosi111@qq.com
+    QQ群: 118258918
+
     ===============================
     """
     pass
 
 
-@main.command
+@cli.command
 def init():
     """
     生成默认配置表项目
     """
     config = Configuration()
 
+    # 询问使用的excel引擎
+
     # 询问数据表存放目录
-    datatable_dir = click.prompt("输出数据表目录名", default="settings", show_default=True)
+    datatable_dir = click.prompt(
+        "输出数据表目录名", default="settings", show_default=True
+    )
     if os.path.exists(datatable_dir) and os.listdir(datatable_dir):
         click.echo(f"{datatable_dir} 已经存在并且非空!")
         return
 
     os.mkdir(datatable_dir)
+    cwd_backup = os.getcwd()
     os.chdir(datatable_dir)
 
-    input_dir = click.prompt("输入存放excel表格目录名称", default=config.input, show_default=True)
-    output_dir = click.prompt("输入存放导出文件目录名称", default=config.output, show_default=True)
+    engine = click.prompt(
+        "使用哪个内置excel引擎？",
+        type=click.Choice(list(Engine.register_engines().names)),
+        default="xlrd",
+    )
+
+    input_dir = click.prompt(
+        "输入存放excel表格目录名称", default=config.input, show_default=True
+    )
+    output_dir = click.prompt(
+        "输入存放导出文件目录名称", default=config.output, show_default=True
+    )
 
-    template = pkg_resources.resource_filename(__package__, "template")
+    template = pkg_resources.resource_filename(__package__, "template")  # type: ignore
 
     generator = click.prompt(
         "使用哪个内置导出器？",
-        type=click.Choice(list(discover_generator().names)),
+        type=click.Choice(list(Generator.register_generators().names)),
         default="GDS2.0",
     )
 
+    config.engine = engine
     config.input = input_dir
     config.output = output_dir
 
     os.mkdir(input_dir)
     os.mkdir(output_dir)
     os.mkdir("lang")  # 创建多语言目录
     config.custom_generator = generator
     config.save()
 
     shutil.copytree(template, os.curdir, dirs_exist_ok=True)
+
+    os.chdir(cwd_backup)
     click.echo("配置表项目生成完毕，后续你可以通过修改export.toml调整配置。")
 
 
-@main.command(name="list")
+@cli.command()
+def version():
+    """
+    打印ee版本号
+    """
+    print(gd_excelexporter.__version__)  # noqa
+
+
+@cli.command(name="list")
 def _list():
     """
-    列出支持的导出器插件
+    列出支持的引擎和导出器
     """
-    generators = discover_generator()
-    if generators.names:
-        for gen in generators.names:
-            print(gen)
+
+    print("Eingine:")
+    engines = Engine.register_engines()
+    for engine in engines.names:
+        print("-", engine)
+
+    print("")
+    print("Generator:")
+    generators = Generator.register_generators()
+    for gen in generators.names:
+        print("-", gen)
 
 
-@main.command
+@cli.command
 def add_context_menu():
     """
     添加上下文菜单（通过注册表）
     """
-    dir = pkg_resources.resource_filename(__package__, "template/reg")
+
+    dir = pkg_resources.resource_filename(__package__, "template/reg")  # type: ignore
     os.system(f"start {dir}")
 
 
 def _find_config():
     if not os.path.exists("export.toml"):
         logger.error("当前目录下没有export.toml配置文件")
         logger.error("尝试往上层找")
@@ -90,71 +134,51 @@
         if not os.path.exists(upper_path):
             logger.error("完全不存在export.toml,终止导表")
             raise FileNotFoundError("完全不存在export.toml,终止导表")
         else:
             os.chdir(os.pardir)
 
 
-@main.command
+@cli.command
 @click.option("--cwd", default=".", help="工作目录，执行命令所在的目录")
 def gen_all(cwd):
     """
     导出所有表
     """
     os.chdir(cwd)
     _find_config()
 
     config = Configuration.load()
 
-    with Engine(config) as engine:
-        engine.gen_all()
+    engine = Engine.create_engine(config.engine, config)
+    engine.gen_all()
 
 
-@main.command()
+@cli.command
 @click.argument("file", type=click.Path(True))
 def gen_one(file: str):
     """
     打开并导出整张excel表
     """
     abs_filepath = os.path.abspath(file)
     _find_config()
 
     config = Configuration.load()
-    with Engine(config) as engine:
-        engine.gen_one(abs_filepath)
+    engine = Engine.create_engine(config.engine, config)
+    engine.gen_one(abs_filepath)
 
 
-@main.command
+@cli.command
 @click.option("--cwd", default=".", help="工作目录，执行命令所在的目录")
 def extract(cwd):
     """
     导出多语言表 gd,供 babel生成语言表用
     """
     os.chdir(cwd)
     _find_config()
     config = Configuration.load()
-    with Engine(config) as engine:
-        engine.extract_pot()
-
-    babel_keywords = config.localization.babel_keywords
-    pot_file = config.localization.pot_file
-
-    keyword_args = [f"-k {kw} " for kw in babel_keywords]
-
-    cfg_file = os.path.abspath("babel.cfg")
-
-    CommandLineInterface().run(  # noqa
-        [
-            "pybabel",
-            "extract",
-            "-F",
-            cfg_file,
-            *keyword_args,
-            "-o",
-            pot_file,
-            config.project_root,
-        ]
-    )
+    engine = Engine.create_engine(config.engine, config)
+    engine.extract_pot()
 
 
 if __name__ == "__main__":
-    main()
+    cli()
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/engine.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/core/engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,253 +1,262 @@
+"""
+author:        kaluluosi111 <kaluluosi@gmail.com>
+date:          2024-04-15 14:55:03
+Copyright © Kaluluosi All rights reserved
+"""
+
+import abc
 import glob
+import logging
 import os
 import sys
-import xlwings as xw
-import logging
-from win32com import client
-from excelexporter.config import Configuration
-from excelexporter.generator import Converter, Generator, CompletedHook, Variant  # noqa
-from excelexporter.sheetdata import SheetData, TypeDefine
-from typing import Dict, Optional
+from typing import Type
 
+from gd_excelexporter.core.models import (
+    Table,
+    TableMap,
+    RawTableMap,
+)
+from gd_excelexporter.core.models import Variant
+from gd_excelexporter.exceptions import IllegalFile
+from gd_excelexporter.config import Configuration
+from gd_excelexporter.core.generator import Generator
+from gd_excelexporter.core.type_define import TrTypeDefine, TypeDefine
+
+from babel.messages.frontend import CommandLineInterface
 
 if sys.version_info < (3, 10):
     from importlib_metadata import entry_points
 else:
     from importlib.metadata import entry_points
 
-# 导表工具引擎
 
 logger = logging.getLogger(__name__)
 
 
-class IllegalFile(Exception):
-    def __init__(self, filename: str, *args: object) -> None:
-        super().__init__(f"{filename} 不是配置表目录下的配置", *args)
+class Engine(abc.ABC):
+    # 配置表抽取出来的多语言文本
+    LANG_FILE = "lang/.settings"
 
+    def __init__(self, config: Configuration) -> None:
+        self.config = config
 
-class IllegalGenerator(Exception):
-    def __init__(self, name: str, *args: object) -> None:
-        super().__init__(name, *args)
+    def _excel2tablemap(self, excel_filename: str) -> TableMap:
+        """
+        将excel转成table map。
 
+        Args:
+            excel_file (str): excel文件路径
 
-def discover_generator():
-    generators = entry_points(group="excelexporter.generator")
-    return generators
+        Returns:
+            dict[str, Table]: 返回sheet名->Table的字典
+        """
+        rawtablemap = self._excel2rawtablemap(excel_filename)
 
+        tablemap: TableMap = {}
 
-class Engine(xw.App):
-    COM_EXCEL = "Excel.Application"
-    COM_WPS = "ket.Application"
+        for sheet_name, rawtable in rawtablemap.items():
+            # 如果sheet名以ignore_sheet_mark开头就跳过
+            # NOTE: 在这里做sheet的忽略
+            if sheet_name.startswith(self.config.ignore_sheet_mark):
+                continue
+
+            table: Table = {}
+            # 先遍历构抽取头三行字段定义define
+            field_types = rawtable[0]
+            field_names = rawtable[2]
+
+            for row in rawtable[3:]:
+                id_type: TypeDefine = TypeDefine.from_str(field_types[0])
+                id_value = id_type.convert(row[0])
+
+                row_data = {}
+                for index, value in enumerate(row):
+                    field_name: str = field_names[index]
+
+                    # field_name 可能是空字符或者None，这时跳过
+                    if not field_name:
+                        continue
+
+                    # 如果字段名以ignore_field_mark开头就跳过
+                    # NOTE: 在这里做字段的忽略
+                    if field_name.startswith(self.config.ignore_field_mark):
+                        continue
+
+                    type_define: TypeDefine = TypeDefine.from_str(field_types[index])
+                    variant: Variant = Variant(
+                        type_define=type_define,
+                        field_name=field_name,
+                        value=type_define.convert(value),
+                        id=id_value,
+                    )
+                    row_data[field_name] = variant
 
-    def __init__(self, config: Configuration) -> None:
-        super().__init__(visible=False)
-        self.config = config
-        self.generator: Optional[Generator] = None
-        self.completed_hook: Optional[CompletedHook] = None
-        self.extension: str | None = None
-
-        self.localized_strs = set()
-        self.cvt = Converter()
-
-        self.setup_com()
-        self.init_generator()
-
-    def setup_com(self):
-        try:
-            client.DispatchEx("Excel.Application")
-        except Exception:
-            logger.info("系统中没有安装Excel，尝试改为WPS")
-            try:
-                _wps = client.DispatchEx("ket.Application")
-                _xl = xw._xlwindows.COMRetryObjectWrapper(_wps)
-                impl = xw._xlwindows.App(visible=False, add_book=False, xl=_xl)
-                self.impl = impl
-            except Exception:
-                logger.info("系统中没有安装WPS")
+                table[id_value] = row_data
 
-    def init_generator(self):
-        generator = None
-        completed_hook = None
-        extension = None
-
-        # 如果有自定义导出器就优先用自定义导出器
-        if self.config.custom_generator.endswith(".py"):
-            with open(self.config.custom_generator) as f:
-                code = f.read()
-                exec(code)
-                self.generator = generator
-                self.completed_hook = completed_hook
-                self.extension = extension
-
-                if (generator and completed_hook and extension) is False:
-                    raise IllegalGenerator(
-                        self.config.custom_generator,
-                        "自定义导出器不完整，generator、completed_hook、extension存在没定义。",
-                    )
+            tablemap[sheet_name] = table
 
-                logger.info(f"使用 {self.config.custom_generator} 自定义导出器")
-        else:
-            # 找出插件
-            generators = discover_generator()
+        return tablemap
+
+    @abc.abstractmethod
+    def _excel2rawtablemap(self, excel_filename: str) -> RawTableMap:
+        """
+        将sheet转换成原始字典数据
+
+        本方法需要具体的Engine实现去实现
+
+        以行号为key，行数组list为value。
+        """
+        pass
+
+    def _generate(self, excel_filename: str):
+        # excel文件绝对路径
+        excel_abs_path: str = os.path.abspath(excel_filename)
+
+        # 输入目录的绝对路径
+        abs_input_path = os.path.abspath(self.config.input)
+        # 输出目录的绝对路径
+        abs_output_path = os.path.abspath(self.config.output)
 
-            if self.config.custom_generator in generators.names:
-                module = generators[self.config.custom_generator].load()
-                logger.info(
-                    f"使用插件导出器 {self.config.custom_generator} :{module.__name__}"
-                )  # noqa
-            else:
-                raise IllegalGenerator(self.config.custom_generator, generators.names)
-
-            self.generator = getattr(module, "generator")
-            self.completed_hook = getattr(module, "completed_hook")
-            self.extension = getattr(module, "extension")
-
-    def _gen(self, excel_file: str):
-        wb_abs_path: str = os.path.abspath(excel_file)
-        abs_input_path: str = os.path.abspath(self.config.input)
-        abs_output_path: str = os.path.abspath(self.config.output)
-        wb_abs_path_without_ext: str = os.path.splitext(wb_abs_path)[0]
+        # excel文件路径（无扩展名）
+        excel_abs_path_without_ext: str = os.path.splitext(excel_abs_path)[0]
 
-        if self.generator is None:
+        generator = Generator.get_generator(self.config.custom_generator)
+
+        if generator is None:
             raise RuntimeError("没有加载任何导出器！")
 
-        if not wb_abs_path.startswith(abs_input_path):
-            raise IllegalFile(wb_abs_path, abs_input_path)
+        if not excel_abs_path.startswith(abs_input_path):
+            # 如果输入目录不是输入文件所在目录，则抛出异常
+            raise IllegalFile(excel_abs_path, abs_input_path)
 
-        sheet_datas = self._excel2dict(wb_abs_path)
+        tablemap = self._excel2tablemap(excel_abs_path)
 
-        for sheet_name, sheetdata in sheet_datas.items():
+        for sheet_name, table in tablemap.items():
             try:
+                # 处理sheet名与导出文件名
                 if "-" in sheet_name:
                     org_name, rename = sheet_name.split("-")
                 else:
                     org_name, rename = sheet_name, None
 
                 relative_path = os.path.join(
-                    wb_abs_path_without_ext.replace(abs_input_path, ""),
+                    excel_abs_path_without_ext.replace(abs_input_path, ""),
                     rename or org_name,
                 )
                 output = abs_output_path + relative_path
 
                 output_dirname = os.path.dirname(output)
                 # 保持输出的文件目录层级结构与输入一致
                 if not os.path.exists(output_dirname):
                     os.makedirs(output_dirname)
 
-                code = self.generator(sheetdata, self.config)
+                code = generator.generate(table, self.config)
 
-                # code = "# 本文件由代码生成，不要手动修改\n"+code
-                output = f"{output}.{self.extension}"
+                output = f"{output}.{generator.__extension__}"
                 with open(output, "w", encoding="utf-8", newline="\n") as f:
                     f.write(code)
-                    logger.info(f"导出：{wb_abs_path}:{sheet_name} => {output}")
+                    logger.info(f"导出：{excel_abs_path}:{sheet_name} => {output}")
             except Exception:
                 logger.error(f"{sheet_name} 导出失败", exc_info=True)
 
-    def _excel2dict(self, wb_file: str) -> Dict[str, SheetData]:
-        """
-        workbook解析加工成字典
-        """
-        with self.books.open(wb_file) as book:
-            ignore_sheet_mark = self.config.ignore_sheet_mark
-            # 过滤掉打了忽略标志的sheet
-            sheets = filter(
-                lambda sheet: not sheet.name.startswith(ignore_sheet_mark), book.sheets
-            )
-
-            wb_data = {}
-
-            # 先讲sheet转sheet_data
-            for sheet in sheets:
-                sheet_data = SheetData()
-                row_values = sheet.range("A1").expand().raw_value
-
-                sheet_data.define.type = list(row_values[0])
-                sheet_data.define.desc = list(row_values[1])
-                sheet_data.define.name = list(row_values[2])
-
-                sheet_data.table = list([list(row) for row in row_values[3:]])
-                # 找出所有被打了忽略标记的字段
-                for col, field in enumerate(sheet_data.define.name):
-                    # 跳过没命令的字段
-
-                    if field is None or field.startswith(
-                        self.config.ignore_field_mark
-                    ):  # noqa
-                        del sheet_data.define.type[col]
-                        del sheet_data.define.desc[col]
-                        del sheet_data.define.name[col]
-                        for row in sheet_data.table:
-                            del row[col]
-
-                wb_data[sheet.name] = sheet_data
-
-            cvt = Converter()
-            for sheet_name, sheet_data in wb_data.items():
-                field_names = sheet_data.define.name
-                field_types = sheet_data.define.type
-                table = {}
-
-                for row in sheet_data.table:
-                    id_type = TypeDefine.from_str(field_types[0])
-                    id_name = field_names[0]
-                    id_value = row[0]
-                    id = cvt(id_value, id_type, id_name, id_value)
-
-                    row_data = {}
-
-                    for index, value in enumerate(row):
-                        field_name: str = field_names[index]
-                        field_type = TypeDefine.from_str(field_types[index])
-                        variant: Variant = cvt(id.value, field_type, field_name, value)
-                        row_data[field_name] = variant
-                        self.localized_strs = self.localized_strs.union(
-                            variant.local_strs()
-                        )
-
-                    table[id.value] = row_data
-                wb_data[sheet_name] = table
-
-            return wb_data
-
-    def save_lang_file(self):
-        with open("language.gd", "w", encoding="utf-8", newline="\n") as f:
+    def _save_lang_file(self, filename: str):
+        with open(filename, "w", encoding="utf-8", newline="\n") as f:
+            f.write("## 这是用于抽取代码中多语言的辅助文件，用来辅助生成POT用的\n")
             f.write("func localization():\n")
             lines = []
-            for txt in self.localized_strs:
-                lines.append(f"  tr('{txt}')\n")
+            for txt in TrTypeDefine.__tr_strs__:
+                if txt:
+                    lines.append(f"  tr('{txt}')\n")
+                    # logger.info(f"抽出 {txt}")
+
             f.writelines(lines)
 
-    def gen_one(self, filename: str):
-        self._gen(filename)
-        if self.completed_hook:
-            self.completed_hook(self.config)
+    def gen_one(self, excel_filename: str):
+        self._generate(excel_filename)
+        generator = Generator.get_generator(self.config.custom_generator)
+        generator.completed_hook(self.config)
 
     def gen_all(self):
-        abs_input = os.path.abspath(self.config.input)
+        abs_input_path = os.path.abspath(self.config.input)
         exts = [".xlsx", ".xls"]
         for ext in exts:
-            full_paths = glob.glob(f"{abs_input}/**/*{ext}", recursive=True)
+            full_paths = glob.glob(f"{abs_input_path}/**/*{ext}", recursive=True)
             for full_path in full_paths:
                 filename = os.path.basename(full_path)
                 if filename.startswith("~$"):
                     logger.warning(f"{filename} 不是配置表，跳过！")
                     continue
-                self._gen(full_path)
+                self._generate(full_path)
 
-        if self.completed_hook:
-            self.completed_hook(self.config)
+        generator = Generator.get_generator(self.config.custom_generator)
+        generator.completed_hook(self.config)
 
     def extract_pot(self):
+        """
+        将配置表中的多语言字符串抽取出来，生成gd文件，用于提取。
+
+        配置表中的多语言字段要能够供Godot babel或者Babel提取需要先抽取到一个gd脚本。
+        这个函数就是用来生成这个gd脚本。当生成POT文件后就删除。
+
+        通过`with`来包裹让其使用完后自动清理。
+
+        ```
+        with engine.extract_lang():
+            ...
+        ```
+        """
         abs_input = os.path.abspath(self.config.input)
         exts = [".xlsx", ".xls"]
         for ext in exts:
             full_paths = glob.glob(f"{abs_input}/**/*{ext}", recursive=True)
             for full_path in full_paths:
                 filename = os.path.basename(full_path)
                 if filename.startswith("~$"):
                     logger.warning(f"{filename} 不是配置表，跳过！")
                     continue
-                self._excel2dict(full_path)  # 直接读所有表，不做转换抽取翻译字符
-                logger.info(f"导出语言表: {full_path}")
-        self.save_lang_file()
+                self._excel2tablemap(full_path)  # 直接读所有表，抽取翻译字符
+                logger.info(f"抽出多语言: {full_path}")
+        self._save_lang_file(self.LANG_FILE)
+        logger.info(f"生成配置语言辅助文件(跳过空字符): {self.LANG_FILE}")
+
+        babel_keywords = self.config.localization.babel_keywords
+        pot_file = self.config.localization.pot_file
+
+        keyword_args = [f"-k {kw} " for kw in babel_keywords]
+
+        cfg_file = os.path.abspath("babel.cfg")
+
+        CommandLineInterface().run(  # noqa
+            [
+                "pybabel",
+                "extract",
+                "-F",
+                cfg_file,
+                *keyword_args,
+                "-o",
+                pot_file,
+                self.config.project_root,
+            ]
+        )
+
+        logger.info("生成POT文件: %s" % pot_file)
+
+        os.remove(self.LANG_FILE)
+
+    @staticmethod
+    def register_engines():
+        engines = entry_points(group="gd_excelexporter.engine")
+        return engines
+
+    @staticmethod
+    def get_engine_cls(name: str) -> Type["Engine"]:
+        engines = entry_points(group="gd_excelexporter.engine")
+        if name in engines.names:
+            engine_cls = engines[name].load()
+            return engine_cls  # type: ignore
+        else:
+            raise RuntimeError(f"没有找到名为 {name} 的引擎！")
+
+    @classmethod
+    def create_engine(cls, name: str, config: Configuration):
+        return cls.get_engine_cls(name)(config)
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/gds1/__init__.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 import glob
 import os
 import logging
 import jinja2
 import pkg_resources
-from excelexporter.config import Configuration
-from excelexporter.sheetdata import SheetData
-from excelexporter.generator import Variant
-from excelexporter.generator import Type
+
+from gd_excelexporter.core.generator import Generator, Table
+from gd_excelexporter.config import Configuration
+from gd_excelexporter.core.models import Variant
+from gd_excelexporter.type_defines import Function
 
 # jinja2 docs: http://doc.yonyoucloud.com/doc/jinja2-docs-cn/templates.html#id2
 
 logger = logging.getLogger(__name__)
 
-# 导出格式
-extension = "gd"
-
-loader = jinja2.FileSystemLoader(
-    pkg_resources.resource_filename(__package__, ""))
-env = jinja2.Environment(autoescape=False, loader=loader)
-
 
 def converter(var: Variant):
     type_define = var.type_define
-    if type_define.type_name == Type.STRING:
+    if isinstance(var.value, str):
         value = var.value.replace("\n", "\\n")
         return f"'{value}'"
-
-    if type_define.type_name == Type.FUNCTION:
-        func_name = f"{var.field_name}_{var.id}"
+    if isinstance(type_define, Function):
+        func_name = f"{var.type_define.type_name}_{var.field_name}_{var.id}"
         return f"funcref(self,'{func_name}')"
-
     return var.value
 
 
-env.filters["cvt"] = converter
-
-
-def generator(sheetdata: SheetData, config: Configuration):
-    # 表格数据脚本模板
-    template = env.get_template("data_template.gd")
-    code = template.render(sheetdata=sheetdata)
-    return code
-
-
-def completed_hook(config: Configuration):
-    output = config.output
-    settings_file_path = os.path.join(output, "settings.gd")
-    project_root = config.project_root
-
-    lines = []
-
-    for path in glob.glob(f"{output}/**/*.{extension}", recursive=True):
-        if path == settings_file_path:
-            continue  # 跳过 settings.gd
-        basename = os.path.basename(path)
-        setting_name = os.path.splitext(basename)[0]
-        relpath = os.path.relpath(path, project_root).replace("\\", "/")
-        lines.append(f"var {setting_name} = load('res://{relpath}').new()")
-
-    template = env.get_template("setting_template.gd")
-    code = template.render(lines=lines)
-
-    with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(code)
-        logger.info("创建setting.gd")
+class GDS1Generator(Generator):
+    # 导出格式
+    __extension__ = "gd"
+
+    loader = jinja2.FileSystemLoader(
+        pkg_resources.resource_filename(__package__, "")  # type: ignore
+    )
+    env = jinja2.Environment(autoescape=False, loader=loader)
+    env.filters["cvt"] = converter
+
+    @classmethod
+    def generate(cls, table: Table, config: Configuration):
+        # 表格数据脚本模板
+        template = cls.env.get_template("data_template.gd")
+        code = template.render(table=table)
+        return code
+
+    @classmethod
+    def completed_hook(cls, config: Configuration):
+        output = config.output
+        settings_file_path = os.path.join(output, "settings.gd")
+        project_root = config.project_root
+
+        lines = []
+
+        for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
+            if path == settings_file_path:
+                continue  # 跳过 settings.gd
+            basename = os.path.basename(path)
+            setting_name = os.path.splitext(basename)[0]
+            relpath = os.path.relpath(path, project_root).replace("\\", "/")
+            lines.append(f"var {setting_name} = load('res://{relpath}').new()")
+
+        template = cls.env.get_template("setting_template.gd")
+        code = template.render(lines=lines)
+
+        with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(code)
+            logger.info(f"创建：{settings_file_path}")
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/gds1/data_template.gd` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds1/data_template.gd`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 var True = true
 var False = false
 var None = null
 
 var data = \
 {
-{% for id,row in sheetdata.items()-%}
+{% for id,row in table.items()-%}
     {{id}}:{% raw %}{{% endraw %}{% for field,value in row.items() %} "{{field}}":{{value|cvt|safe}}, {% endfor %}{% raw %}}{% endraw %},
 {% endfor %}
 }
 
-{% for id,row in sheetdata.items()-%}
+{% for id,row in table.items()-%}
     {% for field,value in row.items() -%} 
 
 {% if value.type_define.type_name == "function" %}
 func {{value.field_name}}_{{id}}{{value.type_define.params}}:
     {% if value.value -%}
     {{value.value}}
     {%- else -%}
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/gds2/__init__.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 import glob
 import os
 import logging
 import jinja2
 import pkg_resources
-from excelexporter.config import Configuration
-from excelexporter.sheetdata import SheetData
-from excelexporter.generator import Variant
-from excelexporter.generator import Type
+
+from gd_excelexporter.core.generator import Generator, Table
+from gd_excelexporter.config import Configuration
+from gd_excelexporter.core.models import Variant
+from gd_excelexporter.type_defines import Function
 
 # jinja2 docs: http://doc.yonyoucloud.com/doc/jinja2-docs-cn/templates.html#id2
 
 logger = logging.getLogger(__name__)
 
-# 导出格式
-extension = "gd"
-
-loader = jinja2.FileSystemLoader(
-    pkg_resources.resource_filename(__package__, ""))
-env = jinja2.Environment(autoescape=False, loader=loader)
-
 
 def converter(var: Variant):
     type_define = var.type_define
-    if type_define.type_name == Type.STRING:
+    if isinstance(var.value, str):
         value = var.value.replace("\n", "\\n")
         return f"'{value}'"
-
-    if type_define.type_name == Type.FUNCTION:
-        func_name = f"{var.field_name}_{var.id}"
+    if isinstance(type_define, Function):
+        func_name = f"{var.type_define.type_name}_{var.field_name}_{var.id}"
         return f"Callable(self,'{func_name}')"
-
     return var.value
 
 
-env.filters["cvt"] = converter
-
-
-def generator(sheetdata: SheetData, config: Configuration):
-    # 表格数据脚本模板
-    template = env.get_template("data_template.gd")
-    code = template.render(sheetdata=sheetdata)
-    return code
-
-
-def completed_hook(config: Configuration):
-    output = config.output
-    settings_file_path = os.path.join(output, "settings.gd")
-    project_root = config.project_root
-
-    lines = []
-
-    for path in glob.glob(f"{output}/**/*.{extension}", recursive=True):
-        if path == settings_file_path:
-            continue  # 跳过 settings.gd
-        basename = os.path.basename(path)
-        setting_name = os.path.splitext(basename)[0]
-        relpath = os.path.relpath(path, project_root).replace("\\", "/")
-        lines.append(f"var {setting_name} = load('res://{relpath}').new()")
-
-    template = env.get_template("setting_template.gd")
-    code = template.render(lines=lines)
-
-    with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(code)
-        logger.info("创建setting.gd")
+class GDS2Generator(Generator):
+    # 导出格式
+    __extension__ = "gd"
+
+    loader = jinja2.FileSystemLoader(
+        pkg_resources.resource_filename(__package__, "")  # type: ignore
+    )
+    env = jinja2.Environment(autoescape=False, loader=loader)
+    env.filters["cvt"] = converter
+
+    @classmethod
+    def generate(cls, table: Table, config: Configuration):
+        # 表格数据脚本模板
+        template = cls.env.get_template("data_template.gd")
+        code = template.render(table=table)
+        return code
+
+    @classmethod
+    def completed_hook(cls, config: Configuration):
+        output = config.output
+        settings_file_path = os.path.join(output, "settings.gd")
+        project_root = config.project_root
+
+        lines = []
+
+        for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
+            if path == settings_file_path:
+                continue  # 跳过 settings.gd
+            basename = os.path.basename(path)
+            setting_name = os.path.splitext(basename)[0]
+            relpath = os.path.relpath(path, project_root).replace("\\", "/")
+            lines.append(f"var {setting_name} = load('res://{relpath}').new()")
+
+        template = cls.env.get_template("setting_template.gd")
+        code = template.render(lines=lines)
+
+        with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(code)
+            logger.info(f"创建：{settings_file_path}")
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/gds2/data_template.gd` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/gds2/data_template.gd`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 var True = true
 var False = false
 var None = null
 
 
 var data = \
 {
-{% for id,row in sheetdata.items()-%}
+{% for id,row in table.items()-%}
     {{id}}:{% raw %}{{% endraw %}{% for field,value in row.items() %} "{{field}}":{{value|cvt|safe}}, {% endfor %}{% raw %}}{% endraw %},
 {% endfor %}
 }
 
-{% for id,row in sheetdata.items()-%}
+{% for id,row in table.items()-%}
     {% for field,value in row.items() -%} 
 {% if value.type_define.type_name == "function" %}
 func {{value.field_name}}_{{id}}{{value.type_define.params}}:
     {% if value.value -%}
     {{value.value}}
     {%- else -%}
     pass
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/json/__init__.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json1/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,78 @@
 import glob
 import json
 import os
 import logging
 import textwrap
-from excelexporter.config import Configuration
-from excelexporter.sheetdata import SheetData
+from gd_excelexporter.core.generator import Table, Generator
+from gd_excelexporter.config import Configuration
 
 
-# 导出格式
-extension = "json"
-
 logger = logging.getLogger(__name__)
 
 
-EE_DATATABLE_CLASS = """
-class_name EEDataTable
-extends Resource
-
-@export
-var data = {}
-"""
-
-
-def generator(sheetdata: SheetData, config: Configuration):
-    # 表格数据脚本模板
-
-    table = {}
-
-    for id, row in sheetdata.items():
-        row_data = {}
-
-        for field, var in row.items():
-            field_name: str = field
-            row_data[field_name] = var.value
-
-        table[id] = row_data
-
-    code = json.dumps(table, ensure_ascii=False, indent=2)
+class JSON1Generator(Generator):
+    # 导出格式
+    __extension__ = "json"
+
+    @classmethod
+    def generate(cls, table: Table, config: Configuration):
+        # 表格数据脚本模板
+
+        # 由于json不支持int做key，所以这里需要转换一下
+        new_table = {}
+        for id, row in table.items():
+            row_data = {}
+
+            for field, var in row.items():
+                field_name: str = field
+                row_data[field_name] = var.value
+
+            new_table[id] = row_data
+
+        code = json.dumps(new_table, ensure_ascii=False, indent=2)
+
+        return code
+
+    @classmethod
+    def completed_hook(cls, config: Configuration):
+        output = config.output
+        settings_file_path = os.path.join(output, "settings.gd")
+        project_root = config.project_root
+
+        lines = []
+
+        loader = textwrap.dedent("""
+        static func loader(path:String):
+            var file = File.new()
+            file.open(path,File.READ)
+            var txt = file.get_as_text()
+            var data = JSON.parse(txt)
+            file.close()
+            return data
+        """)
+
+        for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
+            if path == settings_file_path:
+                continue  # 跳过 settings.gd
+            basename = os.path.basename(path)
+            setting_name = os.path.splitext(basename)[0]
+            relpath = os.path.relpath(path, project_root).replace("\\", "/")
+            lines.append(f"var {setting_name} = loader('res://{relpath}')")
+
+            # 去掉缩进
+        code = textwrap.dedent(
+            """
+        extends Node
+        # 这个脚本你需要挂到游戏的Autoload才能全局读表
 
-    return code
-
-
-def completed_hook(config: Configuration):
-
-    output = config.output
-    settings_file_path = os.path.join(output, "settings.gd")
-    project_root = config.project_root
-
-    lines = []
-
-    loader = textwrap.dedent("""
-    static func loader(path:String):
-        var file = File.new()
-        file.open(path,File.READ)
-        var txt = file.get_as_text()
-        var data = JSON.parse(txt)
-        file.close()
-        return data
-    """)
-
-    for path in glob.glob(f"{output}/**/*.{extension}", recursive=True):
-        if path == settings_file_path:
-            continue  # 跳过 settings.gd
-        basename = os.path.basename(path)
-        setting_name = os.path.splitext(basename)[0]
-        relpath = os.path.relpath(path, project_root).replace("\\", "/")
-        lines.append(f"var {setting_name} = loader('res://{relpath}')")
-
-        # 去掉缩进
-    code = textwrap.dedent(
+        {loader}
+        {refs_code}
         """
-    extends Node
-    # 这个脚本你需要挂到游戏的Autoload才能全局读表
+        )
+        refs_code = "\n".join(lines)
+
+        code = code.format(loader=loader, refs_code=refs_code)
 
-    {loader}
-    {refs_code}
-    """
-    )
-    refs_code = "\n".join(lines)
-
-    code = code.format(loader=loader, refs_code=refs_code)
-
-    with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(code)
-        logger.info("创建setting.gd")
+        with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(code)
+            logger.info(f"创建：{settings_file_path}")
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/json2/__init__.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/json2/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,76 @@
 import glob
 import json
 import os
 import logging
 import textwrap
-from excelexporter.config import Configuration
-from excelexporter.sheetdata import SheetData
-
-
-# 导出格式
-extension = "json"
+from gd_excelexporter.config import Configuration
+from gd_excelexporter.core.generator import Generator, Table
 
 logger = logging.getLogger(__name__)
 
 
-EE_DATATABLE_CLASS = """
-class_name EEDataTable
-extends Resource
-
-@export
-var data = {}
-"""
-
-
-def generator(sheetdata: SheetData, config: Configuration):
-    # 表格数据脚本模板
-
-    table = {}
-
-    for id, row in sheetdata.items():
-        row_data = {}
-
-        for field, var in row.items():
-            field_name: str = field
-            row_data[field_name] = var.value
-
-        table[id] = row_data
-
-    code = json.dumps(table, ensure_ascii=False, indent=2)
-
-    return code
-
-
-def completed_hook(config: Configuration):
-
-    output = config.output
-    settings_file_path = os.path.join(output, "settings.gd")
-    project_root = config.project_root
-
-    lines = []
-
-    loader = textwrap.dedent("""
-    static func loader(path:String):
-        var file = FileAccess.open(path,FileAccess.READ)
-        var txt = file.get_as_text()
-        var data = JSON.parse_string(txt)
-        file.close()
-        return data
-    """)
-
-    for path in glob.glob(f"{output}/**/*.json", recursive=True):
-        if path == settings_file_path:
-            continue  # 跳过 settings.gd
-        basename = os.path.basename(path)
-        setting_name = os.path.splitext(basename)[0]
-        relpath = os.path.relpath(path, project_root).replace("\\", "/")
-        lines.append(f"var {setting_name} = loader('res://{relpath}')")
-
-        # 去掉缩进
-    code = textwrap.dedent(
-        """
-    extends Node
-    # 这个脚本你需要挂到游戏的Autoload才能全局读表
-
-    {loader}
-    {refs_code}
-    """
-    )
-    refs_code = "\n".join(lines)
-
-    code = code.format(loader=loader, refs_code=refs_code)
-
-    with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(code)
-        logger.info("创建setting.gd")
+class JSON2Generator(Generator):
+    # 导出格式
+    __extension__ = "json"
+
+    @classmethod
+    def generate(cls, table: Table, config: Configuration):
+        # 表格数据脚本模板
+
+        # 由于json不支持int做key，所以这里需要转换一下
+        new_table = {}
+        for id, row in table.items():
+            row_data = {}
+
+            for field, var in row.items():
+                field_name: str = field
+                row_data[field_name] = var.value
+
+            new_table[id] = row_data
+
+        code = json.dumps(new_table, ensure_ascii=False, indent=2)
+
+        return code
+
+    @classmethod
+    def completed_hook(cls, config: Configuration):
+        output = config.output
+        settings_file_path = os.path.join(output, "settings.gd")
+        project_root = config.project_root
+
+        lines = []
+
+        loader = textwrap.dedent("""
+        static func loader(path:String):
+            var file = FileAccess.open(path,FileAccess.READ)
+            var txt = file.get_as_text()
+            var data = JSON.parse_string(txt)
+            file.close()
+            return data
+        """)
+
+        for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
+            if path == settings_file_path:
+                continue  # 跳过 settings.gd
+            basename = os.path.basename(path)
+            setting_name = os.path.splitext(basename)[0]
+            relpath = os.path.relpath(path, project_root).replace("\\", "/")
+            lines.append(f"var {setting_name} = loader('res://{relpath}')")
+
+            # 去掉缩进
+        code = textwrap.dedent(
+            """
+            extends Node
+            # 这个脚本你需要挂到游戏的Autoload才能全局读表
+
+            {loader}
+            {refs_code}
+            """
+        )
+        refs_code = "\n".join(lines)
+
+        code = code.format(loader=loader, refs_code=refs_code)
+
+        with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(code)
+            logger.info(f"创建：{settings_file_path}")
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/generators/resource/__init__.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/generators/resource/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 import glob
 import os
 import pprint
 import logging
 import textwrap
 import re
-from excelexporter.config import Configuration
-from excelexporter.sheetdata import SheetData
+from gd_excelexporter.core.generator import Generator, Table
+from gd_excelexporter.config import Configuration
 
+logger = logging.getLogger(__name__)
 
-# 导出格式
-extension = "tres"
 
-logger = logging.getLogger(__name__)
+class ResourceGenerator(Generator):
+    # 导出格式
+    __extension__ = "tres"
+    __datatable_class__ = """
+    class_name EEDataTable
+    extends Resource
 
+    @export
+    var data = {}
+    """
 
-EE_DATATABLE_CLASS = """
-class_name EEDataTable
-extends Resource
-
-@export
-var data = {}
-"""
-
-
-def generator(sheetdata: SheetData, config: Configuration):
-    # 表格数据脚本模板
-    abs_output = os.path.abspath(config.output)
-    relpath = os.path.relpath(
-        abs_output, config.project_root).replace("\\", "/")
-    template = """
-    [gd_resource type="Resource" script_class="EEDataTable" load_steps=2 format=3] 
-
-    [ext_resource type="Script" path="res://{relpath}/ee_data_table.gd" id="1"]
-
-    [resource]
-    script = ExtResource("1")
-    data = {data}
-    """  # noqa
-    template = textwrap.dedent(template)
-    table = {}
-
-    for id, row in sheetdata.items():
-        row_data = {}
-
-        for field, var in row.items():
-            field_name: str = field
-            row_data[field_name] = var.value
-
-        table[id] = row_data
-
-    code = template.format(
-        data=pprint.pformat(
-            table, indent=2, width=1000000000,
-            compact=True, sort_dicts=True),
-        relpath=relpath
-    )
-
-    code = textwrap.dedent(code)
-    code = re.sub(r"\b(True|False)\b", lambda m: m.group(1).lower(), code)
-    code = code.replace("'", '"')
-    return code
-
-
-def completed_hook(config: Configuration):
-
-    output = config.output
-    settings_file_path = os.path.join(output, "settings.gd")
-    data_class_file_path = os.path.join(output, "ee_data_table.gd")
-    project_root = config.project_root
-
-    lines = []
-
-    for path in glob.glob(f"{output}/**/*.{extension}", recursive=True):
-        if path == settings_file_path:
-            continue  # 跳过 settings.gd
-        if path == data_class_file_path:
-            continue  # 跳过数据表类
-        basename = os.path.basename(path)
-        setting_name = os.path.splitext(basename)[0]
-        relpath = os.path.relpath(path, project_root).replace("\\", "/")
-        lines.append(f"var {setting_name} = load('res://{relpath}')")
+    @classmethod
+    def generate(cls, table: Table, config: Configuration):
+        # 表格数据脚本模板
+        abs_output = os.path.abspath(config.output)
+        relpath = os.path.relpath(abs_output, config.project_root).replace("\\", "/")
+        template = """
+        [gd_resource type="Resource" script_class="EEDataTable" load_steps=2 format=3] 
+
+        [ext_resource type="Script" path="res://{relpath}/ee_data_table.gd" id="1"]
+
+        [resource]
+        script = ExtResource("1")
+        data = {data}
+        """  # noqa
+        template = textwrap.dedent(template)
+        new_table = {}
+
+        for id, row in table.items():
+            row_data = {}
+
+            for field, var in row.items():
+                field_name: str = field
+                row_data[field_name] = var.value
+
+            new_table[id] = row_data
+
+        code = template.format(
+            data=pprint.pformat(
+                new_table, indent=4, width=1000000000, compact=True, sort_dicts=True
+            ),
+            relpath=relpath,
+        )
+
+        code = textwrap.dedent(code)
+        code = re.sub(r"\b(True|False)\b", lambda m: m.group(1).lower(), code)
+        code = code.replace("'", '"')
+        return code
+
+    @classmethod
+    def completed_hook(cls, config: Configuration):
+        output = config.output
+        settings_file_path = os.path.join(output, "settings.gd")
+        data_class_file_path = os.path.join(output, "ee_data_table.gd")
+        project_root = config.project_root
+
+        lines = []
+
+        for path in glob.glob(f"{output}/**/*.{cls.__extension__}", recursive=True):
+            if path == settings_file_path:
+                continue  # 跳过 settings.gd
+            if path == data_class_file_path:
+                continue  # 跳过数据表类
+            basename = os.path.basename(path)
+            setting_name = os.path.splitext(basename)[0]
+            relpath = os.path.relpath(path, project_root).replace("\\", "/")
+            lines.append(f"var {setting_name} = load('res://{relpath}')")
+
+            # 去掉缩进
+        code = textwrap.dedent(
+            """
+        extends Node
+        # 这个脚本你需要挂到游戏的Autoload才能全局读表
 
-        # 去掉缩进
-    code = textwrap.dedent(
+        {refs_code}
         """
-    extends Node
-    # 这个脚本你需要挂到游戏的Autoload才能全局读表
-
-    {refs_code}
-    """
-    )
-    refs_code = "\n".join(lines)
+        )
+        refs_code = "\n".join(lines)
 
-    code = code.format(refs_code=refs_code)
+        code = code.format(refs_code=refs_code)
 
-    with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(code)
-        logger.info("创建setting.gd")
-
-    with open(data_class_file_path, "w", encoding="utf-8", newline="\n") as f:
-        f.write(EE_DATATABLE_CLASS)
-        logger.info("创建EEDataTable类")
+        with open(settings_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(code)
+            logger.info("创建setting.gd")
+
+        with open(data_class_file_path, "w", encoding="utf-8", newline="\n") as f:
+            f.write(cls.__datatable_class__)
+            logger.info("创建DataTable类")
```

### Comparing `gd_excelexporter-2.1.5/src/excelexporter/logger.py` & `gd_excelexporter-3.0.0a1/src/gd_excelexporter/logger.py`

 * *Files identical despite different names*

### Comparing `gd_excelexporter-2.1.5/PKG-INFO` & `gd_excelexporter-3.0.0a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
-Name: gd-excelexporter
-Version: 2.1.5
+Name: gd_excelexporter
+Version: 3.0.0a1
 Summary: Godot Excel导表工具
 License: MIT
 Author: kaluluosi
 Author-email: kaluluosi@gamil.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: babel (>=2.12.1,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: importlib-metadata (>=6.1.0,<7.0.0) ; python_version == "38"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: xlwings (>=0.29.0,<0.30.0)
+Requires-Dist: xlrd (==1.2)
+Requires-Dist: xlwings (>=0.31.1,<0.32.0)
 Description-Content-Type: text/markdown
 
-# GDExcelExporter 2.1
+# GD-ExcelExporter
+
+[![Build](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/build.yml/badge.svg)](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/build.yml)
+![Code Coverage](https://img.shields.io/badge/Code%20Coverage-92%25-success?style=flat)
+[![Test](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/test.yml/badge.svg)](https://github.com/kaluluosi/GDExcelExporter/actions/workflows/test.yml)
 
 [English](README.en.md)
 
 GDExcelExpoter 是为Godot设计的Excel表格导出数据资源的工具。
 它内置了好几种数据表导出和读取方案（导出器），支持Godot3.x、Godot4.x。
 
 下面我们用`ee`代指`GDExcelExporter`。
 
 [在线文档](https://kaluluosi.github.io/GDExcelExporter/)
 
 ## 更新日志
 
-2.1版本
-
-> **Warning** 
-> 2.0 开始导出格式已经不兼容1.0，如果你的项目里已经大量使用1.0导出的数据表，可能会导致你要修改代码的地方非常多。
-
-1. 重构导出器
-2. 通过`entry_points`支持导出器插件，现在可以开发自己的导出器插件
-3. 多语言支持，集成了pybabel多语言方案，直接支持配置表、gd脚本、tscn、tres整个godot项目的多语言文本提取。以后出一个文档单独讲解。
-4. 单元测试用例补充
-5. ~~悲报：因为pyinstaller不支持 `entry_points` 因此2.1版本之后不提供独立`exe`了。~~ 2.1.4开始重新提供'ee.exe'
+**3.0版本**
+1. 重构框架，类型转换器、导出器、引擎全部面向接口编程，而且都`entry_points`插件化，以后可以自己写插件自定义。
+2. 默认采用xlrd读取excel，以此支持linux、macos、windows全平台的导出，而且速度更快。用户仍然可以选择用xlwings作为excel读取库（由xlrd其实已经不需要了）。
+3. 修改多语言字段类型，原本是`#`开头，比如`#string`，现在改为`tr_string`。
+4. 包改名为`gd_excelexporter`，因为之前包名`gd-excelexporter`和`src\excelexporter`不一致，整出很多麻烦，现在统一了。因此你需要卸载原来的`gd-excelexporter`包，重新安装这个包。
+5. 其他的没有任何改变，兼容原来的`settings`项目目录。但是安全起见建议重新`ee init`一个目录，然后将`data`下的表迁移过去重新导出。
 
 ## 为什么需要这个工具？
 
 Unreal引擎中有一个工具叫做DataTable，它的作用是充当一个小型的数据库给游戏设计人员编辑配置数值数据。
 
 打个比方，我们游戏中有道具系统，而道具整个对象一旦属性字段建模好，那么就可以通过配置这些属性定义出各种各样的道具。
 
@@ -64,34 +68,31 @@
 1. 就不用手写json
 2. 也不用嵌入sqlite
 3. 由于数据是以项目的文件资源存在，因此也是版本管理工具友好的
 4. 也因为数据是文件资源，因此热更新友好
 5. 你不需要学习别的工具去编辑维护数据，会用excel就可以，你可以用上你excel中所有的技巧去编辑数据
 
 
-## 快速开始
+## 快速上手
 
 ### 系统要求
 Python:^3.8.1
 
 Platform: Windows(xlwings只支持Windows)
 
 Godot版本:^3.4
 
 ### 安装
 通过pip （建议）
 ```
-pip install gd-excelexporter
+pip install gd-gd_excelexporter
 ```
 
 或者直接去右边release里下载已经打包好的可执行文件（ee.exe，你需要将这个exe加到环境变量）。
 
-> **Note** 
-> 2.1.4 版本开始exe的打包问题已经解决，后续版本会继续提供`ee.exe`命令行程序。
-
 ### 创建配置表项目
 
 打开你的Godot游戏项目，项目根目录下右键打开命令行（此处打开powershell）
 ![图 1](docs/images/b0e636c8ece81e8d9a81f663e91db7872e8cbd06f97dbd6edae64f15c3d1173b.gif)  
 ![图 2](docs/images/939a62bfbaec7d9c2e7d2c75715d3ab53624cb1ecd4006ce7ae3163fbda721fc.gif)  
 ![图 3](docs/images/69e876afa54e19f5c9fbd50cc274a1a583a9e4233fa0afcfd6407a6ea683b21f.png)  
 ![图 4](docs/images/7658090be99a6b34b8ca397a76eb4a7462adcd5de98fa21f27e944c024123a95.png)  
@@ -271,7 +272,12 @@
 
 [Godot插件-GDExcelExporter-Plugin](https://github.com/kaluluosi/GDEexcelExporer-Plugin)
 
 ## 最后
 希望这个工具能够给一些独立游戏人或者业余自娱自乐的人一些帮助。
 如果你用上了我的工具，有什么问题最好直接提issue。
 
+如果你在你的独立游戏项目中使用了我的工具，希望你能够在游戏结尾员工名单或者开源证书页面中特别鸣谢加上我的名字，让我也占个光，谢谢。
+
+## 联系方式
+
+![Snipaste_2024-04-19_06-50-25](/assets/Snipaste_2024-04-19_06-50-25_icwxbsqi8.png)
```

