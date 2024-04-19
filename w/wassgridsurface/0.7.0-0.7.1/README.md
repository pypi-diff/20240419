# Comparing `tmp/wassgridsurface-0.7.tar.gz` & `tmp/wassgridsurface-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-36y3l1ge/wassgridsurface-0.7.tar", last modified: Fri Apr 12 19:57:42 2024, max compression
+gzip compressed data, was "/home/fibe/projects/wass/gridding/dist/.tmp-3t_5bo1k/wassgridsurface-0.7.1.tar", last modified: Fri Apr 19 09:14:11 2024, max compression
```

## Comparing `wassgridsurface-0.7.tar` & `wassgridsurface-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.856318 wassgridsurface-0.7/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.7/.gitignore
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-05-09 15:56:57.000000 wassgridsurface-0.7/BUILD.md
--rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-12 19:57:42.856318 wassgridsurface-0.7/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-05-09 15:56:57.000000 wassgridsurface-0.7/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.7/environment.yml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-05-09 15:56:57.000000 wassgridsurface-0.7/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-12 19:57:42.856318 wassgridsurface-0.7/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.852318 wassgridsurface-0.7/wassgridsurface/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4947 2023-05-09 15:56:57.000000 wassgridsurface-0.7/wassgridsurface/DCTInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.7/wassgridsurface/IDWInterpolator.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.7/wassgridsurface/TFVariationalRefinement.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.7/wassgridsurface/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.7/wassgridsurface/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6200 2024-04-12 15:10:55.000000 wassgridsurface-0.7/wassgridsurface/netcdfoutput.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.7/wassgridsurface/wass_utils.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    26002 2024-04-12 19:33:14.000000 wassgridsurface-0.7/wassgridsurface/wassgridsurface.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 19:57:42.856318 wassgridsurface-0.7/wassgridsurface.egg-info/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2024-04-12 19:57:42.000000 wassgridsurface-0.7/wassgridsurface.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-19 09:14:11.518946 wassgridsurface-0.7.1/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       54 2022-08-23 15:16:12.000000 wassgridsurface-0.7.1/.gitignore
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      497 2023-05-09 15:56:57.000000 wassgridsurface-0.7.1/BUILD.md
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-19 09:14:11.514946 wassgridsurface-0.7.1/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1145 2023-05-09 15:56:57.000000 wassgridsurface-0.7.1/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      260 2022-08-22 15:00:31.000000 wassgridsurface-0.7.1/environment.yml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1173 2023-05-09 15:56:57.000000 wassgridsurface-0.7.1/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-19 09:14:11.518946 wassgridsurface-0.7.1/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-19 09:14:11.514946 wassgridsurface-0.7.1/wassgridsurface/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4947 2023-05-09 15:56:57.000000 wassgridsurface-0.7.1/wassgridsurface/DCTInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1867 2022-08-23 14:41:27.000000 wassgridsurface-0.7.1/wassgridsurface/IDWInterpolator.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5232 2022-05-02 07:00:38.000000 wassgridsurface-0.7.1/wassgridsurface/TFVariationalRefinement.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      734 2022-08-23 14:39:43.000000 wassgridsurface-0.7.1/wassgridsurface/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      780 2022-08-23 14:39:51.000000 wassgridsurface-0.7.1/wassgridsurface/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6200 2024-04-16 21:26:37.000000 wassgridsurface-0.7.1/wassgridsurface/netcdfoutput.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     5113 2022-08-23 14:40:49.000000 wassgridsurface-0.7.1/wassgridsurface/wass_utils.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    26042 2024-04-19 09:13:28.000000 wassgridsurface-0.7.1/wassgridsurface/wassgridsurface.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-19 09:14:11.514946 wassgridsurface-0.7.1/wassgridsurface.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     1843 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      562 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       73 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       72 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       16 2024-04-19 09:14:11.000000 wassgridsurface-0.7.1/wassgridsurface.egg-info/top_level.txt
```

### Comparing `wassgridsurface-0.7/PKG-INFO` & `wassgridsurface-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.7.0
+Version: 0.7.1
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
```

### Comparing `wassgridsurface-0.7/README.md` & `wassgridsurface-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/pyproject.toml` & `wassgridsurface-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/DCTInterpolator.py` & `wassgridsurface-0.7.1/wassgridsurface/DCTInterpolator.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/IDWInterpolator.py` & `wassgridsurface-0.7.1/wassgridsurface/IDWInterpolator.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/TFVariationalRefinement.py` & `wassgridsurface-0.7.1/wassgridsurface/TFVariationalRefinement.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/__init__.py` & `wassgridsurface-0.7.1/wassgridsurface/__init__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/__main__.py` & `wassgridsurface-0.7.1/wassgridsurface/__main__.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/netcdfoutput.py` & `wassgridsurface-0.7.1/wassgridsurface/netcdfoutput.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/wass_utils.py` & `wassgridsurface-0.7.1/wassgridsurface/wass_utils.py`

 * *Files identical despite different names*

### Comparing `wassgridsurface-0.7/wassgridsurface/wassgridsurface.py` & `wassgridsurface-0.7.1/wassgridsurface/wassgridsurface.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
-VERSION = "0.7.0"
+VERSION = "0.7.1"
 
+import matplotlib
+matplotlib.use('AGG')
+import matplotlib.pyplot as plt
 
 import argparse
 import configparser
 import scipy.io as sio
 import scipy.interpolate
 import os
 import sys
 import glob
 import time
 import numpy as np
-import matplotlib.pyplot as plt
 import cv2 as cv
 from os import path
 from tqdm import tqdm
 from tqdm.contrib.concurrent import thread_map
 
 
 import colorama
```

### Comparing `wassgridsurface-0.7/wassgridsurface.egg-info/PKG-INFO` & `wassgridsurface-0.7.1/wassgridsurface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassgridsurface
-Version: 0.7.0
+Version: 0.7.1
 Summary: WASS surface gridding tool
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: homepage, https://sites.google.com/unive.it/wass
 Project-URL: repository, https://github.com/fbergama/wass/tree/master/gridding
 Keywords: WASS,3D,Interpolation
```

### Comparing `wassgridsurface-0.7/wassgridsurface.egg-info/SOURCES.txt` & `wassgridsurface-0.7.1/wassgridsurface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

