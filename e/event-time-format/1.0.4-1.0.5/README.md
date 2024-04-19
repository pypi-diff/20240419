# Comparing `tmp/event_time_format-1.0.4-py3-none-any.whl.zip` & `tmp/event_time_format-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 14441 bytes, number of entries: 8
+Zip file size: 14444 bytes, number of entries: 8
 -rw-r--r--  2.0 unx    33241 b- defN 24-Mar-16 03:37 event_time_format/Test_event_time_format.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-16 03:44 event_time_format/__init__.py
 -rw-r--r--  2.0 unx    33660 b- defN 24-Apr-15 12:06 event_time_format/event_time_format.py
--rw-r--r--  2.0 unx     1507 b- defN 24-Apr-19 09:42 event_time_format-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1480 b- defN 24-Apr-19 09:42 event_time_format-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 09:42 event_time_format-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-19 09:42 event_time_format-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      716 b- defN 24-Apr-19 09:42 event_time_format-1.0.4.dist-info/RECORD
-8 files, 70714 bytes uncompressed, 13173 bytes compressed:  81.4%
+-rw-r--r--  2.0 unx     1507 b- defN 24-Apr-19 09:52 event_time_format-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1492 b- defN 24-Apr-19 09:52 event_time_format-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 09:52 event_time_format-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-19 09:52 event_time_format-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      716 b- defN 24-Apr-19 09:52 event_time_format-1.0.5.dist-info/RECORD
+8 files, 70726 bytes uncompressed, 13176 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: event_time_format/__init__.py
 Comment: 
 
 Filename: event_time_format/event_time_format.py
 Comment: 
 
-Filename: event_time_format-1.0.4.dist-info/LICENSE
+Filename: event_time_format-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: event_time_format-1.0.4.dist-info/METADATA
+Filename: event_time_format-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: event_time_format-1.0.4.dist-info/WHEEL
+Filename: event_time_format-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: event_time_format-1.0.4.dist-info/top_level.txt
+Filename: event_time_format-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: event_time_format-1.0.4.dist-info/RECORD
+Filename: event_time_format-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `event_time_format-1.0.4.dist-info/LICENSE` & `event_time_format-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `event_time_format-1.0.4.dist-info/METADATA` & `event_time_format-1.0.5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-time-format
-Version: 1.0.4
+Version: 1.0.5
 Summary: event time format
 Home-page: https://github.com/errord/EventTimeFormat
 Author: errord
 Author-email: errord@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/errord/EventTimeFormat
 Platform: all
@@ -17,20 +17,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
-Requires-Dist: arrow >=1.1.0
-Requires-Dist: requests >=2.20.1
-Requires-Dist: numpy >=1.21.0
-Requires-Dist: pandas >=1.3.3
-Requires-Dist: tensorflow >=2.5.1
-Requires-Dist: bs4 >=0.0.2
+Requires-Dist: arrow (>=1.1.0)
+Requires-Dist: requests (>=2.20.1)
+Requires-Dist: numpy (>=1.21.0)
+Requires-Dist: pandas (>=1.3.3)
+Requires-Dist: tensorflow (>=2.5.1)
+Requires-Dist: bs4 (>=0.0.2)
 
 # Readme
 格式化时间，通过多种中文格式显示
 
 # EventTimeFormat
 时间格式化 ： 11月19日 ~ 2015年1月30日 每周三，日 09:30-22:30 | 11月19日 ~ 2015年1月30日 每周三，日 全天 |  全年 每周四 10:30-21:00 |  每周四 10:30-21:00
```

