# Comparing `tmp/accusort-0.3.tar.gz` & `tmp/accusort-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accusort-0.3.tar", last modified: Fri Apr 19 10:32:04 2024, max compression
+gzip compressed data, was "accusort-0.5.tar", last modified: Fri Apr 19 10:40:41 2024, max compression
```

## Comparing `accusort-0.3.tar` & `accusort-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:32:04.442430 accusort-0.3/
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      238 2024-04-19 10:32:04.442430 accusort-0.3/PKG-INFO
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      363 2024-04-19 07:28:51.000000 accusort-0.3/README.md
-drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:32:04.438427 accusort-0.3/accusort.egg-info/
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      238 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/PKG-INFO
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      352 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/SOURCES.txt
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        1 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/dependency_links.txt
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)       46 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/entry_points.txt
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      518 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/requires.txt
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        6 2024-04-19 10:32:04.000000 accusort-0.3/accusort.egg-info/top_level.txt
-drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:32:04.438427 accusort-0.3/eagle/
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-18 06:28:56.000000 accusort-0.3/eagle/__init__.py
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     4016 2024-04-19 09:20:38.000000 accusort-0.3/eagle/main.py
-drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:32:04.442430 accusort-0.3/eagle/scripts/
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-18 03:31:02.000000 accusort-0.3/eagle/scripts/__init__.py
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      674 2024-04-18 03:31:02.000000 accusort-0.3/eagle/scripts/banner.txt
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     4738 2024-04-18 03:31:02.000000 accusort-0.3/eagle/scripts/document_reader.py
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     1156 2024-04-19 08:47:02.000000 accusort-0.3/eagle/scripts/pl_art.py
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)       38 2024-04-19 10:32:04.442430 accusort-0.3/setup.cfg
--rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     2706 2024-04-19 10:31:58.000000 accusort-0.3/setup.py
+drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:40:41.545206 accusort-0.5/
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     1212 2024-04-19 10:40:41.545206 accusort-0.5/PKG-INFO
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      363 2024-04-19 07:28:51.000000 accusort-0.5/README.md
+drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:40:41.545206 accusort-0.5/accusort.egg-info/
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     1212 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/PKG-INFO
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      352 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/SOURCES.txt
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        1 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/dependency_links.txt
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)       46 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/entry_points.txt
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      518 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/requires.txt
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        6 2024-04-19 10:40:41.000000 accusort-0.5/accusort.egg-info/top_level.txt
+drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:40:41.545206 accusort-0.5/eagle/
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-18 06:28:56.000000 accusort-0.5/eagle/__init__.py
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     4016 2024-04-19 09:20:38.000000 accusort-0.5/eagle/main.py
+drwxrwxr-x   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-19 10:40:41.545206 accusort-0.5/eagle/scripts/
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)        0 2024-04-18 03:31:02.000000 accusort-0.5/eagle/scripts/__init__.py
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)      674 2024-04-18 03:31:02.000000 accusort-0.5/eagle/scripts/banner.txt
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     4738 2024-04-18 03:31:02.000000 accusort-0.5/eagle/scripts/document_reader.py
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     1156 2024-04-19 08:47:02.000000 accusort-0.5/eagle/scripts/pl_art.py
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)       38 2024-04-19 10:40:41.545206 accusort-0.5/setup.cfg
+-rw-rw-r--   0 sangeeth  (1000) sangeeth  (1000)     2870 2024-04-19 10:39:35.000000 accusort-0.5/setup.py
```

### Comparing `accusort-0.3/accusort.egg-info/requires.txt` & `accusort-0.5/accusort.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `accusort-0.3/eagle/main.py` & `accusort-0.5/eagle/main.py`

 * *Files identical despite different names*

### Comparing `accusort-0.3/eagle/scripts/banner.txt` & `accusort-0.5/eagle/scripts/banner.txt`

 * *Files identical despite different names*

### Comparing `accusort-0.3/eagle/scripts/document_reader.py` & `accusort-0.5/eagle/scripts/document_reader.py`

 * *Files identical despite different names*

### Comparing `accusort-0.3/eagle/scripts/pl_art.py` & `accusort-0.5/eagle/scripts/pl_art.py`

 * *Files identical despite different names*

### Comparing `accusort-0.3/setup.py` & `accusort-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 env_file = os.path.join(os.path.dirname(__file__), '.env')
 
 # Load the environment variables from the .env file
 dotenv.load_dotenv(dotenv_path=env_file)
 
 setup(
     name='accusort',
-    version='0.3',
-    description='''
+    version='0.5',
+    description="AccuSort is a Python package that sorts image PDF files into segregated folders based on the accuracy of PN numbers detected in the image and the file name.",
+    long_description='''
     AccuSort
     ========
 
     AccuSort is a Python package that sorts image PDF files into segregated folders based on the accuracy of PN numbers detected in the image and the file name.
 
     Installation
     ------------
@@ -39,15 +40,15 @@
     2. Run the following command to sort the images:
        ```
        accusort <image_master_folder_name>
        ```
     3. The script saves the segragated folders in the respective subfolders of images.
 
     ''',
-    long_description='A more detailed description of your package',
+    long_description_content_type='text/markdown',
     author='Sixtysix Technologies',
     author_email='sangeeth@sixtysixtech.com',
         packages=find_packages(include=['eagle', 'eagle.*','eagle.scripts']),
         package_data={
             'eagle': ['scripts/banner.txt'],
         },
     install_requires=[
```

