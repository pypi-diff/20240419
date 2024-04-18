# Comparing `tmp/deepCR-0.2.1rc0.tar.gz` & `tmp/deepCR-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deepCR-0.2.1rc0.tar", last modified: Wed Oct  2 23:35:57 2019, max compression
+gzip compressed data, was "deepCR-0.3.1.tar", last modified: Thu Apr 18 22:31:59 2024, max compression
```

## Comparing `deepCR-0.2.1rc0.tar` & `deepCR-0.3.1.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/
--rw-r--r--   0 jbloom     (501) staff       (20)     5868 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/PKG-INFO
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/learned_models/
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/learned_models/inpaint/
--rw-r--r--   0 jbloom     (501) staff       (20)  1890231 2019-07-23 05:06:26.000000 deepCR-0.2.1rc0/learned_models/inpaint/ACS-WFC-F606W-3-32.pth
--rw-r--r--   0 jbloom     (501) staff       (20)   417988 2019-07-23 05:06:26.000000 deepCR-0.2.1rc0/learned_models/inpaint/ACS-WFC-F606W-2-32.pth
--rw-r--r--   0 jbloom     (501) staff       (20)      560 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/learned_models/__init__.py
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/learned_models/mask/
--rw-r--r--   0 jbloom     (501) staff       (20)   416836 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/learned_models/mask/decam.pth
--rw-r--r--   0 jbloom     (501) staff       (20)    15979 2019-07-20 16:08:49.000000 deepCR-0.2.1rc0/learned_models/mask/ACS-WFC-F606W-2-4.pth
--rw-r--r--   0 jbloom     (501) staff       (20)   416836 2019-07-23 05:30:52.000000 deepCR-0.2.1rc0/learned_models/mask/example_model.pth
--rw-r--r--   0 jbloom     (501) staff       (20)   416836 2019-07-20 16:08:49.000000 deepCR-0.2.1rc0/learned_models/mask/ACS-WFC-F606W-2-32.pth
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/deepCR.egg-info/
--rw-r--r--   0 jbloom     (501) staff       (20)     1003 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/deepCR.egg-info/SOURCES.txt
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/imgs/
--rw-r--r--   0 jbloom     (501) staff       (20)   500710 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/imgs/acs_wfc_f606w_roc.png
--rw-r--r--   0 jbloom     (501) staff       (20)   295886 2019-07-23 05:06:26.000000 deepCR-0.2.1rc0/imgs/postage-sm.jpg
--rw-r--r--   0 jbloom     (501) staff       (20)   211902 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/imgs/decam.png
--rw-r--r--   0 jbloom     (501) staff       (20)   602203 2019-10-02 23:08:10.000000 deepCR-0.2.1rc0/imgs/network.png
--rw-r--r--   0 jbloom     (501) staff       (20)      215 2019-07-23 06:51:37.000000 deepCR-0.2.1rc0/MANIFEST.in
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/docs/
--rw-r--r--   0 jbloom     (501) staff       (20)     1862 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/docs/index.rst
--rw-r--r--   0 jbloom     (501) staff       (20)     2784 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/docs/tutorial_train.rst
--rw-r--r--   0 jbloom     (501) staff       (20)       14 2019-07-23 07:24:25.000000 deepCR-0.2.1rc0/docs/requirements.txt
--rw-r--r--   0 jbloom     (501) staff       (20)      154 2019-07-23 06:00:13.000000 deepCR-0.2.1rc0/docs/environment.yml
--rw-r--r--   0 jbloom     (501) staff       (20)      634 2019-07-23 06:00:13.000000 deepCR-0.2.1rc0/docs/Makefile
--rw-r--r--   0 jbloom     (501) staff       (20)      174 2019-08-14 13:39:45.000000 deepCR-0.2.1rc0/docs/deepCR.rst
--rw-r--r--   0 jbloom     (501) staff       (20)     2559 2019-07-23 07:21:47.000000 deepCR-0.2.1rc0/docs/conf.py
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/docs/source/
--rw-r--r--   0 jbloom     (501) staff       (20)     1113 2019-08-02 04:04:30.000000 deepCR-0.2.1rc0/docs/source/deepCR.rst
--rw-r--r--   0 jbloom     (501) staff       (20)       55 2019-08-02 04:04:30.000000 deepCR-0.2.1rc0/docs/source/modules.rst
--rw-r--r--   0 jbloom     (501) staff       (20)      977 2019-08-02 04:04:30.000000 deepCR-0.2.1rc0/docs/source/deepCR.test.rst
--rw-r--r--   0 jbloom     (501) staff       (20)     2134 2019-08-14 13:39:45.000000 deepCR-0.2.1rc0/docs/tutorial_use.rst
--rw-r--r--   0 jbloom     (501) staff       (20)       55 2019-07-23 06:00:13.000000 deepCR-0.2.1rc0/docs/modules.rst
--rw-r--r--   0 jbloom     (501) staff       (20)      795 2019-07-23 06:00:13.000000 deepCR-0.2.1rc0/docs/make.bat
--rw-r--r--   0 jbloom     (501) staff       (20)     1954 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/docs/model_zoo.rst
--rw-r--r--   0 jbloom     (501) staff       (20)      491 2019-07-23 06:00:13.000000 deepCR-0.2.1rc0/docs/deepCR.test.rst
--rw-r--r--   0 jbloom     (501) staff       (20)     4300 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/README.md
--rw-r--r--   0 jbloom     (501) staff       (20)      302 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/CHANGES.txt
--rw-r--r--   0 jbloom     (501) staff       (20)     2379 2019-07-23 05:06:26.000000 deepCR-0.2.1rc0/setup.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1288 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/setup.cfg
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/deepCR/
-drwxr-xr-x   0 jbloom     (501) staff       (20)        0 2019-10-02 23:35:57.000000 deepCR-0.2.1rc0/deepCR/test/
--rw-r--r--   0 jbloom     (501) staff       (20)     1641 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/test/test_model.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1471 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/test/test_train.py
--rw-r--r--   0 jbloom     (501) staff       (20)        0 2019-07-16 17:53:05.000000 deepCR-0.2.1rc0/deepCR/test/__init__.py
--rw-r--r--   0 jbloom     (501) staff       (20)      352 2019-07-16 21:19:43.000000 deepCR-0.2.1rc0/deepCR/test/test_util.py
--rw-r--r--   0 jbloom     (501) staff       (20)     3109 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/test/test_evaluate.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1620 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/test/test_dataset.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1112 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/util.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1796 2019-07-16 19:31:30.000000 deepCR-0.2.1rc0/deepCR/unet.py
--rw-r--r--   0 jbloom     (501) staff       (20)      437 2019-10-02 23:35:52.000000 deepCR-0.2.1rc0/deepCR/__init__.py
--rw-r--r--   0 jbloom     (501) staff       (20)    14282 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/model.py
--rw-r--r--   0 jbloom     (501) staff       (20)     6646 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/dataset.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1641 2019-08-02 04:15:50.000000 deepCR-0.2.1rc0/deepCR/parts.py
--rw-r--r--   0 jbloom     (501) staff       (20)     4887 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/evaluate.py
--rw-r--r--   0 jbloom     (501) staff       (20)    12864 2019-10-02 23:31:21.000000 deepCR-0.2.1rc0/deepCR/training.py
--rw-r--r--   0 jbloom     (501) staff       (20)     1519 2019-07-16 17:12:57.000000 deepCR-0.2.1rc0/LICENSE.txt
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.345661 deepCR-0.3.1/
+-rw-r--r--   0 Keming     (502) staff       (20)      302 2024-04-18 16:45:15.000000 deepCR-0.3.1/CHANGES.txt
+-rw-r--r--   0 Keming     (502) staff       (20)     1519 2024-04-18 16:45:15.000000 deepCR-0.3.1/LICENSE.txt
+-rw-r--r--   0 Keming     (502) staff       (20)      215 2024-04-18 16:45:15.000000 deepCR-0.3.1/MANIFEST.in
+-rw-r--r--   0 Keming     (502) staff       (20)     4120 2024-04-18 22:31:59.345722 deepCR-0.3.1/PKG-INFO
+-rw-r--r--   0 Keming     (502) staff       (20)     3401 2024-04-18 18:29:27.000000 deepCR-0.3.1/README.md
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.337954 deepCR-0.3.1/deepCR/
+-rw-r--r--   0 Keming     (502) staff       (20)      433 2024-04-18 22:31:53.000000 deepCR-0.3.1/deepCR/__init__.py
+-rw-r--r--   0 Keming     (502) staff       (20)     9844 2024-04-18 16:45:21.000000 deepCR-0.3.1/deepCR/dataset.py
+-rw-r--r--   0 Keming     (502) staff       (20)     5142 2024-04-18 16:45:21.000000 deepCR-0.3.1/deepCR/evaluate.py
+-rw-r--r--   0 Keming     (502) staff       (20)    13297 2024-04-18 18:08:15.000000 deepCR-0.3.1/deepCR/model.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1602 2024-04-18 16:45:21.000000 deepCR-0.3.1/deepCR/parts.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1640 2024-04-18 17:17:41.000000 deepCR-0.3.1/deepCR/parts_batchnorm.py
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.338687 deepCR-0.3.1/deepCR/test/
+-rw-r--r--   0 Keming     (502) staff       (20)        0 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/test/__init__.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1620 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/test/test_dataset.py
+-rw-r--r--   0 Keming     (502) staff       (20)     3109 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/test/test_evaluate.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1636 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/test/test_model.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1501 2024-04-18 16:45:21.000000 deepCR-0.3.1/deepCR/test/test_train.py
+-rw-r--r--   0 Keming     (502) staff       (20)      352 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/test/test_util.py
+-rw-r--r--   0 Keming     (502) staff       (20)    14012 2024-04-18 16:56:54.000000 deepCR-0.3.1/deepCR/training.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1796 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/unet.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1832 2024-04-18 17:18:41.000000 deepCR-0.3.1/deepCR/unet_batchnorm.py
+-rw-r--r--   0 Keming     (502) staff       (20)     1112 2024-04-18 16:45:15.000000 deepCR-0.3.1/deepCR/util.py
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.345576 deepCR-0.3.1/deepCR.egg-info/
+-rw-r--r--   0 Keming     (502) staff       (20)     1119 2024-04-18 22:31:59.000000 deepCR-0.3.1/deepCR.egg-info/SOURCES.txt
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.340125 deepCR-0.3.1/docs/
+-rw-r--r--   0 Keming     (502) staff       (20)      634 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/Makefile
+-rw-r--r--   0 Keming     (502) staff       (20)     2559 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/conf.py
+-rw-r--r--   0 Keming     (502) staff       (20)      174 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/deepCR.rst
+-rw-r--r--   0 Keming     (502) staff       (20)      491 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/deepCR.test.rst
+-rw-r--r--   0 Keming     (502) staff       (20)      154 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/environment.yml
+-rw-r--r--   0 Keming     (502) staff       (20)     2001 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/index.rst
+-rw-r--r--   0 Keming     (502) staff       (20)      795 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/make.bat
+-rw-r--r--   0 Keming     (502) staff       (20)     3018 2024-04-18 18:23:12.000000 deepCR-0.3.1/docs/model_zoo.rst
+-rw-r--r--   0 Keming     (502) staff       (20)       55 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/modules.rst
+-rw-r--r--   0 Keming     (502) staff       (20)       14 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/requirements.txt
+-rw-r--r--   0 Keming     (502) staff       (20)     4316 2024-04-18 16:45:21.000000 deepCR-0.3.1/docs/tutorial_train.rst
+-rw-r--r--   0 Keming     (502) staff       (20)     1496 2024-04-18 16:45:15.000000 deepCR-0.3.1/docs/tutorial_use.rst
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.341376 deepCR-0.3.1/imgs/
+-rw-r--r--   0 Keming     (502) staff       (20)   500710 2024-04-18 16:45:15.000000 deepCR-0.3.1/imgs/acs_wfc_f606w_roc.png
+-rw-r--r--   0 Keming     (502) staff       (20)   462157 2024-04-18 16:45:15.000000 deepCR-0.3.1/imgs/decam_v1.png
+-rw-r--r--   0 Keming     (502) staff       (20)   602203 2024-04-18 16:45:15.000000 deepCR-0.3.1/imgs/network.png
+-rw-r--r--   0 Keming     (502) staff       (20)   295886 2024-04-18 16:45:15.000000 deepCR-0.3.1/imgs/postage-sm.jpg
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.341680 deepCR-0.3.1/learned_models/
+-rw-r--r--   0 Keming     (502) staff       (20)      575 2024-04-18 18:00:29.000000 deepCR-0.3.1/learned_models/__init__.py
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.342126 deepCR-0.3.1/learned_models/inpaint/
+-rw-r--r--   0 Keming     (502) staff       (20)   417988 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/inpaint/ACS-WFC-F606W-2-32.pth
+-rw-r--r--   0 Keming     (502) staff       (20)  1890231 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/inpaint/ACS-WFC-F606W-3-32.pth
+drwxr-xr-x   0 Keming     (502) staff       (20)        0 2024-04-18 22:31:59.345212 deepCR-0.3.1/learned_models/mask/
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/ACS-WFC-F435W.pth
+-rw-r--r--   0 Keming     (502) staff       (20)    15979 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/ACS-WFC-F606W-2-4.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/ACS-WFC-F606W.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/ACS-WFC-F814W.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/ACS-WFC.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   412323 2024-04-18 16:45:21.000000 deepCR-0.3.1/learned_models/mask/WFC3-UVIS.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/decam.pth
+-rw-r--r--   0 Keming     (502) staff       (20)   416836 2024-04-18 16:45:15.000000 deepCR-0.3.1/learned_models/mask/example_model.pth
+-rw-r--r--   0 Keming     (502) staff       (20)     1434 2024-04-18 22:31:59.345984 deepCR-0.3.1/setup.cfg
+-rw-r--r--   0 Keming     (502) staff       (20)     2379 2024-04-18 16:45:15.000000 deepCR-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `deepCR-0.2.1rc0/learned_models/inpaint/ACS-WFC-F606W-3-32.pth` & `deepCR-0.3.1/learned_models/inpaint/ACS-WFC-F606W-3-32.pth`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/learned_models/inpaint/ACS-WFC-F606W-2-32.pth` & `deepCR-0.3.1/learned_models/inpaint/ACS-WFC-F606W-2-32.pth`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/learned_models/mask/decam.pth` & `deepCR-0.3.1/learned_models/mask/decam.pth`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/learned_models/mask/ACS-WFC-F606W-2-4.pth` & `deepCR-0.3.1/learned_models/mask/ACS-WFC-F606W-2-4.pth`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/learned_models/mask/example_model.pth` & `deepCR-0.3.1/learned_models/mask/example_model.pth`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/deepCR.egg-info/SOURCES.txt` & `deepCR-0.3.1/deepCR.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 setup.cfg
 setup.py
 deepCR/__init__.py
 deepCR/dataset.py
 deepCR/evaluate.py
 deepCR/model.py
 deepCR/parts.py
+deepCR/parts_batchnorm.py
 deepCR/training.py
 deepCR/unet.py
+deepCR/unet_batchnorm.py
 deepCR/util.py
 deepCR/test/__init__.py
 deepCR/test/test_dataset.py
 deepCR/test/test_evaluate.py
 deepCR/test/test_model.py
 deepCR/test/test_train.py
 deepCR/test/test_util.py
@@ -26,21 +28,22 @@
 docs/index.rst
 docs/make.bat
 docs/model_zoo.rst
 docs/modules.rst
 docs/requirements.txt
 docs/tutorial_train.rst
 docs/tutorial_use.rst
-docs/source/deepCR.rst
-docs/source/deepCR.test.rst
-docs/source/modules.rst
 imgs/acs_wfc_f606w_roc.png
-imgs/decam.png
+imgs/decam_v1.png
 imgs/network.png
 imgs/postage-sm.jpg
 learned_models/__init__.py
 learned_models/inpaint/ACS-WFC-F606W-2-32.pth
 learned_models/inpaint/ACS-WFC-F606W-3-32.pth
-learned_models/mask/ACS-WFC-F606W-2-32.pth
+learned_models/mask/ACS-WFC-F435W.pth
 learned_models/mask/ACS-WFC-F606W-2-4.pth
+learned_models/mask/ACS-WFC-F606W.pth
+learned_models/mask/ACS-WFC-F814W.pth
+learned_models/mask/ACS-WFC.pth
+learned_models/mask/WFC3-UVIS.pth
 learned_models/mask/decam.pth
 learned_models/mask/example_model.pth
```

### Comparing `deepCR-0.2.1rc0/imgs/acs_wfc_f606w_roc.png` & `deepCR-0.3.1/imgs/acs_wfc_f606w_roc.png`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/imgs/postage-sm.jpg` & `deepCR-0.3.1/imgs/postage-sm.jpg`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/imgs/network.png` & `deepCR-0.3.1/imgs/network.png`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/docs/index.rst` & `deepCR-0.3.1/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -19,36 +19,43 @@
 :alt: Documentation Status
 
 Identify and remove cosmic rays from astronomical images using trained convolutional neural networks.
 
 .. image:: https://raw.githubusercontent.com/profjsb/deepCR/master/imgs/postage-sm.jpg
 
 
-Installation
-^^^^^^^^^^^^
+Quickstart
+^^^^^^^^^^
 
 .. code-block:: bash
 
    pip install deepCR
 
 Or you can install from source:
 
 .. code-block:: bash
 
    git clone https://github.com/profjsb/deepCR.git
    cd deepCR/
    pip install .
 
+.. code-block:: python
+
+    from deepCR import deepCR
+    import numpy as np
+    mdl = deepCR(mask="ACS-WFC", device="CPU")
+    image = np.zeros((1024, 1024))
+    binary_mask = mdl.clean(image, segment=True, n_jobs=-1)
+
 Currently available models
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. code-block:: python
 
    from deepCR import deepCR
-   decam_model = deepCR(mask='decam', device='CPU')
-   acswfc_model = deepCR(mask='ACS-WFC-F606W-2-32', inpaint='ACS-WFC-F606W-2-32', device='GPU')
+   acswfc_model = deepCR(mask='ACS-WFC', inpaint='ACS-WFC-F606W-2-32')
 ```
 
 For detailed descriptions and requirements of currently available models, please visit the model_zoo page below.
 
 If you run into any issues, please don't hesitate to `open an issue on GitHub
 <https://github.com/profjsb/deepCR/issues>`_.
```

### Comparing `deepCR-0.2.1rc0/docs/Makefile` & `deepCR-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/docs/conf.py` & `deepCR-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/docs/make.bat` & `deepCR-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/setup.py` & `deepCR-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/setup.cfg` & `deepCR-0.3.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -32,26 +32,29 @@
 	Topic :: Internet
 	Topic :: Scientific/Engineering :: Astronomy
 
 [options]
 packages = find:
 python_requires = >=3.5
 install_requires = 
-	astropy>=3.1.2
 	numpy>=1.16.3
+	astropy>=3.1.2
 	astroscrappy>=1.0.8
 	tqdm
-	scikit-image>=0.15.0
-	scipy>=1.2.1
+	scikit-image>=0.15.0;python_version>='3.7'
+	scikit-image==0.15.*;python_version<'3.7'
+	scipy>=1.2.1;python_version>='3.7'
+	scipy==1.2.*;python_version<'3.7'
 	torch>=1.1.0
 	setuptools>=38.3
 	cloudpickle>=0.8
 	joblib>=0.13.2
+	tensorboard>=1.14
 tests_require = 
-	pytest
+	pytest>=4.6
 
 [test]
 addopts = --verbose
 extras = True
 
 [tool:pytest]
 addopts =
```

### Comparing `deepCR-0.2.1rc0/deepCR/test/test_model.py` & `deepCR-0.3.1/deepCR/test/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 import pytest
 
 from deepCR.model import deepCR
 
 
 def test_deepCR_serial():
 
-    mdl = deepCR(mask='ACS-WFC-F606W-2-32', device='CPU')
+    mdl = deepCR(mask='ACS-WFC', device='CPU')
     in_im = np.ones((299, 299))
-    out = mdl.clean(in_im)
+    out = mdl.clean(in_im, inpaint=True)
     assert (out[0].shape, out[1].shape) == (in_im.shape, in_im.shape)
     out = mdl.clean(in_im, inpaint=False)
     assert out.shape == in_im.shape
 
 
 def test_deepCR_parallel():
 
-    mdl = deepCR(mask='ACS-WFC-F606W-2-32', device='CPU')
+    mdl = deepCR(mask='ACS-WFC', device='CPU')
     in_im = np.ones((299, 299))
-    out = mdl.clean(in_im, parallel=True)
+    out = mdl.clean(in_im, n_jobs=-1, inpaint=True)
     assert (out[0].shape, out[1].shape) == (in_im.shape, in_im.shape)
 
     # Is the serial runtime slower than the parallel runtime on a big image?
     # Make sure we have a lot of cores
     # otherwise this can fail on Travis b/c we only get 1-2 at test time.
     if os.cpu_count() > 2:
         in_im = np.ones((1024, 1024))
         t0 = time.time()
-        out = mdl.clean(in_im, inpaint=False, parallel=True)
+        out = mdl.clean(in_im, inpaint=False, n_jobs=4, patch=256)
         par_runtime = time.time() - t0
         assert out.shape == in_im.shape
 
         t0 = time.time()
-        out = mdl.clean(in_im, inpaint=False, parallel=False)
+        out = mdl.clean(in_im, inpaint=False)
         ser_runtime = time.time() - t0
         assert par_runtime < ser_runtime
 
 
 def test_seg():
-    mdl = deepCR(mask='ACS-WFC-F606W-2-32', inpaint='ACS-WFC-F606W-2-32', device='CPU')
+    mdl = deepCR(mask='ACS-WFC', inpaint='ACS-WFC-F606W-2-32', device='CPU')
     in_im = np.ones((300, 500))
-    out = mdl.clean(in_im, segment=True)
+    out = mdl.clean(in_im, segment=True, inpaint=True)
     assert (out[0].shape, out[1].shape) == (in_im.shape, in_im.shape)
     out = mdl.clean(in_im, inpaint=False, segment=True)
     assert out.shape == in_im.shape
 
 
 if __name__ == '__main__':
     test_seg()
```

### Comparing `deepCR-0.2.1rc0/deepCR/test/test_train.py` & `deepCR-0.3.1/deepCR/test/test_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from deepCR.training import train
 
 
 def test_train():
     inputs = np.zeros((6, 64, 64))
     sky = np.ones(6)
-    trainer = train(image=inputs, mask=inputs, sky=sky, aug_sky=[-0.9, 10], verbose=False, epoch=2, save_after=10)
+    trainer = train(image=inputs, mask=inputs, sky=sky, mode='pair', aug_sky=[-0.9, 10], verbose=False, epoch=2, save_after=10)
     trainer.train()
     filename = trainer.save()
     trainer.load(filename)
     trainer.train_phase1(1)
     assert trainer.epoch_mask == 3
 
 
@@ -25,15 +25,15 @@
 
     var = np.zeros((2, 64, 64))
     for i in range(6):
         np.save(cwd + 'temp/image/%d.npy'%i, var)
         np.save(cwd + 'temp/dark/%d.npy'%i, var)
     image_list = [cwd + 'temp/image/' + f for f in os.listdir(cwd + 'temp/image')]
     dark_list = [cwd + 'temp/dark/' + f for f in os.listdir(cwd + 'temp/dark')]
-    trainer = train(image=image_list, mask=dark_list, sky=100, aug_sky=[-0.9, 10], aug_img=[0.5, 5],
+    trainer = train(image=image_list, mask=dark_list, mode='simulate', sky=100, aug_sky=[-0.9, 10], aug_img=[0.5, 5],
                     n_mask_train=2, n_mask_val=1, epoch=2, verbose=False)
     trainer.train()
     filename = trainer.save()
     trainer.load(filename)
     trainer.train_phase1(1)
     assert trainer.epoch_mask == 3
```

### Comparing `deepCR-0.2.1rc0/deepCR/test/test_evaluate.py` & `deepCR-0.3.1/deepCR/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/deepCR/test/test_dataset.py` & `deepCR-0.3.1/deepCR/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/deepCR/util.py` & `deepCR-0.3.1/deepCR/util.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/deepCR/unet.py` & `deepCR-0.3.1/deepCR/unet.py`

 * *Files identical despite different names*

### Comparing `deepCR-0.2.1rc0/deepCR/model.py` & `deepCR-0.3.1/deepCR/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """main module to instantiate deepCR models and use them
 """
 from os import path, mkdir
 import math
 import shutil
+import secrets
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import from_numpy
 from joblib import Parallel, delayed
 from joblib import dump, load
@@ -17,15 +18,15 @@
 from learned_models import mask_dict, inpaint_dict, default_model_path
 
 __all__ = ['deepCR']
 
 
 class deepCR():
 
-    def __init__(self, mask='ACS-WFC-F606W-2-32', inpaint=None, device='CPU', hidden=32):
+    def __init__(self, mask='ACS-WFC', inpaint=None, device='CPU', hidden=32):
 
         """
             Instantiation of deepCR with specified model configurations
 
         Parameters
         ----------
         mask : str
@@ -78,130 +79,104 @@
             self.inpaintNet.eval()
             for p in self.inpaintNet.parameters():
                 p.required_grad = False
         else:
             self.inpaintNet = None
 
         # Unused features to be implemented in a future version
-        self.norm = False
+        self.norm = True if mask == 'WFC3-UVIS' else False
         self.percentile = None
         self.median = None
         self.std = None
 
-    def clean(self, img0, threshold=0.5, inpaint=True, binary=True, segment=False,
-              patch=256, parallel=False, n_jobs=-1):
+    def clean(self, img0, threshold=0.5, inpaint=False, binary=True, segment=True,
+              patch=1024, n_jobs=1):
         """
             Identify cosmic rays in an input image, and (optionally) inpaint with the predicted cosmic ray mask
         :param img0: (np.ndarray) 2D input image conforming to model requirements. For HST ACS/WFC, must be from
         _flc.fits and in units of electrons in native resolution.
         :param threshold: (float; [0, 1]) applied to probabilistic mask to generate binary mask
         :param inpaint: (bool) return clean, inpainted image only if True
         :param binary: return binary CR mask if True. probabilistic mask if False
         :param segment: (bool) if True, segment input image into chunks of patch * patch before performing CR rejection.
           Used for memory control.
         :param patch: (int) Use 256 unless otherwise required. if segment==True, segment image into chunks of
           patch * patch.
-        :param parallel: (bool) run in parallel if True and segment==True
-        :param n_jobs: (int) number of jobs to run in parallel, passed to `joblib.` Beware of memory overflow for
-          larger n_jobs.
+        :param n_jobs: (int) number of jobs to run in parallel, passed to `joblib.` default: 1.
         :return: CR mask and (optionally) clean inpainted image
         """
 
         # data pre-processing
 
-        inpaint = inpaint and binary
-
         img0 = img0.astype(np.float32) / self.scale
         img0 = img0.copy()
         if self.norm:
-            limit = np.percentile(img0, self.percentile)
-            clip = img0[img0 < limit]
-            self.median = np.percentile(clip, 50)
-            self.std = clip.std()
+            self.median = img0.mean()
+            self.std = img0.std()
             img0 -= self.median
             img0 /= self.std
 
-
-        if not segment and not parallel:
+        if not segment and n_jobs == 1:
             return self.clean_(img0, threshold=threshold,
                                inpaint=inpaint, binary=binary)
         else:
-            if not parallel:
+            if n_jobs == 1:
                 return self.clean_large(img0, threshold=threshold,
                                inpaint=inpaint, binary=binary, patch=patch)
             else:
                 return self.clean_large_parallel(img0, threshold=threshold,
                                inpaint=inpaint, binary=binary, patch=patch,
                                n_jobs=n_jobs)
 
     def clean_(self, img0, threshold=0.5, inpaint=True, binary=True):
 
         """
             given input image
             return cosmic ray mask and (optionally) clean image
             mask could be binary or probabilistic
-        :param img0: (np.ndarray) 2D input image
+        :param img0: (np.ndarray) 2D input image with optional batch dimension
         :param threshold: for creating binary mask from probabilistic mask
         :param inpaint: return clean image only if True
         :param binary: return binary mask if True. probabilistic mask otherwise.
         :return: CR mask and (optionally) clean inpainted image
         """
 
+        # pad to be divisible by 4
         shape = img0.shape
-        pad_x = 4 - shape[0] % 4
-        pad_y = 4 - shape[1] % 4
-        if pad_x == 4:
-            pad_x = 0
-        if pad_y == 4:
-            pad_y = 0
+        pad_x = - shape[0] % 4
+        pad_y = - shape[1] % 4
         img0 = np.pad(img0, ((pad_x, 0), (pad_y, 0)), mode='constant')
 
-        shape = img0.shape[-2:]
-        img0 = from_numpy(img0).type(self.dtype).view(1, -1, shape[0], shape[1])
+        img0 = from_numpy(img0).type(self.dtype).view(1, 1, *img0.shape)
         mask = self.maskNet(img0)
-
-        if not binary:
-            return mask.detach().cpu().view(shape[0], shape[1]).numpy()[pad_x:, pad_y:]
-
         binary_mask = (mask > threshold).type(self.dtype)
+        if binary:
+            return_mask = binary_mask.detach().squeeze().cpu().numpy()[pad_x:, pad_y:]
+        else:
+            return_mask = mask.detach().squeeze().cpu().numpy()[pad_x:, pad_y:]
 
-        if inpaint:
+        if not inpaint:
+            return return_mask
+        else:
             if self.inpaintNet is not None:
                 cat = torch.cat((img0 * (1 - binary_mask), binary_mask), dim=1)
-                img1 = self.inpaintNet(cat)
-                img1 = img1.detach()
+                img1 = self.inpaintNet(cat).detach()
                 inpainted = img1 * binary_mask + img0 * (1 - binary_mask)
-                binary_mask = binary_mask.detach().cpu().view(shape[0], shape[1]).numpy()
-                inpainted = inpainted.detach().cpu().view(shape[0], shape[1]).numpy()
+                inpainted = inpainted.detach().cpu().squeeze().numpy()
             else:
-                binary_mask = binary_mask.detach().cpu().view(shape[0], shape[1]).numpy()
-                img0 = img0.detach().cpu().view(shape[0], shape[1]).numpy()
+                binary_mask = binary_mask.detach().cpu().squeeze().numpy()
+                img0 = img0.detach().cpu().squeeze().numpy()
                 img1 = medmask(img0, binary_mask)
                 inpainted = img1 * binary_mask + img0 * (1 - binary_mask)
-            if binary:
-                inpainted = inpainted[pad_x:, pad_y:]
-                if self.norm:
-                    inpainted *= self.std
-                    inpainted += self.median
-                return binary_mask[pad_x:, pad_y:], inpainted * self.scale
-            else:
-                mask = mask.detach().cpu().view(shape[0], shape[1]).numpy()
-                inpainted = inpainted[pad_x:, pad_y:]
-                if self.norm:
-                    inpainted *= self.std
-                    inpainted += self.median
-                return mask[pad_x:, pad_y:], inpainted * self.scale
+            if self.norm:
+                inpainted *= self.std
+                inpainted += self.median
+
+            return return_mask, inpainted[pad_x:, pad_y:] * self.scale
 
-        else:
-            if binary:
-                binary_mask = binary_mask.detach().cpu().view(shape[0], shape[1]).numpy()
-                return binary_mask[pad_x:, pad_y:]
-            else:
-                mask = mask.detach().cpu().view(shape[0], shape[1]).numpy()
-                return mask[pad_x:, pad_y:]
 
     def clean_large_parallel(self, img0, threshold=0.5, inpaint=True, binary=True,
                     patch=256, n_jobs=-1):
         """
             given input image
             return cosmic ray mask and (optionally) clean image
             mask could be binary or probabilistic
@@ -210,19 +185,20 @@
         :param inpaint: return clean image only if True
         :param binary: return binary mask if True. probabilistic mask otherwise.
         :param patch: (int) Use 256 unless otherwise required. patch size to run deepCR on.
         :param n_jobs: (int) number of jobs to run in parallel, passed to `joblib.` Beware of memory overflow for
           larger n_jobs.
         :return: CR mask and (optionally) clean inpainted image
         """
-        folder = './joblib_memmap'
+        folder = './joblib_memmap_' + secrets.token_hex(3)
         try:
             mkdir(folder)
         except FileExistsError:
-            pass
+            folder = './joblib_memmap_' + secrets.token_hex(3)
+            mkdir(folder)
 
         im_shape = img0.shape
         img0_dtype = img0.dtype
         hh = int(math.ceil(im_shape[0]/patch))
         ww = int(math.ceil(im_shape[1]/patch))
 
         img0_filename_memmap = path.join(folder, 'img0_memmap')
```

### Comparing `deepCR-0.2.1rc0/deepCR/dataset.py` & `deepCR-0.3.1/deepCR/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 from torch.utils.data import Dataset
+import os
 
 __all__ = ['dataset', 'DatasetSim']
 
 
 class DatasetSim(Dataset):
     def __init__(self, image, cr, sky=None, aug_sky=(0, 0), aug_img=(1, 1), noise=False, saturation=1e5,
-                 n_mask=1, norm=False, percentile_limit=50, part=None, f_val=0.1, seed=1):
+                 n_mask=1, norm=False, percentile_limit=100, part=None, f_val=0.1, seed=1):
         """ custom pytorch dataset class to load deepCR-mask training data
         :param image: list of complete path to npy arrays, each containing one 2D image
         :param cr: list of complete path to npy arrays, each containing one 2D mask
         :param sky: np.ndarray [N,] or float, sky background level
         :param aug_sky: (float, float). If sky is provided, use random sky background in the range
           [aug_sky[0] * sky, aug_sky[1] * sky]. This serves as a regularizers to allow the trained model to adapt to a
           wider range of sky background or equivalently exposure time. Remedy the fact that exposure time in the
@@ -38,15 +39,15 @@
         assert f_val < 1 and f_val > 0
         f_train = 1 - f_val
         if part == 'train':
             s = np.s_[:int(self.len_image * f_train)]
             s_cr = np.s_[:int(self.len_mask * f_train)]
         elif part == 'val':
             s = np.s_[int(self.len_image * f_train):]
-            s_cr = np.s_[:int(self.len_mask * f_train)]
+            s_cr = np.s_[int(self.len_mask * f_train):]
         else:
             s = np.s_[0:]
             s_cr = np.s_[0:]
 
         if sky is None:
             sky = np.zeros(self.len_image)
         elif type(sky) != np.ndarray:
@@ -68,23 +69,23 @@
         Generate cosmic ray images from stacked dark frames.
         Sample self.n_mask number of cr masks and add them together.
         :return: (cr_img, cr_mask): sampled and added dark image containing only cr and accumulative cr mask
         """
         cr_id = np.random.randint(0, self.len_mask, self.n_mask)
         crs = []; masks = []
         for i in cr_id:
-            arr = np.load(self.cr[i])
+            arr = np.load(self.cr[i]) if type(self.cr[i]) == str else self.cr[i]
             crs.append(arr[0][None,:])
             masks.append(arr[1][None,:])
         masks = np.concatenate(masks).sum(axis=0) > 0
         crs = np.concatenate(crs).sum(axis=0)
         return crs, masks
 
     def get_image(self, i):
-        data = np.load(self.image[i])
+        data = np.load(self.image[i]) if type(self.image[i]) == str else self.image[i]
         if len(data.shape) == 3:
             return data[0], data[1]
         else:
             return data, np.zeros_like(data)
 
     def __len__(self):
         return self.len_image
@@ -117,17 +118,18 @@
 
         return img, mask, ignore
 
 
 class dataset(Dataset):
     def __init__(self, image, mask, ignore=None, sky=None, aug_sky=[0, 0], part=None, f_val=0.1, seed=1):
         """ custom pytorch dataset class to load deepCR-mask training data
-        :param image: image with CR
-        :param mask: CR mask
-        :param ignore: loss mask, e.g., bad pixel, saturation, etc.
+        :param image: image with CR. Could be (N, W, H) array or list of path to single (W, H) images.
+        :param mask: CR mask. Could be (N, W, H) array or list of path to single (W, H) images.
+        :param ignore: (optional) loss mask, e.g., bad pixel, saturation, etc. Could be (N, W, H) array or list
+        of path to single (W, H) images
         :param sky: (np.ndarray) [N,] sky background level
         :param aug_sky: [float, float]. If sky is provided, use random sky background in the range
           [aug_sky[0] * sky, aug_sky[1] * sky]. This serves as a regularizers to allow the trained model to adapt to a
           wider range of sky background or equivalently exposure time. Remedy the fact that exposure time in the
           training set is discrete and limited.
         :param part: either 'train' or 'val'. split by 0.8, 0.2
         :param f_val: percentage of dataset reserved as validation set.
@@ -140,17 +142,17 @@
         f_train = 1 - f_val
         if sky is None:
             sky = np.zeros_like(image)
         if ignore is None:
             ignore = np.zeros_like(image)
 
         if part == 'train':
-            s = np.s_[:int(len * f_train)]
+            s = np.s_[:max(1, int(len * f_train))]
         elif part == 'val':
-            s = np.s_[int(len * f_train):]
+            s = np.s_[min(len - 1, int(len * f_train)):]
         else:
             s = np.s_[0:]
 
         self.image = image[s]
         self.mask = mask[s]
         self.ignore = ignore[s]
         self.sky = sky[s]
@@ -158,8 +160,76 @@
         self.aug_sky = aug_sky
 
     def __len__(self):
         return self.image.shape[0]
 
     def __getitem__(self, i):
         a = (self.aug_sky[0] + np.random.rand() * (self.aug_sky[1] - self.aug_sky[0])) * self.sky[i]
-        return self.image[i] + a, self.mask[i], self.ignore[i]
+        ignore = self.ignore[i] if type(self.ignore[i]) != str else np.load(self.ignore[i])
+        if type(self.image[i]) == str:
+            return np.load(self.image[i]) + a, np.load(self.mask[i]), ignore
+        else:
+            return self.image[i] + a, self.mask[i], ignore
+
+
+class PairedDatasetImagePath(Dataset):
+    def __init__(self, paths, skyaug_min=0, skyaug_max=0, part=None, f_val=0.1, seed=1):
+        """ custom pytorch dataset class to load deepCR-mask training data
+        :param paths: (list) list of file paths to (3, W, H) images: image, cr, ignore.
+        :param skyaug_min: [float, float]. If sky is provided, use random sky background in the range
+          [aug_sky[0] * sky, aug_sky[1] * sky]. This serves as a regularizers to allow the trained model to adapt to a
+          wider range of sky background or equivalently exposure time. Remedy the fact that exposure time in the
+          training set is discrete and limited.
+        :param skyaug_min: float. subtract maximum amount of abs(skyaug_min) * sky_level as data augmentation
+        :param skyaug_max: float. add maximum amount of skyaug_max * sky_level as data augmentation
+        :param part: either 'train' or 'val'.
+        :param f_val: percentage of dataset reserved as validation set.
+        :param seed: fix numpy random seed to seed, for reproducibility.
+        """
+        assert 0 < f_val < 1
+        np.random.seed(seed)
+        n_total = len(paths)
+        n_train = int(n_total * (1 - f_val)) #int(len * (1 - f_val)) JK
+
+        if part == 'train':
+            s = np.s_[:max(1, n_train)]
+        elif part == 'val':
+            s = np.s_[min(n_total - 1, n_train):]
+        else:
+            s = np.s_[0:]
+
+        self.paths = paths[s]
+        self.skyaug_min = skyaug_min
+        self.skyaug_max = skyaug_max
+
+    def __len__(self):
+        return len(self.paths)
+
+    def get_skyaug(self, i):
+        """
+        Return the amount of background flux to be added to image
+        The original sky background should be saved in sky.npy in each sub-directory
+        Otherwise always return 0
+        :param i: index of file
+        :return: amount of flux to add to image
+        """
+        path = os.path.split(self.paths[i])[0]
+        sky_path = os.path.join(path, 'sky.npy') #JK
+        if os.path.isfile(sky_path):
+            f_img = self.paths[i].split('/')[-1]
+            sky_idx = int(f_img.split('_')[0])
+            sky = np.load(sky_path)[sky_idx-1]
+            return sky * np.random.uniform(self.skyaug_min, self.skyaug_max)
+        else:
+            return 0
+
+    def __getitem__(self, i):
+        data = np.load(self.paths[i])
+        image = data[0]
+        mask = data[1]
+        if data.shape[0] == 3:
+            ignore = data[2]
+        else:
+            ignore = np.zeros_like(data[0])
+        # try:#JK
+        skyaug = self.get_skyaug(i)
+        return image + skyaug, mask, ignore
```

### Comparing `deepCR-0.2.1rc0/deepCR/parts.py` & `deepCR-0.3.1/deepCR/parts_batchnorm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 class outconv(nn.Module):
     def __init__(self, in_ch, out_ch):
         super(type(self), self).__init__()
         self.conv = nn.Conv2d(in_ch, out_ch, 1)
 
     def forward(self, x):
         x = self.conv(x)
-        return x
+        return x
```

### Comparing `deepCR-0.2.1rc0/deepCR/evaluate.py` & `deepCR-0.3.1/deepCR/evaluate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from tqdm import tqdm as tqdm
 
 from deepCR.util import maskMetric
-from deepCR.dataset import dataset, DatasetSim
+from deepCR.dataset import dataset, DatasetSim, PairedDatasetImagePath
 from skimage.morphology import disk, dilation
 import astroscrappy.astroscrappy as lac
 
 
 __all__ = ['roc', 'roc_lacosmic']
 
 
@@ -65,34 +65,39 @@
     FPR = FP / (FP + TN)
     TPR1 = TP1 / (TP1 + FN1)
     FPR1 = FP1 / (FP1 + TN1)
 
     return (TPR * 100, FPR * 100), (TPR1 * 100, FPR1 * 100)
 
 
-def roc(model, image, mask, ignore=None, sky=None, n_mask=1, seed=1, thresholds=np.linspace(0.001, 0.999, 500),
+def roc(model, image, mask=None, ignore=None, mode='pair', sky=None, n_mask=1, seed=1, thresholds=np.linspace(0.001, 0.999, 500),
         dilate=False, rad=1):
     """ evaluate model on test set with the ROC curve
 
     :param model: deepCR object
     :param image: np.ndarray((N, W, H)) image array
     :param mask: np.ndarray((N, W, H)) CR mask array
     :param ignore: np.ndarray((N, W, H)) bad pixel array incl. saturation, etc.
     :param thresholds: np.ndarray(N) FPR grid on which to evaluate ROC curves
     :return: np.ndarray(N), np.ndarray(N): TPR and FPR
     """
     kernel = None
     if dilate:
         kernel = disk(rad)
-    if type(image) == np.ndarray and len(image.shape) == 3:
-        data = dataset(image, mask, ignore)
-    elif type(image[0]) == str:
-        data = DatasetSim(image, mask, sky=sky, n_mask=n_mask, seed=seed)
+    if mode == 'pair':
+        if type(image) == np.ndarray and len(image.shape) == 3:
+            data = dataset(image, mask, ignore)
+        elif type(image[0]) == str or type(image[0]) == np.str_:
+            data = PairedDatasetImagePath(image, seed=seed)
+        else:
+            raise TypeError('Input must be numpy data arrays or list of file paths!')
+    elif mode == 'simulate':
+        print('simulate mode will be implemented')
     else:
-        raise TypeError('Input must be numpy data arrays or list of file paths!')
+        raise ValueError('Mode must be either pair or simulate')
     (tpr, fpr), (tpr_dilate, fpr_dilate) = _roc(model, data, thresholds=thresholds, dilate=kernel)
     if dilate:
         return (tpr, fpr), (tpr_dilate, fpr_dilate)
     else:
         return tpr, fpr
```

### Comparing `deepCR-0.2.1rc0/deepCR/training.py` & `deepCR-0.3.1/deepCR/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.autograd import Variable
 from torch.utils.data import DataLoader
 from torch.optim.lr_scheduler import ReduceLROnPlateau
+from torch.utils.tensorboard import SummaryWriter
 
 from deepCR.util import maskMetric
-from deepCR.dataset import dataset, DatasetSim
+from deepCR.dataset import dataset, DatasetSim, PairedDatasetImagePath
 from deepCR.unet import WrappedModel, UNet2Sigmoid
 
 __all__ = 'train'
 
 
 class VoidLRScheduler:
     def __init__(self):
@@ -29,25 +30,28 @@
 
     def step(self):
         pass
 
 
 class train:
 
-    def __init__(self, image, mask, ignore=None, sky=None, aug_sky=(0, 0), aug_img=(1, 1), noise=False, saturation=1e5,
+    def __init__(self, image, mask=None, ignore=None, sky=None, mode='pair', aug_sky=(0, 0), aug_img=(1, 1), noise=False, saturation=1e5,
                  n_mask_train=1, n_mask_val=1, norm=False, percentile_limit=50, name='model', hidden=32, epoch=50,
                  epoch_phase0=None, batch_size=16, lr=0.005, auto_lr_decay=True, lr_decay_patience=4,
                  lr_decay_factor=0.1, save_after=1e5, plot_every=10, verbose=True, use_tqdm=False,
                  use_tqdm_notebook=False, directory='./'):
 
         """ This is the class for training deepCR-mask.
-        :param image: np.ndarray (N*W*W) training data: image array with CR.
-        :param mask: np.ndarray (N*W*W) training data: CR mask array
+        :param image: np.ndarray (N*W*W) of CR affected images or list of npy arrays of shape (2or3,W,W), where
+        the 1st dim is CR affect image, 2nd dim is CR mask, (optional) 3rd dimension is ignore mask.
+        See documentation: training tutorial.
+        :param mask: np.ndarray (N*W*W) training data: CR mask array.
         :param ignore: training data: Mask for taking loss. e.g., bad pixel, saturation, etc.
-        :param sky: np.ndarray (N,) (optional) sky background
+        :param sky: np.ndarray (N,) (optional) sky background. When param: iamge is list to npy files, provide sky level
+        as sky.npy in each image subdirectory (see documentation: training tutorial).
         :param aug_sky: [float, float]. If sky is provided, use random sky background in the range
           [aug_sky[0] * sky, aug_sky[1] * sky]. This serves as a regularizers to allow the trained model to adapt to a
           wider range of sky background or equivalently exposure time. Remedy the fact that exposure time in the
           training set is discrete and limited.
         :param n_mask: number of dark images to sample to create one cosmic ray image and mask
         :param name: model name. model saved to name_epoch.pth
         :param hidden: number of channels for the first convolution layer. default: 50
@@ -74,26 +78,28 @@
             gpu = False
             print('No GPU detected on this device! Training on CPU.')
 
         if sky is None and aug_sky != (0, 0):
             raise AttributeError('Var (sky) is required for sky background augmentation!')
         if ignore is None:
             ignore = np.zeros_like(image)
-        if type(image) == np.ndarray and len(image.shape) == 3:
-            assert image.shape == mask.shape == ignore.shape
-            assert image.shape[1] == image.shape[2]
-            data_train = dataset(image, mask, ignore, sky, part='train', aug_sky=aug_sky)
-            data_val = dataset(image, mask, ignore, sky, part='val', aug_sky=aug_sky)
-        elif type(image[0]) == str:
+        if mode == 'pair':
+            if type(image[0]) == str or type(image[0]) == np.str_:
+                data_train = PairedDatasetImagePath(image, aug_sky[0], aug_sky[1], part='train')
+                data_val = PairedDatasetImagePath(image, aug_sky[0], aug_sky[1], part='val')
+            else:
+                data_train = dataset(image, mask, ignore, sky, part='train', aug_sky=aug_sky)
+                data_val = dataset(image, mask, ignore, sky, part='val', aug_sky=aug_sky)
+        elif mode == 'simulate':
             data_train = DatasetSim(image, mask, sky, aug_sky=aug_sky, aug_img=aug_img, saturation=saturation,
                                     norm=norm, percentile_limit=percentile_limit, part='train', noise=noise, n_mask=n_mask_train)
             data_val = DatasetSim(image, mask, sky, aug_sky=aug_sky, aug_img=aug_img, saturation=saturation,
                                   norm=norm, percentile_limit=percentile_limit, part='val', noise=noise, n_mask=n_mask_val)
         else:
-            raise TypeError('Input must be numpy data arrays or list of file paths!')
+            raise TypeError('Mode must be one of pair or simulate!')
 
         self.TrainLoader = DataLoader(data_train, batch_size=batch_size, shuffle=True, num_workers=8)
         self.ValLoader = DataLoader(data_val, batch_size=batch_size, shuffle=False, num_workers=8)
         self.shape = data_train[0][0].shape[1]
         self.name = name
 
         if gpu:
@@ -107,15 +113,14 @@
             self.network = WrappedModel(UNet2Sigmoid(1,1,hidden))
             self.network.type(self.dtype)
 
         self.optimizer = optim.Adam(self.network.parameters(), lr=lr)
         if auto_lr_decay:
             self.lr_scheduler = ReduceLROnPlateau(self.optimizer, factor=lr_decay_factor, patience=lr_decay_patience,
                                                   cooldown=2, verbose=True, threshold=0.005)
-
         else:
             self.lr_scheduler = VoidLRScheduler()
         self.lr = lr
         self.BCELoss = nn.BCELoss()
         self.validation_loss = []
         self.epoch_mask = 0
         self.save_after = save_after
@@ -131,26 +136,30 @@
 
         if use_tqdm_notebook:
             self.tqdm = tqdm_notebook
         else:
             self.tqdm = tqdm
         self.disable_tqdm = not (use_tqdm_notebook or use_tqdm)
 
+        # tensorboard to record and visualize training log (require pytorch 1.1 and up)
+        self.writer = SummaryWriter(log_dir=directory)
+
     def set_input(self, img0, mask, ignore):
         """
         :param img0: input image
         :param mask: CR mask
         :param ignore: loss mask
         :return: None
         """
-        self.img0 = Variable(img0.type(self.dtype)).view(-1, 1, self.shape, self.shape)
-        self.mask = Variable(mask.type(self.dtype)).view(-1, 1, self.shape, self.shape)
-        self.ignore = Variable(ignore.type(self.dtype)).view(-1, 1, self.shape, self.shape)
+        img0 = (img0 - img0.mean())/img0.std()
+        self.img0 = Variable(img0.type(self.dtype)).view(-1,1, self.shape, self.shape)
+        self.mask = Variable(mask.type(self.dtype)).view(-1,1, self.shape, self.shape)
+        self.ignore = Variable(ignore.type(self.dtype)).view(-1,1, self.shape, self.shape)
 
-    def validate_mask(self):
+    def validate_mask(self, epoch=None):
         """
         :return: validation loss. print TPR and FPR at threshold = 0.5.
         """
         torch.random.manual_seed(0)
         np.random.seed(0)
         lmask = 0; count = 0
         metric = np.zeros(4)
@@ -164,14 +173,19 @@
             metric += maskMetric(self.pdt_mask.reshape(-1, self.shape, self.shape).detach().cpu().numpy() > 0.5, dat[1].numpy())
         lmask /= count
         TP, TN, FP, FN = metric[0], metric[1], metric[2], metric[3]
         TPR = TP / (TP + FN)
         FPR = FP / (FP + TN)
         if self.verbose:
             print('[TPR=%.3f, FPR=%.3f] @threshold = 0.5' % (TPR, FPR))
+        if epoch:
+            self.writer.add_scalar('TPR', TPR, epoch)
+            self.writer.add_scalar('FPR', FPR, epoch)
+            self.writer.add_scalar('validate_loss', lmask, epoch)
+
         return (lmask)
 
     def train(self):
         """ call this function to start training network
         :return: None
         """
         if self.verbose:
@@ -198,15 +212,15 @@
             self.epoch_mask += 1
 
             if self.epoch_mask % self.every == 0:
                 self.plot_example()
 
             if self.verbose:
                 print('----------- epoch = %d -----------' % self.epoch_mask)
-            val_loss = self.validate_mask()
+            val_loss = self.validate_mask(epoch)
             self.validation_loss.append(val_loss)
             if self.verbose:
                 print('loss = %.4f' % (self.validation_loss[-1]))
             if (np.array(self.validation_loss)[-1] == np.array(
                     self.validation_loss).min() and self.epoch_mask > self.save_after):
                 filename = self.save()
                 if self.verbose:
@@ -224,39 +238,42 @@
             self.epoch_mask += 1
 
             if self.epoch_mask % self.every==0:
                 self.plot_example()
 
             if self.verbose:
                 print('----------- epoch = %d -----------' % self.epoch_mask)
-            valLossMask = self.validate_mask()
+            valLossMask = self.validate_mask(epoch)
             self.validation_loss.append(valLossMask)
             if self.verbose:
                 print('loss = %.4f' % (self.validation_loss[-1]))
             if (np.array(self.validation_loss)[-1] == np.array(
                     self.validation_loss).min() and self.epoch_mask > self.save_after):
                 filename = self.save()
                 if self.verbose:
                     print('Saved to {}.pth'.format(filename))
             self.lr_scheduler.step(self.validation_loss[-1])
             if self.verbose:
                 print('')
 
     def plot_example(self):
-        plt.figure(figsize=(10, 30))
+        plt.figure(figsize=(30,10))
         plt.subplot(131)
         plt.imshow(np.log(self.img0[0, 0].detach().cpu().numpy()), cmap='gray')
         plt.title('epoch=%d' % self.epoch_mask)
         plt.subplot(132)
         plt.imshow(self.pdt_mask[0, 0].detach().cpu().numpy() > 0.5, cmap='gray')
         plt.title('prediction > 0.5')
         plt.subplot(133)
         plt.imshow(self.mask[0, 0].detach().cpu().numpy(), cmap='gray')
         plt.title('ground truth')
-        plt.show()
+        filename = 'epoch%d' % self.epoch_mask
+        print('Save trainplot')
+        plt.savefig(self.directory+self.name+filename+'trainplot.png')
+        #plt.show()
 
     def set_to_eval(self):
         self.network.eval()
 
     def optimize_network(self, dat):
         self.set_input(*dat)
         self.pdt_mask = self.network(self.img0)
@@ -274,15 +291,16 @@
         :return: None
         """
         plt.figure(figsize=(10,5))
         plt.plot(range(self.epoch_mask), self.validation_loss)
         plt.xlabel('epoch')
         plt.ylabel('loss')
         plt.title('Validation loss')
-        plt.show()
+        plt.savefig(self.directory+self.name+'trainplot.png')
+        #plt.show()
 
     def save(self):
         """ save trained network parameters to date_model_name_epoch*.pth
         :return: None
         """
         time = datetime.datetime.now()
         time = str(time)[:10]
```

### Comparing `deepCR-0.2.1rc0/LICENSE.txt` & `deepCR-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

