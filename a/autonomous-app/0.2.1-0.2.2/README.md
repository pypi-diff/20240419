# Comparing `tmp/autonomous_app-0.2.1.tar.gz` & `tmp/autonomous_app-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous_app-0.2.1.tar", last modified: Wed Apr 17 22:35:12 2024, max compression
+gzip compressed data, was "autonomous_app-0.2.2.tar", last modified: Thu Apr 18 20:46:26 2024, max compression
```

## Comparing `autonomous_app-0.2.1.tar` & `autonomous_app-0.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.714723 autonomous_app-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-17 22:34:51.000000 autonomous_app-0.2.1/src/autonomous/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.1/src/autonomous/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7979 2024-04-17 22:33:38.000000 autonomous_app-0.2.1/src/autonomous/ai/oaiagent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/auth/
--rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.1/src/autonomous/auth/autoauth.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/auth/github.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/auth/google.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.1/src/autonomous/auth/user.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/db/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.1/src/autonomous/db/autodb.py
--rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.1/src/autonomous/db/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/errors/
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/errors/danglingreferenceerror.py
--rw-r--r--   0 root         (0) root         (0)     1460 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/model/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.1/src/autonomous/model/autoattribute.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.1/src/autonomous/model/automodel.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.1/src/autonomous/model/orm.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.1/src/autonomous/model/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.718723 autonomous_app-0.2.1/src/autonomous/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.1/src/autonomous/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.1/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/localstorage.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.1/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/src/autonomous/storage/version_control/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/version_control/GHCallbacks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/version_control/GHOrganization.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/version_control/GHRepo.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/version_control/GHVersionControl.py
--rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/storage/version_control/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/src/autonomous/tasks/
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.1/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 22:35:12.722723 autonomous_app-0.2.1/src/autonomous_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-17 22:35:12.000000 autonomous_app-0.2.1/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1372 2024-04-17 22:35:12.000000 autonomous_app-0.2.1/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 22:35:12.000000 autonomous_app-0.2.1/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-17 22:35:12.000000 autonomous_app-0.2.1/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-17 22:35:12.000000 autonomous_app-0.2.1/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.965169 autonomous_app-0.2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-18 20:45:45.000000 autonomous_app-0.2.2/src/autonomous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.2/src/autonomous/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2024-04-18 20:45:36.000000 autonomous_app-0.2.2/src/autonomous/ai/oaiagent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/auth/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.2/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/auth/github.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/auth/google.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.2/src/autonomous/auth/user.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/db/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.2/src/autonomous/db/autodb.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2024-02-26 19:40:28.000000 autonomous_app-0.2.2/src/autonomous/db/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/errors/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/errors/danglingreferenceerror.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.2/src/autonomous/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/model/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.2/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 16:19:39.000000 autonomous_app-0.2.2/src/autonomous/model/automodel.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.2/src/autonomous/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.2/src/autonomous/model/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.969169 autonomous_app-0.2.2/src/autonomous/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.2/src/autonomous/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.2/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.2/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/src/autonomous/storage/version_control/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/version_control/GHCallbacks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/version_control/GHOrganization.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/version_control/GHRepo.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/version_control/GHVersionControl.py
+-rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/storage/version_control/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/src/autonomous/tasks/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.2/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 20:46:26.973169 autonomous_app-0.2.2/src/autonomous_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-18 20:46:26.000000 autonomous_app-0.2.2/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-18 20:46:26.000000 autonomous_app-0.2.2/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 20:46:26.000000 autonomous_app-0.2.2/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-18 20:46:26.000000 autonomous_app-0.2.2/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-18 20:46:26.000000 autonomous_app-0.2.2/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous_app-0.2.1/LICENSE` & `autonomous_app-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/PKG-INFO` & `autonomous_app-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.1
+Version: 0.2.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.1/README.md` & `autonomous_app-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/pyproject.toml` & `autonomous_app-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/requirements.txt` & `autonomous_app-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/ai/oaiagent.py` & `autonomous_app-0.2.2/src/autonomous/ai/oaiagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,19 @@
         return self._agent_id
 
     @agent_id.setter
     def agent_id(self, value):
         self._agent_id = value
 
     def clear_agent(self):
-        self.client.beta.assistants.delete(self._agent_id)
+        self.client.beta.assistants.delete(self.agent_id)
         self.agent_id = ""
 
     def get_agent(self):
-        return self.client.beta.assistants.retrieve(self._agent_id)
+        return self.client.beta.assistants.retrieve(self.agent_id)
 
     def clear_files(self, file_id=None):
         if self.vector_store:
             if not file_id:
                 vector_store_files = self.client.beta.vector_stores.files.list(
                     vector_store_id=self.vector_store
                 ).data
```

### Comparing `autonomous_app-0.2.1/src/autonomous/auth/autoauth.py` & `autonomous_app-0.2.2/src/autonomous/auth/autoauth.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/auth/github.py` & `autonomous_app-0.2.2/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/auth/google.py` & `autonomous_app-0.2.2/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/auth/user.py` & `autonomous_app-0.2.2/src/autonomous/auth/user.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/db/autodb.py` & `autonomous_app-0.2.2/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/db/table.py` & `autonomous_app-0.2.2/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/logger.py` & `autonomous_app-0.2.2/src/autonomous/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import inspect
 import logging
 import os
 
 # class LogFilter(logging.Filter):
 #     def filter(self, record):
 #         return record.levelno == LOG_LEVEL
@@ -23,14 +24,18 @@
     """
 
     def __init__(self):
         self.logger = logging.getLogger("gunicorn.error")
         level = os.environ.get("LOG_LEVEL") or self.logger.level
         self.logger.setLevel(log_levels.get(level, "DEBUG"))
         self.enabled = True
+        self.logfile = "logs/current_run_error_log.log"
+        self.logarchive = (
+            f"logs/error_log-{datetime.datetime.now().strftime('%Y-%m-%d')}.log"
+        )
 
     def set_level(self, level):
         self.logger.setLevel(log_levels[level])
 
     def enable(self, enable=True):
         self.enabled = enable
 
@@ -42,10 +47,14 @@
             msg += f"\n{'='*20}\n"
             if args:
                 msg += "\n---\n".join([f"{v}" for v in args])
             if kwargs:
                 msg += "\n---\n".join([f"{k} : {v}" for k, v in kwargs.items()])
             msg += f"\n{'='*20}\n"
             self.logger.log(self.logger.level, f"{msg}\n")
+            with open(self.logfile, "w") as current:
+                current.write(f"{msg}\n")
+            with open(self.logarchive, "a") as archive:
+                archive.write(f"{msg}\n")
 
 
 log = Logger()
```

### Comparing `autonomous_app-0.2.1/src/autonomous/model/autoattribute.py` & `autonomous_app-0.2.2/src/autonomous/model/autoattribute.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/model/automodel.py` & `autonomous_app-0.2.2/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/model/orm.py` & `autonomous_app-0.2.2/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/model/serializer.py` & `autonomous_app-0.2.2/src/autonomous/model/serializer.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/imagestorage.py` & `autonomous_app-0.2.2/src/autonomous/storage/imagestorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/localstorage.py` & `autonomous_app-0.2.2/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/markdown.py` & `autonomous_app-0.2.2/src/autonomous/storage/markdown.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/version_control/GHCallbacks.py` & `autonomous_app-0.2.2/src/autonomous/storage/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/version_control/GHOrganization.py` & `autonomous_app-0.2.2/src/autonomous/storage/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/storage/version_control/GHRepo.py` & `autonomous_app-0.2.2/src/autonomous/storage/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous/tasks/autotask.py` & `autonomous_app-0.2.2/src/autonomous/tasks/autotask.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.1/src/autonomous_app.egg-info/PKG-INFO` & `autonomous_app-0.2.2/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.1
+Version: 0.2.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.1/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous_app-0.2.2/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

