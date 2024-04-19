# Comparing `tmp/rHDPE_Data_Analysis-1.0.0.tar.gz` & `tmp/rHDPE_Data_Analysis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rHDPE_Data_Analysis-1.0.0.tar", last modified: Fri Apr 19 15:40:58 2024, max compression
+gzip compressed data, was "rHDPE_Data_Analysis-1.0.1.tar", last modified: Fri Apr 19 16:08:37 2024, max compression
```

## Comparing `rHDPE_Data_Analysis-1.0.0.tar` & `rHDPE_Data_Analysis-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 15:40:58.119763 rHDPE_Data_Analysis-1.0.0/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 15:40:58.119007 rHDPE_Data_Analysis-1.0.0/PKG-INFO
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 15:40:58.051453 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 15:40:58.097683 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/
--rw-r--r--   0 philsmith   (501) staff       (20)     2704 2024-02-20 12:55:58.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
--rw-r--r--   0 philsmith   (501) staff       (20)     7997 2024-04-18 15:38:31.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
--rw-r--r--   0 philsmith   (501) staff       (20)     1878 2023-12-22 10:54:22.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
--rw-r--r--   0 philsmith   (501) staff       (20)     9844 2024-03-14 15:29:24.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
--rw-r--r--   0 philsmith   (501) staff       (20)    43726 2024-03-12 12:08:57.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
--rw-r--r--   0 philsmith   (501) staff       (20)    35882 2024-02-22 10:08:47.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/Global_Utilities.py
--rw-r--r--   0 philsmith   (501) staff       (20)       37 2022-08-08 17:17:04.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/__init__.py
-drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 15:40:58.059544 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/
--rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 15:40:57.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/PKG-INFO
--rw-r--r--   0 philsmith   (501) staff       (20)      553 2024-04-19 15:40:57.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/SOURCES.txt
--rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-19 15:40:57.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/dependency_links.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-04-19 15:40:57.000000 rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/top_level.txt
--rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-04-19 15:40:58.119937 rHDPE_Data_Analysis-1.0.0/setup.cfg
--rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-04-19 15:40:44.000000 rHDPE_Data_Analysis-1.0.0/setup.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:08:37.123275 rHDPE_Data_Analysis-1.0.1/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 16:08:37.122315 rHDPE_Data_Analysis-1.0.1/PKG-INFO
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:08:37.090045 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:08:37.114935 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2704 2024-02-20 12:55:58.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     7997 2024-04-18 15:38:31.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1878 2023-12-22 10:54:22.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     9844 2024-03-14 15:29:24.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    43726 2024-03-12 12:08:57.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      148 2023-12-22 10:54:51.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:08:37.121046 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/
+-rw-r--r--   0 philsmith   (501) staff       (20)     2122 2024-02-27 12:52:11.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     1446 2024-01-09 12:15:24.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+-rw-r--r--   0 philsmith   (501) staff       (20)     3534 2024-03-18 15:04:29.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    37985 2024-03-28 13:43:47.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)      120 2024-01-03 12:56:03.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Analysis/__init__.py
+-rw-r--r--   0 philsmith   (501) staff       (20)    35882 2024-02-22 10:08:47.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Utilities.py
+-rw-r--r--   0 philsmith   (501) staff       (20)       37 2022-08-08 17:17:04.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/__init__.py
+drwxr-xr-x   0 philsmith   (501) staff       (20)        0 2024-04-19 16:08:37.092026 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/
+-rw-r--r--   0 philsmith   (501) staff       (20)      353 2024-04-19 16:08:36.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/PKG-INFO
+-rw-r--r--   0 philsmith   (501) staff       (20)      813 2024-04-19 16:08:36.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)        1 2024-04-19 16:08:36.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       20 2024-04-19 16:08:36.000000 rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/top_level.txt
+-rw-r--r--   0 philsmith   (501) staff       (20)       38 2024-04-19 16:08:37.123502 rHDPE_Data_Analysis-1.0.1/setup.cfg
+-rw-r--r--   0 philsmith   (501) staff       (20)      416 2024-04-19 16:01:26.000000 rHDPE_Data_Analysis-1.0.1/setup.py
```

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis/Global_Utilities.py` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis/Global_Utilities.py`

 * *Files identical despite different names*

### Comparing `rHDPE_Data_Analysis-1.0.0/rHDPE_Data_Analysis.egg-info/SOURCES.txt` & `rHDPE_Data_Analysis-1.0.1/rHDPE_Data_Analysis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,8 +6,13 @@
 rHDPE_Data_Analysis.egg-info/dependency_links.txt
 rHDPE_Data_Analysis.egg-info/top_level.txt
 rHDPE_Data_Analysis/FTIR_Analysis/Analysis.py
 rHDPE_Data_Analysis/FTIR_Analysis/FTIR_plotting.py
 rHDPE_Data_Analysis/FTIR_Analysis/Input_Parameters_Class.py
 rHDPE_Data_Analysis/FTIR_Analysis/Preprocessing.py
 rHDPE_Data_Analysis/FTIR_Analysis/Utilities.py
-rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+rHDPE_Data_Analysis/FTIR_Analysis/__init__.py
+rHDPE_Data_Analysis/Global_Analysis/Analysis.py
+rHDPE_Data_Analysis/Global_Analysis/Input_Parameters_Class.py
+rHDPE_Data_Analysis/Global_Analysis/Preprocessing.py
+rHDPE_Data_Analysis/Global_Analysis/Utilities.py
+rHDPE_Data_Analysis/Global_Analysis/__init__.py
```

