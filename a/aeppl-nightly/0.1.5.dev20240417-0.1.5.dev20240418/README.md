# Comparing `tmp/aeppl_nightly-0.1.5.dev20240417.tar.gz` & `tmp/aeppl_nightly-0.1.5.dev20240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl_nightly-0.1.5.dev20240417.tar", last modified: Wed Apr 17 00:29:43 2024, max compression
+gzip compressed data, was "aeppl_nightly-0.1.5.dev20240418.tar", last modified: Thu Apr 18 00:29:30 2024, max compression
```

## Comparing `aeppl_nightly-0.1.5.dev20240417.tar` & `aeppl_nightly-0.1.5.dev20240418.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:29:43.308529 aeppl_nightly-0.1.5.dev20240417/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-17 00:29:43.308529 aeppl_nightly-0.1.5.dev20240417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:29:43.308529 aeppl_nightly-0.1.5.dev20240417/aeppl/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-17 00:29:43.308529 aeppl_nightly-0.1.5.dev20240417/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:29:43.304529 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 00:29:43.000000 aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-17 00:29:43.308529 aeppl_nightly-0.1.5.dev20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:29:43.304529 aeppl_nightly-0.1.5.dev20240417/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-17 00:29:31.000000 aeppl_nightly-0.1.5.dev20240417/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24383 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30605 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 00:29:30.000000 aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 00:29:30.707375 aeppl_nightly-0.1.5.dev20240418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:29:30.703374 aeppl_nightly-0.1.5.dev20240418/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25605 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40106 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22582 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-18 00:29:24.000000 aeppl_nightly-0.1.5.dev20240418/versioneer.py
```

### Comparing `aeppl_nightly-0.1.5.dev20240417/LICENSE` & `aeppl_nightly-0.1.5.dev20240418/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/PKG-INFO` & `aeppl_nightly-0.1.5.dev20240418/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20240417
+Version: 0.1.5.dev20240418
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl_nightly-0.1.5.dev20240417/README.md` & `aeppl_nightly-0.1.5.dev20240418/README.md`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/abstract.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/censoring.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/convolutions.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/cumsum.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/dists.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/joint_logprob.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/logprob.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/mixture.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/printing.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/rewriting.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/scan.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/tensor.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/transforms.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl/utils.py` & `aeppl_nightly-0.1.5.dev20240418/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/PKG-INFO` & `aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.5.dev20240417
+Version: 0.1.5.dev20240418
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl_nightly-0.1.5.dev20240417/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl_nightly-0.1.5.dev20240418/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/setup.cfg` & `aeppl_nightly-0.1.5.dev20240418/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/setup.py` & `aeppl_nightly-0.1.5.dev20240418/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_abstract.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_censoring.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_composite_logprob.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_convolutions.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_cumsum.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_dist.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_joint_logprob.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_logprob.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_mixture.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_printing.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_rewriting.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_scan.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_tensor.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_transforms.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/tests/test_utils.py` & `aeppl_nightly-0.1.5.dev20240418/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl_nightly-0.1.5.dev20240417/versioneer.py` & `aeppl_nightly-0.1.5.dev20240418/versioneer.py`

 * *Files identical despite different names*
