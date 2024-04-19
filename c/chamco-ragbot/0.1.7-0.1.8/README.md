# Comparing `tmp/chamco_ragbot-0.1.7.tar.gz` & `tmp/chamco_ragbot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamco_ragbot-0.1.7.tar", last modified: Fri Apr 19 04:45:41 2024, max compression
+gzip compressed data, was "chamco_ragbot-0.1.8.tar", last modified: Fri Apr 19 07:45:52 2024, max compression
```

## Comparing `chamco_ragbot-0.1.7.tar` & `chamco_ragbot-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:45:41.978831 chamco_ragbot-0.1.7/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:45:41.978831 chamco_ragbot-0.1.7/PKG-INFO
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:45:41.978831 chamco_ragbot-0.1.7/chamco_ragbot/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3008 2024-04-19 02:14:39.000000 chamco_ragbot-0.1.7/chamco_ragbot/acl.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.7/chamco_ragbot/datasource.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.7/chamco_ragbot/dept.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/filetransfer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.7/chamco_ragbot/index.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/indexer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7531 2024-04-19 03:49:52.000000 chamco_ragbot-0.1.7/chamco_ragbot/main.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/search.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.7/chamco_ragbot/skillset.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.7/chamco_ragbot/utils.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:45:41.978831 chamco_ragbot-0.1.7/chamco_ragbot.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:45:41.000000 chamco_ragbot-0.1.7/chamco_ragbot.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 04:45:41.000000 chamco_ragbot-0.1.7/chamco_ragbot.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 04:45:41.000000 chamco_ragbot-0.1.7/chamco_ragbot.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 04:45:41.000000 chamco_ragbot-0.1.7/chamco_ragbot.egg-info/top_level.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 04:45:41.978831 chamco_ragbot-0.1.7/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-19 04:45:40.000000 chamco_ragbot-0.1.7/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/PKG-INFO
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.081364 chamco_ragbot-0.1.8/chamco_ragbot/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3284 2024-04-19 06:34:49.000000 chamco_ragbot-0.1.8/chamco_ragbot/acl.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.8/chamco_ragbot/datasource.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.8/chamco_ragbot/dept.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/filetransfer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.8/chamco_ragbot/index.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/indexer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2320 2024-04-19 07:45:14.000000 chamco_ragbot-0.1.8/chamco_ragbot/main.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/search.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.8/chamco_ragbot/skillset.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.8/chamco_ragbot/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 07:45:52.081364 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 07:45:52.000000 chamco_ragbot-0.1.8/chamco_ragbot.egg-info/top_level.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 07:45:52.085364 chamco_ragbot-0.1.8/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-19 07:45:38.000000 chamco_ragbot-0.1.8/setup.py
```

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/acl.py` & `chamco_ragbot-0.1.8/chamco_ragbot/acl.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,41 @@
 )
 scopes = ['https://graph.microsoft.com/.default']
 
 # Create an API client with the credentials and scopes.
 client = GraphServiceClient(credentials=credential, scopes=scopes)
 
 
+from asgiref.sync import async_to_sync
 
-# dept_name = "GPTKB_HRTest"
+# # dept_name = "GPTKB_HRTest"
+# @async_to_sync
 async def get_departments_group_ids():
     groups = await client.groups.get()
     depts_dict = {group.display_name: group.id for group in groups.value}
     return depts_dict
 
-# def get_department_group_id(depts_dict, dept_name):
 
-#     return depts_dict[dept_name]
 
-# depts_dict = await get_departments_group_ids()
-# depts_dict = asyncio.run(get_departments_group_ids())
-# department_group_id = depts_dict[dept_name]
-# department_group_id
 
 
+# import asyncio
+
+
+# def get_departments_group_ids():
+#     loop = asyncio.get_event_loop()
+#     if loop.is_running():
+#         groups = loop.run_until_complete(client.groups.get())
+#     else:
+#         new_loop = asyncio.new_event_loop()
+#         asyncio.set_event_loop(new_loop)
+#         groups = new_loop.run_until_complete(client.groups.get())
+#         new_loop.close()
+#     depts_dict = {group.display_name: group.id for group in groups.value}
+#     return depts_dict
 
 
 
 
 storage_account_name = os.getenv('STORAGE_ACCOUNT_NAME', "datalakegen2chamco")
 storage_account_key = os.getenv('STORAGE_ACCOUNT_KEY', "19jjtOaErMgLfp3TMpzNpk0DTqhzV3TdlIt4Ya2I0mqpuf/drmEVAIEGSMxbtbneb9fglsPiaMLJ+AStvbU1nw==")
 # blob_container_name = os.getenv('BLOB_CONTAINER_NAME', "gptkbcontainer")
```

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/chat.py` & `chamco_ragbot-0.1.8/chamco_ragbot/chat.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/datasource.py` & `chamco_ragbot-0.1.8/chamco_ragbot/datasource.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/dept.py` & `chamco_ragbot-0.1.8/chamco_ragbot/dept.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/filetransfer.py` & `chamco_ragbot-0.1.8/chamco_ragbot/filetransfer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/index.py` & `chamco_ragbot-0.1.8/chamco_ragbot/index.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/indexer.py` & `chamco_ragbot-0.1.8/chamco_ragbot/indexer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/search.py` & `chamco_ragbot-0.1.8/chamco_ragbot/search.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/skillset.py` & `chamco_ragbot-0.1.8/chamco_ragbot/skillset.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.7/chamco_ragbot/utils.py` & `chamco_ragbot-0.1.8/chamco_ragbot/utils.py`

 * *Files identical despite different names*

