# Comparing `tmp/ado_wrapper-1.1.2.tar.gz` & `tmp/ado_wrapper-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.1.2.tar", max compression
+gzip compressed data, was "ado_wrapper-1.1.3.tar", max compression
```

## Comparing `ado_wrapper-1.1.2.tar` & `ado_wrapper-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.1.2/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.1.2/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.1.2/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.1.2/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.1.2/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.1.2/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.1.2/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.1.2/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.1.2/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      936 2024-04-17 20:35:57.592719 ado_wrapper-1.1.2/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.1.2/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.1.2/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14507 2024-04-19 08:11:40.921543 ado_wrapper-1.1.2/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.1.2/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3891 2024-04-19 08:13:44.700559 ado_wrapper-1.1.2/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.1.2/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    14951 2024-04-19 10:06:29.170184 ado_wrapper-1.1.2/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.1.2/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.1.2/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.1.2/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10223 2024-04-19 08:59:23.116079 ado_wrapper-1.1.2/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.1.2/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.1.2/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.1.2/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4905 2024-04-18 15:13:38.570059 ado_wrapper-1.1.2/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8988 2024-04-19 08:06:50.425296 ado_wrapper-1.1.2/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-18 15:00:31.824976 ado_wrapper-1.1.2/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4412 2024-04-19 09:09:37.626208 ado_wrapper-1.1.2/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2446 2024-04-19 10:06:40.995463 ado_wrapper-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.1.3/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.1.3/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.1.3/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.1.3/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.1.3/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.1.3/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.1.3/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.1.3/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.1.3/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      936 2024-04-17 20:35:57.592719 ado_wrapper-1.1.3/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.1.3/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.1.3/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14507 2024-04-19 08:11:40.921543 ado_wrapper-1.1.3/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.1.3/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3891 2024-04-19 08:13:44.700559 ado_wrapper-1.1.3/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.1.3/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    14986 2024-04-19 10:09:09.141487 ado_wrapper-1.1.3/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.1.3/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.1.3/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.1.3/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10223 2024-04-19 08:59:23.116079 ado_wrapper-1.1.3/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.1.3/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.1.3/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.1.3/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4905 2024-04-18 15:13:38.570059 ado_wrapper-1.1.3/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8988 2024-04-19 08:06:50.425296 ado_wrapper-1.1.3/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-18 15:00:31.824976 ado_wrapper-1.1.3/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4412 2024-04-19 09:09:37.626208 ado_wrapper-1.1.3/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2446 2024-04-19 10:09:39.459385 ado_wrapper-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.1.3/PKG-INFO
```

### Comparing `ado_wrapper-1.1.2/LICENSE` & `ado_wrapper-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/README.md` & `ado_wrapper-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/__main__.py` & `ado_wrapper-1.1.3/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/client.py` & `ado_wrapper-1.1.3/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/dumps.py` & `ado_wrapper-1.1.3/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.1.3/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/branches.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/builds.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/commits.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/environment.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/groups.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/merge_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,17 +123,18 @@
             data["id"], settings["scope"][0]["repositoryId"], (branch_name.removeprefix("refs/heads/") if branch_name else None),
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
             when_new_changes_are_pushed, from_ado_date_string(data["createdDate"]),  # type: ignore[arg-type]
             is_inherited  # fmt: skip
         )
 
     @classmethod
-    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "MergeBranchPolicy":
+    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> "MergeBranchPolicy | None":
         """Gets the latest merge requirements for a pull request."""
-        return MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id, branch_name)[0]  # type: ignore[index]
+        policy = MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id, branch_name)
+        return policy[0] if policy else None
 
     @staticmethod
     def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
                           when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:  # fmt: skip
         """Sets the perms for a pull request, can also be used as a "update" function."""
         existing_policy = MergePolicies.get_all_by_repo_id(ado_client, repo_id, branch_name)
@@ -247,9 +248,9 @@
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
                           when_new_changes_are_pushed: WhenChangesArePushed, branch_name: str = "main") -> None:  # fmt: skip
         return MergeBranchPolicy.set_branch_policy(ado_client, repo_id, minimum_approver_count, creator_vote_counts,
                                                    prohibit_last_pushers_vote, allow_completion_with_rejects,
                                                    when_new_changes_are_pushed, branch_name)  # fmt: skip
 
     @staticmethod
-    def get_branch_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy:
+    def get_branch_policy(ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy | None:
         return MergeBranchPolicy.get_branch_policy(ado_client, repo_id, branch_name)
```

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/projects.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/releases.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/repo.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/teams.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/users.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.1.3/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.1.3/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/state_manager.py` & `ado_wrapper-1.1.3/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/ado_wrapper/utils.py` & `ado_wrapper-1.1.3/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.2/pyproject.toml` & `ado_wrapper-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.1.2"
+version = "1.1.3"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.1.2/PKG-INFO` & `ado_wrapper-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.1.2
+Version: 1.1.3
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

