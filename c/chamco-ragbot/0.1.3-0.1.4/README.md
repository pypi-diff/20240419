# Comparing `tmp/chamco_ragbot-0.1.3.tar.gz` & `tmp/chamco_ragbot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamco_ragbot-0.1.3.tar", last modified: Fri Apr 19 04:06:59 2024, max compression
+gzip compressed data, was "chamco_ragbot-0.1.4.tar", last modified: Fri Apr 19 04:35:59 2024, max compression
```

## Comparing `chamco_ragbot-0.1.3.tar` & `chamco_ragbot-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/PKG-INFO
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/chamco_ragbot/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3008 2024-04-19 02:14:39.000000 chamco_ragbot-0.1.3/chamco_ragbot/acl.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.3/chamco_ragbot/datasource.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.3/chamco_ragbot/dept.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/filetransfer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.3/chamco_ragbot/index.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/indexer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7531 2024-04-19 03:49:52.000000 chamco_ragbot-0.1.3/chamco_ragbot/main.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/search.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/skillset.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.3/chamco_ragbot/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/top_level.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:35:59.277279 chamco_ragbot-0.1.4/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:35:59.277279 chamco_ragbot-0.1.4/PKG-INFO
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:35:59.277279 chamco_ragbot-0.1.4/chamco_ragbot/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3008 2024-04-19 02:14:39.000000 chamco_ragbot-0.1.4/chamco_ragbot/acl.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.4/chamco_ragbot/datasource.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.4/chamco_ragbot/dept.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/filetransfer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.4/chamco_ragbot/index.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/indexer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7531 2024-04-19 03:49:52.000000 chamco_ragbot-0.1.4/chamco_ragbot/main.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/search.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.4/chamco_ragbot/skillset.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.4/chamco_ragbot/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:35:59.277279 chamco_ragbot-0.1.4/chamco_ragbot.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:35:59.000000 chamco_ragbot-0.1.4/chamco_ragbot.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 04:35:59.000000 chamco_ragbot-0.1.4/chamco_ragbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 04:35:59.000000 chamco_ragbot-0.1.4/chamco_ragbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 04:35:59.000000 chamco_ragbot-0.1.4/chamco_ragbot.egg-info/top_level.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 04:35:59.277279 chamco_ragbot-0.1.4/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-19 04:34:45.000000 chamco_ragbot-0.1.4/setup.py
```

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/acl.py` & `chamco_ragbot-0.1.4/chamco_ragbot/acl.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/chat.py` & `chamco_ragbot-0.1.4/chamco_ragbot/chat.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/datasource.py` & `chamco_ragbot-0.1.4/chamco_ragbot/datasource.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/dept.py` & `chamco_ragbot-0.1.4/chamco_ragbot/dept.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/filetransfer.py` & `chamco_ragbot-0.1.4/chamco_ragbot/filetransfer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/index.py` & `chamco_ragbot-0.1.4/chamco_ragbot/index.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/indexer.py` & `chamco_ragbot-0.1.4/chamco_ragbot/indexer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/main.py` & `chamco_ragbot-0.1.4/chamco_ragbot/main.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/search.py` & `chamco_ragbot-0.1.4/chamco_ragbot/search.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/skillset.py` & `chamco_ragbot-0.1.4/chamco_ragbot/skillset.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.3/chamco_ragbot/utils.py` & `chamco_ragbot-0.1.4/chamco_ragbot/utils.py`

 * *Files identical despite different names*

