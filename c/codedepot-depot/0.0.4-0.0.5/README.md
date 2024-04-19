# Comparing `tmp/codedepot_depot-0.0.4.tar.gz` & `tmp/codedepot_depot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.4.tar", last modified: Fri Apr 19 07:14:14 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.5.tar", last modified: Fri Apr 19 09:04:46 2024, max compression
```

## Comparing `codedepot_depot-0.0.4.tar` & `codedepot_depot-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.4/depot/__init__.py
--rw-r--r--   0        0        0     5854 2024-04-19 07:09:25.884418 codedepot_depot-0.0.4/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.4/depot/cluster_spec.py
--rw-r--r--   0        0        0     3775 2024-04-19 06:40:42.000435 codedepot_depot-0.0.4/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.4/depot/jobfile.py
--rw-r--r--   0        0        0     4323 2024-04-19 07:13:36.027843 codedepot_depot-0.0.4/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.4/depot/provider_spec.py
--rw-r--r--   0        0        0      793 2024-04-19 07:14:14.988747 codedepot_depot-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.4/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.4/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.4/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.4/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.4/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.4/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.4/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.4/test/utils.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 codedepot_depot-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.5/depot/__init__.py
+-rw-r--r--   0        0        0     6140 2024-04-19 09:02:23.661519 codedepot_depot-0.0.5/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.5/depot/cluster_spec.py
+-rw-r--r--   0        0        0     3775 2024-04-19 06:40:42.000435 codedepot_depot-0.0.5/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.5/depot/jobfile.py
+-rw-r--r--   0        0        0     4323 2024-04-19 09:02:57.885847 codedepot_depot-0.0.5/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.5/depot/provider_spec.py
+-rw-r--r--   0        0        0      793 2024-04-19 09:04:46.208878 codedepot_depot-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.5/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.5/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.5/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.5/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.5/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.5/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.5/test/utils.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 codedepot_depot-0.0.5/PKG-INFO
```

### Comparing `codedepot_depot-0.0.4/depot/api.py` & `codedepot_depot-0.0.5/depot/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import yaml
+from ast import pattern
+import re
 from depot.config import DepotConfig
 from prettytable import PrettyTable
 from depot.cluster_spec import ClusterSpec
 from depot.jobfile import JobSpec
 from depot.provider_spec import ProviderSpec
 from depot_api.api import default_api
 from depot_api.api.default_api import DefaultApi
@@ -62,14 +63,21 @@
     table = PrettyTable()
     table.field_names = ['Name', 'Status']
     for job in response:
         table.add_row([job['name'], job['status']])
     print(table)
 
 
+def __http_to_ssh(url: str) -> str:
+    pattern = re.compile(r'(http://|https://)(.*)/(.*)/(.*).git$')
+    match = pattern.match(url)
+    if not match:
+        return url
+    return f"git@{match.group(2)}:{match.group(3)}/{match.group(4)}.git"
+    
 def start_job(config: DepotConfig, cluster_name: str):
     try:
         repo_folder = pygit2.discover_repository(os.getcwd())
         if not repo_folder:
             print("Cannot find a git repository in the current folder. Please run this command from a git repository.")
             return
 
@@ -79,15 +87,15 @@
         job_instance_name = get_new_exp_name(repo)
         clusters = config.api().list_clusters_clusters_get()
         cluster = [c for c in clusters if c['name'] == cluster_name]
         if not cluster:
             print(f"Cluster {cluster_name} does not exist.")
             return
         cluster = cluster[0]
-        repo_url = repo.remotes['origin'].url
+        repo_url = __http_to_ssh(repo.remotes['origin'].url)
         response = config.api().create_job_instance_job_instances_post(JobInstanceIn(
             repository_url=repo_url,
             starting_commit=repo.head.target.hex,
             userlogin=config.login,
             job_name=job_spec.name,
             cluster_id=cluster['id'],
             name=job_instance_name
```

### Comparing `codedepot_depot-0.0.4/depot/cluster_spec.py` & `codedepot_depot-0.0.5/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.4/depot/config.py` & `codedepot_depot-0.0.5/depot/config.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.4/depot/main.py` & `codedepot_depot-0.0.5/depot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.4")
+        print("0.0.5")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
```

### Comparing `codedepot_depot-0.0.4/depot/provider_spec.py` & `codedepot_depot-0.0.5/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.4/pyproject.toml` & `codedepot_depot-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.4"
+version = "0.0.5"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_depot-0.0.4/test/utils.py` & `codedepot_depot-0.0.5/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.4/PKG-INFO` & `codedepot_depot-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
```

