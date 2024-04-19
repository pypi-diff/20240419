# Comparing `tmp/opengate-data-1.0.4.tar.gz` & `tmp/opengate_data-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opengate-data-1.0.4.tar", last modified: Fri Feb 16 11:54:56 2024, max compression
+gzip compressed data, was "opengate_data-1.0.5.tar", last modified: Fri Apr 19 11:36:56 2024, max compression
```

## Comparing `opengate-data-1.0.4.tar` & `opengate_data-1.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      790 2024-02-16 11:54:56.000000 opengate-data-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)      790 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       75 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1143 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-16 11:54:56.000000 opengate-data-1.0.4/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      549 2024-02-16 11:50:46.000000 opengate-data-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/provision_processor/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/provision_processor/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6025 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/provision_processor/provision_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/rules/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/rules/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18233 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/rules/rules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/test/
--rw-rw-r--   0 root         (0) root         (0)    12885 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/test/test_steps_cucumber.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      525 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/test/ownworld.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/ai_pipelines/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_pipelines/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14795 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_pipelines/ai_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/datapoints/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/datapoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4506 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/datapoints/datapoints.py
--rw-rw-r--   0 root         (0) root         (0)     4158 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/opengate_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/timeseries/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/timeseries/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3360 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/timeseries/timeseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/ai_transformers/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_transformers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16353 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_transformers/ai_transformers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/entities/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/entities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7420 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/entities/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/ai_models/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15395 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/ai_models/ai_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/operations/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/operations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2732 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/operations/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 11:54:56.000000 opengate-data-1.0.4/opengate_data/datasets/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/datasets/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3407 2024-02-16 11:50:46.000000 opengate-data-1.0.4/opengate_data/datasets/datasets.py
--rw-rw-r--   0 root         (0) root         (0)      773 2024-02-16 11:50:46.000000 opengate-data-1.0.4/setup.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      974 2024-04-19 11:36:56.820613 opengate_data-1.0.5/PKG-INFO
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      549 2024-04-15 07:45:27.000000 opengate_data-1.0.5/README.md
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.812613 opengate_data-1.0.5/opengate_data/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      249 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/__init__.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_models/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_models/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    15395 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_models/ai_models.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_pipelines/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_pipelines/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    14795 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_pipelines/ai_pipelines.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/ai_transformers/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/ai_transformers/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    16353 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/ai_transformers/ai_transformers.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/datapoints/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/datapoints/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     4492 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/datapoints/datapoints.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/datasets/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/datasets/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3393 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/datasets/datasets.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.816613 opengate_data-1.0.5/opengate_data/entities/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/entities/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     6978 2024-04-19 10:51:35.000000 opengate_data-1.0.5/opengate_data/entities/entities.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     4027 2024-04-19 10:57:54.000000 opengate_data-1.0.5/opengate_data/opengate_client.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/operations/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/operations/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3085 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/operations/operations.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/provision_processor/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 13:58:53.000000 opengate_data-1.0.5/opengate_data/provision_processor/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     6205 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/provision_processor/provision_processor.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/rules/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/rules/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    18199 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/rules/rules.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/test/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/test/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      525 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/test/ownworld.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)    12881 2024-04-19 08:44:45.000000 opengate_data-1.0.5/opengate_data/test/test_steps_cucumber.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data/timeseries/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        0 2024-04-15 07:45:27.000000 opengate_data-1.0.5/opengate_data/timeseries/__init__.py
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     3342 2024-04-19 08:44:12.000000 opengate_data-1.0.5/opengate_data/timeseries/timeseries.py
+drwxr-xr-x   0 manuel    (1000) manuel    (1000)        0 2024-04-19 11:36:56.820613 opengate_data-1.0.5/opengate_data.egg-info/
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      974 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/PKG-INFO
+-rw-r--r--   0 manuel    (1000) manuel    (1000)     1143 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)        1 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       88 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/requires.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       14 2024-04-19 11:36:56.000000 opengate_data-1.0.5/opengate_data.egg-info/top_level.txt
+-rw-r--r--   0 manuel    (1000) manuel    (1000)       38 2024-04-19 11:36:56.820613 opengate_data-1.0.5/setup.cfg
+-rw-r--r--   0 manuel    (1000) manuel    (1000)      793 2024-04-19 10:28:57.000000 opengate_data-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opengate-data-1.0.4/opengate_data.egg-info/SOURCES.txt` & `opengate_data-1.0.5/opengate_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/README.md` & `opengate_data-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/opengate_data/provision_processor/provision_processor.py` & `opengate_data-1.0.5/opengate_data/provision_processor/provision_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,50 +54,54 @@
         ''' bulk_provision_processor '''
         self.requires = {
             'organization_name': self.organization_name,
             'provision_processor_id': self.provision_processor_id,
             'bulk_file': self.bulk_file
         }
         self.method = 'bulk_provision_processor'
+        self.headers['Accept'] = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/{self.provision_processor_id}/bulk'
         return self
     
         
     def search_by_name(self) -> 'ProvisionProcessorBuilder':
         ''' search_provision_processor '''
         self.requires = {
             'organization_name': self.organization_name,
             'provision_processor_name': self.provision_processor_name,
             
         }
         self.method = 'search_provision_processor'
+        self.headers['Accept'] = 'application/json'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}'
         return self
     
         
     def bulk_status(self) -> 'ProvisionProcessorBuilder':
         ''' bulk_status '''
         self.requires = {
             'organization_name': self.organization_name,
             'bulk_process_id': self.bulk_process_id,
             
         }
         self.method = 'bulk_status'
+        self.headers['Accept'] = 'application/json'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/bulk/{self.bulk_process_id}'
         return self
     
         
     def bulk_details(self) -> 'ProvisionProcessorBuilder':
         ''' bulk_details '''
         self.requires = {
             'organization_name': self.organization_name,
             'bulk_process_id': self.bulk_process_id,
             
         }
         self.method = 'bulk_details'
+        self.headers['Accept'] = 'application/vnd.openxmlformats-officedocument.spreadsheetml.sheet'
         self.url = f'{self.client.url}/north/v80/provisionProcessors/provision/organizations/{self.organization_name}/bulk/{self.bulk_process_id}/details'
         return self
     
     def build(self) -> 'ProvisionProcessorBuilder':
         ''' Check if any parameter is missing. '''
         if self.requires is not None:
             for key, value in self.requires.items():
@@ -113,19 +117,14 @@
             'bulk_status': self._execute_bulk_status,
             'bulk_details': self._execute_bulk_details,
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
-    
-      
-    def add_header(self, key: str, value: str) -> 'ProvisionProcessorBuilder':
-        self.headers[key] = value
-
 
     def _execute_bulk(self) -> Union[int, List[Dict[str, Any]]]:
         return requests.post(self.url, headers=self.headers, files=self.bulk_file, verify=False, timeout=3000)
 
 
     def _execute_searching(self) -> Union[int, List[Dict[str, Any]]]:
         request_response = requests.get(self.url, headers=self.headers, verify=False, timeout=3000)
```

### Comparing `opengate-data-1.0.4/opengate_data/rules/rules.py` & `opengate_data-1.0.5/opengate_data/rules/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class RulesBuilder:
     ''' Class rules builder'''
     def __init__(self, opengate_client):
         self.client = opengate_client
         self.rule_data: Dict[str, Any] = {}
         self.method: str = None
         self.url: str = None
-        self.filter_data: Dict[str, Any] = None
+        self.body_data: Dict[str, Any] = None
         self.requires: Dict[str, Any] = {}
         self.config_file: str = None
         self.section: str = None
         self.config_key: str = None
         self.find_name: str = None
         self.data_env: str = None
     
@@ -111,17 +111,17 @@
         return self
 
     def with_env(self, data_env: str) -> 'RulesBuilder':
         ''' env '''
         self.data_env = data_env
         return self
 
-    def with_filter(self, filter_data: Dict[str, Any]) -> 'RulesBuilder':
-        '''filter'''
-        self.filter_data = filter_data
+    def with_body(self, body_data: Dict[str, Any]) -> 'RulesBuilder':
+        '''body'''
+        self.body_data = body_data
         return self
     
     def with_config_file(self,config_file: str, section: str, config_key: str) -> 'RulesBuilder':
         ''' config file. '''
         self.config_file = config_file
         self.section = section
         self.config_key = config_key
@@ -144,17 +144,17 @@
         self.url = f'{self.client.url}/north/v80/rules/provision/organizations/{self.rule_data["organization"]}/channels/{self.rule_data["channel"]}'
         self.method = 'create'
         return self
 
     def search(self) -> 'RulesBuilder':
         ''' search '''
         self.requires = {
-            'filter': self.filter_data,
+            'filter': self.body_data,
         }
-        self.requires['filter'] = self.filter_data
+        self.requires['filter'] = self.body_data
         self.url = f'{self.client.url}/north/v80/rules/search'
         self.method = 'search'
         return self
     
     def find_one(self) -> 'RulesBuilder':
         '''Find one '''
         identifier = self._get_identifier()
@@ -298,19 +298,19 @@
         if self.config_file is not None and self.section is not None and self.config_key is not None :
             try:
                 return self._read_config_file().get(self.section, self.config_key)
             except configparser.NoOptionError as error:
                 raise ValueError('The "rule_id" parameter was not found in the configuration file.') from error
 
         if self.find_name is not None:
-            filter_data = {
+            body_data = {
                 "filter": {"and": [{"eq": {"rule.organization": self.rule_data['organization']}}]},
                 "limit": {"size": 1000, "start": 1}
             }
-            all_identifiers = self.with_filter(filter_data).search().build().execute().json()
+            all_identifiers = self.with_body(body_data).search().build().execute().json()
             if isinstance(all_identifiers, dict) and 'rules' in all_identifiers:
                 identifier_list = all_identifiers['rules']
             else:
                 raise ValueError('Unexpected response format from the server.')
 
             name_identifier = [
                 item['identifier'] for item in identifier_list if item.get('name') == self.find_name
@@ -359,32 +359,32 @@
                         raise ValueError('The environment variable was not found in the .env file.') from error
         return response
     
     def _get_created_rule_identifier(self):
         name = self.rule_data.get('name')
         if not name:
             raise ValueError('The "name" attribute is missing or empty.')
-        filter_data = {
+        body_data = {
             "filter": {"and": [{"eq": {"rule.organization": self.rule_data['organization']}}]},
             "limit": {"size": 1000, "start": 1}
         }
-        all_identifiers = self.with_filter(filter_data).search().build().execute().json()
+        all_identifiers = self.with_body(body_data).search().build().execute().json()
         if 'rules' in all_identifiers:
             for rule in all_identifiers['rules']:
                 if 'name' in rule and rule['name'] == name:
                     return rule['identifier']
 
         raise ValueError(f'No rule with the name "{name}" was found.')
 
     def _execute_search(self) -> List[Dict[str, Any]]:
-        response = requests.post(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.post(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         return response
     
     def _execute_find_one(self) -> List[Dict[str, Any]]:
-        response = requests.get(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.get(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         return response
     
     def _execute_update(self) -> int:
         response = requests.put(self.url, headers=self.client.headers, json=self.rule_data, verify=False,timeout=3000)
         return response
         
     def _execute_delete(self) -> int:
@@ -392,15 +392,15 @@
         return response
     
     def _execute_update_parameters(self) -> int:
         response = requests.put(self.url, headers=self.client.headers, json=self.rule_data['parameters'], verify=False, timeout=3000)
         return response
     
     def _execute_catalog(self) -> List[Dict[str, Any]]:
-        response = requests.get(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.get(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         return response
     
     def _execute_save(self):
         if self.data_env is not None or self.config_file is not None:
             if self.data_env is not None:
                 identifier = dotenv_values('.env')[self.data_env]
                 self.identifier = identifier
```

### Comparing `opengate-data-1.0.4/opengate_data/test/test_steps_cucumber.py` & `opengate_data-1.0.5/opengate_data/test/test_steps_cucumber.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 
 @given(parsers.parse('I want to use a name "{name}"'))
 def step_with_name(name):
     ''' with name '''
     ai_builder_instance.with_name(name)
 
 @given(parsers.parse('I want to use a filter "{filter_data}"'))
-def step_with_filter(filter_data):
+def step_with_body(filter_data):
     ''' filter '''
-    ai_builder_instance.with_filter(ast.literal_eval(filter_data))
+    ai_builder_instance.with_body(ast.literal_eval(filter_data))
 
 @given(parsers.parse('I want to use a channel "{channel}"'))
 def step_with_channel(channel):
     ''' channel '''
     ai_builder_instance.with_channel(get_value_from_path(testing_data, channel))
 
 @given(parsers.parse('I want to use a active "{active_rule}"'))
```

### Comparing `opengate-data-1.0.4/opengate_data/test/ownworld.py` & `opengate_data-1.0.5/opengate_data/test/ownworld.py`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/opengate_data/ai_pipelines/ai_pipelines.py` & `opengate_data-1.0.5/opengate_data/ai_pipelines/ai_pipelines.py`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/opengate_data/datapoints/datapoints.py` & `opengate_data-1.0.5/opengate_data/datapoints/datapoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 import urllib3
 from typing import Callable, Union, List, Dict, Any
 
 class DataPointsBuilder:
     ''' Builder datapoints '''
     def __init__(self, opengate_client):
         self.client = opengate_client
-        self.filter_data: Dict[str, Any] = {}
+        self.body_data: Dict[str, Any] = {}
         self.transpose: bool = False
         self.mapping: Union[None, Dict[str, Dict[str, str]]] = None
         self.is_built: bool = False
         self.url: Union[None, str] = None
         self.method: Union[None, str] = None
         self.requires: Dict[str, Any] = {}
 
-    def with_filter(self, filter_data: Dict[str, Any]) -> 'DataPointsBuilder':
-        ''' filter '''
-        self.filter_data = filter_data
+    def with_body(self, body_data: Dict[str, Any]) -> 'DataPointsBuilder':
+        ''' body '''
+        self.body_data = body_data
         return self
 
     def with_transpose(self) -> 'DataPointsBuilder':
         ''' transpose '''
         if self.mapping is not None:
             raise ValueError('Cannot use with_transpose and with_mapped_transpose together')
         self.transpose = True
@@ -80,15 +80,15 @@
         data = data.pivot_table(index=['at', 'entity'], columns='datastream', fill_value=np.nan, aggfunc='first')
         data = data.sort_values(by='at')
         data = data['value']
         data = data.reset_index()
         return data
     
     def _execute_searching(self) -> Union[str, List[Dict[str, Any]], pd.DataFrame]:
-        response = requests.post(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.post(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         if response.status_code == 200:
             data_str = StringIO(response.content.decode('utf-8'))
             data = pd.read_csv(data_str, sep=';')
 
             if self.transpose:
                 data = self._transpose_data(data)
             print("self.mapping", self.mapping)
```

### Comparing `opengate-data-1.0.4/opengate_data/opengate_client.py` & `opengate_data-1.0.5/opengate_data/opengate_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 ''' Class representing the OpenGateClient '''
 
 from typing import Dict, Optional
 import requests
-import pandas as pd
 from .datapoints.datapoints import DataPointsBuilder
 from .datasets.datasets import DataSetsBuilder
 from .timeseries.timeseries import TimeSeriesBuilder
 from .entities.entities import EntitiesBuilder
 from .provision_processor.provision_processor import ProvisionProcessorBuilder
 from .operations.operations import OperationsBuilder
 from .ai_models.ai_models import AIModelsBuilder
@@ -91,9 +90,7 @@
     def ai_transformers_builder(self) -> AITransformersBuilder:
         ''' Represents the builder of artificial intelligence models '''
         return AITransformersBuilder(self)
     
     def rules_builder(self) -> RulesBuilder:
         ''' Represents the builder of artificial intelligence models '''
         return RulesBuilder(self)
-    
-client = OpenGateClient(url='https://172.19.18.132:9082', api_key="bdef865c-bad0-4587-917f-6b7de8cf7d59")
```

### Comparing `opengate-data-1.0.4/opengate_data/timeseries/timeseries.py` & `opengate_data-1.0.5/opengate_data/timeseries/timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class TimeSeriesBuilder:
     ''' Timeserie Builder '''
     def __init__(self, opengate_client):
         self.client = opengate_client
         self.organization_name: str = None
         self.identifier: str = None
-        self.filter_data: Dict[str, Any] = {}
+        self.body_data: Dict[str, Any] = {}
         self.format_data: str = None
         self.url: str = None
         self.method: str = None
         self.requires: Dict[str, Any] = {}
     
     def with_organization(self, organization_name: str) -> 'TimeSeriesBuilder':
         ''' Organizartion '''
@@ -20,31 +20,31 @@
         return self
 
     def with_identifier(self, identifier: str) -> 'TimeSeriesBuilder':
         ''' Identifier '''
         self.identifier = identifier
         return self
 
-    def with_filter(self, filter_data: Dict[str, Any]) -> 'TimeSeriesBuilder':
-        ''' Filter'''
-        self.filter_data = filter_data
+    def with_body(self, body_data: Dict[str, Any]) -> 'TimeSeriesBuilder':
+        ''' Body'''
+        self.body_data = body_data
         return self
 
     def with_format(self, format_data: str) -> 'TimeSeriesBuilder':
         ''' Format '''
         self.format_data = format_data
         return self
 
     def search(self) -> 'TimeSeriesBuilder':
         ''' search'''
         self.requires = {
             'identifier': self.identifier,
             'format': self.format_data,
             'organization': self.organization_name,
-            'filter': self.filter_data
+            'body': self.body_data
         }
         self.method = 'search'
         self.url = f'{self.client.url}/north/v80/timeseries/provision/organizations/{self.organization_name}/{self.identifier}/data'
         return self
 
     def build(self) -> 'TimeSeriesBuilder':
         ''' Builder and check if any parameter is missing. '''
@@ -60,15 +60,15 @@
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
 
     def _execute_searching(self) -> Union[str, List[Dict[str, Any]], pd.DataFrame]:
-        response = requests.post(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.post(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         if response.status_code == 200:
             data = response.json()
             if self.format_data == 'csv':
                 csv = ','.join(data['columns']) + '\n'
                 for fila in data['data']:
                     csv += ','.join(map(str, fila)) + '\n'
                 return csv
```

### Comparing `opengate-data-1.0.4/opengate_data/ai_transformers/ai_transformers.py` & `opengate_data-1.0.5/opengate_data/ai_transformers/ai_transformers.py`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/opengate_data/entities/entities.py` & `opengate_data-1.0.5/opengate_data/entities/entities.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,161 +1,161 @@
 '''  EntitiesBuilder '''
 
 import requests
 import pandas as pd
 from typing import Callable, Union, List, Dict, Any
+from flatten_dict import flatten
 
 
 class EntitiesBuilder:
     ''' Builder entities'''
     def __init__(self, opengate_client):
         self.client = opengate_client
-        self.filter_data: Dict[str, Any] = {}
-        self.format_data: str = None
+        self.filter: Dict[str, Any] = {}
+        self.format_data: str | None = None
+        self.flatten: bool = False
+        self.utc: bool = False
+        self.summary: bool = False
         self.default_sorted: bool = False
         self.case_sensitive: bool = False
-        self.organization_name: str = None
-        self.bulk_action: str = None
-        self.bulk_type: str = None
-        self.csv_data: str = None
-        self.url: str = None
-        self.method: str = None
+        self.organization_name: str | None = None
+        self.bulk_action: str | None = None
+        self.bulk_type: str | None = None
+        self.csv_data: str | None = None
+        self.url: str | None = None
+        self.method: str | None = None
         self.requires: Dict[str, Any] = {}
-        self.select_data: Dict[str, Any] = {}
         self.headers: Dict[str, Any] = self.client.headers
 
     def with_filter(self, filter_data: Dict[str, Any]) -> 'EntitiesBuilder':
-        ''' Filter '''
-        self.filter_data = filter_data
+        ''' Body '''
+        self.filter = filter_data
         return self
-      
-    def with_select(self, select_data: Dict[str, Any]) -> 'EntitiesBuilder':
-        ''' Select '''
-        self.select_data = select_data
+
+    def with_body(self, filter_data: Dict[str, Any]) -> 'EntitiesBuilder':
+        ''' Body '''
+        self.filter = filter_data
         return self
 
     def with_format(self, format_data: str) -> 'EntitiesBuilder':
         ''' Formats the flat entities data based on the specified format ('csv', 'dict', or 'pandas'). '''
         self.format_data = format_data
+        if self.format_data == 'csv':
+            self.headers['Accept'] = 'text/plain'
+        else:
+            self.headers['Accept'] = 'application/json'
+        return self
+
+    def with_flattened(self):
+        self.flatten = True
         return self
 
-    def with_default_sorted(self, default_sorted: bool) -> 'EntitiesBuilder':
-        ''' default sorted'''
-        self.default_sorted = default_sorted
+    def with_utc(self):
+        self.utc = True
         return self
-    
-    def with_case_sensitive(self, case_sensitive: bool) -> 'EntitiesBuilder':
+
+    def with_summary(self):
+        self.summary = True
+        return self
+
+    def with_default_sorted(self) -> 'EntitiesBuilder':
+        """ default sorted"""
+        self.default_sorted = True
+        return self
+
+    def with_case_sensitive(self) -> 'EntitiesBuilder':
         ''' case sensitive'''
-        self.case_sensitive = case_sensitive
+        self.case_sensitive = True
         return self
 
     def search(self) -> 'EntitiesBuilder':
         ''' searching '''
         self.requires = {
-            'default sorted': self.default_sorted,
-            'filter_data': self.filter_data,
-            'select_data': self.select_data
+            'default sorted': self.default_sorted
         }
         self.method = 'search'
-        self.url = f'{self.client.url}/north/v80/search/entities?defaultSorted={self.default_sorted}'
+        if self.format_data == "pandas":
+            self.flatten = False
+
+        self.url = f'{self.client.url}/north/v80/search/entities?flattened={self.flatten}&utc={self.utc}&summary={self.summary}&defaultSorted={self.default_sorted}&caseSensitive={self.case_sensitive}'
+        print("url", self.url)
         return self
-    
+
     def with_organization_name(self, organization_name: str) -> 'EntitiesBuilder':
         ''' organization_name '''
         self.organization_name = organization_name
         return self
-    
+
     def with_bulk_action(self, bulk_action: str) -> 'EntitiesBuilder':
         ''' bulk_action '''
         self.bulk_action = bulk_action
         return self
-    
+
     def with_bulk_type(self, bulk_type: str) -> 'EntitiesBuilder':
         ''' bulk_type '''
         self.bulk_type = bulk_type
         return self
-    
+
     def with_csv_data(self, csv_data: str) -> 'EntitiesBuilder':
         ''' csv_data '''
         self.csv_data = csv_data
         return self
-    
+
     def bulk_provisioning(self) -> 'EntitiesBuilder':
         ''' bulk provisioning '''
         self.requires = {
             'organization_name': self.organization_name,
             'action': self.bulk_action,
             'type': self.bulk_type,
             'data': self.csv_data
         }
         self.method = 'bulk_provisioning'
         self.url = f'{self.client.url}/north/v80/provision/organizations/{self.organization_name}/bulk/async?action={self.bulk_action}&type={self.bulk_type}'
         return self
 
     def build(self) -> 'EntitiesBuilder':
-        ''' Check if any parameter is missing. '''
+        """ Check if any parameter is missing. """
         if self.requires is not None:
             for key, value in self.requires.items():
                 assert value is not None, f'{key} is required'
         return self
 
     def execute(self) -> Union[int, List[Dict[str, Any]]]:
-        ''' Execute and return the responses '''
+        """ Execute and return the responses """
         methods: Dict[str, Callable[[], Union[int, List[Dict[str, Any]]]]] = {
             'search': self._execute_searching,
             'bulk_provisioning': self._execute_bulk_provisioning
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
-      
-    def add_header(self, key: str, value: str) -> 'EntitiesBuilder':
-        self.headers[key] = value
 
     def _execute_searching(self) -> Union[int, List[Dict[str, Any]]]:
         response = self._send_request()
         if response.status_code == 200:
-          if self.format_data is 'csv':
-            return response.text
-          else:
-            data = response.json()
-            flat_entities = self._flatten_entities(data['entities'])
-            return self._format_data(flat_entities)
+            if self.format_data == 'csv':
+                return response.text
+            else:
+                data = response.json()
+                return self._format_data(data)
+
+        else:
+            error_message = response.json().get('message', 'Unknown error')
+            error_code = response.status_code
+            raise Exception(f"Error: Request failed with status code {error_code}. Message: {error_message}")
         return response
 
     def _execute_bulk_provisioning(self) -> Union[int, List[Dict[str, Any]]]:
         print(self.csv_data)
         response = requests.post(self.url, headers=self.headers, data=self.csv_data, verify=False, timeout=3000)
         return response
 
     def _send_request(self) -> requests.Response:
-        body = {}
-        
-        if(self.filter_data is not None):
-          body['filter'] = self.filter_data
-          
-        if(self.select_data is not None):
-          body['select'] = self.select_data
-          
-        return requests.post(self.url, headers=self.headers, json=body, verify=False, timeout=3000)
-
-    def _flatten_entities(self, entities: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
-        flat_entities = []
-        for entity in entities:
-            flat_entity = self._flatten_entity(entity)
-            flat_entities.append(flat_entity)
-        return flat_entities
-
-    def _flatten_entity(self, entity: Dict[str, Any]) -> Dict[str, Any]:
-        flat_entity = {}
-        for entity_key, entity_value in entity.items():
-            for key_level_1, value_level_1 in entity_value.items():
-                self._process_entity(entity_key, key_level_1, value_level_1, flat_entity)
-        return flat_entity
+        return requests.post(self.url, headers=self.headers, json=self.filter, verify=False, timeout=3000)
 
     def _process_entity(self, entity_prefix: str, key_prefix: str, value_dict: Any, flat_entity: Dict[str, Any]) -> None:
         if isinstance(value_dict, list):
             for i, item in enumerate(value_dict):
                 for sub_key, sub_value in item.items():
                     new_key = f'{entity_prefix}_{key_prefix}_{i}_{sub_key}'
                     self._assign_value(new_key, sub_value, flat_entity)
@@ -166,24 +166,18 @@
 
     def _assign_value(self, key: str, value: Any, flat_entity: Dict[str, Any]) -> None:
         if isinstance(value, dict) and '_current' in value:
             flat_entity[key] = value['_current']['value']
         else:
             flat_entity[key] = value
 
-    def _format_data(self, flat_entities: List[Dict[str, Any]]) -> Union[str, List[Dict[str, Any]], pd.DataFrame]:
-        if self.format_data == 'csv':
-            return self._format_as_csv(flat_entities)
-        elif self.format_data == 'dict':
-            return flat_entities
+    def _format_data(self, data: List[Dict[str, Any]]) -> Union[str, List[Dict[str, Any]], pd.DataFrame]:
+        if self.format_data == 'dict':
+            return data
         elif self.format_data == 'pandas':
-            return pd.DataFrame(flat_entities)
+            entities_flattened = []
+            for entity in data['entities']:
+                entities_flattened.append(flatten(entity, reducer='underscore', enumerate_types=(list,)))
+            pd.set_option('display.max_columns', 200)
+            return pd.DataFrame(entities_flattened)
         else:
             raise ValueError('Format not valid')
-
-    def _format_as_csv(self, flat_entities: List[Dict[str, Any]]) -> str:
-        columnas = flat_entities[0].keys()
-        csv_string = ','.join(columnas) + '\n'
-        for flat_entity in flat_entities:
-            fila = list(flat_entity.values())
-            csv_string += ','.join(map(str, fila)) + '\n'
-        return csv_string
```

### Comparing `opengate-data-1.0.4/opengate_data/ai_models/ai_models.py` & `opengate_data-1.0.5/opengate_data/ai_models/ai_models.py`

 * *Files identical despite different names*

### Comparing `opengate-data-1.0.4/opengate_data/operations/operations.py` & `opengate_data-1.0.5/opengate_data/operations/operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,52 @@
 
 class OperationsBuilder:
     ''' Builder operations'''
     def __init__(self, opengate_client):
         self.client = opengate_client
         self.default_sorted: bool = False
         self.case_sensitive: bool = False
-        self.filter_data: Dict[str, Any] = {}
+        self.body_data: Dict[str, Any] = {}
+        self.format_data: str = None
         self.url: str = None
         self.method: str = None
         self.requires: Dict[str, Any] = {}
         self.headers: Dict[str, Any] = self.client.headers
 
-    def with_filter(self, filter_data: Dict[str, Any]) -> 'OperationsBuilder':
-        ''' Filter '''
-        self.filter_data = filter_data
+    def with_body(self, body_data: Dict[str, Any]) -> 'OperationsBuilder':
+        ''' Body '''
+        self.body_data = body_data
+        return self
+
+    def with_format(self, format_data: str) -> 'OperationsBuilder':
+        ''' Formats the flat operations data based on the specified format ('csv', 'dict'). '''
+        self.format_data = format_data
+        if self.format_data is 'csv':
+            self.headers['Accept'] = 'text/plain'
+        else:
+            self.headers['Accept'] = 'application/json'
+
         return self
 
     def with_default_sorted(self, default_sorted: bool) -> 'OperationsBuilder':
         ''' default sorted'''
         self.default_sorted = default_sorted
         return self
     
     def with_case_sensitive(self, case_sensitive: bool) -> 'OperationsBuilder':
         ''' default sorted'''
         self.case_sensitive = case_sensitive
         return self
     
-    def add_header(self, key: str, value: str) -> 'OperationsBuilder':
-        self.headers[key] = value
-    
     def search(self) -> 'OperationsBuilder':
         ''' Searching '''
         self.requires = {
             'default_sorted': self.default_sorted,
             'case_sensitive': self.case_sensitive,
-            'filter_data': self.filter_data
+            'body_data': self.body_data
         }
         self.method = 'search'
         self.url = f'{self.client.url}/north/v80/search/entities/operations/history?utc=true&defaultSorted={self.default_sorted}&caseSensitive={self.case_sensitive}'
         return self
     
     def build(self) -> 'OperationsBuilder':
         ''' Check if any parameter is missing. '''
@@ -60,17 +68,17 @@
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
 
     def _execute_searching(self) -> Union[int, List[Dict[str, Any]]]:
         response = self._send_request()
-        return response.text
+        if response.status_code == 200:
+          if self.format_data is 'csv':
+            return response.text
+          else:
+            return response.json()
+        return response
     
+    def _send_request(self) -> requests.Response:          
+        return requests.post(self.url, headers=self.headers, json=self.body_data, verify=False, timeout=3000)    
 
-    def _send_request(self) -> requests.Response:
-        body = {}
-        
-        if(self.filter_data is not None):
-          body['filter'] = self.filter_data
-          
-        return requests.post(self.url, headers=self.headers, json=body, verify=False, timeout=3000)
```

### Comparing `opengate-data-1.0.4/opengate_data/datasets/datasets.py` & `opengate_data-1.0.5/opengate_data/datasets/datasets.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class DataSetsBuilder:
     ''' Dataset Builder '''
     def __init__(self, opengate_client):
         self.client = opengate_client
         self.organization_name: str = None
         self.identifier: str = None
-        self.filter_data: Dict[str, Any] = {}
+        self.body_data: Dict[str, Any] = {}
         self.format_data: str = None
         self.url: str = None
         self.method: str = None
         self.requires: Dict[str, Any] = {}
 
     def with_organization(self, organization_name: str) -> 'DataSetsBuilder':
         ''' Sets the organization name '''
@@ -22,17 +22,17 @@
         return self
 
     def with_identifier(self, identifier: str) -> 'DataSetsBuilder':
         ''' Sets the identifier '''
         self.identifier = identifier
         return self
 
-    def with_filter(self, filter_data: Dict[str, Any]) -> 'DataSetsBuilder':
-        ''' Sets the filter data '''
-        self.filter_data = filter_data
+    def with_body(self, body_data: Dict[str, Any]) -> 'DataSetsBuilder':
+        ''' Sets the body data '''
+        self.body_data = body_data
         return self
 
     def with_format(self, format_data: str) -> 'DataSetsBuilder':
         ''' Sets the format data '''
         self.format_data = format_data
         return self
 
@@ -61,15 +61,15 @@
         }
         function = methods.get(self.method)
         if function is None:
             raise ValueError(f'Unsupported method: {self.method}')
         return function()
 
     def _execute_searching(self) -> Union[str, List[Dict[str, Any]], pd.DataFrame]:
-        response = requests.post(self.url, headers=self.client.headers, json=self.filter_data, verify=False, timeout=3000)
+        response = requests.post(self.url, headers=self.client.headers, json=self.body_data, verify=False, timeout=3000)
         if response.status_code == 200:
             data = response.json()
             if self.format_data == 'csv':
                 csv = ','.join(data['columns']) + '\n'
                 for fila in data['data']:
                     csv += ','.join(map(str, fila)) + '\n'
                 return csv
```

### Comparing `opengate-data-1.0.4/setup.py` & `opengate_data-1.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.4'
+VERSION = '1.0.5'
 PACKAGE_NAME = 'opengate-data'
 AUTHOR = 'amplia soluciones'
 AUTHOR_EMAIL = 'pipy@amplia.es'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'description'
 
@@ -15,15 +15,16 @@
     'pandas',
     'requests',
     'jsonpath_ng',
     'numpy',
     'urllib3',
     'configparser',
     'parse',
-    'python-dotenv'
+    'python-dotenv',
+    'flatten-dict'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     author=AUTHOR,
```

