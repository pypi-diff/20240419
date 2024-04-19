# Comparing `tmp/aeroterra_ds-1.0.5.tar.gz` & `tmp/aeroterra_ds-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.5.tar", last modified: Fri Apr 19 19:53:59 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.0.6.tar", last modified: Fri Apr 19 20:12:50 2024, max compression
```

## Comparing `aeroterra_ds-1.0.5.tar` & `aeroterra_ds-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 19:53:59.334448 aeroterra_ds-1.0.5/
--rw-rw-rw-   0        0        0     1306 2024-04-19 19:53:59.333450 aeroterra_ds-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      835 2024-04-19 19:51:22.000000 aeroterra_ds-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 19:53:59.332447 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1306 2024-04-19 19:53:59.000000 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-19 19:53:59.000000 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:53:59.000000 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-19 19:53:59.000000 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 19:53:59.000000 aeroterra_ds-1.0.5/aeroterra_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 19:53:59.334448 aeroterra_ds-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-04-19 19:53:47.000000 aeroterra_ds-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:12:50.683110 aeroterra_ds-1.0.6/
+-rw-rw-rw-   0        0        0     1306 2024-04-19 20:12:50.683110 aeroterra_ds-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2024-04-19 19:51:22.000000 aeroterra_ds-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-19 20:12:50.684110 aeroterra_ds-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-04-19 20:12:49.000000 aeroterra_ds-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:12:50.663454 aeroterra_ds-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 20:12:50.671152 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1306 2024-04-19 20:12:50.000000 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-04-19 20:12:50.000000 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 20:12:50.000000 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-19 20:12:50.000000 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-19 20:12:50.000000 aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 20:12:50.674150 aeroterra_ds-1.0.6/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.0.6/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     2908 2024-04-19 15:50:56.000000 aeroterra_ds-1.0.6/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.0.6/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-04-19 20:12:50.682103 aeroterra_ds-1.0.6/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.0.6/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1405 2024-04-18 20:25:51.000000 aeroterra_ds-1.0.6/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.0.6/src/layers/constants.py
+-rw-rw-rw-   0        0        0     3096 2024-04-19 19:15:15.000000 aeroterra_ds-1.0.6/src/layers/fields.py
+-rw-rw-rw-   0        0        0    10642 2024-04-19 19:51:23.000000 aeroterra_ds-1.0.6/src/layers/layers.py
+-rw-rw-rw-   0        0        0     3897 2024-04-18 20:36:52.000000 aeroterra_ds-1.0.6/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.0.6/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.0.5/PKG-INFO` & `aeroterra_ds-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.0.5/README.md` & `aeroterra_ds-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.5/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.0.6/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.0.5/setup.py` & `aeroterra_ds-1.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
-#print(find_packages("src"))
-
 setup(
     name='aeroterra_ds',
-    version='1.0.5',
+    version='1.0.6',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
-    packages=find_packages(),
+    package_dir={'': "src"},
+    packages=find_packages("src"),
     classifiers=[
         'Programming Language :: Python :: 3',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     keywords='arcgis',
     python_requires='>=3.6',
```

