# Comparing `tmp/aeroterra_ds-1.0.0.tar.gz` & `tmp/aeroterra_ds-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.0.tar", last modified: Fri Apr 19 15:55:53 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.0.1.tar", last modified: Fri Apr 19 16:00:32 2024, max compression
```

## Comparing `aeroterra_ds-1.0.0.tar` & `aeroterra_ds-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:53.764425 aeroterra_ds-1.0.0/
--rw-rw-rw-   0        0        0      488 2024-04-19 15:55:53.763394 aeroterra_ds-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 15:55:53.760305 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0      488 2024-04-19 15:55:53.000000 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-19 15:55:53.000000 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:55:53.000000 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-19 15:55:53.000000 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 15:55:53.000000 aeroterra_ds-1.0.0/aeroterra_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 15:55:53.765934 aeroterra_ds-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-19 15:55:35.000000 aeroterra_ds-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 16:00:32.023395 aeroterra_ds-1.0.1/
+-rw-rw-rw-   0        0        0      488 2024-04-19 16:00:32.023395 aeroterra_ds-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 16:00:32.021406 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-04-19 16:00:31.000000 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-19 16:00:31.000000 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:00:31.000000 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-19 16:00:31.000000 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 16:00:31.000000 aeroterra_ds-1.0.1/aeroterra_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 16:00:32.024901 aeroterra_ds-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-04-19 16:00:25.000000 aeroterra_ds-1.0.1/setup.py
```

### Comparing `aeroterra_ds-1.0.0/setup.py` & `aeroterra_ds-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.0.0',
+    version='1.0.1',
     author='Data Science',
     author_email='pedrofuentes7799@gmail.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     packages=find_packages(),
@@ -17,14 +17,14 @@
     ],
     keywords='arcgis',
     python_requires='>=3.11',
     install_requires=[
         "gssapi",
         "dask",
         "arcgis",
-        "pyproj"
+        "pyproj",
         "shapely",
         "matplotlib",
         "geopandas",
         "pandas",
     ],
 )
```

