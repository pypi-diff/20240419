# Comparing `tmp/jsonffi-1.0.0-py3-none-any.whl.zip` & `tmp/jsonffi-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1789 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      949 b- defN 24-Apr-19 03:01 jsonffi/__init__.py
--rw-rw-rw-  2.0 fat      568 b- defN 24-Apr-19 03:05 jsonffi-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 03:05 jsonffi-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 03:05 jsonffi-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      371 b- defN 24-Apr-19 03:05 jsonffi-1.0.0.dist-info/RECORD
-5 files, 1988 bytes uncompressed, 1093 bytes compressed:  45.0%
+Zip file size: 1780 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      945 b- defN 24-Apr-19 03:13 jsonffi/__init__.py
+-rw-rw-rw-  2.0 fat      565 b- defN 24-Apr-19 03:14 jsonffi-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 03:14 jsonffi-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 03:14 jsonffi-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      371 b- defN 24-Apr-19 03:14 jsonffi-1.0.1.dist-info/RECORD
+5 files, 1981 bytes uncompressed, 1084 bytes compressed:  45.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jsonffi/__init__.py
 Comment: 
 
-Filename: jsonffi-1.0.0.dist-info/METADATA
+Filename: jsonffi-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: jsonffi-1.0.0.dist-info/WHEEL
+Filename: jsonffi-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: jsonffi-1.0.0.dist-info/top_level.txt
+Filename: jsonffi-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonffi-1.0.0.dist-info/RECORD
+Filename: jsonffi-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonffi/__init__.py

```diff
@@ -1,17 +1,17 @@
 import json
 from cffi import FFI
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.0'
+__version__      = '1.0.1'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/javacommons/py-jsonffi'
-    __all__ = ['JsonFFI']
+__all__ = ['JsonFFI']
 
 class JsonFFI:
     def __init__(self, dllSpec):
         self.ffi = FFI()
         self.ffi.cdef("const char *Call(const char *, const char *);")
         self.ffi.cdef("const char *LastError();")
         self.clib = self.ffi.dlopen(dllSpec)
```

## Comparing `jsonffi-1.0.0.dist-info/METADATA` & `jsonffi-1.0.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: jsonffi
-Version: 1.0.0
+Version: 1.0.1
 Summary: 一言で書けるパッケージ概要
 Home-page: https://github.com/javacommons/py-jsonffi
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: cffi
 
-# winjsonapi
+# jsonffi
```

