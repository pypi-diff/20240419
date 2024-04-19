# Comparing `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.3.tar.gz` & `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.3.tar", last modified: Thu Apr 18 19:07:57 2024, max compression
+gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.4.tar", last modified: Fri Apr 19 12:05:36 2024, max compression
```

## Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.3.tar` & `pkg_newfinalcustom_pipeline_staging_final-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 19:07:57.250676 pkg_newfinalcustom_pipeline_staging_final-0.0.3/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-18 19:07:57.240676 pkg_newfinalcustom_pipeline_staging_final-0.0.3/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/README.md
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 19:07:57.240676 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pipeline_staging_properties_pkg/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pipeline_staging_properties_pkg/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1046 2024-04-18 19:07:10.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pipeline_staging_properties_pkg/pipeline_staging_properties.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-18 19:07:57.240676 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-18 19:07:57.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-18 19:07:57.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-18 19:07:57.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-18 19:07:57.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-18 19:07:57.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-18 19:07:57.250676 pkg_newfinalcustom_pipeline_staging_final-0.0.3/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-18 19:07:40.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.3/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:05:36.341859 pkg_newfinalcustom_pipeline_staging_final-0.0.4/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 12:05:36.341859 pkg_newfinalcustom_pipeline_staging_final-0.0.4/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/README.md
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:05:36.331859 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pipeline_staging_properties_pkg/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pipeline_staging_properties_pkg/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1706 2024-04-19 12:04:03.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pipeline_staging_properties_pkg/pipeline_staging_properties.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:05:36.341859 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 12:05:36.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-19 12:05:36.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-19 12:05:36.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-19 12:05:36.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-19 12:05:36.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-19 12:05:36.341859 pkg_newfinalcustom_pipeline_staging_final-0.0.4/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-19 12:04:41.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.4/setup.py
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.3/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.3/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.4/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.3/setup.py` & `pkg_newfinalcustom_pipeline_staging_final-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pkg-newfinalcustom-pipeline-staging-final",
-    version="0.0.3",
+    version="0.0.4",
     author="Vinay Sriram Iyer",
     author_email="x23203595@student.ncirl.ie",
     description="A package where Custom Pipeline Stages can be managed at the behest of the user",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/x23203595/PipelineStagingSalesManagementSystem.git",
     packages=setuptools.find_packages(),
```

