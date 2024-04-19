# Comparing `tmp/pyarmor.cli.core.windows-6.5.0-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.windows-6.5.1-cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 850654 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 24-Feb-29 02:11 pyarmor/cli/core/windows/__init__.py
--rwxr-xr-x  2.0 unx   777742 b- defN 24-Feb-29 02:11 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   593408 b- defN 24-Feb-29 02:11 pyarmor/cli/core/windows/x86/pytransform3.pyd
--rwxr-xr-x  2.0 unx   632832 b- defN 24-Feb-29 02:11 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   454656 b- defN 24-Feb-29 02:11 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
--rw-r--r--  2.0 unx      808 b- defN 24-Feb-29 02:11 pyarmor.cli.core.windows-6.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 24-Feb-29 02:11 pyarmor.cli.core.windows-6.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-29 02:11 pyarmor.cli.core.windows-6.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 24-Feb-29 02:11 pyarmor.cli.core.windows-6.5.0.dist-info/RECORD
-9 files, 2460452 bytes uncompressed, 849100 bytes compressed:  65.5%
+Zip file size: 852082 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/__init__.py
+-rwxr-xr-x  2.0 unx   776718 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   594432 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86/pytransform3.pyd
+-rwxr-xr-x  2.0 unx   630784 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   454656 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
+-rw-r--r--  2.0 unx      808 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       94 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      883 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/RECORD
+9 files, 2458405 bytes uncompressed, 850528 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/windows/x86_64/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.0.dist-info/METADATA
+Filename: pyarmor.cli.core.windows-6.5.1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.0.dist-info/WHEEL
+Filename: pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.0.dist-info/top_level.txt
+Filename: pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.0.dist-info/RECORD
+Filename: pyarmor.cli.core.windows-6.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/windows/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '6.5.0'
+__VERSION__ = '6.5.1'
```

## Comparing `pyarmor.cli.core.windows-6.5.0.dist-info/METADATA` & `pyarmor.cli.core.windows-6.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.windows
-Version: 6.5.0
+Version: 6.5.1
 Summary: Provide pre-built extension modules `pytransform3` and `pyarmor_runtime` for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.windows-6.5.0.dist-info/RECORD` & `pyarmor.cli.core.windows-6.5.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyarmor/cli/core/windows/__init__.py,sha256=pVBffWsZD_nFNvoHuMuhiLzzQeJCr_2Vmij92sTENZE,22
-pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=BiQ3YVbBrojV7fSMg3A1sS-GeHF6GaT9AWNX5VhlEr8,777742
-pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=xQS4Gjgz0N3tgc0v9Ku77zXAqTYC5YN84HQHgOaNZic,593408
-pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=3X1DqNJkkZWcPWO6ZllU1JCtJnJ-daD50fm4KFFlc2U,632832
-pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=f1Jdbdst4um8-b0K9p_v1uMYZaLfy-ai9QPkPBT4xH4,454656
-pyarmor.cli.core.windows-6.5.0.dist-info/METADATA,sha256=I2i9Nz0RCzqPESoOOlJY2YI1mSSiSlfpC8bE04kPZf4,808
-pyarmor.cli.core.windows-6.5.0.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.windows-6.5.0.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.windows-6.5.0.dist-info/RECORD,,
+pyarmor/cli/core/windows/__init__.py,sha256=M2yOPgFwbZl3SpSI2ME2BW4rRl7JQ9OzeQSR2orDhUc,22
+pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=6C6mIzj_ClhLsUHhY112FSJddU8mo3KFQLYhd1iq-iE,776718
+pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=qXW0E-8q6NCHzMT3P6r3_0_Pf43ayPccp9Vf5242TzY,594432
+pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=hjz9cgNrF4I3H2wC_nSZG15FLxbZjIMcsWLgzRoFtso,630784
+pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=zdXVzSaILzZxw3m2svK4LRwmaDaurAo1u_zvHoj3Djw,454656
+pyarmor.cli.core.windows-6.5.1.dist-info/METADATA,sha256=ZBwY8X4kGYWyRXlBY6n_pYYudOAi7nokOQjn14XnRb0,808
+pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL,sha256=-3aXCvPnPZoJT9_CW7Ktbz89d6UlQzqzh62Pk7rxQbY,94
+pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.windows-6.5.1.dist-info/RECORD,,
```

