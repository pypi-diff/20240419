# Comparing `tmp/BioUtensils-0.4.tar.gz` & `tmp/BioUtensils-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioUtensils-0.4.tar", last modified: Thu Apr 18 06:45:18 2024, max compression
+gzip compressed data, was "BioUtensils-0.5.tar", last modified: Fri Apr 19 14:46:51 2024, max compression
```

## Comparing `BioUtensils-0.4.tar` & `BioUtensils-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:45:18.755973 BioUtensils-0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:45:18.755973 BioUtensils-0.4/BioUtensils/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 06:45:16.000000 BioUtensils-0.4/BioUtensils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-18 06:45:16.000000 BioUtensils-0.4/BioUtensils/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-18 06:45:16.000000 BioUtensils-0.4/BioUtensils/rgb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:45:18.755973 BioUtensils-0.4/BioUtensils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 06:45:18.000000 BioUtensils-0.4/BioUtensils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 06:45:18.000000 BioUtensils-0.4/BioUtensils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:45:18.000000 BioUtensils-0.4/BioUtensils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 06:45:18.000000 BioUtensils-0.4/BioUtensils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 06:45:18.000000 BioUtensils-0.4/BioUtensils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-18 06:45:18.755973 BioUtensils-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 06:45:16.000000 BioUtensils-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:45:18.755973 BioUtensils-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-18 06:45:18.000000 BioUtensils-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.736076 BioUtensils-0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.732076 BioUtensils-0.5/BioUtensils/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 14:46:42.000000 BioUtensils-0.5/BioUtensils/rgb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:46:51.732076 BioUtensils-0.5/BioUtensils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 14:46:51.000000 BioUtensils-0.5/BioUtensils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-19 14:46:51.736076 BioUtensils-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 14:46:42.000000 BioUtensils-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:46:51.736076 BioUtensils-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 14:46:49.000000 BioUtensils-0.5/setup.py
```

### Comparing `BioUtensils-0.4/BioUtensils/normalize.py` & `BioUtensils-0.5/BioUtensils/normalize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from scipy.ndimage import binary_dilation
 from skimage.morphology import disk
 
 def subtract_background(image, masks, expand_masks=None):
     
+    masks = masks.copy()
     masks[masks != 0] = 1
     
     if expand_masks is not None:
         masks = binary_dilation(masks, iterations=expand_masks, structure=disk(5)).astype(masks.dtype)
         
     background = np.median(image[masks == 0], axis=0)
```

### Comparing `BioUtensils-0.4/BioUtensils/rgb_utils.py` & `BioUtensils-0.5/BioUtensils/rgb_utils.py`

 * *Files identical despite different names*

### Comparing `BioUtensils-0.4/setup.py` & `BioUtensils-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read_requirements():
     with open('requirements.txt', 'r') as file:
         return [line.strip() for line in file.readlines()]
 
 setup(
     name=package_name,
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=read_requirements(),
     author="Simon Gutwein",
     include_package_data=True,
     author_email="simon.gutwein@ccri.at",
     description="",
     long_description=open('README.md').read(),
```

