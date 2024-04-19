# Comparing `tmp/aeroterra_ds-1.0.2.tar.gz` & `tmp/aeroterra_ds-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.2.tar", last modified: Fri Apr 19 18:26:00 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.0.3.tar", last modified: Fri Apr 19 18:26:58 2024, max compression
```

## Comparing `aeroterra_ds-1.0.2.tar` & `aeroterra_ds-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 18:26:00.089219 aeroterra_ds-1.0.2/
--rw-rw-rw-   0        0        0      487 2024-04-19 18:26:00.087195 aeroterra_ds-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 18:26:00.086196 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0      487 2024-04-19 18:25:59.000000 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-19 18:26:00.000000 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 18:25:59.000000 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-19 18:25:59.000000 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 18:25:59.000000 aeroterra_ds-1.0.2/aeroterra_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 18:26:00.090738 aeroterra_ds-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      856 2024-04-19 18:25:58.000000 aeroterra_ds-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/
+-rw-rw-rw-   0        0        0      484 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-19 15:53:17.000000 aeroterra_ds-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 18:26:58.028451 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0      484 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 18:26:57.000000 aeroterra_ds-1.0.3/aeroterra_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 18:26:58.029463 aeroterra_ds-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      853 2024-04-19 18:26:54.000000 aeroterra_ds-1.0.3/setup.py
```

### Comparing `aeroterra_ds-1.0.2/setup.py` & `aeroterra_ds-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.0.2',
+    version='1.0.3',
     author='Data Science',
     author_email='pedrofuentes7799@gmail.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     packages=find_packages(),
     classifiers=[
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     keywords='arcgis',
     python_requires='>=3.6',
     install_requires=[
         "gssapi",
```

