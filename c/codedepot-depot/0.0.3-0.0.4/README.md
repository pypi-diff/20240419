# Comparing `tmp/codedepot_depot-0.0.3.tar.gz` & `tmp/codedepot_depot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.3.tar", last modified: Thu Apr 18 11:38:47 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.4.tar", last modified: Fri Apr 19 07:14:14 2024, max compression
```

## Comparing `codedepot_depot-0.0.3.tar` & `codedepot_depot-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.3/depot/__init__.py
--rw-r--r--   0        0        0     5825 2024-04-18 09:14:30.404632 codedepot_depot-0.0.3/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.3/depot/cluster_spec.py
--rw-r--r--   0        0        0     2876 2024-04-18 11:37:37.734898 codedepot_depot-0.0.3/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.3/depot/jobfile.py
--rw-r--r--   0        0        0     4323 2024-04-18 11:38:01.659087 codedepot_depot-0.0.3/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.3/depot/provider_spec.py
--rw-r--r--   0        0        0      737 2024-04-18 11:38:47.015249 codedepot_depot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.3/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.3/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.3/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.3/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.3/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.3/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.3/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.3/test/utils.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 codedepot_depot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.4/depot/__init__.py
+-rw-r--r--   0        0        0     5854 2024-04-19 07:09:25.884418 codedepot_depot-0.0.4/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.4/depot/cluster_spec.py
+-rw-r--r--   0        0        0     3775 2024-04-19 06:40:42.000435 codedepot_depot-0.0.4/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.4/depot/jobfile.py
+-rw-r--r--   0        0        0     4323 2024-04-19 07:13:36.027843 codedepot_depot-0.0.4/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.4/depot/provider_spec.py
+-rw-r--r--   0        0        0      793 2024-04-19 07:14:14.988747 codedepot_depot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.4/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.4/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.4/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.4/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.4/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.4/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.4/test/utils.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 codedepot_depot-0.0.4/PKG-INFO
```

### Comparing `codedepot_depot-0.0.3/depot/api.py` & `codedepot_depot-0.0.4/depot/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import yaml
 from depot.config import DepotConfig
 from prettytable import PrettyTable
 from depot.cluster_spec import ClusterSpec
 from depot.jobfile import JobSpec
 from depot.provider_spec import ProviderSpec
 from depot_api.api import default_api
+from depot_api.api.default_api import DefaultApi
 from depot_api.models.job_instance_in import JobInstanceIn
 from depot_api.models.cluster_in import ClusterIn
 from depot_api.models.provider import Provider
 from git_ai.metrics.experiment import get_new_exp_name
 from git_ai.cmd.ai_repo import AIRepo
 import pygit2
 import os
@@ -107,15 +108,14 @@
     instance = [i for i in instances if i['name'] == job_name]
     if not instance:
         print(f"Job {job_name} does not exist.")
         return
     
     instance = instance[0]
     response = config.api().read_log_logs_job_instance_id_get(instance['id'])
-    print(response)
     print(response['log'])
 
 
 def create_provider(config: DepotConfig, spec_file: str) -> int:
 
     try:
         spec = ProviderSpec.from_file(spec_file)
```

### Comparing `codedepot_depot-0.0.3/depot/cluster_spec.py` & `codedepot_depot-0.0.4/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.3/depot/config.py` & `codedepot_depot-0.0.4/depot/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 
 
 class DepotConfig(object):
     DEFAULT_CONFIG_FOLDER = '.depot'
     DEFAULT_CONFIG_FILE = 'config.json'
 
     def __init__(self, login: str, token: str, endpoint: str, email: str):
-        self.default_api = DefaultApi(ApiClient(Configuration(host=endpoint)))
+        config = Configuration(host=endpoint)
+        config.access_token = token
+        self.default_api = DefaultApi(ApiClient(config))
 
         self.login = login
         self.token = token
         self.endpoint = endpoint
         self.email = email
 
     def api(self) -> DefaultApi:
@@ -34,40 +36,63 @@
             file.write(json.dumps({
                 'login': self.login,
                 'token': self.token,
                 'endpoint': self.endpoint,
                 'email': self.email
             }))
 
+    @staticmethod
+    def default_config_path():
+        return os.path.join(
+            os.path.expanduser('~'),
+            DepotConfig.DEFAULT_CONFIG_FOLDER,
+            DepotConfig.DEFAULT_CONFIG_FILE)
+
     @classmethod
     def from_file(cls, filename: str) -> 'DepotConfig':
         if not os.path.exists(filename):
             return None
 
         with open(filename, 'r') as file:
             y = json.load(file)
             return cls(**y)
 
     @classmethod
     def default(cls) -> 'DepotConfig':
-        config_path = os.path.join(
-            os.path.expanduser('~'),
-            DepotConfig.DEFAULT_CONFIG_FOLDER,
-            DepotConfig.DEFAULT_CONFIG_FILE)
+        config_path = os.path.join(cls.default_config_path())
 
         return cls.from_file(config_path)
 
     @staticmethod
     def create():
-        default_endpoint = 'https://depot.staging.codedepot.ai'
+        if os.path.exists(DepotConfig.default_config_path()):
+            # Ask if the user wants to login again
+            r = prompt(
+                'You are already logged in. Do you want to log in again? [y/N]: ')
+            if r.lower() != 'y':
+                return
+            with open(DepotConfig.default_config_path(), 'r') as file:
+                y = json.load(file)
+            default_endpoint = y['endpoint']
+            default_login = y['login']
+        else:
+            default_endpoint = 'https://depot.staging.codedepot.ai'
+            default_login = None
         endpoint = prompt(
             f'Enter your API endpoint [{default_endpoint}]: ')
         if not endpoint:
             endpoint = default_endpoint
-        username = prompt('Enter your login: ')
+
+        if not default_login:
+            username = prompt('Enter your login: ')
+        else:
+            username = prompt(f'Enter your login [{default_login}]: ')
+            if not username:
+                username = default_login
+
         # Check if the username is empty TODO: check if the username is valid
         if not username:
             print('Username is required')
             return None
 
         email = prompt('Enter your email: ')
         # Check if the username is empty TODO: check if the username is valid
@@ -75,14 +100,16 @@
             print('Email is required')
             return None
 
         password = prompt(
             f'Enter the password for {username}: ', is_password=True)
         print('endpoint: ', endpoint)
         default_api = DefaultApi(ApiClient(Configuration(host=endpoint)))
-        response = default_api.login_login_post(
+
+        response = default_api.login_token_post(
             username=email, password=password)
+        print(response)
 
         config = DepotConfig(
             token=response['token'], endpoint=endpoint, login=username, email=email)
         config.save()
         print('The user is logged in, the token is stored at ~/.depot/config.json')
```

### Comparing `codedepot_depot-0.0.3/depot/main.py` & `codedepot_depot-0.0.4/depot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.3")
+        print("0.0.4")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
```

### Comparing `codedepot_depot-0.0.3/depot/provider_spec.py` & `codedepot_depot-0.0.4/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.3/pyproject.toml` & `codedepot_depot-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.3"
+version = "0.0.4"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -20,14 +20,16 @@
     "prompt-toolkit",
     "py",
     "pyaml",
     "pydantic",
     "pygit2",
     "requests",
     "depot_api",
+    "codedepot-git-ai>=0.0.20",
+    "depot-api>=1.0.3",
 ]
 
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 
 [project.scripts]
 depot = "depot.main:main"
```

### Comparing `codedepot_depot-0.0.3/test/utils.py` & `codedepot_depot-0.0.4/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.3/PKG-INFO` & `codedepot_depot-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
@@ -13,12 +13,14 @@
 Requires-Dist: prompt-toolkit
 Requires-Dist: py
 Requires-Dist: pyaml
 Requires-Dist: pydantic
 Requires-Dist: pygit2
 Requires-Dist: requests
 Requires-Dist: depot_api
+Requires-Dist: codedepot-git-ai>=0.0.20
+Requires-Dist: depot-api>=1.0.3
 Description-Content-Type: text/markdown
 
 # Depot
 
 This is the depot client. More docs to come.
```

