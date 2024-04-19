# Comparing `tmp/nisupply-1.1.0.tar.gz` & `tmp/nisupply-2023.3.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nisupply-1.1.0.tar", last modified: Fri Apr 19 10:06:42 2024, max compression
+gzip compressed data, was "nisupply-2023.3.10.tar", last modified: Fri Mar 10 14:29:54 2023, max compression
```

## Comparing `nisupply-1.1.0.tar` & `nisupply-2023.3.10.tar`

### file list

```diff
@@ -1,31 +1,18 @@
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.342530 nisupply-1.1.0/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      394 2024-04-19 09:54:28.000000 nisupply-1.1.0/.gitignore
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     1073 2024-04-19 09:54:28.000000 nisupply-1.1.0/LICENSE
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     5807 2024-04-19 10:06:42.339530 nisupply-1.1.0/PKG-INFO
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     5158 2024-04-19 09:54:28.000000 nisupply-1.1.0/README.md
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.234530 nisupply-1.1.0/docs/
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.249530 nisupply-1.1.0/docs/example_dataset/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/fmri_nback_subject_3_session_2.nii.gz
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.260530 nisupply-1.1.0/docs/example_dataset/subject_1/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/subject_1/fmri_gambling.nii.gz
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/subject_1/fmri_nback.nii.gz
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.266530 nisupply-1.1.0/docs/example_dataset/subject_1/session_2/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/subject_1/session_2/fmri_nback.nii.gz
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/subject_2_fmri_nback.nii.gz
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_dataset/subject_4.txt
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      527 2024-04-19 09:54:28.000000 nisupply-1.1.0/docs/example_script.py
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.289530 nisupply-1.1.0/nisupply/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2024-04-19 09:54:28.000000 nisupply-1.1.0/nisupply/__init__.py
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     8709 2024-04-19 10:02:03.000000 nisupply-1.1.0/nisupply/io.py
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     1949 2024-04-19 09:54:28.000000 nisupply-1.1.0/nisupply/structure.py
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     2354 2024-04-19 09:54:28.000000 nisupply-1.1.0/nisupply/utils.py
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.331530 nisupply-1.1.0/nisupply.egg-info/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     5807 2024-04-19 10:06:42.000000 nisupply-1.1.0/nisupply.egg-info/PKG-INFO
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      629 2024-04-19 10:06:42.000000 nisupply-1.1.0/nisupply.egg-info/SOURCES.txt
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        1 2024-04-19 10:06:42.000000 nisupply-1.1.0/nisupply.egg-info/dependency_links.txt
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)       13 2024-04-19 10:06:42.000000 nisupply-1.1.0/nisupply.egg-info/requires.txt
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        9 2024-04-19 10:06:42.000000 nisupply-1.1.0/nisupply.egg-info/top_level.txt
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      813 2024-04-19 10:05:13.000000 nisupply-1.1.0/pyproject.toml
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)       38 2024-04-19 10:06:42.344530 nisupply-1.1.0/setup.cfg
-drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2024-04-19 10:06:42.325530 nisupply-1.1.0/testing/
--rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     2350 2024-04-19 09:54:28.000000 nisupply-1.1.0/testing/test_nisupply.py
+drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2023-03-10 14:29:54.911918 nisupply-2023.3.10/
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)       70 2023-03-07 19:28:41.000000 nisupply-2023.3.10/.gitignore
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     1524 2023-03-07 19:28:41.000000 nisupply-2023.3.10/LICENSE
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     3576 2023-03-10 14:29:54.911918 nisupply-2023.3.10/PKG-INFO
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     2966 2023-03-10 11:41:44.000000 nisupply-2023.3.10/README.md
+drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2023-03-10 14:29:54.911918 nisupply-2023.3.10/nisupply/
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        2 2023-03-09 19:46:48.000000 nisupply-2023.3.10/nisupply/__init__.py
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     5153 2023-03-09 20:53:23.000000 nisupply-2023.3.10/nisupply/bids.py
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     7868 2023-03-09 20:53:28.000000 nisupply-2023.3.10/nisupply/io.py
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     4256 2023-03-09 20:15:46.000000 nisupply-2023.3.10/nisupply/utils.py
+drwxr-xr-x   0 johannes.wiesner (154520) domänen-benutzer (100513)        0 2023-03-10 14:29:54.911918 nisupply-2023.3.10/nisupply.egg-info/
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)     3576 2023-03-10 14:29:54.000000 nisupply-2023.3.10/nisupply.egg-info/PKG-INFO
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      273 2023-03-10 14:29:54.000000 nisupply-2023.3.10/nisupply.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        1 2023-03-10 14:29:54.000000 nisupply-2023.3.10/nisupply.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)       13 2023-03-10 14:29:54.000000 nisupply-2023.3.10/nisupply.egg-info/requires.txt
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)        9 2023-03-10 14:29:54.000000 nisupply-2023.3.10/nisupply.egg-info/top_level.txt
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)      817 2023-03-10 14:29:25.000000 nisupply-2023.3.10/pyproject.toml
+-rw-r--r--   0 johannes.wiesner (154520) domänen-benutzer (100513)       38 2023-03-10 14:29:54.911918 nisupply-2023.3.10/setup.cfg
```

### Comparing `nisupply-1.1.0/pyproject.toml` & `nisupply-2023.3.10/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nisupply"
-version= "1.1.0"
+version= "2023.03.10"
 authors = [
     {name = "Johannes Wiesner", email = "joh.wiesner@gmail.com"},
 ]
 description = "A python module for dealing with unstructured or semi-structured neuroimaging datasets which do not conform to the BIDS data structure"
 readme = "README.md"
 keywords = ["files","utility","neuroscience","neuroimaging","file-management"]
 license = {text = "MIT"}
@@ -22,8 +22,8 @@
     "pandas"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/JohannesWiesner/nisupply"
 
 [tool.setuptools]
-packages = ["nisupply"]
+packages = ["nisupply"]
```

