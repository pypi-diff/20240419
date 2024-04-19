# Comparing `tmp/ado_wrapper-1.1.0.tar.gz` & `tmp/ado_wrapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.1.0.tar", max compression
+gzip compressed data, was "ado_wrapper-1.1.1.tar", max compression
```

## Comparing `ado_wrapper-1.1.0.tar` & `ado_wrapper-1.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.1.0/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.1.0/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.1.0/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.1.0/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.1.0/ado_wrapper/client.py
--rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.1.0/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.1.0/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.1.0/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.1.0/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      936 2024-04-17 20:35:57.592719 ado_wrapper-1.1.0/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.1.0/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.1.0/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14358 2024-04-18 10:11:16.564382 ado_wrapper-1.1.0/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.1.0/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     4878 2024-04-18 10:11:58.176749 ado_wrapper-1.1.0/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.1.0/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    14785 2024-04-15 19:15:13.133919 ado_wrapper-1.1.0/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.1.0/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.1.0/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.1.0/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10086 2024-04-15 15:16:12.399073 ado_wrapper-1.1.0/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.1.0/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.1.0/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.1.0/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4877 2024-04-14 10:59:52.033985 ado_wrapper-1.1.0/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8749 2024-04-18 09:52:24.036512 ado_wrapper-1.1.0/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8158 2024-04-18 10:06:27.938348 ado_wrapper-1.1.0/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4412 2024-04-18 10:11:16.535800 ado_wrapper-1.1.0/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2446 2024-04-18 10:08:47.532362 ado_wrapper-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.1.1/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.1.1/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-1.1.1/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6504 2024-04-13 22:32:43.045229 ado_wrapper-1.1.1/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-15 19:13:07.849775 ado_wrapper-1.1.1/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-1.1.1/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.1.1/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.1.1/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-1.1.1/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-12 10:52:50.915024 ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1197 2024-04-14 14:26:49.075843 ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      936 2024-04-17 20:35:57.592719 ado_wrapper-1.1.1/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3697 2024-04-15 19:19:32.967229 ado_wrapper-1.1.1/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3399 2024-04-15 19:15:02.852905 ado_wrapper-1.1.1/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14507 2024-04-19 08:11:40.921543 ado_wrapper-1.1.1/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-17 12:27:37.565922 ado_wrapper-1.1.1/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3891 2024-04-19 08:13:44.700559 ado_wrapper-1.1.1/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3318 2024-04-15 19:13:07.863404 ado_wrapper-1.1.1/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    14785 2024-04-15 19:15:13.133919 ado_wrapper-1.1.1/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-1.1.1/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13973 2024-04-17 12:29:03.443391 ado_wrapper-1.1.1/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12505 2024-04-15 09:20:30.240006 ado_wrapper-1.1.1/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10223 2024-04-19 08:59:23.116079 ado_wrapper-1.1.1/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     5972 2024-04-17 09:03:01.080407 ado_wrapper-1.1.1/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4569 2024-04-14 10:59:03.753536 ado_wrapper-1.1.1/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8320 2024-04-14 15:16:24.207939 ado_wrapper-1.1.1/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4905 2024-04-18 15:13:38.570059 ado_wrapper-1.1.1/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8988 2024-04-19 08:06:50.425296 ado_wrapper-1.1.1/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-18 15:00:31.824976 ado_wrapper-1.1.1/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4412 2024-04-18 10:11:16.535800 ado_wrapper-1.1.1/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2446 2024-04-19 09:00:21.802034 ado_wrapper-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.1.1/PKG-INFO
```

### Comparing `ado_wrapper-1.1.0/LICENSE` & `ado_wrapper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/README.md` & `ado_wrapper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/__main__.py` & `ado_wrapper-1.1.1/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/client.py` & `ado_wrapper-1.1.1/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/dumps.py` & `ado_wrapper-1.1.1/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.1.1/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/branches.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/builds.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/builds.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,22 +156,22 @@
         return super().get_all(
             ado_client,
             f"/{ado_client.ado_project}/_apis/build/builds?definitions={definition_id}&api-version=7.1",
         )  # type: ignore[return-value]
 
     @classmethod
     def allow_approvers(cls, ado_client: "AdoClient", build_definition_id: str, approvers_ids: str) -> None:
-        """This is a PATCH request, so it doesn't return anything."""
         return NotImplementedError("This method is not implemented yet!")  # type: ignore[return-value]
+        # https://dev.azure.com/VFCloudEngineering/Platform/_environments/170/security
+        # https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project_id}/_apis/pipelines/pipelinePermissions/environment/170
         # ado_client.session.patch(
         #     f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/pipelines/pipelinePermissions/approvers?api-version=7.1",
         #     json={"approvers": [{"id": approvers_ids}]},
         # )
 
-
 # ========================================================================================================
 
 
 @dataclass
 class BuildDefinition(StateManagedResource):
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/build/definitions?view=azure-devops-rest-7.1"""
```

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/commits.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/groups.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/projects.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/releases.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/repo.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
         try:
             request = ado_client.session.get(
                 f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
             )
         except requests.exceptions.ConnectionError:
             print(f"=== Connection error, failed to download {self.repo_id}")
             return {}
+        if request.status_code == 404:
+            raise ResourceNotFound(f"Repo {self.repo_id} does not have any branches or content!")
         if request.status_code != 200:
             print(f"Error getting repo contents for {self.name} ({self.repo_id}):", request.text)
             return {}
         # ============ We do this because ADO ===================
         bytes_io = io.BytesIO()
         for chunk in request.iter_content(chunk_size=128):
             bytes_io.write(chunk)
```

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/teams.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/users.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.1.1/ado_wrapper/resources/variable_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     created_on: datetime
     created_by: Member
     modified_by: Member
     modified_on: datetime | None = None
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> "VariableGroup":
+        # print("\n", data)
         created_by = Member.from_request_payload(data["createdBy"])
         modified_by = Member.from_request_payload(data["modifiedBy"])
         return cls(str(data["id"]), data["name"], data.get("description", ""),
                    {key: value["value"] if isinstance(value, dict) else value for key, value in data["variables"].items()},
                    from_ado_date_string(data["createdOn"]), created_by, modified_by, from_ado_date_string(data.get("modifiedOn")))  # fmt: skip
 
     @classmethod
```

### Comparing `ado_wrapper-1.1.0/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.1.1/ado_wrapper/state_managed_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,28 +73,31 @@
             raise ValueError(f"Error getting {cls.__name__} by id: {request.text}")
         if "value" in request.json():
             return cls.from_request_payload(request.json()["value"][0])
         return cls.from_request_payload(request.json())
 
     @classmethod
     def create(
-        cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None
+        cls, ado_client: "AdoClient", url: str, payload: dict[str, Any] | None = None, refetch: bool = False
     ) -> "StateManagedResource | PlannedStateManagedResource":
+        """When creating, often the response doesn't contain all the data, refetching does a .get_by_id() after creation."""
         if ado_client.plan_mode:
             return PlannedStateManagedResource.create(cls, ado_client, url, payload)
         if not url.startswith("https://"):
             url = f"https://dev.azure.com/{ado_client.ado_org}" + url
         request = ado_client.session.post(url, json=payload or {})  # Create a brand new dict
         if request.status_code >= 300:
             if request.status_code == 401:
                 raise PermissionError(f"You do not have permission to create this {cls.__name__}!")
             if request.status_code == 409:
                 raise ResourceAlreadyExists(f"The {cls.__name__} with that identifier already exist!")
             raise ValueError(f"Error creating {cls.__name__}: {request.status_code} - {request.text}")
         resource = cls.from_request_payload(request.json())
+        if refetch:
+            resource = cls.get_by_id(ado_client, extract_id(resource))
         ado_client.state_manager.add_resource_to_state(cls.__name__, extract_id(resource), resource.to_json())  # type: ignore[arg-type]
         return resource
 
     @classmethod
     def delete_by_id(cls, ado_client: "AdoClient", url: str, resource_id: str) -> None:
         """Deletes an object by its id. The id is passed so it can be removed from state"""
         if not url.startswith("https://"):
```

### Comparing `ado_wrapper-1.1.0/ado_wrapper/state_manager.py` & `ado_wrapper-1.1.1/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/ado_wrapper/utils.py` & `ado_wrapper-1.1.1/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.1.0/pyproject.toml` & `ado_wrapper-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.1.0"
+version = "1.1.1"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.1.0/PKG-INFO` & `ado_wrapper-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

