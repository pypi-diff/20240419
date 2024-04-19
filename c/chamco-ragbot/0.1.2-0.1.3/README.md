# Comparing `tmp/chamco_ragbot-0.1.2.tar.gz` & `tmp/chamco_ragbot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chamco_ragbot-0.1.2.tar", last modified: Sun Apr 14 18:14:55 2024, max compression
+gzip compressed data, was "chamco_ragbot-0.1.3.tar", last modified: Fri Apr 19 04:06:59 2024, max compression
```

## Comparing `chamco_ragbot-0.1.2.tar` & `chamco_ragbot-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 18:14:55.272222 chamco_ragbot-0.1.2/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 18:14:55.272222 chamco_ragbot-0.1.2/PKG-INFO
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 18:14:55.272222 chamco_ragbot-0.1.2/chamco_ragbot/
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-11 21:28:21.000000 chamco_ragbot-0.1.2/chamco_ragbot/__init__.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-13 11:53:51.000000 chamco_ragbot-0.1.2/chamco_ragbot/chat.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1873 2024-04-14 18:04:40.000000 chamco_ragbot-0.1.2/chamco_ragbot/datasource.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-14 18:01:15.000000 chamco_ragbot-0.1.2/chamco_ragbot/filetransfer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6205 2024-04-14 18:03:27.000000 chamco_ragbot-0.1.2/chamco_ragbot/index.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-14 18:06:01.000000 chamco_ragbot-0.1.2/chamco_ragbot/indexer.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1637 2024-04-14 18:06:53.000000 chamco_ragbot-0.1.2/chamco_ragbot/main.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-13 12:22:44.000000 chamco_ragbot-0.1.2/chamco_ragbot/search.py
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-14 18:05:29.000000 chamco_ragbot-0.1.2/chamco_ragbot/skillset.py
-drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-14 18:14:55.272222 chamco_ragbot-0.1.2/chamco_ragbot.egg-info/
--rw-r--r--   0 azureuser  (1000) azureuser  (1000)      127 2024-04-14 18:14:55.000000 chamco_ragbot-0.1.2/chamco_ragbot.egg-info/PKG-INFO
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      382 2024-04-14 18:14:55.000000 chamco_ragbot-0.1.2/chamco_ragbot.egg-info/SOURCES.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-14 18:14:55.000000 chamco_ragbot-0.1.2/chamco_ragbot.egg-info/dependency_links.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-14 18:14:55.000000 chamco_ragbot-0.1.2/chamco_ragbot.egg-info/top_level.txt
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-14 18:14:55.272222 chamco_ragbot-0.1.2/setup.cfg
--rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      287 2024-04-14 18:14:45.000000 chamco_ragbot-0.1.2/setup.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/PKG-INFO
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/chamco_ragbot/
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        0 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/__init__.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3008 2024-04-19 02:14:39.000000 chamco_ragbot-0.1.3/chamco_ragbot/acl.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2075 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/chat.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1933 2024-04-19 03:12:20.000000 chamco_ragbot-0.1.3/chamco_ragbot/datasource.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     1739 2024-04-19 03:45:28.000000 chamco_ragbot-0.1.3/chamco_ragbot/dept.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2117 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/filetransfer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     6212 2024-04-19 03:26:57.000000 chamco_ragbot-0.1.3/chamco_ragbot/index.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     2477 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/indexer.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     7531 2024-04-19 03:49:52.000000 chamco_ragbot-0.1.3/chamco_ragbot/main.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     4195 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/search.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)     3663 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/chamco_ragbot/skillset.py
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      892 2024-04-19 03:28:31.000000 chamco_ragbot-0.1.3/chamco_ragbot/utils.py
+drwxrwxr-x   0 azureuser  (1000) azureuser  (1000)        0 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/
+-rw-r--r--   0 azureuser  (1000) azureuser  (1000)      108 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/PKG-INFO
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      448 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)        1 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       14 2024-04-19 04:06:59.000000 chamco_ragbot-0.1.3/chamco_ragbot.egg-info/top_level.txt
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)       38 2024-04-19 04:06:59.190686 chamco_ragbot-0.1.3/setup.cfg
+-rw-rw-r--   0 azureuser  (1000) azureuser  (1000)      268 2024-04-18 14:27:21.000000 chamco_ragbot-0.1.3/setup.py
```

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/chat.py` & `chamco_ragbot-0.1.3/chamco_ragbot/chat.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/datasource.py` & `chamco_ragbot-0.1.3/chamco_ragbot/datasource.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 AZURE_SEARCH_SERVICE_ENDPOINT = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
 AZURE_SEARCH_ADMIN_KEY = os.getenv("AZURE_SEARCH_ADMIN_KEY")
 
 credential = AzureKeyCredential(AZURE_SEARCH_ADMIN_KEY) if len(AZURE_SEARCH_ADMIN_KEY) > 0 else DefaultAzureCredential()
 
 
 def create_datasource(blob_folder_name, index_name, blob_container_name=BLOB_CONTAINER_NAME, blob_connection_string=BLOB_CONNECTION_STRING):
+    
+    logging.info(f"[Ok] index_name name {index_name}")
 
     # Create a data source
     indexer_client = SearchIndexerClient(AZURE_SEARCH_SERVICE_ENDPOINT, credential)
     # container = SearchIndexerDataContainer(name=blob_container_name)
     container = SearchIndexerDataContainer(name=blob_container_name, query=blob_folder_name)
     data_source_connection = SearchIndexerDataSourceConnection(
         name=f"{index_name}-datasource",
```

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/filetransfer.py` & `chamco_ragbot-0.1.3/chamco_ragbot/filetransfer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/index.py` & `chamco_ragbot-0.1.3/chamco_ragbot/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,27 +74,27 @@
     SearchField(name="chunk_id", type=SearchFieldDataType.String, key=True, sortable=True, filterable=True, facetable=True, analyzer_name="keyword"),
     SearchField(name="chunk", type=SearchFieldDataType.String, sortable=False, filterable=False, facetable=False),
     SearchField(name="vector", type=SearchFieldDataType.Collection(SearchFieldDataType.Single), vector_search_dimensions=1536, vector_search_profile_name="myHnswProfile"),
 ]
 
 
 
-def create_index(file_url):
+def create_index(index_name):
 
     # # Create a search index
     # index_client = SearchIndexClient(endpoint=endpoint, credential=credential)
     # fields = [
     #     SearchField(name="parent_id", type=SearchFieldDataType.String, sortable=True, filterable=True, facetable=True),
     #     SearchField(name="title", type=SearchFieldDataType.String),
     #     SearchField(name="chunk_id", type=SearchFieldDataType.String, key=True, sortable=True, filterable=True, facetable=True, analyzer_name="keyword"),
     #     SearchField(name="chunk", type=SearchFieldDataType.String, sortable=False, filterable=False, facetable=False),
     #     SearchField(name="vector", type=SearchFieldDataType.Collection(SearchFieldDataType.Single), vector_search_dimensions=1536, vector_search_profile_name="myHnswProfile"),
     # ]
 
-    index_name = file_url.split('/')[-2].lower()
+    # index_name = file_url.split('/')[-2].lower()
 
     # Configure the vector search configuration
     vector_search = VectorSearch(
         algorithms=[
             HnswAlgorithmConfiguration(
                 name="myHnsw",
                 parameters=HnswParameters(
@@ -144,13 +144,15 @@
     )
 
     # Create the semantic search with the configuration
     semantic_search = SemanticSearch(configurations=[semantic_config])
 
     # Create the search index
     index = SearchIndex(name=index_name, fields=FIELDS, vector_search=vector_search, semantic_search=semantic_search)
-    logging.info(f"[Ok] {index.name} created")
+    logging.info(f"[Ok] {index_name} created")
 
     result = index_client.create_or_update_index(index)
     logging.info(f"[Ok] index client created or updated")
 
-    return result
+    return result
+
+
```

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/indexer.py` & `chamco_ragbot-0.1.3/chamco_ragbot/indexer.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/search.py` & `chamco_ragbot-0.1.3/chamco_ragbot/search.py`

 * *Files identical despite different names*

### Comparing `chamco_ragbot-0.1.2/chamco_ragbot/skillset.py` & `chamco_ragbot-0.1.3/chamco_ragbot/skillset.py`

 * *Files identical despite different names*

