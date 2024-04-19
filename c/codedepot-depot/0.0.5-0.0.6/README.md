# Comparing `tmp/codedepot_depot-0.0.5.tar.gz` & `tmp/codedepot_depot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.5.tar", last modified: Fri Apr 19 09:04:46 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.6.tar", last modified: Fri Apr 19 09:44:45 2024, max compression
```

## Comparing `codedepot_depot-0.0.5.tar` & `codedepot_depot-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.5/depot/__init__.py
--rw-r--r--   0        0        0     6140 2024-04-19 09:02:23.661519 codedepot_depot-0.0.5/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.5/depot/cluster_spec.py
--rw-r--r--   0        0        0     3775 2024-04-19 06:40:42.000435 codedepot_depot-0.0.5/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.5/depot/jobfile.py
--rw-r--r--   0        0        0     4323 2024-04-19 09:02:57.885847 codedepot_depot-0.0.5/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.5/depot/provider_spec.py
--rw-r--r--   0        0        0      793 2024-04-19 09:04:46.208878 codedepot_depot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.5/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.5/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.5/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.5/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.5/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.5/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.5/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.5/test/utils.py
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 codedepot_depot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.6/depot/__init__.py
+-rw-r--r--   0        0        0     6140 2024-04-19 09:02:23.661519 codedepot_depot-0.0.6/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.6/depot/cluster_spec.py
+-rw-r--r--   0        0        0     3713 2024-04-19 09:37:38.563990 codedepot_depot-0.0.6/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.6/depot/jobfile.py
+-rw-r--r--   0        0        0     4233 2024-04-19 09:44:31.893716 codedepot_depot-0.0.6/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.6/depot/provider_spec.py
+-rw-r--r--   0        0        0      793 2024-04-19 09:44:45.989796 codedepot_depot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.6/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.6/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.6/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.6/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.6/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.6/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.6/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.6/test/utils.py
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 codedepot_depot-0.0.6/PKG-INFO
```

### Comparing `codedepot_depot-0.0.5/depot/api.py` & `codedepot_depot-0.0.6/depot/api.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.5/depot/cluster_spec.py` & `codedepot_depot-0.0.6/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.5/depot/config.py` & `codedepot_depot-0.0.6/depot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,16 @@
         # Check if the username is empty TODO: check if the username is valid
         if not email:
             print('Email is required')
             return None
 
         password = prompt(
             f'Enter the password for {username}: ', is_password=True)
-        print('endpoint: ', endpoint)
         default_api = DefaultApi(ApiClient(Configuration(host=endpoint)))
 
         response = default_api.login_token_post(
             username=email, password=password)
-        print(response)
 
         config = DepotConfig(
             token=response['token'], endpoint=endpoint, login=username, email=email)
         config.save()
         print('The user is logged in, the token is stored at ~/.depot/config.json')
```

### Comparing `codedepot_depot-0.0.5/depot/main.py` & `codedepot_depot-0.0.6/depot/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.5")
+        print("0.0.6")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
@@ -84,16 +84,14 @@
     if args.command == 'job':
         if args.job_command == 'start':
             start_job(config, args.cluster_name)
         elif args.job_command == 'list':
             list_jobs(config)
         elif args.job_command == 'stop':
             print(f"Stopping job {args.name}...")
-        elif args.job_command == 'log':
-            print(f"Stopping job {args.name}...")
     elif args.command == 'cluster':
         if args.cluster_command == 'create':
             print(f"Creating cluster from {args.spec}...")
             create_cluster(config, args.spec)
         elif args.cluster_command == 'list':
             list_clusters(config)
     elif args.command == 'provider':
```

### Comparing `codedepot_depot-0.0.5/depot/provider_spec.py` & `codedepot_depot-0.0.6/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.5/pyproject.toml` & `codedepot_depot-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.5"
+version = "0.0.6"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_depot-0.0.5/test/utils.py` & `codedepot_depot-0.0.6/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.5/PKG-INFO` & `codedepot_depot-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
```

