# Comparing `tmp/scipion-em-eman2-3.6.tar.gz` & `tmp/scipion-em-eman2-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-eman2-3.6.tar", last modified: Sat Sep  9 13:01:04 2023, max compression
+gzip compressed data, was "scipion-em-eman2-3.6.1.tar", last modified: Fri Apr 19 13:25:07 2024, max compression
```

## Comparing `scipion-em-eman2-3.6.tar` & `scipion-em-eman2-3.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/eman2/
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/eman2/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/e2converter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/e2ih.py
--rw-r--r--   0 runner    (1001) docker     (127)    48928 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/eman2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/eman2/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_autopick_boxer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_boxing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12483 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_ctf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_initialmodel_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)    30336 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_refine2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    20499 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_refine2d_bispec.py
--rw-r--r--   0 runner    (1001) docker     (127)    26265 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_refineasy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols/protocol_tiltvalidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/eman2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18052 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/tests/test_protocols_eman.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/eman2/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38965 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/eman2/viewers/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-09 13:01:04.000000 scipion-em-eman2-3.6/scipion_em_eman2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-09 13:01:04.886715 scipion-em-eman2-3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2023-09-09 12:59:00.000000 scipion-em-eman2-3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.336451 scipion-em-eman2-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-19 13:25:07.336451 scipion-em-eman2-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.332451 scipion-em-eman2-3.6.1/eman2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.332451 scipion-em-eman2-3.6.1/eman2/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/e2converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2602 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/e2ih.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48928 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/eman2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.332451 scipion-em-eman2-3.6.1/eman2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_autopick_boxer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7217 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_boxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_initialmodel_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16518 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30332 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_refine2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_refine2d_bispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_refineasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols/protocol_tiltvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.332451 scipion-em-eman2-3.6.1/eman2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17216 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/tests/test_protocols_eman.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.332451 scipion-em-eman2-3.6.1/eman2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38747 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/eman2/viewers/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:25:07.336451 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 13:25:07.000000 scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:25:07.336451 scipion-em-eman2-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-19 13:24:39.000000 scipion-em-eman2-3.6.1/setup.py
```

### Comparing `scipion-em-eman2-3.6/CHANGES.txt` & `scipion-em-eman2-3.6.1/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.6.1: add 2.99.55
 3.6:
     - add 2.99.52
     - removing direct pointers where I can
     - update parameters for protocols
 3.5 - use conda for installation, older versions not supported
 3.4.2 - eman 2.9 binary dropped
 3.4.1 - add possible outputs dict
```

### Comparing `scipion-em-eman2-3.6/LICENSE` & `scipion-em-eman2-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/PKG-INFO` & `scipion-em-eman2-3.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-eman2
-Version: 3.6
+Version: 3.6.1
 Summary: Plugin to use EMAN programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-eman2
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-eman2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-eman2/
@@ -68,15 +68,15 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.52):
+        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.55):
         Command to activate the EMAN environment.
         
         The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
         
         To check the installation, simply run one of the following Scipion tests:
         
         .. code-block::
@@ -93,15 +93,15 @@
            scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
         
         A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
         
         Supported versions
         ------------------
         
-        2.99.47, 2.99.52
+        2.99.47, 2.99.52, 2.99.55
         
         Protocols
         ---------
         
         * boxer
         * boxer auto
         * ctf auto
@@ -116,10 +116,10 @@
         References
         ----------
         
         1. \G. Tang, L. Peng, P.R. Baldwin, D.S. Mann, W. Jiang, I. Rees & S.J. Ludtke. (2007) EMAN2: an extensible image processing suite for electron microscopy. J Struct Biol. 157, 38-46. PMID: 16859925
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-eman2-3.6/README.rst` & `scipion-em-eman2-3.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 -----------------------
 *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
 PATH (not recommended), which can lead to execution problems mixing scipion
 python with conda ones. One example of this could can be seen below but
 depending on your conda version and shell you will need something different:
 CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
 
-*EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.52):
+*EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.55):
 Command to activate the EMAN environment.
 
 The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
 
 To check the installation, simply run one of the following Scipion tests:
 
 .. code-block::
@@ -83,15 +83,15 @@
    scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
 
 A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
 
 Supported versions
 ------------------
 
-2.99.47, 2.99.52
+2.99.47, 2.99.52, 2.99.55
 
 Protocols
 ---------
 
 * boxer
 * boxer auto
 * ctf auto
```

### Comparing `scipion-em-eman2-3.6/eman2/__init__.py` & `scipion-em-eman2-3.6.1/eman2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 
 from .constants import (EMAN2SCRATCHDIR, VERSIONS, EMAN_ENV_ACTIVATION,
                         DEFAULT_ACTIVATION_CMD, EMAN_DEFAULT_VER_NUM)
 
 
-__version__ = '3.6'
+__version__ = '3.6.1'
 _logo = "eman2_logo.png"
 _references = ['Tang2007']
 
 
 class Plugin(pwem.Plugin):
     _supportedVersions = VERSIONS
     _url = "https://github.com/scipion-em/scipion-em-eman2"
@@ -77,15 +77,15 @@
         """ Return True if current version of eman is newer
          or equal than the input argument.
          Params:
             version: string version (semantic version, e.g 2.91)
         """
         v1 = cls.getActiveVersion()
         if v1 not in VERSIONS:
-            raise Exception("This version of EMAN is not supported: ", v1)
+            raise ValueError("This version of EMAN is not supported: ", v1)
 
         if VERSIONS.index(v1) < VERSIONS.index(version):
             return False
         return True
 
     @classmethod
     def getActiveVersion(cls, *args):
```

### Comparing `scipion-em-eman2-3.6/eman2/bibtex.py` & `scipion-em-eman2-3.6.1/eman2/bibtex.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 journal = "JSB",
 volume = "157",
 number = "1",
 pages = "38 - 46",
 year = "2007",
 note = "Software tools for macromolecular microscopy ",
 issn = "1047-8477",
-doi = "http://dx.doi.org/10.1016/j.jsb.2006.05.009",
-url = "http://www.sciencedirect.com/science/article/pii/S1047847706001894",
+doi = "https://dx.doi.org/10.1016/j.jsb.2006.05.009",
+url = "https://www.sciencedirect.com/science/article/pii/S1047847706001894",
 author = "Guang Tang and Liwei Peng and Philip R. Baldwin and Deepinder S. Mann and Wen Jiang and Ian Rees and Steven J. Ludtke",
 keywords = "EMAN, Single particle analysis , cryoEM, TEM, Software, Image processing, Electron microscopy"}
 
 @article{Bell2016,
 title = "High resolution single particle refinement in EMAN2.1.",
 journal = "Methods",
 volume = "100",
 pages = "25 - 34",
 year = "2016",
-doi = "http://dx.doi.org/10.1016/j.ymeth.2016.02.018",
-url = "http://www.sciencedirect.com/science/article/pii/S1046202316300342",
+doi = "https://dx.doi.org/10.1016/j.ymeth.2016.02.018",
+url = "https://www.sciencedirect.com/science/article/pii/S1046202316300342",
 author = "James M. Bell and Muyuan Chen and Philip R. Baldwin and Steven J. Ludtke",
 keywords = "CryoEM, Single particle analysis, Image processing, 3-D reconstruction, Structural biology"}
 
 """
```

### Comparing `scipion-em-eman2-3.6/eman2/constants.py` & `scipion-em-eman2-3.6.1/eman2/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 EMAN2SCRATCHDIR = 'EMAN2SCRATCHDIR'
 
 # Supported versions
-VERSIONS = ['2.99.47', '2.99.52']
+VERSIONS = ['2.99.47', '2.99.52', '2.99.55']
 EMAN_DEFAULT_VER_NUM = VERSIONS[-1]
 
 DEFAULT_ENV_NAME = f"eman-{EMAN_DEFAULT_VER_NUM}"
 DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
 EMAN_ENV_ACTIVATION = 'EMAN_ENV_ACTIVATION'
 
 # ------------------ Constants values -----------------------------------------
@@ -270,15 +270,15 @@
 
 # e2boxer autopick modes
 AUTO_LOCAL = 0
 AUTO_REF = 1
 AUTO_CONVNET = 2
 AUTO_GAUSS = 3
 
-WIKI_URL = "[[http://blake.bcm.edu/emanwiki/EMAN2][Wiki]]"
+WIKI_URL = "[[https://blake.bcm.edu/emanwiki/EMAN2][Wiki]]"
 
 # viewer.py constants
 LAST_ITER = 0
 ALL_ITERS = 1
 SELECTED_ITERS = 2
 
 ANGDIST_2DPLOT = 0
```

### Comparing `scipion-em-eman2-3.6/eman2/convert/__init__.py` & `scipion-em-eman2-3.6.1/eman2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/convert/convert.py` & `scipion-em-eman2-3.6.1/eman2/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/convert/dataimport.py` & `scipion-em-eman2-3.6.1/eman2/convert/dataimport.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/e2converter.py` & `scipion-em-eman2-3.6.1/eman2/e2converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,10 +230,10 @@
             inputParts = sys.argv[2]
             inputCls = sys.argv[3]
             inputClasses = sys.argv[4]
             outputTxt = sys.argv[5]
             alitype = sys.argv[6]
             readParticles(inputParts, inputCls, inputClasses, outputTxt, alitype)
         else:
-            raise Exception("e2converter: Unknown mode '%s'" % mode)
+            raise ValueError("e2converter: Unknown mode '%s'" % mode)
     else:
         print("usage: %s outputFile" % os.path.basename(sys.argv[0]))
```

### Comparing `scipion-em-eman2-3.6/eman2/e2ih.py` & `scipion-em-eman2-3.6.1/eman2/e2ih.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/eman2_logo.png` & `scipion-em-eman2-3.6.1/eman2/eman2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/protocols/__init__.py` & `scipion-em-eman2-3.6.1/eman2/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_autopick_boxer.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_initialmodel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **************************************************************************
 # *
-# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
+# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
 # *
-# * MRC Laboratory of Molecular Biology (MRC-LMB)
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,189 +21,218 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
+from glob import glob
+from enum import Enum
 
-from pyworkflow.protocol.params import (IntParam, FloatParam,
-                                        EnumParam, PointerParam,
-                                        StringParam, USE_GPU,
-                                        GPU_LIST, BooleanParam)
-from pyworkflow.utils import makePath, createLink
+from pyworkflow.utils.path import cleanPattern
 from pyworkflow.constants import PROD
-from pwem.protocols import ProtParticlePickingAuto
+from pyworkflow.protocol.params import (PointerParam, IntParam,
+                                        BooleanParam, LEVEL_ADVANCED,
+                                        StringParam)
+from pwem.protocols import ProtInitialVolume
+from pwem.objects.data import SetOfClasses2D, Volume, SetOfVolumes
 
 from .. import Plugin
-from ..convert import readSetOfCoordinates, convertReferences
-from ..constants import *
+from ..constants import EMAN2SCRATCHDIR
 
 
-class EmanProtAutopick(ProtParticlePickingAuto):
-    """ Automated particle picker for SPA. Uses EMAN2 (versions 2.2+) e2boxer.py
+class outputs(Enum):
+    outputVolumes = SetOfVolumes
+
+
+class EmanProtInitModel(ProtInitialVolume):
     """
-    _label = 'boxer auto'
-    _devStatus = PROD
+    This protocol wraps *e2initialmodel.py* EMAN2 program.
 
-    def _createFilenameTemplates(self):
-        """ Centralize the names of the files. """
+    It will take a set of class-averages/projections and build a set
+    of 3-D models suitable for use as initial models in single
+    particle reconstruction. The output set is theoretically sorted
+    in order of quality (best one is numbered 1), though it's best
+    to look at the other answers as well.
 
-        myDict = {'goodRefsFn': self._getExtraPath('info/boxrefs.hdf'),
-                  'badRefsFn': self._getExtraPath('info/boxrefsbad.hdf'),
-                  'bgRefsFn': self._getExtraPath('info/boxrefsbg.hdf'),
-                  'nnetFn': self._getExtraPath('nnet_pickptcls.hdf'),
-                  'nnetClFn': self._getExtraPath('nnet_classify.hdf'),
-                  'trainoutFn': self._getExtraPath('trainout_pickptcl.hdf'),
-                  'trainoutClFn': self._getExtraPath('trainout_classify.hdf')
-                  }
-        self._updateFilenamesDict(myDict)
+    See more details in:
+    https://blake.bcm.edu/emanwiki/EMAN2/Programs/e2initialmodel
+    """
 
-    def __init__(self, **kwargs):
-        ProtParticlePickingAuto.__init__(self, **kwargs)
+    _label = 'initial model'
+    _devStatus = PROD
+    _possibleOutputs = outputs
 
     # --------------------------- DEFINE param functions ----------------------
+
     def _defineParams(self, form):
-        ProtParticlePickingAuto._defineParams(self, form)
-        form.addHidden(USE_GPU, BooleanParam, default=False,
-                       label="Use GPU?",
-                       help="Set to Yes if you want to run Neural Net "
-                            "boxer on GPU. Default is CPU.")
-        form.addHidden(GPU_LIST, StringParam, default='0',
-                       label="Choose GPU ID",
-                       help="GPU may have several cores. Set it to zero"
-                            " if you do not know what we are talking about."
-                            " First core index is 0, second 1 and so on.\n"
-                            "Eman boxer can use only one GPU.")
-        form.addParam('boxSize', IntParam, default=128,
-                      allowsPointers=True,
-                      label='Box size (px)',
-                      help="Box size in pixels. See http://eman2.org/BoxSize")
-        form.addParam('particleSize', IntParam, default=100,
-                      label='Particle size (px)',
-                      help="Longest axis of particle in pixels (diameter, "
-                           "not radius).")
-        form.addParam('boxerMode', EnumParam,
-                      choices=['local search', 'by ref', 'neural net', 'gauss'],
-                      label="Autopicker mode:", default=AUTO_CONVNET,
-                      display=EnumParam.DISPLAY_COMBO,
-                      help="Choose autopicker mode:\n\n"
-                           " _local search_ - Reference based search by "
-                           "downsampling and 2-D alignment to references.\n"
-                           " _by ref_ - simple reference-based "
-                           "cross-correlation picker with exhaustive "
-                           "rotational search.\n"
-                           " _neural net_ - convolutional neural network "
-                           "boxer.\n"
-                           " _gauss_ - simple reference-free picker.")
-        form.addParam('threshold', FloatParam, default=5.0,
-                      label='Threshold',
-                      condition='boxerMode!=%d' % AUTO_GAUSS)
-        form.addParam('threshold2', FloatParam, default=-5.0,
-                      condition='boxerMode==%d' % AUTO_CONVNET,
-                      label='Threshold2')
-        form.addParam('gaussLow', FloatParam, default=1.,
-                      condition='boxerMode==%d' % AUTO_GAUSS,
-                      label='Threshold low')
-        form.addParam('gaussHigh', FloatParam, default=2.,
-                      condition='boxerMode==%d' % AUTO_GAUSS,
-                      label='Threshold high')
-        form.addParam('gaussWidth', FloatParam, default=1.,
-                      condition='boxerMode==%d' % AUTO_GAUSS,
-                      label='Gaussian width')
-
-        form.addSection('References')
-        form.addParam('boxerProt', PointerParam,
-                      pointerClass='EmanProtBoxing',
-                      condition='boxerMode==%d' % AUTO_CONVNET,
-                      label='Previous e2boxer protocol',
-                      help='Provide previously executed e2boxer protocol '
-                           'that has all 3 types of references and '
-                           'pre-trained neural network.')
-        form.addParam('goodRefs', PointerParam,
-                      pointerClass='SetOfAverages',
-                      condition='boxerMode<%d' % AUTO_CONVNET,
-                      label="Good references",
-                      help="Good particle references.")
+        form.addSection(label='Input')
+        form.addParam('inputSet', PointerParam,
+                      pointerClass='SetOfClasses2D, SetOfAverages',
+                      label="Input averages", important=True,
+                      help='Select the your class averages to build your '
+                           '3D model.\nYou can select SetOfAverages or '
+                           'SetOfClasses2D as input.')
+        form.addParam('symmetry', StringParam, default='c1',
+                      label='Symmetry group',
+                      help='Specify the symmetry.\nChoices are: c(n), d(n), '
+                           'h(n), tet, oct, icos.\n'
+                           'See https://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
+                           'for a detailed description of symmetry in Eman.')
+        form.addParam('numberOfIterations', IntParam, default=8,
+                      label='Number of iterations to perform',
+                      help='The total number of refinement to perform.')
+        form.addParam('numberOfModels', IntParam, default=10,
+                      label='Number of different initial models',
+                      help='The number of different initial models to '
+                           'generate in search of a good one.')
+        form.addParam('shrink', IntParam, default=1,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='Shrink factor',
+                      help='Using a box-size >64 is not optimal for making '
+                           'initial models. Suggest using this option to '
+                           'shrink the input particles by an integer amount '
+                           'prior to reconstruction. Default = 1, no shrinking')
+        form.addParam('randOrient', BooleanParam, default=False,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='Use random orientations?',
+                      help='Instead of seeding with a random volume, '
+                           'seeds by randomizing input orientations')
+        form.addParam('autoMaskExp', IntParam, default=-1,
+                      expertLevel=LEVEL_ADVANCED,
+                      label='Automask expand (px)',
+                      help='Number of voxels of post-threshold expansion '
+                           'in the mask, for use when peripheral '
+                           'features are truncated '
+                           '(default=shrunk boxsize/20)')
+        form.addParam('extraParams', StringParam, default='',
+                      expertLevel=LEVEL_ADVANCED,
+                      label='Additional arguments:',
+                      help='In this box command-line arguments may be provided '
+                           'that are not generated by the GUI. This may be '
+                           'useful for testing developmental options and/or '
+                           'expert use of the program. \n'
+                           'The command "e2initialmodel.py -h" will print a list '
+                           'of possible options.')
 
-        form.addParallelSection(threads=1, mpi=0)
+        form.addParallelSection(threads=8, mpi=1)
 
     # --------------------------- INSERT steps functions ----------------------
-    def _insertInitialSteps(self):
-        self._createFilenameTemplates()
-        initId = self._insertFunctionStep('convertInputStep')
-        return [initId]
 
-    # --------------------------- STEPS functions -----------------------------
-    def convertInputStep(self):
-        goodRefs = self.goodRefs.get() if self.goodRefs.hasValue() else None
-        boxerProt = self.boxerProt.get() if self.boxerProt.hasValue() else None
-        storePath = self._getExtraPath("info")
-        makePath(storePath)
-
-        if goodRefs is not None:
-            convertReferences(goodRefs, self._getFileName('goodRefsFn'))
-
-        if boxerProt is not None:
-            boxerProt._createFilenameTemplates()
-            keys = ['goodRefsFn', 'badRefsFn', 'bgRefsFn',
-                    'nnetFn', 'nnetClFn',
-                    'trainoutFn', 'trainoutClFn']
-
-            for fn in keys:
-                if os.path.exists(boxerProt._getFileName(fn)):
-                    createLink(boxerProt._getFileName(fn),
-                               self._getFileName(fn))
-
-    def _pickMicrograph(self, mic, *args):
-        micFile = os.path.relpath(mic.getFileName(), self.getCoordsDir())
-        params = " --apix=%f --no_ctf" % self.inputMicrographs.get().getSamplingRate()
-        params += " --boxsize=%d" % self.boxSize.get()
-        params += " --ptclsize=%d" % self.particleSize.get()
-        params += " --threads=%d" % self.numberOfThreads.get()
-
-        modes = ['auto_local', 'auto_ref', 'auto_convnet', 'auto_gauss']
-        params += " --autopick=%s" % modes[self.boxerMode.get()]
-
-        if self.boxerMode.get() == AUTO_GAUSS:
-            params += ":gauss_width=%0.3f:thr_low=%0.3f:thr_high=%0.3f:boxsize=%d" % (
-                self.gaussWidth.get(), self.gaussLow.get(),
-                self.gaussHigh.get(), self.boxSize.get())
+    def _insertAllSteps(self):
+        self._prepareDefinition()
+        self._insertFunctionStep('createStackImgsStep')
+        self._insertInitialModelStep()
+        self._insertFunctionStep('createOutputStep')
+
+    def _insertInitialModelStep(self):
+        args = '--input=%(relImgsFn)s --sym=%(symmetry)s'
+        if self.shrink > 1:
+            args += ' --shrink=%(shrink)d'
+        if not self._isHighSym():
+            args += ' --tries=%(numberOfModels)d --iter=%(numberOfIterations)d'
+            if self.randOrient:
+                args += ' --randorient'
+            if self.autoMaskExp.get() != -1:
+                args += '--automaskexpand %d'
+            if self.numberOfMpi > 1:
+                args += ' --parallel=mpi:%(mpis)d:%(scratch)s'
+            else:
+                args += ' --parallel=thread:%(threads)d'
         else:
-            params += ":threshold=%0.2f" % self.threshold.get()
+            args += ' --threads=%(threads)d'
+        if self.extraParams.hasValue():
+            args += " " + self.extraParams.get()
 
-        if self.boxerMode.get() == AUTO_CONVNET:
-            params += ":threshold2=%0.2f" % self.threshold2.get()
+        self._insertFunctionStep('createInitialModelStep', args % self._params)
 
-            if self.useGpu:
-                params += " --device=gpu%s" % self.gpuList.get().strip()
-            else:
-                params += " --device=cpu"
+    # --------------------------- STEPS functions -----------------------------
+    def createStackImgsStep(self):
+        if isinstance(self.inputSet.get(), SetOfClasses2D):
+            pixSize = self.inputSet.get().getImages().getSamplingRate()
+            imgSet = self._createSetOfParticles("_averages")
+            for i, cls in enumerate(self.inputSet.get()):
+                img = cls.getRepresentative()
+                img.setSamplingRate(pixSize)
+                img.setObjId(i + 1)
+                imgSet.append(img)
+        else:
+            imgSet = self.inputSet.get()
+            pixSize = imgSet.getSamplingRate()
 
-        params += ' %s' % micFile
-        program = Plugin.getProgram('e2boxer.py')
+        tmpStack = self._getTmpPath("averages.spi")
+        imgSet.writeStack(tmpStack)
+        orig = os.path.relpath(tmpStack,
+                               self._getExtraPath())
+        args = "%s %s --apix=%0.3f" % (orig, self._params['relImgsFn'], pixSize)
+        self.runJob(Plugin.getProgram('e2proc2d.py'), args,
+                    cwd=self._getExtraPath(),
+                    numberOfMpi=1, numberOfThreads=1)
+
+    def createInitialModelStep(self, args):
+        """ Run the EMAN program to create the initial model. """
+        cleanPattern(self._getExtraPath('initial_models'))
+        if self._isHighSym():
+            program = Plugin.getProgram('e2initialmodel_hisym.py')
+        else:
+            program = Plugin.getProgram('e2initialmodel.py')
 
-        self.runJob(program, params, cwd=self.getCoordsDir())
+        self.runJob(program, args, cwd=self._getExtraPath(),
+                    numberOfMpi=1, numberOfThreads=1)
 
     def createOutputStep(self):
-        pass
+        classes2DSet = self.inputSet.get()
+        volumes = self._createSetOfVolumes()
+        shrink = self.shrink.get()
+        if isinstance(self.inputSet.get(), SetOfClasses2D):
+            volumes.setSamplingRate(classes2DSet.getImages().getSamplingRate() * shrink)
+        else:
+            volumes.setSamplingRate(self.inputSet.get().getSamplingRate() * shrink)
+        outputVols = self._getVolumes()
+        for k, volFn in enumerate(outputVols):
+            vol = Volume()
+            vol.setFileName(volFn)
+            vol.setObjComment('eman initial model %02d' % (k + 1))
+            volumes.append(vol)
+
+        self._defineOutputs(**{outputs.outputVolumes.name: volumes})
+        self._defineSourceRelation(self.inputSet, volumes)
 
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
-
-        if self.useGpu and (self.boxerMode.get() != AUTO_CONVNET):
-            errors.append("You can use GPU only for neural net picker!")
-
         return errors
 
+    def _summary(self):
+        summary = []
+        if not hasattr(self, 'outputVolumes'):
+            summary.append("Output volumes not ready yet.")
+        else:
+            summary.append("Input images: %s" % self.getObjectTag('inputSet'))
+            summary.append("Output initial volumes: %s" % self.outputVolumes.getSize())
+            if self._isHighSym():
+                summary.append("Used e2initialmodel_hisym.py for high symmetry reconstruction.")
+        return summary
+
     # --------------------------- UTILS functions -----------------------------
-    def getCoordsDir(self):
-        return self._getExtraPath()
 
-    def getFiles(self):
-        return (self.inputMicrographs.get().getFiles() |
-                ProtParticlePickingAuto.getFiles(self))
-
-    def readCoordsFromMics(self, workingDir, micList, coordSet):
-        coordSet.setBoxSize(self.boxSize.get())
-        readSetOfCoordinates(workingDir, micList, coordSet)
+    def _prepareDefinition(self):
+        self._params = {'imgsFn': self._getExtraPath('representatives.hdf'),
+                        'relImgsFn': 'representatives.hdf',
+                        'numberOfIterations': self.numberOfIterations.get(),
+                        'numberOfModels': self.numberOfModels.get(),
+                        'shrink': self.shrink.get(),
+                        'symmetry': self.symmetry.get(),
+                        'threads': self.numberOfThreads.get(),
+                        'mpis': self.numberOfMpi.get(),
+                        'scratch': Plugin.getVar(EMAN2SCRATCHDIR)}
+
+    def _isHighSym(self):
+        return self.symmetry.get() in ["oct", "tet", "icos"]
+
+    def _getVolumes(self):
+        if self._isHighSym():
+            outputVols = [self._getExtraPath('final.hdf')]
+        else:
+            outputVols = glob(self._getExtraPath('initial_models/model_??_??.hdf'))
+            outputVols.sort()
+        return outputVols
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_boxing.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_boxing.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         program = Plugin.getProgram('e2boxer.py')
         arguments = " --apix=%(pixSize)f --boxsize=%(boxSize)d"
         arguments += " --ptclsize=%(ptclSize)d --gui --threads=%(thr)d --no_ctf"
 
         acq = self.inputMics.getAcquisition()
         arguments += " --voltage %d" % acq.getVoltage()
         arguments += " --cs %0.2f" % acq.getSphericalAberration()
-        arguments += " --ac %0.2f" % acq.getAmplitudeContrast()
+        arguments += " --ac %0.2f" % (100 * acq.getAmplitudeContrast())
 
         self._params.update({
             'pixSize': self.inputMics.getSamplingRate(),
             'boxSize': self.boxSize.get(),
             'ptclSize': self.particleSize.get(),
             'thr': self.numberOfThreads.get()
         })
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_ctf.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_ctf.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                                         BooleanParam)
 from pyworkflow.constants import PROD
 import pyworkflow.utils as pwutils
 from pwem.objects.data import CTFModel, SetOfParticles
 from pwem.protocols import ProtProcessParticles
 
 from .. import Plugin
-from ..constants import *
+from ..constants import HIRES, INVAR_AUTO
 from ..convert import writeSetOfParticles, iterLstFile, jsonToCtfModel
 
 
 class EmanProtCTFAuto(ProtProcessParticles):
     """
     This protocol wraps *e2ctf_auto.py* EMAN2 program.
     It automates the CTF fitting and structure factor
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_initialmodel.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_autopick_boxer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **************************************************************************
 # *
-# * Authors:     Josue Gomez Blanco (josue.gomez-blanco@mcgill.ca)
+# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# * MRC Laboratory of Molecular Biology (MRC-LMB)
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,219 +21,216 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
-from glob import glob
-from enum import Enum
 
-from pyworkflow.utils.path import cleanPattern
+from pyworkflow.protocol.params import (IntParam, FloatParam,
+                                        EnumParam, PointerParam,
+                                        StringParam, USE_GPU,
+                                        GPU_LIST, BooleanParam)
+from pyworkflow.utils import makePath, createLink
 from pyworkflow.constants import PROD
-from pyworkflow.protocol.params import (PointerParam, IntParam,
-                                        BooleanParam, LEVEL_ADVANCED,
-                                        StringParam)
-from pwem.protocols import ProtInitialVolume
-from pwem.objects.data import SetOfClasses2D, Volume, SetOfVolumes
+from pwem.protocols import ProtParticlePickingAuto
 
 from .. import Plugin
-from ..constants import EMAN2SCRATCHDIR
+from ..convert import readSetOfCoordinates, convertReferences
+from ..constants import AUTO_CONVNET, AUTO_GAUSS
 
 
-class outputs(Enum):
-    outputVolumes = SetOfVolumes
-
-
-class EmanProtInitModel(ProtInitialVolume):
+class EmanProtAutopick(ProtParticlePickingAuto):
+    """ Automated particle picker for SPA. Uses EMAN2 (versions 2.2+) e2boxer.py
     """
-    This protocol wraps *e2initialmodel.py* EMAN2 program.
+    _label = 'boxer auto'
+    _devStatus = PROD
 
-    It will take a set of class-averages/projections and build a set
-    of 3-D models suitable for use as initial models in single
-    particle reconstruction. The output set is theoretically sorted
-    in order of quality (best one is numbered 1), though it's best
-    to look at the other answers as well.
+    def _createFilenameTemplates(self):
+        """ Centralize the names of the files. """
 
-    See more details in:
-    http://blake.bcm.edu/emanwiki/EMAN2/Programs/e2initialmodel
-    """
+        myDict = {'goodRefsFn': self._getExtraPath('info/boxrefs.hdf'),
+                  'badRefsFn': self._getExtraPath('info/boxrefsbad.hdf'),
+                  'bgRefsFn': self._getExtraPath('info/boxrefsbg.hdf'),
+                  'nnetFn': self._getExtraPath('nnet_pickptcls.hdf'),
+                  'nnetClFn': self._getExtraPath('nnet_classify.hdf'),
+                  'trainoutFn': self._getExtraPath('trainout_pickptcl.hdf'),
+                  'trainoutClFn': self._getExtraPath('trainout_classify.hdf')
+                  }
+        self._updateFilenamesDict(myDict)
 
-    _label = 'initial model'
-    _devStatus = PROD
-    _possibleOutputs = outputs
+    def __init__(self, **kwargs):
+        ProtParticlePickingAuto.__init__(self, **kwargs)
 
     # --------------------------- DEFINE param functions ----------------------
-
     def _defineParams(self, form):
-        form.addSection(label='Input')
-        form.addParam('inputSet', PointerParam,
-                      pointerClass='SetOfClasses2D, SetOfAverages',
-                      # pointerCondition='hasRepresentatives',
-                      label="Input averages", important=True,
-                      help='Select the your class averages to build your '
-                           '3D model.\nYou can select SetOfAverages or '
-                           'SetOfClasses2D as input.')
-        form.addParam('symmetry', StringParam, default='c1',
-                      label='Symmetry group',
-                      help='Specify the symmetry.\nChoices are: c(n), d(n), '
-                           'h(n), tet, oct, icos.\n'
-                           'See http://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
-                           'for a detailed description of symmetry in Eman.')
-        form.addParam('numberOfIterations', IntParam, default=8,
-                      label='Number of iterations to perform',
-                      help='The total number of refinement to perform.')
-        form.addParam('numberOfModels', IntParam, default=10,
-                      label='Number of different initial models',
-                      help='The number of different initial models to '
-                           'generate in search of a good one.')
-        form.addParam('shrink', IntParam, default=1,
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Shrink factor',
-                      help='Using a box-size >64 is not optimal for making '
-                           'initial models. Suggest using this option to '
-                           'shrink the input particles by an integer amount '
-                           'prior to reconstruction. Default = 1, no shrinking')
-        form.addParam('randOrient', BooleanParam, default=False,
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Use random orientations?',
-                      help='Instead of seeding with a random volume, '
-                           'seeds by randomizing input orientations')
-        form.addParam('autoMaskExp', IntParam, default=-1,
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Automask expand (px)',
-                      help='Number of voxels of post-threshold expansion '
-                           'in the mask, for use when peripheral '
-                           'features are truncated '
-                           '(default=shrunk boxsize/20)')
-        form.addParam('extraParams', StringParam, default='',
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Additional arguments:',
-                      help='In this box command-line arguments may be provided '
-                           'that are not generated by the GUI. This may be '
-                           'useful for testing developmental options and/or '
-                           'expert use of the program. \n'
-                           'The command "e2initialmodel.py -h" will print a list '
-                           'of possible options.')
+        ProtParticlePickingAuto._defineParams(self, form)
+        form.addHidden(USE_GPU, BooleanParam, default=False,
+                       label="Use GPU?",
+                       help="Set to Yes if you want to run Neural Net "
+                            "boxer on GPU. Default is CPU.")
+        form.addHidden(GPU_LIST, StringParam, default='0',
+                       label="Choose GPU ID",
+                       help="GPU may have several cores. Set it to zero"
+                            " if you do not know what we are talking about."
+                            " First core index is 0, second 1 and so on.\n"
+                            "Eman boxer can use only one GPU.")
+        form.addParam('boxSize', IntParam, default=128,
+                      allowsPointers=True,
+                      label='Box size (px)',
+                      help="Box size in pixels. See https://eman2.org/BoxSize")
+        form.addParam('particleSize', IntParam, default=100,
+                      label='Particle size (px)',
+                      help="Longest axis of particle in pixels (diameter, "
+                           "not radius).")
+        form.addParam('boxerMode', EnumParam,
+                      choices=['local search', 'by ref', 'neural net', 'gauss'],
+                      label="Autopicker mode:", default=AUTO_CONVNET,
+                      display=EnumParam.DISPLAY_COMBO,
+                      help="Choose autopicker mode:\n\n"
+                           " _local search_ - Heavily downsamples the "
+                           "particles and references, and actually performs "
+                           "a 2-D alignment of each putative particle to each "
+                           "reference to identify the best particles in the "
+                           "image. In theory this should produce fewer "
+                           "false positives. Reference requirements are "
+                           "similar to By Ref, though a smaller number of "
+                           "references may be fine.\n"
+                           " _by ref_ - This is a classic reference based "
+                           "particle picker. To use it, you need to have "
+                           "high quality good references in all possible "
+                           "3-D orientations. The algorithm will do in-plane "
+                           "rotation of the references and cross-correlate "
+                           "to look for peaks. It is recommended that you "
+                           "use projections of a 3-D map (low resolution) "
+                           "as references.\n"
+                           " _neural net_ - This is the most accurate boxer "
+                           "by far, both in terms of false positives and "
+                           "false negatives, when trained properly. It is "
+                           "based on a pair of neural networks, one to "
+                           "discriminate between putative particles and "
+                           "the background, and a second to discriminate "
+                           "between real particles and contamination or "
+                           "other high contrast non-particles, which is "
+                           "why it has two thresholds.\n"
+                           " _gauss_ - This is a simple and fast "
+                           "reference-free picker, which provides a simple "
+                           "solution for easy particle picking cases, "
+                           "where the particles have good contrast and are "
+                           "monodisperse. This may work well for things "
+                           "like viruses or ribosomes. It is very fast "
+                           "and since it requires no references, it's "
+                           "easy to try. It likely won't work well for "
+                           "most projects. It was ported from the old "
+                           "boxer program by a volunteer (Vadim Kotov).")
+        form.addParam('threshold', FloatParam, default=5.0,
+                      label='Threshold',
+                      condition='boxerMode!=%d' % AUTO_GAUSS)
+        form.addParam('threshold2', FloatParam, default=-5.0,
+                      condition='boxerMode==%d' % AUTO_CONVNET,
+                      label='Threshold2')
+        form.addParam('gaussLow', FloatParam, default=1.,
+                      condition='boxerMode==%d' % AUTO_GAUSS,
+                      label='Threshold low')
+        form.addParam('gaussHigh', FloatParam, default=2.,
+                      condition='boxerMode==%d' % AUTO_GAUSS,
+                      label='Threshold high')
+        form.addParam('gaussWidth', FloatParam, default=1.,
+                      condition='boxerMode==%d' % AUTO_GAUSS,
+                      label='Gaussian width')
+
+        form.addSection('References')
+        form.addParam('boxerProt', PointerParam,
+                      pointerClass='EmanProtBoxing',
+                      condition='boxerMode==%d' % AUTO_CONVNET,
+                      label='Previous e2boxer protocol',
+                      help='Provide previously executed e2boxer protocol '
+                           'that has all 3 types of references and '
+                           'pre-trained neural network.')
+        form.addParam('goodRefs', PointerParam,
+                      pointerClass='SetOfAverages',
+                      condition='boxerMode<%d' % AUTO_CONVNET,
+                      label="Good references",
+                      help="Good particle references.")
 
-        form.addParallelSection(threads=8, mpi=1)
+        form.addParallelSection(threads=1, mpi=0)
 
     # --------------------------- INSERT steps functions ----------------------
+    def _insertInitialSteps(self):
+        self._createFilenameTemplates()
+        initId = self._insertFunctionStep('convertInputStep')
+        return [initId]
 
-    def _insertAllSteps(self):
-        self._prepareDefinition()
-        self._insertFunctionStep('createStackImgsStep')
-        self._insertInitialModelStep()
-        self._insertFunctionStep('createOutputStep')
-
-    def _insertInitialModelStep(self):
-        args = '--input=%(relImgsFn)s --sym=%(symmetry)s'
-        if self.shrink > 1:
-            args += ' --shrink=%(shrink)d'
-        if not self._isHighSym():
-            args += ' --tries=%(numberOfModels)d --iter=%(numberOfIterations)d'
-            if self.randOrient:
-                args += ' --randorient'
-            if self.autoMaskExp.get() != -1:
-                args += '--automaskexpand %d'
-            if self.numberOfMpi > 1:
-                args += ' --parallel=mpi:%(mpis)d:%(scratch)s'
-            else:
-                args += ' --parallel=thread:%(threads)d'
+    # --------------------------- STEPS functions -----------------------------
+    def convertInputStep(self):
+        goodRefs = self.goodRefs.get() if self.goodRefs.hasValue() else None
+        boxerProt = self.boxerProt.get() if self.boxerProt.hasValue() else None
+        storePath = self._getExtraPath("info")
+        makePath(storePath)
+
+        if goodRefs is not None:
+            convertReferences(goodRefs, self._getFileName('goodRefsFn'))
+
+        if boxerProt is not None:
+            boxerProt._createFilenameTemplates()
+            keys = ['goodRefsFn', 'badRefsFn', 'bgRefsFn',
+                    'nnetFn', 'nnetClFn',
+                    'trainoutFn', 'trainoutClFn']
+
+            for fn in keys:
+                if os.path.exists(boxerProt._getFileName(fn)):
+                    createLink(boxerProt._getFileName(fn),
+                               self._getFileName(fn))
+
+    def _pickMicrograph(self, mic, *args):
+        micFile = os.path.relpath(mic.getFileName(), self.getCoordsDir())
+        params = " --apix=%f --no_ctf" % self.inputMicrographs.get().getSamplingRate()
+        params += " --boxsize=%d" % self.boxSize.get()
+        params += " --ptclsize=%d" % self.particleSize.get()
+        params += " --threads=%d" % self.numberOfThreads.get()
+
+        modes = ['auto_local', 'auto_ref', 'auto_convnet', 'auto_gauss']
+        params += " --autopick=%s" % modes[self.boxerMode.get()]
+
+        if self.boxerMode.get() == AUTO_GAUSS:
+            params += ":gauss_width=%0.3f:thr_low=%0.3f:thr_high=%0.3f:boxsize=%d" % (
+                self.gaussWidth.get(), self.gaussLow.get(),
+                self.gaussHigh.get(), self.boxSize.get())
         else:
-            args += ' --threads=%(threads)d'
-        if self.extraParams.hasValue():
-            args += " " + self.extraParams.get()
+            params += ":threshold=%0.2f" % self.threshold.get()
 
-        self._insertFunctionStep('createInitialModelStep', args % self._params)
+        if self.boxerMode.get() == AUTO_CONVNET:
+            params += ":threshold2=%0.2f" % self.threshold2.get()
 
-    # --------------------------- STEPS functions -----------------------------
-    def createStackImgsStep(self):
-        if isinstance(self.inputSet.get(), SetOfClasses2D):
-            pixSize = self.inputSet.get().getImages().getSamplingRate()
-            imgSet = self._createSetOfParticles("_averages")
-            for i, cls in enumerate(self.inputSet.get()):
-                img = cls.getRepresentative()
-                img.setSamplingRate(pixSize)
-                img.setObjId(i + 1)
-                imgSet.append(img)
-        else:
-            imgSet = self.inputSet.get()
-            pixSize = imgSet.getSamplingRate()
+            if self.useGpu:
+                params += " --device=gpu%s" % self.gpuList.get().strip()
+            else:
+                params += " --device=cpu"
 
-        tmpStack = self._getTmpPath("averages.spi")
-        imgSet.writeStack(tmpStack)
-        orig = os.path.relpath(tmpStack,
-                               self._getExtraPath())
-        args = "%s %s --apix=%0.3f" % (orig, self._params['relImgsFn'], pixSize)
-        self.runJob(Plugin.getProgram('e2proc2d.py'), args,
-                    cwd=self._getExtraPath(),
-                    numberOfMpi=1, numberOfThreads=1)
-
-    def createInitialModelStep(self, args):
-        """ Run the EMAN program to create the initial model. """
-        cleanPattern(self._getExtraPath('initial_models'))
-        if self._isHighSym():
-            program = Plugin.getProgram('e2initialmodel_hisym.py')
-        else:
-            program = Plugin.getProgram('e2initialmodel.py')
+        params += ' %s' % micFile
+        program = Plugin.getProgram('e2boxer.py')
 
-        self.runJob(program, args, cwd=self._getExtraPath(),
-                    numberOfMpi=1, numberOfThreads=1)
+        self.runJob(program, params, cwd=self.getCoordsDir())
 
     def createOutputStep(self):
-        classes2DSet = self.inputSet.get()
-        volumes = self._createSetOfVolumes()
-        shrink = self.shrink.get()
-        if isinstance(self.inputSet.get(), SetOfClasses2D):
-            volumes.setSamplingRate(classes2DSet.getImages().getSamplingRate() * shrink)
-        else:
-            volumes.setSamplingRate(self.inputSet.get().getSamplingRate() * shrink)
-        outputVols = self._getVolumes()
-        for k, volFn in enumerate(outputVols):
-            vol = Volume()
-            vol.setFileName(volFn)
-            vol.setObjComment('eman initial model %02d' % (k + 1))
-            volumes.append(vol)
-
-        self._defineOutputs(**{outputs.outputVolumes.name: volumes})
-        self._defineSourceRelation(self.inputSet, volumes)
+        pass
 
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
-        return errors
 
-    def _summary(self):
-        summary = []
-        if not hasattr(self, 'outputVolumes'):
-            summary.append("Output volumes not ready yet.")
-        else:
-            summary.append("Input images: %s" % self.getObjectTag('inputSet'))
-            summary.append("Output initial volumes: %s" % self.outputVolumes.getSize())
-            if self._isHighSym():
-                summary.append("Used e2initialmodel_hisym.py for high symmetry reconstruction.")
-        return summary
+        if self.useGpu and (self.boxerMode.get() != AUTO_CONVNET):
+            errors.append("You can use GPU only for neural net picker!")
+
+        return errors
 
     # --------------------------- UTILS functions -----------------------------
+    def getCoordsDir(self):
+        return self._getExtraPath()
 
-    def _prepareDefinition(self):
-        self._params = {'imgsFn': self._getExtraPath('representatives.hdf'),
-                        'relImgsFn': 'representatives.hdf',
-                        'numberOfIterations': self.numberOfIterations.get(),
-                        'numberOfModels': self.numberOfModels.get(),
-                        'shrink': self.shrink.get(),
-                        'symmetry': self.symmetry.get(),
-                        'threads': self.numberOfThreads.get(),
-                        'mpis': self.numberOfMpi.get(),
-                        'scratch': Plugin.getVar(EMAN2SCRATCHDIR)}
-
-    def _isHighSym(self):
-        return self.symmetry.get() in ["oct", "tet", "icos"]
-
-    def _getVolumes(self):
-        if self._isHighSym():
-            outputVols = [self._getExtraPath('final.hdf')]
-        else:
-            outputVols = glob(self._getExtraPath('initial_models/model_??_??.hdf'))
-            outputVols.sort()
-        return outputVols
+    def getFiles(self):
+        return (self.inputMicrographs.get().getFiles() |
+                ProtParticlePickingAuto.getFiles(self))
+
+    def readCoordsFromMics(self, workingDir, micList, coordSet):
+        coordSet.setBoxSize(self.boxSize.get())
+        readSetOfCoordinates(workingDir, micList, coordSet)
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_initialmodel_sgd.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_initialmodel_sgd.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pyworkflow.protocol.params import (PointerParam, IntParam,
                                         BooleanParam, StringParam,
                                         EnumParam, FloatParam)
 from pwem.protocols import ProtInitialVolume
 from pwem.objects.data import SetOfClasses2D, SetOfAverages, Volume, SetOfVolumes
 
 from .. import Plugin
-from ..constants import *
+from ..constants import SGD_INPUT_AVG, SGD_INPUT_PTCLS
 
 
 class outputs(Enum):
     outputVolumes = SetOfVolumes
 
 
 class EmanProtInitModelSGD(ProtInitialVolume):
@@ -65,30 +65,29 @@
                       default=SGD_INPUT_AVG,
                       label='Select input type',
                       help='You can choose either class averages '
                       'or particles as input.')
         form.addParam('inputAvg', PointerParam,
                       pointerClass='SetOfClasses2D, SetOfAverages',
                       condition='inputType==%d' % SGD_INPUT_AVG,
-                      # pointerCondition='hasRepresentatives',
                       label="Input averages", important=True,
                       help='Select the class averages to build your '
                            '3D model.\nYou can select SetOfAverages or '
                            'SetOfClasses2D as input.')
         form.addParam('inputPart', PointerParam,
                       pointerClass='SetOfParticles',
                       condition='inputType==%d' % SGD_INPUT_PTCLS,
                       label="Input particles", important=True,
                       help='Select the particles to build your '
                            '3D model.')
         form.addParam('symmetry', StringParam, default='c1',
                       label='Symmetry group',
                       help='Specify the symmetry.\nChoices are: c(n), d(n), '
                            'h(n), tet, oct, icos.\n'
-                           'See http://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
+                           'See https://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
                            'for a detailed description of symmetry in Eman.')
         form.addParam('batchSize', IntParam, default=10,
                       label='Batch size',
                       help='Batch size of stochastic gradient descent. '
                            'N particles are randomly selected to '
                            'generate an initial model at each step.')
         form.addParam('numberOfIterations', IntParam, default=20,
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_reconstruct.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_reconstruct.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 from pyworkflow.constants import PROD
 from pyworkflow.utils.path import cleanPattern, makePath
 from pwem.objects.data import Volume
 from pwem.protocols import ProtReconstruct3D
 
 from .. import Plugin
 from ..convert import writeSetOfParticles
-from ..constants import *
+from ..constants import (RECON_FOURIER, FOURIER_GAUSS2, KEEP_PERCENTAGE,
+                         KEEP_STDDEV, KEEP_ABSQUAL)
 
 
 class outputs(Enum):
     outputVolume = Volume
 
 
 class EmanProtReconstruct(ProtReconstruct3D):
@@ -98,15 +99,15 @@
                            'reconstructed volume, and allows for the '
                            'exclusion of the poorer quality images.')
         form.addParam('symmetry', StringParam, default='c1',
                       label='Symmetry group',
                       help='Set the symmetry; if no value is given then the '
                            'model is assumed to have no symmetry. \n'
                            'Choices are: *i, c, d, tet, icos, or oct* \n'
-                           'See http://blake.bcm.edu/emanwiki/EMAN2/Symmetry \n'
+                           'See https://blake.bcm.edu/emanwiki/EMAN2/Symmetry \n'
                            'for a detailed description of symmetry in Eman.')
         line = form.addLine('Padding to Reconstruct: ',
                             expertLevel=LEVEL_ADVANCED,
                             help='Will zero-pad images to the specifed size '
                                  '(x,y) or (x,x) prior to reconstruction. '
                                  'If not specified no padding occurs.')
         line.addParam('padX', IntParam, default=0, label='X ')
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_refine2d.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_refine2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,10 +641,10 @@
             item.setTransform(rowToAlignment(row[3:], ALIGN_2D))
         else:
             setattr(item, "_appendItem", False)
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
-            index, fn = self._classesInfo[classId]
+            _, fn = self._classesInfo[classId]
             item.setAlignment2D()
             item.getRepresentative().setLocation(classId, fn)
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_refine2d_bispec.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_refine2d_bispec.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,12 +451,12 @@
             item.setClassId(row[2] + 1)
         else:
             setattr(item, "_appendItem", False)
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
-            index, fn = self._classesInfo[classId]
+            _, fn = self._classesInfo[classId]
             item.getRepresentative().setLocation(classId, fn)
 
     def _inputProt(self):
         return self.inputBispec.get()
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_refineasy.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_refineasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from pyworkflow.constants import PROD
 from pyworkflow.protocol.params import (PointerParam, FloatParam, IntParam,
                                         EnumParam, StringParam, BooleanParam)
 from pyworkflow.utils.path import cleanPattern, makePath, createLink
 
 from .. import Plugin
 from ..convert import rowToAlignment, writeSetOfParticles
-from ..constants import *
+from ..constants import TOPHAT_NONE, SPEED_5, AMP_AUTO, EMAN2SCRATCHDIR
 
 
 class outputs(Enum):
     outputVolume = Volume
     outputParticles = SetOfParticles
 
 
@@ -155,15 +155,15 @@
                            'filters. Danger of feature exaggeration.')
         form.addParam('symmetry', StringParam, default='c1',
                       condition='not doContinue',
                       label='Symmetry group',
                       help='Set the symmetry; if no value is given then the '
                            'model is assumed to have no symmetry. \n'
                            'Choices are: c(n), d(n), tet, icos, or oct.\n'
-                           'See http://blake.bcm.edu/emanwiki/EMAN2/Symmetry '
+                           'See https://blake.bcm.edu/emanwiki/EMAN2/Symmetry '
                            'for a detailed description of symmetry in Eman.')
         form.addParam('doBreaksym', BooleanParam, default=False,
                       label='Break symmetry?',
                       help='If set True, reconstruction will be asymmetric '
                            'with *Symmetry group* parameter specifying a '
                            'known pseudosymmetry, not an imposed symmetry.')
         form.addParam('resol', FloatParam, default=25.0,
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols/protocol_tiltvalidate.py` & `scipion-em-eman2-3.6.1/eman2/protocols/protocol_tiltvalidate.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                                         LabelParam, EnumParam, StringParam,
                                         BooleanParam, IntParam, LEVEL_ADVANCED)
 import pyworkflow.utils as pwutils
 from pyworkflow.constants import PROD
 from pwem.protocols import ProtAnalysis3D
 
 from .. import Plugin
-from ..constants import *
+from ..constants import (WIKI_URL, SIMCMP_CHOICES, CMP_CCC, SIMALIGN_CHOICES,
+                         ALN_ROTATE_TRANSLATE, RALN_NONE, CMP_DOT)
 from ..convert import writeSetOfParticles
 
 
 class EmanProtTiltValidate(ProtAnalysis3D):
     """
     This protocol wraps the *e2tiltvalidate.py* EMAN2 program.
     It performs tilt validation using
@@ -72,15 +73,15 @@
                       pointerClass='ParticlesTiltPair',
                       help='Select the input set of tilt pair particles.')
         form.addParam('symmetry', StringParam, default='c1',
                       label='Symmetry group',
                       help='Set the symmetry; if no value is given then '
                            'the model is assumed to have no symmetry. \n'
                            'Choices are: *i, c, d, tet, icos, or oct* \n'
-                           'See http://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
+                           'See https://blake.bcm.edu/emanwiki/EMAN2/Symmetry\n'
                            'for a detailed description of symmetry in Eman.')
         form.addParam('maxtilt', FloatParam, default=180.0,
                       label='Max tilt angle',
                       help='Maximum tilt angle permitted when finding tilt '
                            'distances.')
         form.addParam('quaternion', BooleanParam, default=False,
                       label='Use quaternions', expertLevel=LEVEL_ADVANCED,
```

### Comparing `scipion-em-eman2-3.6/eman2/protocols.conf` & `scipion-em-eman2-3.6.1/eman2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/tests/test_protocols_eman.py` & `scipion-em-eman2-3.6.1/eman2/tests/test_protocols_eman.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 from pyworkflow.tests import BaseTest, setupTestProject, DataSet
 from pwem.protocols import (ProtImportMicrographs, ProtImportParticles, ProtImportVolumes,
                             ProtImportAverages, ProtImportCoordinatesPairs,
                             ProtImportMicrographsTiltPairs)
 from pwem import Domain
 from pyworkflow.utils import magentaStr
 
-from ..protocols import *
-from ..constants import CMP_FRC, ALN_ROTATE_TRANSLATE, RALN_REFINE, AUTO_REF
+from eman2.protocols import *
+from eman2.constants import CMP_FRC, ALN_ROTATE_TRANSLATE, RALN_REFINE, AUTO_REF
 
 
 class TestEmanBase(BaseTest):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dsRelion = DataSet.getDataSet('relion_tutorial')
@@ -47,75 +47,67 @@
         cls.micsFn = cls.dataset.getFile('allMics')
         cls.crdsDir = cls.dataset.getFile('boxingDir')
         cls.particlesFn = cls.dataset.getFile('particles')
         cls.vol = cls.dataset.getFile('volumes')
 
     @classmethod
     def runImportMicrograph(cls, pattern, samplingRate, voltage,
-                            scannedPixelSize, magnification, sphericalAberration):
+                            sphericalAberration):
         """ Run an Import micrograph protocol. """
-        # We have two options: pass the SamplingRate or
-        # the ScannedPixelSize + microscope magnification
-        if samplingRate is not None:
-            cls.protImport = cls.newProtocol(ProtImportMicrographs,
-                                             samplingRateMode=0, filesPath=pattern,
-                                             samplingRate=samplingRate, magnification=magnification,
-                                             voltage=voltage, sphericalAberration=sphericalAberration)
-        else:
-            cls.protImport = cls.newProtocol(ProtImportMicrographs,
-                                             samplingRateMode=1, filesPath=pattern,
-                                             scannedPixelSize=scannedPixelSize,
-                                             voltage=voltage, magnification=magnification,
-                                             sphericalAberration=sphericalAberration)
-
-        cls.proj.launchProtocol(cls.protImport, wait=True)
+        cls.protImport = cls.newProtocol(ProtImportMicrographs,
+                                         filesPath=pattern,
+                                         samplingRate=samplingRate,
+                                         voltage=voltage,
+                                         sphericalAberration=sphericalAberration)
+        cls.launchProtocol(cls.protImport, wait=True)
         cls.assertIsNotNone(cls.protImport.outputMicrographs,
                             "SetOfMicrographs has not been produced.")
 
         return cls.protImport
 
     @classmethod
-    def runImportParticles(cls, pattern, samplingRate, checkStack=False):
+    def runImportParticles(cls, pattern, samplingRate):
         """ Run an Import particles protocol. """
         cls.protImport = cls.newProtocol(ProtImportParticles,
-                                         filesPath=pattern, samplingRate=samplingRate,
-                                         checkStack=checkStack)
+                                         filesPath=pattern,
+                                         samplingRate=samplingRate)
         cls.launchProtocol(cls.protImport)
         cls.assertIsNotNone(cls.protImport.outputParticles,
                             "SetOfParticles has not been produced.")
 
         return cls.protImport
 
     @classmethod
     def runImportParticlesSqlite(cls, pattern, samplingRate):
         """ Run an Import particles protocol. """
         cls.protImport = cls.newProtocol(ProtImportParticles,
                                          importFrom=4,  # from scipion
-                                         sqliteFile=pattern, samplingRate=samplingRate)
+                                         sqliteFile=pattern,
+                                         samplingRate=samplingRate)
         cls.launchProtocol(cls.protImport)
         cls.assertIsNotNone(cls.protImport.outputParticles,
                             "SetOfParticles has not been produced.")
 
         return cls.protImport
 
     @classmethod
     def runImportVolumes(cls, pattern, samplingRate):
         """ Run an Import particles protocol. """
         protImport = cls.newProtocol(ProtImportVolumes,
-                                     filesPath=pattern, samplingRate=samplingRate)
+                                     filesPath=pattern,
+                                     samplingRate=samplingRate)
         cls.launchProtocol(protImport)
         return protImport
 
     @classmethod
     def runImportAverages(cls, pattern, samplingRate):
         """ Run an Import averages protocol. """
         cls.protImportAvg = cls.newProtocol(ProtImportAverages,
                                             filesPath=pattern,
-                                            samplingRate=samplingRate,
-                                            checkStack=True)
+                                            samplingRate=samplingRate)
         cls.launchProtocol(cls.protImportAvg)
         return cls.protImportAvg
 
 
 class TestEmanInitialModelGroel(TestEmanBase):
     @classmethod
     def setUpClass(cls):
@@ -171,16 +163,15 @@
     def test_ReconstructEman(self):
         print(magentaStr("\n==> Importing data - particles:"))
         prot1 = self.newProtocol(ProtImportParticles,
                                  objLabel='from scipion (to-reconstruct)',
                                  importFrom=ProtImportParticles.IMPORT_FROM_SCIPION,
                                  sqliteFile=self.dsRelion.getFile('import/case2/particles.sqlite'),
                                  magnification=10000,
-                                 samplingRate=7.08
-                                 )
+                                 samplingRate=7.08)
         self.launchProtocol(prot1)
 
         print(magentaStr("\n==> Testing eman2 - recostruct:"))
         protReconstruct = self.newProtocol(EmanProtReconstruct)
         protReconstruct.inputParticles.set(prot1.outputParticles)
         self.launchProtocol(protReconstruct)
         self.assertIsNotNone(protReconstruct.outputVolume,
@@ -323,15 +314,15 @@
 class TestEmanCtfAuto(TestEmanBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         TestEmanBase.setData('relion_tutorial')
         cls.partsFn = cls.dataset.getFile('import/case2/particles.sqlite')
         print(magentaStr("\n==> Importing data - particles:"))
-        cls.protImport = cls.runImportParticlesSqlite(cls.partsFn, 3.5)
+        cls.protImport = cls.runImportParticlesSqlite(cls.partsFn, 7.08)
 
     def test_CtfAutoEman(self):
         print(magentaStr("\n==> Testing eman2 - ctf auto:"))
         protCtf = self.newProtocol(EmanProtCTFAuto,
                                    numberOfThreads=3)
         protCtf.inputParticles.set(self.protImport.outputParticles)
         self.launchProtocol(protCtf)
@@ -346,17 +337,15 @@
         TestEmanBase.setData('igbmc_gempicker')
         cls.micsFn = cls.dataset.getFile('micrographs/*.mrc')
         cls.avgFn = cls.dataset.getFile('templates/templates_white.stk')
         print(magentaStr("\n==> Importing data - micrographs:"))
         cls.protImportMics = cls.runImportMicrograph(cls.micsFn,
                                                      samplingRate=4.4,
                                                      voltage=120,
-                                                     sphericalAberration=2.0,
-                                                     scannedPixelSize=None,
-                                                     magnification=60000)
+                                                     sphericalAberration=2.0)
         print(magentaStr("\n==> Importing data - class averages:"))
         cls.protImportAvg = cls.runImportAverages(cls.avgFn, 4.4)
 
     def test_AutopickEman(self):
         print(magentaStr("\n==> Testing eman2 - e2boxer auto:"))
         protPick = self.newProtocol(EmanProtAutopick,
                                     boxerMode=AUTO_REF,
```

### Comparing `scipion-em-eman2-3.6/eman2/viewers/__init__.py` & `scipion-em-eman2-3.6.1/eman2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/eman2/viewers/viewers.py` & `scipion-em-eman2-3.6.1/eman2/viewers/viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,18 +305,16 @@
                             ' Chimera with red spheres.')
         group.addParam('spheresScale', IntParam, default=100,
                        expertLevel=LEVEL_ADVANCED,
                        label='Spheres size',
                        help='')
 
         group = form.addGroup('Resolution')
-        group.addParam('figure', EnumParam, default=0,
-                       choices=['new', 'active'],
-                       label='Figure',
-                       display=EnumParam.DISPLAY_HLIST)
+        group.addHidden('figure', EnumParam, default=0,
+                       choices=['new', 'active'])
         group.addParam('resolutionPlotsFSC', EnumParam,
                        choices=['unmasked', 'masked', 'masked tight', 'all'],
                        default=FSC_UNMASK, display=EnumParam.DISPLAY_COMBO,
                        label='Display resolution plots (FSC)',
                        help='*unmasked*: display FSC of unmasked maps.\n'
                             '*masked*: display FSC of masked maps.\n'
                             '*masked tight*: display FSC of masked tight maps.')
@@ -510,25 +508,22 @@
             return xplotter
         else:
             return
 
     # =========================================================================
     # plotFSC
     # =========================================================================
-    def _getFigure(self):
-        return None if self.figure == 0 else 'active'
-
     def _showFSC(self, paramName=None):
         threshold = self.resolutionThresholdFSC.get()
         fscPlot = self.resolutionPlotsFSC.get()
 
         fscViewer = FscViewer(project=self.protocol.getProject(),
                               threshold=threshold,
                               protocol=self.protocol,
-                              figure=self._getFigure(),
+                              figure=None,
                               addButton=True)
         fscSet = self.protocol._createSetOfFSCs()
 
         for it in self._iterations:
             label = self._getLabel(fscPlot, it)
 
             if label is not None:
@@ -553,15 +548,14 @@
                     fscM = self._plotFSC(fscMask, label='masked it %d' % it)
                     fscT = self._plotFSC(fscMaskTight, label='masked tight it %d' % it)
                     fscSet.append(fscU)
                     fscSet.append(fscM)
                     fscSet.append(fscT)
 
         fscViewer.visualize(fscSet)
-        return [fscViewer]
 
     def _plotFSC(self, fscFn, label):
         res_inv, frc = self._getFscValues(fscFn)
         fsc = FSC(objLabel=label)
         fsc.setData(res_inv, frc)
 
         return fsc
@@ -643,15 +637,15 @@
         """ Figure out the layout of the plots given the number of
         references. """
         if n == 1:
             gridsize = [1, 1]
         elif n == 2:
             gridsize = [2, 1]
         else:
-            gridsize = [(n + 1) / 2, 2]
+            gridsize = [(n + 1) // 2, 2]
 
         return gridsize
 
     def _getFscValues(self, fscFn):
         resolution_inv, frc = [], []
         with open(fscFn) as f1:
             for l in f1:
@@ -753,15 +747,15 @@
         gridsize = self._getGridSize(1)
         xplotter = EmPlotter(x=gridsize[0], y=gridsize[1],
                              windowTitle='Tilt geometry plot')
         plot_title = 'Tilt pair parameter plot'
         a = xplotter.createSubPlot(plot_title, 'Tilt axis', 'Tilt angle',
                                    projection='polar')
 
-        datap, r, theta, zaxis = self._getValues()
+        _, r, theta, zaxis = self._getValues()
 
         if colorzaxis:
             a.scatter(theta, r, c=zaxis)
         else:
             a.scatter(theta, r)
         a.set_rmax(rmax)
```

### Comparing `scipion-em-eman2-3.6/scipion_em_eman2.egg-info/PKG-INFO` & `scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-eman2
-Version: 3.6
+Version: 3.6.1
 Summary: Plugin to use EMAN programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-eman2
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-eman2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-eman2/
@@ -68,15 +68,15 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.52):
+        *EMAN_ENV_ACTIVATION* (default = conda activate eman-2.99.55):
         Command to activate the EMAN environment.
         
         The default scratch directory is assumed */tmp/*. You can change it by setting *EMAN2SCRATCHDIR* in ``scipion.conf`` or your shell environment.
         
         To check the installation, simply run one of the following Scipion tests:
         
         .. code-block::
@@ -93,15 +93,15 @@
            scipion test eman2.tests.test_protocols_eman.TestEmanAutopick
         
         A complete list of tests can also be seen by executing ``scipion test --show --grep eman``
         
         Supported versions
         ------------------
         
-        2.99.47, 2.99.52
+        2.99.47, 2.99.52, 2.99.55
         
         Protocols
         ---------
         
         * boxer
         * boxer auto
         * ctf auto
@@ -116,10 +116,10 @@
         References
         ----------
         
         1. \G. Tang, L. Peng, P.R. Baldwin, D.S. Mann, W. Jiang, I. Rees & S.J. Ludtke. (2007) EMAN2: an extensible image processing suite for electron microscopy. J Struct Biol. 157, 38-46. PMID: 16859925
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-eman2-3.6/scipion_em_eman2.egg-info/SOURCES.txt` & `scipion-em-eman2-3.6.1/scipion_em_eman2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-eman2-3.6/setup.py` & `scipion-em-eman2-3.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
 
         # Indicate who your project is intended for
         #   'Intended Audience :: Users',
 
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

