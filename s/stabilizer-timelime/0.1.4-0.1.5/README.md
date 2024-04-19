# Comparing `tmp/stabilizer_timelime-0.1.4.tar.gz` & `tmp/stabilizer_timelime-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.1.4.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.1.5.tar", max compression
```

## Comparing `stabilizer_timelime-0.1.4.tar` & `stabilizer_timelime-0.1.5.tar`

### file list

```diff
@@ -1,58 +1,29 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.1.4/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.1.4/README.md
--rw-r--r--   0        0        0      774 2024-04-15 22:24:20.789467 stabilizer_timelime-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.4/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.1.4/stabilizer_timelime/src/dataslurper/__init__.py
--rw-r--r--   0        0        0     7449 2024-04-12 21:48:22.444899 stabilizer_timelime-0.1.4/stabilizer_timelime/src/dataslurper/slurpdata.py
--rw-r--r--   0        0        0      466 2024-04-15 19:47:05.100154 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/config.py
--rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/.DS_Store
--rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/CFS.py
--rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
--rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/DE.py
--rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
--rw-r--r--   0        0        0    10624 2024-04-15 19:30:51.521486 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
--rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Stats_files.py
--rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__init__.py
--rw-r--r--   0        0        0    20141 2024-04-14 16:32:19.968508 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-311.pyc
--rw-r--r--   0        0        0    12066 2024-04-14 16:32:20.199210 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-36.pyc
--rw-r--r--   0        0        0    11544 2024-04-14 16:32:19.680899 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS.cpython-39.pyc
--rw-r--r--   0        0        0    20865 2024-04-14 16:32:20.001262 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-311.pyc
--rw-r--r--   0        0        0    12443 2024-04-14 16:32:20.226350 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-36.pyc
--rw-r--r--   0        0        0    12008 2024-04-14 16:32:19.635109 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/CFS_regression.cpython-39.pyc
--rw-r--r--   0        0        0    13950 2024-04-14 16:32:19.945143 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-311.pyc
--rw-r--r--   0        0        0     7415 2024-04-14 16:32:20.173581 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-36.pyc
--rw-r--r--   0        0        0     7464 2024-04-14 16:32:19.570655 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/DE.cpython-39.pyc
--rw-r--r--   0        0        0    11789 2024-04-14 16:32:19.727169 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-311.pyc
--rw-r--r--   0        0        0     7152 2024-04-14 16:32:20.063052 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-36.pyc
--rw-r--r--   0        0        0     7307 2024-04-14 16:32:19.656571 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch.cpython-39.pyc
--rw-r--r--   0        0        0    13876 2024-04-14 16:32:19.747287 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-311.pyc
--rw-r--r--   0        0        0     7330 2024-04-14 16:32:20.044202 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-36.pyc
--rw-r--r--   0        0        0     7398 2024-04-14 16:32:19.549450 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/birch_bellwether_p_CFS.cpython-39.pyc
--rw-r--r--   0        0        0    14400 2024-04-14 16:32:19.922687 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-311.pyc
--rw-r--r--   0        0        0     9271 2024-04-14 16:32:20.153414 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-36.pyc
--rw-r--r--   0        0        0     9024 2024-04-14 16:32:19.477117 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/learners.cpython-39.pyc
--rw-r--r--   0        0        0     7670 2024-04-14 16:32:19.792034 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-311.pyc
--rw-r--r--   0        0        0     3370 2024-04-14 16:32:20.106860 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-36.pyc
--rw-r--r--   0        0        0     3392 2024-04-14 16:32:19.613566 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/optimizer.cpython-39.pyc
--rw-r--r--   0        0        0    16154 2024-04-14 16:32:19.770017 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-311.pyc
--rw-r--r--   0        0        0     8113 2024-04-14 16:32:20.085417 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-36.pyc
--rw-r--r--   0        0        0     7710 2024-04-14 16:32:19.591425 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_advance_v1.cpython-39.pyc
--rw-r--r--   0        0        0     7603 2024-04-14 16:32:19.901567 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-311.pyc
--rw-r--r--   0        0        0     3804 2024-04-14 16:32:20.127744 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-36.pyc
--rw-r--r--   0        0        0     3630 2024-04-14 16:32:19.502452 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/predictor_baseline.cpython-39.pyc
--rw-r--r--   0        0        0     9209 2024-04-14 16:32:19.705103 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     4609 2024-04-14 16:32:20.023240 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0        0        0     4801 2024-04-14 16:32:19.528105 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
--rwxr-xr-x   0        0        0     8459 2024-04-14 16:32:21.663496 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/birch.py
--rw-r--r--   0        0        0    11413 2024-04-15 22:13:14.951421 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
--rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
--rw-r--r--   0        0        0     9282 2024-04-15 19:40:19.503100 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
--rw-r--r--   0        0        0     4056 2024-04-15 21:39:00.614598 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
--rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/learners.py
--rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/optimizer.py
--rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
--rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
--rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/utils.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1492 2024-04-16 18:48:45.808071 stabilizer_timelime-0.1.5/LICENSE
+-rw-r--r--   0        0        0      776 2024-04-16 20:19:56.407964 stabilizer_timelime-0.1.5/README.md
+-rw-r--r--   0        0        0      774 2024-04-19 17:50:35.134940 stabilizer_timelime-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.5/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.1.5/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     4970 2024-04-19 17:00:10.043081 stabilizer_timelime-0.1.5/stabilizer_timelime/src/dataslurper/prudenceChecker.py
+-rw-r--r--   0        0        0     8133 2024-04-19 17:15:29.046008 stabilizer_timelime-0.1.5/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      466 2024-04-15 19:47:05.100154 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-15 00:35:54.693095 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10716 2024-04-15 23:28:50.247476 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8784 2024-04-15 22:32:53.920281 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11445 2024-04-15 22:40:20.361407 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9306 2024-04-15 23:03:18.017939 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     4072 2024-04-15 23:17:41.353624 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
+-rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.5/PKG-INFO
```

### Comparing `stabilizer_timelime-0.1.4/pyproject.toml` & `stabilizer_timelime-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.1.4"
+version = "0.1.5"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/dataslurper/slurpdata.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from github import Github
 from github import Auth
 
 import pandas as pd
 
 from tqdm import tqdm
 
+from .prudenceChecker import PrudenceChecker
+
+DEFAULT_PRUDENCE_CHECKER = PrudenceChecker()
+
 def inc_value_in_dict(result: dict, date: str, column: str) -> None:
     """
         Helper function that increments the indicator value for given date.
         Parameters:
             result: Python dictionary containing indicator value for a date
             date: String representation of the date
             coulmn: Indicator
@@ -114,40 +118,53 @@
     """
     stargazers = repo.get_stargazers_with_dates()
     for star in stargazers:
         starred_at = star.starred_at.replace(day=1)
         inc_value_in_dict(result, starred_at.strftime('%Y-%m-%d'), "monthly_stargazer")
 
 
-def create_dataset(repo_list_csv: str, access_tokens: list, dest_folder: str) -> None:
+def create_dataset(repo_list_csv: str, access_tokens_dict: dict, dest_folder: str, prudence_checker: PrudenceChecker=DEFAULT_PRUDENCE_CHECKER) -> None:
     """
         Creates the dataset and stores in csv files in dest_folder. 
         Parameters:
             repo_list_csv: Path of the csv file that contains organization and repo name info
-            access_tokens: List of github access tokens
+            access_tokens_dict: dict of github access tokens with key as username as value as the token
             dest_folder: Path of the destination folder
     """
     token_ind = 0
 
+    access_tokens = list(access_tokens_dict.values())
+    access_usernames = list(access_tokens_dict.keys())
+
     repo_list = pd.read_csv(repo_list_csv)
 
-    print("Number of projects to slurp:", repo_list.shape[0])
+    print("Number of projects to process:", repo_list.shape[0])
 
     Path(dest_folder).mkdir(parents=True, exist_ok=True)
 
     if ("organization" not in repo_list.columns) or ("repo" not in repo_list.columns):
         raise Exception("CSV missing column organization or/and repo")
+    
+
+    if ("url" not in repo_list.columns):
+        raise Exception("CSV missing column url")
 
     funcs = [get_commits, get_prs, get_issues, get_stargazers]
 
     for _, row in tqdm(repo_list.iterrows()):
 
         org_name = row["organization"]
         repo_name = row["repo"]
 
+        repo_url = row["url"]
+
+        if not prudence_checker.is_passing_prudence(url=repo_url, token=access_tokens[token_ind], username=access_usernames[token_ind]):
+            print("Failed prudence check: {0}/{1}".format(org_name, repo_name))
+            continue
+
         if os.path.isfile(os.path.join(dest_folder, org_name+"_"+repo_name+".csv")):
             continue
 
         auth = Auth.Token(access_tokens[token_ind%len(access_tokens)])
 
         g = Github(auth=auth)
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/config.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/config.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/.DS_Store` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/CFS.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/CFS_regression.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/CFS_regression.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/DE.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/DE.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
 def get_predicted(cluster_data, project_data, goal_num, metrics, month,seed, config=DEFAULT_CONFIG):
     try:
         train_data = pd.read_pickle(cluster_data + '/train_data.pkl')
         
         cluster,cluster_tree,max_depth = cluster_driver(train_data,goal_num,config)
         goal = get_goal(goal_num, config)
+        path  = 'results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/' + goal
         print("GOAL NO: ",goal)
         conv_bell_df = pd.read_pickle('results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/' + goal + '/default_bellwether.pkl')
         conv_bell_df = pd.DataFrame.from_dict(conv_bell_df, orient = 'index')
         # print("conv bell", conv_bell_df)
         conv_bell = conv_bell_df.median(axis = 0).idxmin()
         conv_bell_model_df = pd.read_pickle('results/with_CFS_DE/'+str(seed)+'/month_' + str(month) + '_models/' + goal + '/default_bellwether_models.pkl')
         conv_bell_clf = conv_bell_model_df[conv_bell]
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/Stats_files.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/Stats_files.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/attribute_selector.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/attribute_selector.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/birch.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/birch.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,31 +74,45 @@
     #Calculate the d1 distance(point farthest away from centroid)
     def calculate_d1(self,centroid,data_points):
         d1 = 0
         u = centroid
         d1_v = None
         for point in data_points:
             v = point
+            
+            if type(u) is int:
+                u = np.array([u])
+            
+            if type(v) is int:
+                v = np.array([v])
+
+            print(u, v)
             distance = euclidean(u,v)
             if distance>d1:
                 d1 = distance
                 d1_v = v
         return d1,d1_v
     
     #Calculate the d2 distance(point farthest away from d1 and its distance from centroid)
     def calculate_d2(self,centroid,data_points,d1_v):
         d2_d1 = 0
         u = d1_v
         d2_v = None
         for point in data_points:
             v = point
+            if type(u) is int:
+                u = np.array([u])
+            
+            if type(v) is int:
+                v = np.array([v])
             distance = euclidean(u,v)
             if distance>d2_d1:
                 d2_d1 = distance
                 d2_v = v
+
         d2 = euclidean(centroid,v)
         return d2
     
     # Display's the tree
     def show_clutser_tree(self):
         self.htree.display_tree()
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,17 @@
 
     def apply_cfs(self, df):
         goal = utils.get_goal(self.goal, self.config)
         y = df[goal].values
         X_df = df.drop(labels = [goal],axis = 1)
         X = X_df.values
         selected_cols = CFS.cfs(X,y)
-        cols = X_df.columns[[selected_cols]].tolist()
+        cols = X_df.columns[[selected_cols]].tolist()[0]
         cols.append(goal)
+
         return df[cols],cols
 
 
     # Cluster Driver
     def cluster_driver(self,df,print_tree = True):
         X = df.apply(pd.to_numeric)
         cluster = birch.birch(branching_factor=self.config.branching_factor)
@@ -149,14 +150,15 @@
             print("starting thread ",i)
             t = ThreadWithReturnValue(target = self.bellwether, args = [split_projects[i],projects])
             threads.append(t)
         for th in threads:
             th.start()
         for th in threads:
             response = th.join()
+            print(response)
             results.update(response[0])
             models.update(response[1])
             features.update(response[2])
         return results, models, features
 
     # For every cluster : Train model on a project and test on other projects
     # store in .pkl file
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/default_bellwether.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/default_bellwether.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         # df = pd.read_pickle(data_store_path + str(cluster_id)  + '/700_RF_default_bellwether.pkl')
 
 
 def default_bellwether(config=DEFAULT_CONFIG):
     month = config.month
     no_goals = config.no_goals
     seed = config.seed
+    cores = cpu_count()
 
 
     for i in range(no_goals):
         print('Running Goal:', i)
         goal = utils.get_goal(i, config)
         start = timeit.default_timer()
         path = "data/data_use/"
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/init_datafiles.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/init_datafiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pandas as pd
 
 from ..config import Config
 
 DEFAULT_CONFIG = Config()
 
 def create_folders(config=DEFAULT_CONFIG):
-    folders_to_create = ["data/data_use/","results/attribute/", "results/with_CFS_DE/", "meta_data/"]
+    folders_to_create = ["data/data_use/","results/attribute/", "results/with_CFS_DE/", "meta_data/", "bellwethers/"]
 
     for folder in folders_to_create:
         shutil.rmtree(folder, ignore_errors=True)
         Path(folder).mkdir(parents=True, exist_ok=True)
     
     shutil.rmtree("data/data_use_{0}_months/".format(config.month), ignore_errors=True)
     Path("data/data_use_{0}_months/".format(config.month)).mkdir(parents=True, exist_ok=True)
```

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/learners.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/learners.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/optimizer.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/optimizer.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.4/stabilizer_timelime/src/stabilizer/src/utils.py` & `stabilizer_timelime-0.1.5/stabilizer_timelime/src/stabilizer/src/utils.py`

 * *Files identical despite different names*

