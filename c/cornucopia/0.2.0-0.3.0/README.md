# Comparing `tmp/cornucopia-0.2.0.tar.gz` & `tmp/cornucopia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cornucopia-0.2.0.tar", last modified: Sat Jan 13 22:24:50 2024, max compression
+gzip compressed data, was "dist/cornucopia-0.3.0.tar", last modified: Fri Apr 19 14:35:23 2024, max compression
```

## Comparing `cornucopia-0.2.0.tar` & `cornucopia-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:50.000000 cornucopia-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-13 22:24:25.000000 cornucopia-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-01-13 22:24:50.000000 cornucopia-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-01-13 22:24:25.000000 cornucopia-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia/
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35934 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7703 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/baseutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/ctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/fov.py
--rw-r--r--   0 runner    (1001) docker     (127)    53527 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)    28788 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    13741 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/kspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    53175 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    22077 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/qmri.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/special.py
--rw-r--r--   0 runner    (1001) docker     (127)    24527 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/synth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_fov.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_kspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_qmri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/tests/test_run_synth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/b0.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/gmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    28180 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/morpho.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-01-13 22:24:25.000000 cornucopia-0.2.0/cornucopia/utils/warps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-13 22:24:50.000000 cornucopia-0.2.0/cornucopia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-13 22:24:25.000000 cornucopia-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-13 22:24:50.000000 cornucopia-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-13 22:24:25.000000 cornucopia-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-01-13 22:24:25.000000 cornucopia-0.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:23.000000 cornucopia-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1072 2024-04-19 14:34:58.000000 cornucopia-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-19 14:35:23.000000 cornucopia-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2424 2024-04-19 14:34:58.000000 cornucopia-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3224 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37285 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7703 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/baseutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6829 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/contrast.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/ctx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17279 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/fov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53495 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/geometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28788 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/intensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3491 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13741 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/kspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53175 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12813 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11111 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/psf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22077 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/qmri.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14270 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/random.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4432 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/special.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24527 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/synth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      632 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_contrast.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_fov.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4427 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_geometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5081 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_intensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1784 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_kspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6491 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3741 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3013 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_psf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3154 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_qmri.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1797 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/tests/test_run_synth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20219 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/b0.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11513 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10067 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/conv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4487 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/gmm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28180 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/indexing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4885 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3170 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/jit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9483 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/kernels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6418 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/morpho.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5801 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/padding.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10619 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/patch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9565 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/py.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1481 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16210 2024-04-19 14:34:58.000000 cornucopia-0.3.0/cornucopia/utils/warps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 14:35:23.000000 cornucopia-0.3.0/cornucopia.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-04-19 14:34:59.000000 cornucopia-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      965 2024-04-19 14:35:23.000000 cornucopia-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      203 2024-04-19 14:34:59.000000 cornucopia-0.3.0/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    83607 2024-04-19 14:34:59.000000 cornucopia-0.3.0/versioneer.py
```

### Comparing `cornucopia-0.2.0/LICENSE` & `cornucopia-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/PKG-INFO` & `cornucopia-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornucopia
-Version: 0.2.0
+Version: 0.3.0
 Summary: An abundance of augmentation layers
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/cornucopia
 Description: <picture align="center">
@@ -25,37 +25,40 @@
         
         Since gradients are not expected to backpropagate through its layers, it can
         theoretically be used within any dataloader pipeline,
         independent of the downstream learning framework (pytorch, tensorflow, jax, ...).
         
         ## Installation
         
-        
-        ## Installation
-        
         ### Dependencies
         
         - `pytorch >= 1.8`
         - `numpy`
         - `nibabel`
         - `torch-interpol`
         - `torch-distmap`
         
         ### Conda
         
         ```sh
         conda install cornucopia -c balbasty -c pytorch -c conda-forge
         ```
         
-        ### Pip
+        ### Pip (release)
         
         ```sh
         pip install cornucopia
         ```
         
+        ### Pip (dev)
+        
+        ```sh
+        pip install cornucopia@git+https://github.com/balbasty/cornucopia
+        ```
+        
         ## Documentation
         
         Read the [documentation](https://cornucopia.readthedocs.io) and in particular:
         - [installation](https://cornucopia.readthedocs.io/en/latest/install/)
         - [get started](https://cornucopia.readthedocs.io/en/latest/start/)
         - [examples](https://cornucopia.readthedocs.io/en/latest/examples/overview/)
         - [API](https://cornucopia.readthedocs.io/en/latest/api/overview/)
```

### Comparing `cornucopia-0.2.0/README.md` & `cornucopia-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,37 +16,40 @@
 
 Since gradients are not expected to backpropagate through its layers, it can
 theoretically be used within any dataloader pipeline,
 independent of the downstream learning framework (pytorch, tensorflow, jax, ...).
 
 ## Installation
 
-
-## Installation
-
 ### Dependencies
 
 - `pytorch >= 1.8`
 - `numpy`
 - `nibabel`
 - `torch-interpol`
 - `torch-distmap`
 
 ### Conda
 
 ```sh
 conda install cornucopia -c balbasty -c pytorch -c conda-forge
 ```
 
-### Pip
+### Pip (release)
 
 ```sh
 pip install cornucopia
 ```
 
+### Pip (dev)
+
+```sh
+pip install cornucopia@git+https://github.com/balbasty/cornucopia
+```
+
 ## Documentation
 
 Read the [documentation](https://cornucopia.readthedocs.io) and in particular:
 - [installation](https://cornucopia.readthedocs.io/en/latest/install/)
 - [get started](https://cornucopia.readthedocs.io/en/latest/start/)
 - [examples](https://cornucopia.readthedocs.io/en/latest/examples/overview/)
 - [API](https://cornucopia.readthedocs.io/en/latest/api/overview/)
```

### Comparing `cornucopia-0.2.0/cornucopia/base.py` & `cornucopia-0.3.0/cornucopia/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         - '' or False: A different transform is applied to each
             channel and each tensor.
     """
     def __init__(self, *, shared=False, **kwargs):
         super().__init__(**kwargs)
         self.shared = self._prepare_shared(shared)
 
-    def make_final(self, x, max_depth=float('inf'), *args, **kwargs):
+    def make_final(self, x, max_depth=float('inf')):
         if self.is_final or max_depth == 0:
             return self
         return NotImplemented
 
 
 class SpecialMixin:
     """Mixin for special transforms (i.e. transforms of transforms)"""
@@ -1064,41 +1064,75 @@
         return f'{type(self).__name__}({s})'
 
 
 class RandomizedTransform(NonFinalTransform):
     """
     Transform generated by randomizing some parameters of another transform.
 
+    !!! note "`ctx.randomize` is an alias for `RandomizedTransform`"
+
     !!! example "Gaussian noise with randomized variance"
         Object call
         ```python
         import cornucopia as cc
-        hypernoise = RandomizedTransform(cc.GaussianNoise, [cc.Uniform(0, 10)])
+        hypernoise = cc.RandomizedTransform(cc.GaussianNoise, [cc.Uniform()])
         img = hypernoise(img)
         ```
-        Functional call
+
+        Delayed call
         ```python
         import cornucopia as cc
-        hypernoise = cc.randomize(cc.GaussianNoise)(cc.Uniform(0, 10))
+        MyRandomNoise = cc.randomize(cc.GaussianNoise)
+        hypernoise = MyRandomNoise(cc.Uniform())
         img = hypernoise(img)
         ```
 
     """
 
-    def __init__(self, transform, sample, ksample=None,
+    class Delayed:
+        # Temproary parameter holder for delayed calls
+        def __init__(self, transform, **kwargs):
+            self.transform = transform
+            self.kwargs = kwargs
+
+        def __call__(self, *args, **kwargs):
+            return RandomizedTransform(
+                self.transform, args, kwargs, **self.kwargs)
+
+    def __new__(cls, *args, **kwargs):
+        if cls is RandomizedTransform:
+            return cls._base_new(*args, **kwargs)
+        return super().__new__(cls)
+
+    @classmethod
+    def _base_new(cls, transform, sample=tuple(), ksample=dict(),
+                  *, shared=False, **kwargs):
+        assert cls is RandomizedTransform
+        if not sample and not ksample:
+            # If no arguments are passed, it means that the user calls
+            # this in "delayed/functional" mode. In that case, we return
+            # a callable object that returns the constructed instance
+            # using the call-time arguments.
+            return cls.Delayed(transform, shared=shared, **kwargs)
+        # Otherwise, we're in object mode and we instantiate the
+        # randomized object.
+        return super().__new__(cls)
+
+    def __init__(self, transform, sample=tuple(), ksample=dict(),
                  *, shared=False, **kwargs):
         """
-
         Parameters
         ----------
         transform : callable(...) -> Transform
             A Transform subclass or a function that constructs a Transform.
         sample : [list or dict of] callable
             A collection of functions that generate parameter values provided
-            to `transform`.
+            to `transform`. Can be args-like or kwargs-like arguments.
+        ksample : dict[callable]
+            Must be kwargs-like arguments.
 
         Other Parameters
         ----------------
         shared : {'channels', 'tensors', 'channels+tensors', ''}
             Share random parameters across tensors and/or channels
         """
         super().__init__(shared=shared, **kwargs)
@@ -1126,13 +1160,11 @@
                            for k, f in self.ksample.items()})
         xform = self.subtransform(*args, **kwargs)
         xform = xform.make_final(x, max_depth-1)
         return xform
 
     def __repr__(self):
         if type(self) is RandomizedTransform:
-            try:
-                if issubclass(self.subtransform, Transform):
-                    return f'Randomized{self.subtransform.__name__}()'
-            except TypeError:
-                pass
+            xform = self.subtransform
+            if isinstance(xform, type) and issubclass(xform, Transform):
+                return f'Randomized{xform.__name__}()'
         return super().__repr__()
```

### Comparing `cornucopia-0.2.0/cornucopia/baseutils.py` & `cornucopia-0.3.0/cornucopia/baseutils.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/contrast.py` & `cornucopia-0.3.0/cornucopia/contrast.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/fov.py` & `cornucopia-0.3.0/cornucopia/fov.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,30 +4,31 @@
     'PermuteAxesTransform',
     'RandomPermuteAxesTransform',
     'PatchTransform',
     'RandomPatchTransform',
     'CropTransform',
     'PadTransform',
     'PowerTwoTransform',
+    'Rot90Transform',
+    'Rot180Transform',
+    'RandomRot90Transform',
 ]
-
 import math
 from random import shuffle
-from .base import FinalTransform, NonFinalTransform
+from .base import FinalTransform, NonFinalTransform, PerChannelTransform
 from .utils.py import ensure_list
 from .utils.padding import pad
-from .random import Uniform, RandKFrom, Sampler
+from .random import Uniform, RandKFrom, Sampler, RandInt, make_range
 
 
 class FlipTransform(FinalTransform):
     """Flip one or more axes"""
 
     def __init__(self, axis=None, **kwargs):
         """
-
         Parameters
         ----------
         axis : [list of] int
             Axes to flip. By default, flip all axes.
         """
         super().__init__(**kwargs)
         self.axis = axis
@@ -42,45 +43,50 @@
     def make_inverse(self):
         return self
 
 
 class RandomFlipTransform(NonFinalTransform):
     """Randomly flip one or more axes"""
 
-    def __init__(self, axes=None, **kwargs):
+    def __init__(self, axes=None, *, shared=True, **kwargs):
         """
-
         Parameters
         ----------
         axes : Sampler or [list of] int
             Axes that can be flipped (default: all)
+
+        Other Parameters
+        ----------------
         shared : {'channels', 'tensors', 'channels+tensors', ''}
             Apply the same flip to all channels and/or tensors
         """
         axes = kwargs.pop('axis', axes)
-        kwargs.setdefault('shared', True)
-        super().__init__(**kwargs)
+        super().__init__(shared=shared, **kwargs)
         self.axes = axes
 
     def make_final(self, x, max_depth=float('inf')):
         if max_depth == 0:
             return self
+        if 'channels' not in self.shared and len(x) > 1:
+            return PerChannelTransform(
+                [self.make_final(x[i:i+1], max_depth) for i in range(len(x))],
+                **self.get_prm()
+            ).make_final(x, max_depth-1)
         axes = self.axes or range(1, x.ndim)
         if not isinstance(axes, Sampler):
             rand_axes = RandKFrom(ensure_list(axes))
         rand_axes = rand_axes()
         return FlipTransform(rand_axes).make_final(x, max_depth-1)
 
 
 class PermuteAxesTransform(FinalTransform):
     """Permute axes"""
 
     def __init__(self, permutation=None, **kwargs):
         """
-
         Parameters
         ----------
         permutation : [list of] int
             Axes permutation. By default, reverse axes.
             Only applies to spatial axes, so axes are numbered [C, 0, 1, 2]
         """
         super().__init__(**kwargs)
@@ -101,38 +107,157 @@
         else:
             return self
 
 
 class RandomPermuteAxesTransform(NonFinalTransform):
     """Randomly permute axes"""
 
-    def __init__(self, axes=None, **kwargs):
+    def __init__(self, axes=None, *, shared=True, **kwargs):
         """
-
         Parameters
         ----------
         axes : [list of] int
             Axes that can be permuted (default: all)
+
+        Other Parameters
+        ----------------
         shared : {'channels', 'tensors', 'channels+tensors', ''}
             Apply the same permutation to all channels and/or tensors
         """
-        kwargs.setdefault('shared', True)
-        super().__init__(**kwargs)
+        super().__init__(shared=shared, **kwargs)
         self.axes = axes
 
     def make_final(self, x, max_depth=float('inf')):
         if max_depth == 0:
             return self
+        if 'channels' not in self.shared and len(x) > 1:
+            return PerChannelTransform(
+                [self.make_final(x[i:i+1], max_depth) for i in range(len(x))],
+                **self.get_prm()
+            ).make_final(x, max_depth-1)
         axes = list(self.axes or range(x.ndim-1))
         shuffle(axes)
         return PermuteAxesTransform(
             axes, **self.get_prm()
         ).make_final(x, max_depth-1)
 
 
+class Rot90Transform(FinalTransform):
+    """
+    Apply a 90 (or 180) rotation along one or several axes
+    """
+
+    def __init__(self, axis=0, negative=False, double=False, **kwargs):
+        """
+        Parameters
+        ----------
+        axis : int or list[int]
+            Rotation axis (indexing does not account for the channel axis)
+        negative : bool or list[bool]
+            Rotate by -90 deg instead of 90 deg
+        double : bool or list[bool]
+            Rotate be 180 instead of 90 (`negative` is then unused)
+        """
+        super().__init__(**kwargs)
+        self.axis = ensure_list(axis)
+        self.negative = ensure_list(negative, len(self.axis))
+        self.double = ensure_list(double, len(self.axis))
+
+    def xform(self, x):
+        # this implementation is suboptimal. We should fuse all transpose
+        # and all flips into a single "transpose + flip" operation so that
+        # a single allocation happens. This will be fine for now.
+
+        ndim = x.ndim - 1
+        axis = [1 + (ndim + a if a < 0 else a) for a in self.axis]
+        for ax, neg, dbl in zip(axis, self.negative, self.double):
+            if dbl:
+                if ndim == 2:
+                    dims = [1, 2]
+                else:
+                    assert ndim == 3
+                    dims = [d for d in (1, 2, 3) if d != ax]
+                x = x.flip(dims)
+            else:
+                if ndim == 2:
+                    dims = [1, 2]
+                else:
+                    assert ndim == 3
+                    dims = [d for d in (1, 2, 3) if d != ax]
+                x = x.transpose(*dims).flip(dims[1] if neg else dims[0])
+        return x
+
+
+class Rot180Transform(Rot90Transform):
+    """Apply a 180 deg rotation along one or several axes"""
+
+    def __init__(self, axis=0, **kwargs):
+        """
+        Parameters
+        ----------
+        axis : int or list[int]
+            Rotation axis (indexing does not account for the channel axis)
+        """
+        super().__init__(axis, double=True, **kwargs)
+
+
+class RandomRot90Transform(NonFinalTransform):
+    """Random set of 90 transforms"""
+
+    def __init__(self, axes=None, max_rot=2, negative=True,
+                 *, shared=True, **kwargs):
+        """
+        Parameters
+        ----------
+        axes : int or list[int]
+            Axes along which rotations can happen.
+            If `None`, all axes.
+        max_rot : int or Sampler
+            Maximum number of consecutive rotations.
+        negative : bool
+            Whether to authorize negative rotations.
+
+        Other Parameters
+        ----------------
+        shared : {'channels', 'tensors', 'channels+tensors', ''}
+            Apply the same permutation to all channels and/or tensors
+        """
+        super().__init__(shared=shared, **kwargs)
+        self.axes = axes
+        self.max_rot = RandInt.make(make_range(1, max_rot))
+        self.negative = negative
+
+    def make_final(self, x, max_depth=float('inf')):
+        if max_depth == 0:
+            return self
+        if 'channels' not in self.shared and len(x) > 1:
+            return PerChannelTransform(
+                [self.make_final(x[i:i+1], max_depth) for i in range(len(x))],
+                **self.get_prm()
+            ).make_final(x, max_depth-1)
+        ndim = x.ndim - 1
+        max_rot = self.max_rot
+        if isinstance(max_rot, Sampler):
+            max_rot = max_rot()
+        axes = self.axes
+        if axes is None:
+            axes = list(range(ndim))
+        if isinstance(axes, (int, list, tuple)):
+            axes = ensure_list(axes, max_rot, crop=False)
+        if not isinstance(axes, Sampler):
+            axes = RandKFrom(axes, max_rot, replacement=True)
+
+        axes = ensure_list(axes(), max_rot)
+        negative = RandKFrom([False, True], max_rot, replacement=True)() \
+            if self.negative else [False] * max_rot
+        return Rot90Transform(
+            axes, negative, **self.get_prm()
+        ).make_final(max_depth-1)
+
+
 class CropPadTransform(FinalTransform):
     """Crop and/or pad a tensor"""
 
     def __init__(self, crop, pad, bound='zero', value=0, **kwargs):
         """
         Parameters
         ----------
```

### Comparing `cornucopia-0.2.0/cornucopia/geometric.py` & `cornucopia-0.3.0/cornucopia/geometric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1115,15 +1115,14 @@
             torch.as_tensor(bulk_zooms, **backend))
         offsets = torch.as_tensor(offsets, **backend)
 
         E = torch.eye(ndim+1, **backend).expand([nb_slice, ndim+1, ndim+1])
         F = torch.eye(ndim+1, **backend)
         F[:ndim, -1] = -offsets
         Z = E.clone()
-        print(zooms.shape, Z.shape)
         Z.diagonal(0, -1, -2)[:, :-1].copy_(1 + zooms)
         T = E.clone()
         T[:, :ndim, -1] = translations
 
         A = F               # origin at center of FOV
         A = Z.matmul(A)     # zoom
         if ndim == 2:
@@ -1358,15 +1357,15 @@
             return self.make_per_channel(x, max_depth, flow=True)
 
         ndim = x.ndim - 1
 
         # get slice direction
         slice = self.slice
         if slice is None:
-            slice = RandInt(0, ndim)
+            slice = RandInt(0, ndim - 1)
         if isinstance(slice, Sampler):
             slice = slice()
 
         # get slice spacing
         spacing, subsample, shots = self.spacing, self.subsample, self.shots
         if isinstance(spacing, Sampler):
             spacing = spacing()
```

### Comparing `cornucopia-0.2.0/cornucopia/intensity.py` & `cornucopia-0.3.0/cornucopia/intensity.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/io.py` & `cornucopia-0.3.0/cornucopia/io.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/kspace.py` & `cornucopia-0.3.0/cornucopia/kspace.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/labels.py` & `cornucopia-0.3.0/cornucopia/labels.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/noise.py` & `cornucopia-0.3.0/cornucopia/noise.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/psf.py` & `cornucopia-0.3.0/cornucopia/psf.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """Apply Gaussian smoothing with random FWHM"""
 
     def __init__(self, fwhm=2, *, shared=False, **kwargs):
         """
 
         Parameters
         ----------
-        fwhm : Sampler or  float
+        fwhm : Sampler or float
             Sampler or upper bound for the full-width at half-maximum
 
         Other Parameters
         ------------------
         returns : [list or dict of] {'input', 'output'}
             Which tensors to return.
         shared : {'channels', 'tensors', 'channels+tensors', ''}
```

### Comparing `cornucopia-0.2.0/cornucopia/qmri.py` & `cornucopia-0.3.0/cornucopia/qmri.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/random.py` & `cornucopia-0.3.0/cornucopia/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,36 +159,35 @@
 
 class Uniform(Sampler):
     """Continuous uniform sampler"""
 
     def __init__(self, *args, **kwargs):
         """
         ```python
+        Uniform()
         Uniform(max)
         Uniform(min, max)
         ```
 
         Parameters
         ----------
         min : float or sequence[float], default=0
             Lower bound (inclusive)
-        max : float or sequence[float]
+        max : float or sequence[float], default=1
             Upper bound (inclusive or exclusive, depending on rounding)
         """
-        min, max = 0, None
+        min, max = 0, 1
         if len(args) == 2:
             min, max = args
         elif len(args) == 1:
             max = args[0]
         if 'min' in kwargs:
             min = kwargs['min']
         if 'max' in kwargs:
             max = kwargs['max']
-        if max is None:
-            raise ValueError('Expected at least one argument')
         super().__init__(min=min, max=max)
 
     def __call__(self, n=None, **backend):
         if isinstance(n, (list, tuple)):
             return torch.rand(
                 n, **backend
             ).mul_(self.max - self.min).add_(self.min)
@@ -257,23 +256,23 @@
                 'To sample with replacement, use `replacement=True`'
             )
         self.range = range
         self.k = k
         self.replacement = replacement
 
     def __call__(self, n=None, **backend):
-        k = self.k or RandInt(len(self.range))()
+        k = self.k or RandInt(1, len(self.range))()
         if isinstance(n, (list, tuple)) or n:
             raise ValueError('RandKFrom cannot sample multiple elements')
         if not self.replacement:
             range = list(self.range)
             random.shuffle(range)
             return range[:k]
         else:
-            index = RandInt(len(self.range))(k)
+            index = RandInt(0, len(self.range)-1)(k)
             return [self.range[i] for i in index]
 
 
 class Normal(Sampler):
     """Gaussian sampler"""
 
     def __init__(self, mu=0, sigma=1):
```

### Comparing `cornucopia-0.2.0/cornucopia/special.py` & `cornucopia-0.3.0/cornucopia/special.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/synth.py` & `cornucopia-0.3.0/cornucopia/synth.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_contrast.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_contrast.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_geometric.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_geometric.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_intensity.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_intensity.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_kspace.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_kspace.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_labels.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_labels.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_noise.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_noise.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_psf.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_psf.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_qmri.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_qmri.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/tests/test_run_synth.py` & `cornucopia-0.3.0/cornucopia/tests/test_run_synth.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/b0.py` & `cornucopia-0.3.0/cornucopia/utils/b0.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/bounds.py` & `cornucopia-0.3.0/cornucopia/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/conv.py` & `cornucopia-0.3.0/cornucopia/utils/conv.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/gmm.py` & `cornucopia-0.3.0/cornucopia/utils/gmm.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/indexing.py` & `cornucopia-0.3.0/cornucopia/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/io.py` & `cornucopia-0.3.0/cornucopia/utils/io.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/jit.py` & `cornucopia-0.3.0/cornucopia/utils/jit.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/kernels.py` & `cornucopia-0.3.0/cornucopia/utils/kernels.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/morpho.py` & `cornucopia-0.3.0/cornucopia/utils/morpho.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/padding.py` & `cornucopia-0.3.0/cornucopia/utils/padding.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/patch.py` & `cornucopia-0.3.0/cornucopia/utils/patch.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/py.py` & `cornucopia-0.3.0/cornucopia/utils/py.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/version.py` & `cornucopia-0.3.0/cornucopia/utils/version.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia/utils/warps.py` & `cornucopia-0.3.0/cornucopia/utils/warps.py`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/cornucopia.egg-info/PKG-INFO` & `cornucopia-0.3.0/cornucopia.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornucopia
-Version: 0.2.0
+Version: 0.3.0
 Summary: An abundance of augmentation layers
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/cornucopia
 Description: <picture align="center">
@@ -25,37 +25,40 @@
         
         Since gradients are not expected to backpropagate through its layers, it can
         theoretically be used within any dataloader pipeline,
         independent of the downstream learning framework (pytorch, tensorflow, jax, ...).
         
         ## Installation
         
-        
-        ## Installation
-        
         ### Dependencies
         
         - `pytorch >= 1.8`
         - `numpy`
         - `nibabel`
         - `torch-interpol`
         - `torch-distmap`
         
         ### Conda
         
         ```sh
         conda install cornucopia -c balbasty -c pytorch -c conda-forge
         ```
         
-        ### Pip
+        ### Pip (release)
         
         ```sh
         pip install cornucopia
         ```
         
+        ### Pip (dev)
+        
+        ```sh
+        pip install cornucopia@git+https://github.com/balbasty/cornucopia
+        ```
+        
         ## Documentation
         
         Read the [documentation](https://cornucopia.readthedocs.io) and in particular:
         - [installation](https://cornucopia.readthedocs.io/en/latest/install/)
         - [get started](https://cornucopia.readthedocs.io/en/latest/start/)
         - [examples](https://cornucopia.readthedocs.io/en/latest/examples/overview/)
         - [API](https://cornucopia.readthedocs.io/en/latest/api/overview/)
```

### Comparing `cornucopia-0.2.0/cornucopia.egg-info/SOURCES.txt` & `cornucopia-0.3.0/cornucopia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/setup.cfg` & `cornucopia-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cornucopia-0.2.0/versioneer.py` & `cornucopia-0.3.0/versioneer.py`

 * *Files identical despite different names*

