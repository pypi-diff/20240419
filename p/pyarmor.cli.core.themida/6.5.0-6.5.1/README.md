# Comparing `tmp/pyarmor.cli.core.themida-6.5.0-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-6.5.1-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7658447 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 24-Feb-29 02:12 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  3752990 b- defN 24-Feb-29 02:12 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  4864528 b- defN 24-Feb-29 02:12 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      809 b- defN 24-Feb-29 02:12 pyarmor.cli.core.themida-6.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 24-Feb-29 02:12 pyarmor.cli.core.themida-6.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-29 02:12 pyarmor.cli.core.themida-6.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 24-Feb-29 02:12 pyarmor.cli.core.themida-6.5.0.dist-info/RECORD
-7 files, 8619140 bytes uncompressed, 7657199 bytes compressed:  11.2%
+Zip file size: 7909645 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-19 07:51 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  3926558 b- defN 24-Apr-19 07:51 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  4946960 b- defN 24-Apr-19 07:51 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      809 b- defN 24-Apr-19 07:51 pyarmor.cli.core.themida-6.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-19 07:51 pyarmor.cli.core.themida-6.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 07:51 pyarmor.cli.core.themida-6.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      690 b- defN 24-Apr-19 07:51 pyarmor.cli.core.themida-6.5.1.dist-info/RECORD
+7 files, 8875140 bytes uncompressed, 7908397 bytes compressed:  10.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-6.5.0.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-6.5.1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-6.5.0.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-6.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-6.5.0.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-6.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-6.5.0.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-6.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '6.5.0'
+__VERSION__ = '6.5.1'
```

## Comparing `pyarmor.cli.core.themida-6.5.0.dist-info/METADATA` & `pyarmor.cli.core.themida-6.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 6.5.0
+Version: 6.5.1
 Summary: Provide pre-built extension module `pyarmor_runtime` protected by Themida for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.themida-6.5.0.dist-info/RECORD` & `pyarmor.cli.core.themida-6.5.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyarmor/cli/core/themida/__init__.py,sha256=pVBffWsZD_nFNvoHuMuhiLzzQeJCr_2Vmij92sTENZE,22
-pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=iaiG6jsfpCEpcKcVYVh47EYv-HyFqtCqlU4dh4ytlCY,3752990
-pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=WvI7dO7s3X4WPIJo9LRx0qrdEuhN6a7WLqQrUabM6Pw,4864528
-pyarmor.cli.core.themida-6.5.0.dist-info/METADATA,sha256=m6WXHWZApCrDTkzB3PLmUc3qErttX8IhKFIKmcM4828,809
-pyarmor.cli.core.themida-6.5.0.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.themida-6.5.0.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.themida-6.5.0.dist-info/RECORD,,
+pyarmor/cli/core/themida/__init__.py,sha256=M2yOPgFwbZl3SpSI2ME2BW4rRl7JQ9OzeQSR2orDhUc,22
+pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=l_-3bqhBVbHq0kMtw0azxYzkaPuthk0_K6bHLgjaHsI,3926558
+pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=HzVJ-cYZNj1APQS9vpZhtlJKTbnsh9TIiqFGBDLmd6w,4946960
+pyarmor.cli.core.themida-6.5.1.dist-info/METADATA,sha256=UinV7n6bg1gdGfCtqrOSErIeK9aDrE5sGQeNWJYosoo,809
+pyarmor.cli.core.themida-6.5.1.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.themida-6.5.1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.themida-6.5.1.dist-info/RECORD,,
```

