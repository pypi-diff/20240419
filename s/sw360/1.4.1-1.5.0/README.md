# Comparing `tmp/sw360-1.4.1.tar.gz` & `tmp/sw360-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw360-1.4.1.tar", max compression
+gzip compressed data, was "sw360-1.5.0.tar", max compression
```

## Comparing `sw360-1.4.1.tar` & `sw360-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1221 2023-05-27 09:40:39.889958 sw360-1.4.1/License.md
-drwxr-xr-x   0        0        0        0 2023-05-27 09:26:46.746551 sw360-1.4.1/LICENSES/
--rw-r--r--   0        0        0     2032 2024-03-08 10:53:59.187964 sw360-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     3569 2024-03-08 12:06:26.468456 sw360-1.4.1/Readme.md
--rw-r--r--   0        0        0      533 2024-03-08 10:57:19.119783 sw360-1.4.1/sw360/__init__.py
--rw-r--r--   0        0        0    10368 2023-12-25 11:53:58.650360 sw360-1.4.1/sw360/attachments.py
--rw-r--r--   0        0        0     4463 2023-12-06 21:26:35.908933 sw360-1.4.1/sw360/base.py
--rw-r--r--   0        0        0     1745 2023-12-07 17:07:16.238541 sw360-1.4.1/sw360/clearing.py
--rw-r--r--   0        0        0    11250 2023-12-09 10:55:44.020997 sw360-1.4.1/sw360/components.py
--rw-r--r--   0        0        0     4643 2023-12-09 10:48:03.748773 sw360-1.4.1/sw360/license.py
--rw-r--r--   0        0        0    20045 2024-03-08 10:53:59.187964 sw360-1.4.1/sw360/project.py
--rw-r--r--   0        0        0        0 2023-12-09 10:15:18.182314 sw360-1.4.1/sw360/py.typed
--rw-r--r--   0        0        0     9933 2023-12-08 21:44:33.265803 sw360-1.4.1/sw360/releases.py
--rw-r--r--   0        0        0     4879 2023-12-09 10:21:03.602004 sw360-1.4.1/sw360/sw360_api.py
--rw-r--r--   0        0        0     1446 2023-12-09 10:21:14.547304 sw360-1.4.1/sw360/sw360error.py
--rw-r--r--   0        0        0     4840 2023-12-09 10:21:32.507818 sw360-1.4.1/sw360/sw360oauth2.py
--rw-r--r--   0        0        0     3723 2023-12-09 10:37:18.666518 sw360-1.4.1/sw360/vendor.py
--rw-r--r--   0        0        0     1580 2023-12-09 10:36:53.203617 sw360-1.4.1/sw360/vulnerabilities.py
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 sw360-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1221 2023-05-27 09:40:39.889958 sw360-1.5.0/License.md
+drwxr-xr-x   0        0        0        0 2023-05-27 09:26:46.746551 sw360-1.5.0/LICENSES/
+-rw-r--r--   0        0        0     2032 2024-04-19 16:04:18.400078 sw360-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3569 2024-03-08 12:06:26.468456 sw360-1.5.0/Readme.md
+-rw-r--r--   0        0        0      533 2024-04-19 16:03:57.187776 sw360-1.5.0/sw360/__init__.py
+-rw-r--r--   0        0        0    10394 2024-04-19 16:02:29.584652 sw360-1.5.0/sw360/attachments.py
+-rw-r--r--   0        0        0     9092 2024-04-19 16:04:54.062612 sw360-1.5.0/sw360/base.py
+-rw-r--r--   0        0        0     1745 2023-12-07 17:07:16.238541 sw360-1.5.0/sw360/clearing.py
+-rw-r--r--   0        0        0    11023 2024-04-19 16:02:29.587651 sw360-1.5.0/sw360/components.py
+-rw-r--r--   0        0        0     4634 2024-04-19 16:02:29.588651 sw360-1.5.0/sw360/license.py
+-rw-r--r--   0        0        0    19735 2024-04-19 16:02:29.589650 sw360-1.5.0/sw360/project.py
+-rw-r--r--   0        0        0        0 2023-12-09 10:15:18.182314 sw360-1.5.0/sw360/py.typed
+-rw-r--r--   0        0        0     9734 2024-04-19 16:02:29.589650 sw360-1.5.0/sw360/releases.py
+-rw-r--r--   0        0        0     5430 2024-04-19 16:02:29.590649 sw360-1.5.0/sw360/sw360_api.py
+-rw-r--r--   0        0        0     1446 2023-12-09 10:21:14.547304 sw360-1.5.0/sw360/sw360error.py
+-rw-r--r--   0        0        0     4840 2023-12-09 10:21:32.507818 sw360-1.5.0/sw360/sw360oauth2.py
+-rw-r--r--   0        0        0     3552 2024-04-19 16:02:29.591650 sw360-1.5.0/sw360/vendor.py
+-rw-r--r--   0        0        0     1580 2023-12-09 10:36:53.203617 sw360-1.5.0/sw360/vulnerabilities.py
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 sw360-1.5.0/PKG-INFO
```

### Comparing `sw360-1.4.1/License.md` & `sw360-1.5.0/License.md`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/pyproject.toml` & `sw360-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: (c) 2018-2023 Siemens
 # SPDX-License-Identifier: MIT
 
 [tool.poetry]
 name = "sw360"
-version = "1.4.1"
+version = "1.5.0"
 description = "Python interface to the SW360 software component catalogue"
 authors = ["Thomas Graf <thomas.graf@siemens.com>",
 "Gernot Hillier <gernot.hillier@siemens.com>"]
 license = "MIT License"
 readme="Readme.md"
 include = ["LICENSE.md"]
 repository = "https://github.com/sw360/sw360python"
```

### Comparing `sw360-1.4.1/Readme.md` & `sw360-1.5.0/Readme.md`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/sw360/__init__.py` & `sw360-1.5.0/sw360/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # All Rights Reserved.
 # Author: thomas.graf@siemens.com
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
-__version__ = (1, 4, 1)
+__version__ = (1, 5, 0)
 
 from .sw360_api import SW360
 from .sw360error import SW360Error
 from .sw360oauth2 import SW360OAuth2
 
 __all__ = [
     "SW360",
```

### Comparing `sw360-1.4.1/sw360/attachments.py` & `sw360-1.5.0/sw360/attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,21 +215,22 @@
             "file": (filename, open(upload_file, "rb"), "multipart/form-data"),
             "attachment": (
                 "",  # dummy filename
                 json.dumps(attachment_data),
                 "application/json",
             ),
         }
-        response = requests.post(url, headers=self.api_headers, files=file_data)  # type: ignore
-        if response.status_code == HTTPStatus.ACCEPTED:
-            logger.warning(
-                f"Attachment upload was accepted by {url} but might not be visible yet: {response.text}"
-            )
-        if not response.ok:
-            raise SW360Error(response, url)
+        response = self.api_post_multipart(url, files=file_data)
+        if response is not None:
+            if response.status_code == HTTPStatus.ACCEPTED:
+                logger.warning(
+                    f"Attachment upload was accepted by {url} but might not be visible yet: {response.text}"
+                )
+            if not response.ok:
+                raise SW360Error(response, url)
 
     def upload_release_attachment(self, release_id: str, upload_file: str, upload_type: str = "SOURCE",
                                   upload_comment: str = "") -> None:
         """Upload `upload_file` as attachment to SW360 for `release_id`,
         using `upload_comment` for it. `upload_type` can be
         "DOCUMENT"
         "SOURCE"
```

### Comparing `sw360-1.4.1/sw360/clearing.py` & `sw360-1.5.0/sw360/clearing.py`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/sw360/components.py` & `sw360-1.5.0/sw360/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 from typing import Any, Dict, List, Optional
 
-import requests
-
 from .base import BaseMixin
 from .sw360error import SW360Error
 
 
 class ComponentsMixin(BaseMixin):
     # return type List[Dict[str, Any]] | Optional[Dict[str, Any]] for Python 3.11 is good,
     # Union[List[Dict[str, Any]], Optional[Dict[str, Any]]] for lower Python versions is not good
@@ -193,21 +191,20 @@
 
         url = self.url + "resource/api/components"
 
         for param in "name", "description", "homepage":
             component_details[param] = locals()[param]
         component_details["componentType"] = component_type
 
-        response = requests.post(
-            url, json=component_details, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_post(
+            url, json=component_details)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def update_component(self, component: Dict[str, Any], component_id: str) -> Optional[Dict[str, Any]]:
         """Update an existing component
 
         API endpoint: PATCH /components
 
         :param component: the new component data
@@ -219,22 +216,15 @@
         :raises SW360Error: if there is a negative HTTP response
         """
 
         if not component_id:
             raise SW360Error(message="No component id provided!")
 
         url = self.url + "resource/api/components/" + component_id
-        response = requests.patch(
-            url, json=component, headers=self.api_headers,
-        )
-
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        return self.api_patch(url, json=component)
 
     def update_component_external_id(self, ext_id_name: str, ext_id_value: str,
                                      component_id: str, update_mode: str = "none") -> Optional[Dict[str, Any]]:
         """Set or update external id of a component. If the id is already set, it
         will only be changed if `update_mode=="overwrite"`. The id can be
         deleted using `update_mode=="delete"`.
 
@@ -278,21 +268,19 @@
         :raises SW360Error: if there is a negative HTTP response
         """
 
         if not component_id:
             raise SW360Error(message="No component id provided!")
 
         url = self.url + "resource/api/components/" + component_id
-        response = requests.delete(
-            url, headers=self.api_headers,
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_delete(url)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def get_users_of_component(self, component_id: str) -> Optional[Dict[str, Any]]:
         """Get information of about the users of a component
 
         API endpoint: GET /components/usedBy/{id}
 
         :param component_id: the id of the component to be requested
```

### Comparing `sw360-1.4.1/sw360/license.py` & `sw360-1.5.0/sw360/license.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,21 +46,21 @@
         url = self.url + "resource/api/licenses"
 
         license_details["shortName"] = shortName
         license_details["fullName"] = fullName
         license_details["text"] = text
         license_details["checked"] = checked
 
-        response = requests.post(url, json=license_details, headers=self.api_headers)
-        if response.ok:
-            return response.json()
-
+        response = self.api_post(url, json=license_details)
+        if response is not None:
+            if response.ok:
+                return response.json()
         raise SW360Error(response, url)
 
-    def delete_license(self, license_shortname: str) -> bool:
+    def delete_license(self, license_shortname: str) -> Optional[bool]:
         """Delete an existing license
 
         API endpoint: PATCH /licenses
 
         :param license_shortname: license shortname as the id
         :type license_shortname: string
         :return: SW360 result
@@ -69,22 +69,19 @@
         """
 
         if not license_shortname:
             raise SW360Error(message="No license shortname provided!")
 
         url = self.url + "resource/api/licenses/" + license_shortname
         print(url)
-        response = requests.delete(
-            url, headers=self.api_headers,
-        )
-
-        if response.ok:
-            return True
-
-        raise SW360Error(response, url)
+        response = self.api_delete(url)
+        if response is not None:
+            if response.ok:
+                return True
+        return None
 
     def download_license_info(
         self, project_id: str, filename: str, generator: str = "XhtmlGenerator", variant: str = "DISCLOSURE"
     ) -> None:
         """Gets the license information, aka Readme_OSS for the project
         with the given id
```

### Comparing `sw360-1.4.1/sw360/project.py` & `sw360-1.5.0/sw360/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 from typing import Any, Dict, List, Optional
 
-import requests
-
 from .base import BaseMixin
 from .sw360error import SW360Error
 
 
 class ProjectMixin(BaseMixin):
     def get_project(self, project_id: str) -> Optional[Dict[str, Any]]:
         """Get information of about a project
@@ -301,21 +299,19 @@
         :raises SW360Error: if there is a negative HTTP response
         """
         for param in "name", "visibility", "version", "description":
             project_details[param] = locals()[param]
         project_details["projectType"] = project_type
 
         url = self.url + "resource/api/projects"
-        response = requests.post(
-            url, json=project_details, headers=self.api_headers
-        )
-
-        if response.ok:
-            return response.json()
-
+        response = self.api_post(
+            url, json=project_details)
+        if response is not None:
+            if response.ok:
+                return response.json()
         raise SW360Error(response, url)
 
     def update_project(self, project: Dict[str, Any], project_id: str,
                        add_subprojects: bool = False) -> Optional[Dict[str, Any]]:
         """Update an existing project
 
         API endpoint: PATCH /projects
@@ -341,22 +337,20 @@
                 for sp in current["linkedProjects"]:
                     pid = self.get_id_from_href(sp["project"])
                     if pid not in project["linkedProjects"]:
                         nsp = {}
                         nsp["projectRelationship"] = sp.get("relation", "CONTAINED")
                         project["linkedProjects"][pid] = nsp
 
-        response = requests.patch(url, json=project, headers=self.api_headers)
+        return self.api_patch(url, json=project)
 
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
-
-    def update_project_releases(self, releases: List[Dict[str, Any]], project_id: str, add: bool = False) -> bool:
+    def update_project_releases(
+        self,
+        releases: List[Dict[str, Any]], project_id: str, add: bool = False
+    ) -> Optional[bool]:
         """Update the releases of an existing project. If `add` is True,
         given `releases` are added to the project, otherwise, the existing
         releases will be replaced.
 
         API endpoint: POST /projects/<id>/releases
 
         :param releases: list of relase_ids to be linked in the project
@@ -379,20 +373,19 @@
                     and "sw360:releases" in old_releases["_embedded"]):
                 old_releases = old_releases["_embedded"]["sw360:releases"]
                 old_releases = [r["_links"]["self"]["href"] for r in old_releases]
                 old_releases = [r.split("/")[-1] for r in old_releases]
                 releases = old_releases + list(releases)
 
         url = self.url + "resource/api/projects/" + project_id + "/releases"
-        response = requests.post(url, json=releases, headers=self.api_headers)
-
-        if response.ok:
-            return True
-
-        raise SW360Error(response, url)
+        response = self.api_post(url, json=releases)
+        if response is not None:
+            if response.ok:
+                return True
+        return None
 
     def update_project_external_id(self, ext_id_name: str, ext_id_value: str,
                                    project_id: str, update_mode: str = "none") -> Any:
         """Set or update external id of a project. If the id is already set, it
         will only be changed if `update_mode=="overwrite"`. The id can be
         deleted using `update_mode=="delete"`.
 
@@ -437,21 +430,19 @@
         """
         # 2019-04-03: error 405 - method not allowed
 
         if not project_id:
             raise SW360Error(message="No project id provided!")
 
         url = self.url + "resource/api/projects/" + project_id
-        response = requests.delete(
-            url, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_delete(url)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def get_users_of_project(self, project_id: str) -> Optional[Dict[str, Any]]:
         """Get information of about users of a project
 
         API endpoint: GET /projects/usedBy/{id}
 
         :param project_id: the id of the project to be requested
@@ -482,22 +473,20 @@
 
         project_details = {}
         project_details["version"] = new_version
         # force clearing state to OPEN
         project_details["clearingState"] = "OPEN"
 
         url = self.url + "resource/api/projects/duplicate/" + project_id
-        response = requests.post(
-            url, json=project_details, headers=self.api_headers
-        )
-
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_post(
+            url, json=project_details)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def update_project_release_relationship(
         self, project_id: str, release_id: str, new_state: str,
             new_relation: str, comment: str) -> Optional[Dict[str, Any]]:
         """Update the relationship for a specific release of a project
 
         API endpoint PATCH /projects/{pid}/release{rid}
@@ -524,13 +513,8 @@
 
         relation = {}
         relation["releaseRelation"] = new_relation
         relation["mainlineState"] = new_state
         relation["comment"] = comment
 
         url = self.url + "resource/api/projects/" + project_id + "/release/" + release_id
-        response = requests.patch(url, json=relation, headers=self.api_headers)
-
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        return self.api_patch(url, json=relation)
```

### Comparing `sw360-1.4.1/sw360/releases.py` & `sw360-1.5.0/sw360/releases.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 from typing import Any, Dict, List, Optional
 
-import requests
-
 from .base import BaseMixin
 from .sw360error import SW360Error
 
 
 class ReleasesMixin(BaseMixin):
     def get_release(self, release_id: str) -> Optional[Dict[str, Any]]:
         """Get information of about a release
@@ -151,21 +149,20 @@
         """
 
         for param in "name", "version":
             release_details[param] = locals()[param]
         release_details["componentId"] = component_id
 
         url = self.url + "resource/api/releases"
-        response = requests.post(
-            url, json=release_details, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_post(
+            url, json=release_details)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def update_release(self, release: Dict[str, Any], release_id: str) -> Optional[Dict[str, Any]]:
         """Update an existing release
 
         API endpoint: PATCH /releases
 
         :param release: the new release data
@@ -177,19 +174,15 @@
         :raises SW360Error: if there is a negative HTTP response
         """
 
         if not release_id:
             raise SW360Error(message="No release id provided!")
 
         url = self.url + "resource/api/releases/" + release_id
-        response = requests.patch(url, json=release, headers=self.api_headers)
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        return self.api_patch(url, json=release)
 
     def update_release_external_id(self, ext_id_name: str, ext_id_value: str,
                                    release_id: str, update_mode: str = "none") -> Optional[Dict[str, Any]]:
         """Set or update external id of a release. If the id is already set, it
         will only be changed if `update_mode=="overwrite"`. The id can be
         deleted using `update_mode=="delete"`.
 
@@ -233,21 +226,19 @@
         :raises SW360Error: if there is a negative HTTP response
         """
 
         if not release_id:
             raise SW360Error(message="No release id provided!")
 
         url = self.url + "resource/api/releases/" + release_id
-        response = requests.delete(
-            url, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        response = self.api_delete(url)
+        if response is not None:
+            if response.ok:
+                return response.json()
+        return None
 
     def get_users_of_release(self, release_id: str) -> Optional[Dict[str, Any]]:
         """Get information of about the users of a release
 
         API endpoint: GET /releases/usedBy/{id}
 
         :param release_id: the id of the release to be requested
```

### Comparing `sw360-1.4.1/sw360/sw360_api.py` & `sw360-1.5.0/sw360/sw360_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,39 @@
 # -------------------------------------------------------------------------------
 
 """Python interface to the Siemens SW360 platform"""
 
 from typing import Any, Dict, Optional
 
 import requests
+from requests.adapters import HTTPAdapter
+from urllib3.util.retry import Retry
 
 from .attachments import AttachmentsMixin
 from .clearing import ClearingMixin
 from .components import ComponentsMixin
 from .license import LicenseMixin
 from .project import ProjectMixin
 from .releases import ReleasesMixin
 from .sw360error import SW360Error
 from .vendor import VendorMixin
 from .vulnerabilities import VulnerabilitiesMixin
 
+# Retry mechanism for rate limiting
+adapter = HTTPAdapter(max_retries=Retry(
+    total=5,
+    status_forcelist=[429, 500, 502, 503, 504],
+    respect_retry_after_header=True,
+    backoff_factor=30,
+    allowed_methods=["HEAD", "GET", "OPTIONS", "POST", "PUT", "PATCH"]
+))
+session_default = requests.Session()
+session_default.mount("http://", adapter)
+session_default.mount("https://", adapter)
+
 
 class SW360(
     AttachmentsMixin,
     ClearingMixin,
     ComponentsMixin,
     LicenseMixin,
     ProjectMixin,
@@ -48,20 +62,26 @@
      "Authorization:" and `token_type`).
     :param oauth2: flag indicating whether this is an OAuth2 token
     :type url: string
     :type token: string
     :type oauth2: boolean
     """
 
-    def __init__(self, url: str, token: str, oauth2: bool = False) -> None:
+    def __init__(
+        self,
+        url: str,
+        token: str,
+        oauth2: bool = False,
+        session: Optional[requests.Session] = session_default
+    ) -> None:
         """Constructor"""
         if url[-1] != "/":
             url += "/"
         self.url: str = url
-        self.session: Optional[requests.Session] = None
+        self.session: Optional[requests.Session] = session
 
         if oauth2:
             self.api_headers = {"Authorization": "Bearer " + token}
         else:
             self.api_headers = {"Authorization": "Token " + token}
 
         self.force_no_session = False
@@ -71,15 +91,14 @@
         due to historic reasons which is ignored.
 
         You need to call this before any other method accessing SW360.
 
         :raises SW360Error: if the login fails
         """
         if not self.force_no_session:
-            self.session = requests.Session()
             self.session.headers = self.api_headers.copy()  # type: ignore
 
         url = self.url + "resource/api/"
         try:
             if self.force_no_session:
                 resp = requests.get(url, headers=self.api_headers)
             else:
```

### Comparing `sw360-1.4.1/sw360/sw360error.py` & `sw360-1.5.0/sw360/sw360error.py`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/sw360/sw360oauth2.py` & `sw360-1.5.0/sw360/sw360oauth2.py`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/sw360/vendor.py` & `sw360-1.5.0/sw360/vendor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
 from typing import Any, Dict, List, Optional
 
-import requests
-
 from .base import BaseMixin
 from .sw360error import SW360Error
 
 
 class VendorMixin(BaseMixin):
     def get_all_vendors(self) -> List[Dict[str, Any]]:
         """Returns all vendors
@@ -62,23 +60,22 @@
 
         :param vendor: the new vedor data
         :type vendor: JSON vendor object
         :raises SW360Error: if there is a negative HTTP response
         """
 
         url = self.url + "resource/api/vendors"
-        response = requests.post(
-            url, json=vendor, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
+        response = self.api_post(
+            url, json=vendor)
+        if response is not None:
+            if response.ok:
+                return response.json()
         raise SW360Error(response, url)
 
-    def update_vendor(self, vendor: Dict[str, Any], vendor_id: str) -> Dict[str, Any]:
+    def update_vendor(self, vendor: Dict[str, Any], vendor_id: str) -> Optional[Dict[str, Any]]:
         """Update an existing vendor
 
         API endpoint: PATCH /vendors
 
         :param vendor_id: the id of the vendor to be updated
         :type vendor_id: string
         :raises SW360Error: if there is a negative HTTP response
@@ -86,21 +83,15 @@
 
         # 2019-04-03: error 405 - not allowed
 
         if not vendor_id:
             raise SW360Error(message="No vendor id provided!")
 
         url = self.url + "resource/api/vendors/" + vendor_id
-        response = requests.patch(
-            url, json=vendor, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
-
-        raise SW360Error(response, url)
+        return self.api_patch(url, json=vendor)
 
     def delete_vendor(self, vendor_id: str) -> Dict[str, Any]:
         """Delete an existing vendor
 
         API endpoint: DELETE /vendors
 
         :param vendor_id: the id of the vendor
@@ -110,14 +101,13 @@
 
         # 2019-04-03: error 405 - not allowed
 
         if not vendor_id:
             raise SW360Error(message="No vendor id provided!")
 
         url = self.url + "resource/api/vendors/" + vendor_id
-        response = requests.delete(
-            url, headers=self.api_headers
-        )
-        if response.ok:
-            return response.json()
 
+        response = self.api_delete(url)
+        if response is not None:
+            if response.ok:
+                return response.json()
         raise SW360Error(response, url)
```

### Comparing `sw360-1.4.1/sw360/vulnerabilities.py` & `sw360-1.5.0/sw360/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `sw360-1.4.1/PKG-INFO` & `sw360-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw360
-Version: 1.4.1
+Version: 1.5.0
 Summary: Python interface to the SW360 software component catalogue
 Home-page: https://github.com/sw360/sw360python
 License: MIT
 Author: Thomas Graf
 Author-email: thomas.graf@siemens.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

