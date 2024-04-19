# Comparing `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.7.tar.gz` & `tmp/pkg_newfinalcustom_pipeline_staging_final-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.7.tar", last modified: Fri Apr 19 12:54:14 2024, max compression
+gzip compressed data, was "pkg_newfinalcustom_pipeline_staging_final-0.0.8.tar", last modified: Fri Apr 19 13:16:18 2024, max compression
```

## Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.7.tar` & `pkg_newfinalcustom_pipeline_staging_final-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:54:14.715600 pkg_newfinalcustom_pipeline_staging_final-0.0.7/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 12:54:14.715600 pkg_newfinalcustom_pipeline_staging_final-0.0.7/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/README.md
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:54:14.705600 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pipeline_staging_properties_pkg/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pipeline_staging_properties_pkg/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2125 2024-04-19 12:53:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pipeline_staging_properties_pkg/pipeline_staging_properties.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 12:54:14.715600 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 12:54:14.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-19 12:54:14.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-19 12:54:14.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-19 12:54:14.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-19 12:54:14.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-19 12:54:14.715600 pkg_newfinalcustom_pipeline_staging_final-0.0.7/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-19 12:53:05.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.7/setup.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 13:16:17.990887 pkg_newfinalcustom_pipeline_staging_final-0.0.8/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:58.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 13:16:17.990887 pkg_newfinalcustom_pipeline_staging_final-0.0.8/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:52.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/README.md
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 13:16:17.980887 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pipeline_staging_properties_pkg/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-16 21:51:24.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pipeline_staging_properties_pkg/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2044 2024-04-19 13:11:46.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pipeline_staging_properties_pkg/pipeline_staging_properties.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-19 13:16:17.990887 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      574 2024-04-19 13:16:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      457 2024-04-19 13:16:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-19 13:16:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        6 2024-04-19 13:16:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/requires.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       32 2024-04-19 13:16:17.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/top_level.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-19 13:16:17.990887 pkg_newfinalcustom_pipeline_staging_final-0.0.8/setup.cfg
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      836 2024-04-19 13:16:03.000000 pkg_newfinalcustom_pipeline_staging_final-0.0.8/setup.py
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.7/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.7/pipeline_staging_properties_pkg/pipeline_staging_properties.py` & `pkg_newfinalcustom_pipeline_staging_final-0.0.8/pipeline_staging_properties_pkg/pipeline_staging_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,18 @@
         except ClientError as e:
             if e.response['Error']['Code'] == '404':
                 return False
             else:
                 print(f"An error occurred while checking if stage '{stage_name}' exists: {e}")
                 return False
             
-    def upload_stage(self, stage_name):
+    def upload_stage(self, stage_name, new_content):
         try:
-            response = self.s3_client.get_object(Bucket=self.bucket_name, Key=stage_name)
-            current_content = response['Body'].read().decode('utf-8')
-            modified_content = modify_content(current_content)
+            modified_content = modify_content(new_content)
             self.s3_client.put_object(Bucket=self.bucket_name, Key=stage_name, Body=modified_content.encode('utf-8'))
+            print(f"Stage '{stage_name}' successfully updated in S3")
         except ClientError as e:
             print(f"An error occurred while editing stage {stage_name}: {e}")
 
 def modify_content(current_content):
     modified_content = current_content + "\nModified content"
     return modified_content
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.7/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO` & `pkg_newfinalcustom_pipeline_staging_final-0.0.8/pkg_newfinalcustom_pipeline_staging_final.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-newfinalcustom-pipeline-staging-final
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package where Custom Pipeline Stages can be managed at the behest of the user
 Home-page: https://github.com/x23203595/PipelineStagingSalesManagementSystem.git
 Author: Vinay Sriram Iyer
 Author-email: x23203595@student.ncirl.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pkg_newfinalcustom_pipeline_staging_final-0.0.7/setup.py` & `pkg_newfinalcustom_pipeline_staging_final-0.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pkg-newfinalcustom-pipeline-staging-final",
-    version="0.0.7",
+    version="0.0.8",
     author="Vinay Sriram Iyer",
     author_email="x23203595@student.ncirl.ie",
     description="A package where Custom Pipeline Stages can be managed at the behest of the user",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/x23203595/PipelineStagingSalesManagementSystem.git",
     packages=setuptools.find_packages(),
```

