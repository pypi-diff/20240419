# Comparing `tmp/aeroterra_ds-1.0.3.tar.gz` & `tmp/aeroterra_ds-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.3.tar", last modified: Fri Apr 19 18:26:58 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.0.4.tar", last modified: Fri Apr 19 18:41:09 2024, max compression
```

## Comparing `aeroterra_ds-1.0.3.tar` & `aeroterra_ds-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/
--rw-rw-rw-   0        0        0      484 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 18:26:58.028451 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0      484 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      853 2024-04-19 18:26:54.000000 aeroterra_ds-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:41:09.530485 aeroterra_ds-1.0.4/
+-rw-rw-rw-   0        0        0      529 2024-04-19 18:41:09.530485 aeroterra_ds-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2024-04-19 18:35:35.000000 aeroterra_ds-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      660 2024-04-19 18:41:09.532847 aeroterra_ds-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-19 18:41:08.000000 aeroterra_ds-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:41:09.505973 aeroterra_ds-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 18:41:09.519070 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0      529 2024-04-19 18:41:09.000000 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-19 18:41:09.000000 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 18:41:09.000000 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-19 18:41:09.000000 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-19 18:41:09.000000 aeroterra_ds-1.0.4/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 18:41:09.529485 aeroterra_ds-1.0.4/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.0.4/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-04-19 15:50:56.000000 aeroterra_ds-1.0.4/src/layers/change_crs.py
+-rw-rw-rw-   0        0        0     1405 2024-04-18 20:25:51.000000 aeroterra_ds-1.0.4/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.0.4/src/layers/constants.py
+-rw-rw-rw-   0        0        0     5385 2024-04-18 20:36:38.000000 aeroterra_ds-1.0.4/src/layers/geometry.py
+-rw-rw-rw-   0        0        0    13621 2024-04-18 21:03:10.000000 aeroterra_ds-1.0.4/src/layers/layers.py
+-rw-rw-rw-   0        0        0     3897 2024-04-18 20:36:52.000000 aeroterra_ds-1.0.4/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.0.4/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.0.3/setup.py` & `aeroterra_ds-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import setup, find_packages
 
+#print(find_packages("src"))
+
 setup(
     name='aeroterra_ds',
-    version='1.0.3',
+    version='1.0.4',
     author='Data Science',
-    author_email='pedrofuentes7799@gmail.com',
+    author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
```

