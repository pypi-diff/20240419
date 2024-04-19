# Comparing `tmp/CachedFileDic-0.2.1.tar.gz` & `tmp/CachedFileDic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CachedFileDic-0.2.1.tar", last modified: Fri Apr 19 05:17:31 2024, max compression
+gzip compressed data, was "CachedFileDic-0.2.2.tar", last modified: Fri Apr 19 11:22:22 2024, max compression
```

## Comparing `CachedFileDic-0.2.1.tar` & `CachedFileDic-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 05:17:31.063846 CachedFileDic-0.2.1/
-drwxrwxrwx   0        0        0        0 2024-04-19 05:17:31.055919 CachedFileDic-0.2.1/CachedFileDic/
--rw-rw-rw-   0        0        0     6595 2024-04-19 05:15:49.000000 CachedFileDic-0.2.1/CachedFileDic/__init__.py
--rw-rw-rw-   0        0        0      833 2024-03-07 09:47:59.000000 CachedFileDic-0.2.1/CachedFileDic/test.py
-drwxrwxrwx   0        0        0        0 2024-04-19 05:17:31.063846 CachedFileDic-0.2.1/CachedFileDic.egg-info/
--rw-rw-rw-   0        0        0     8550 2024-04-19 05:17:30.000000 CachedFileDic-0.2.1/CachedFileDic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-04-19 05:17:30.000000 CachedFileDic-0.2.1/CachedFileDic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 05:17:30.000000 CachedFileDic-0.2.1/CachedFileDic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-19 05:17:30.000000 CachedFileDic-0.2.1/CachedFileDic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-19 05:17:30.000000 CachedFileDic-0.2.1/CachedFileDic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8550 2024-04-19 05:17:31.063846 CachedFileDic-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6931 2023-12-22 09:17:16.000000 CachedFileDic-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-19 05:17:31.063846 CachedFileDic-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-19 05:17:17.000000 CachedFileDic-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:22.671783 CachedFileDic-0.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:22.655757 CachedFileDic-0.2.2/CachedFileDic/
+-rw-rw-rw-   0        0        0     6894 2024-04-19 11:21:36.000000 CachedFileDic-0.2.2/CachedFileDic/__init__.py
+-rw-rw-rw-   0        0        0     6595 2024-04-19 09:37:57.000000 CachedFileDic-0.2.2/CachedFileDic/__init__BACKUP_commit効率化変更前.py
+-rw-rw-rw-   0        0        0      833 2024-03-07 09:47:59.000000 CachedFileDic-0.2.2/CachedFileDic/test.py
+drwxrwxrwx   0        0        0        0 2024-04-19 11:22:22.671783 CachedFileDic-0.2.2/CachedFileDic.egg-info/
+-rw-rw-rw-   0        0        0     8550 2024-04-19 11:22:22.000000 CachedFileDic-0.2.2/CachedFileDic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-04-19 11:22:22.000000 CachedFileDic-0.2.2/CachedFileDic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 11:22:22.000000 CachedFileDic-0.2.2/CachedFileDic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-19 11:22:22.000000 CachedFileDic-0.2.2/CachedFileDic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-19 11:22:22.000000 CachedFileDic-0.2.2/CachedFileDic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8550 2024-04-19 11:22:22.671783 CachedFileDic-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6931 2023-12-22 09:17:16.000000 CachedFileDic-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 11:22:22.671783 CachedFileDic-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-04-19 11:22:03.000000 CachedFileDic-0.2.2/setup.py
```

### Comparing `CachedFileDic-0.2.1/CachedFileDic/__init__.py` & `CachedFileDic-0.2.2/CachedFileDic/__init__BACKUP_commit効率化変更前.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.1/CachedFileDic/test.py` & `CachedFileDic-0.2.2/CachedFileDic/test.py`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.1/CachedFileDic.egg-info/PKG-INFO` & `CachedFileDic-0.2.2/CachedFileDic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CachedFileDic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fast Dictionary-Type Database
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `CachedFileDic-0.2.1/PKG-INFO` & `CachedFileDic-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CachedFileDic
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fast Dictionary-Type Database
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: - The explanations in English, Simplified Chinese, and Spanish are provided below.
         - 下面提供了英语、简体中文和西班牙语的说明。
```

### Comparing `CachedFileDic-0.2.1/README.md` & `CachedFileDic-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `CachedFileDic-0.2.1/setup.py` & `CachedFileDic-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 4361 6368 6564 4669  develop_CachedFi
 000000c0: 6c65 4469 632f 2229 2061 7320 703a 0d0a  leDic/") as p:..
 000000d0: 0973 6574 7570 280d 0a09 096e 616d 6520  .setup(....name 
 000000e0: 3d20 2243 6163 6865 6446 696c 6544 6963  = "CachedFileDic
 000000f0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-00000100: 2230 2e32 2e31 222c 0d0a 0909 6465 7363  "0.2.1",....desc
+00000100: 2230 2e32 2e32 222c 0d0a 0909 6465 7363  "0.2.2",....desc
 00000110: 7269 7074 696f 6e20 3d20 2246 6173 7420  ription = "Fast 
 00000120: 4469 6374 696f 6e61 7279 2d54 7970 6520  Dictionary-Type 
 00000130: 4461 7461 6261 7365 222c 0d0a 0909 6175  Database",....au
 00000140: 7468 6f72 203d 2022 6269 625f 696e 6622  thor = "bib_inf"
 00000150: 2c0d 0a09 0961 7574 686f 725f 656d 6169  ,....author_emai
 00000160: 6c20 3d20 2263 6f6e 7461 6374 2e62 6962  l = "contact.bib
 00000170: 696e 6640 676d 6169 6c2e 636f 6d22 2c0d  inf@gmail.com",.
```

