# Comparing `tmp/tenzir_platform-0.3.2.tar.gz` & `tmp/tenzir_platform-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenzir_platform-0.3.2.tar", max compression
+gzip compressed data, was "tenzir_platform-0.4.1.tar", max compression
```

## Comparing `tenzir_platform-0.3.2.tar` & `tenzir_platform-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/README.md
--rw-r--r--   0        0        0      878 2024-04-17 10:01:10.615745 tenzir_platform-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/auth_rule.py
--rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/cache.py
--rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/helpers/client.py
--rw-r--r--   0        0        0      818 2024-04-17 10:00:10.402949 tenzir_platform-0.3.2/tenzir_platform/helpers/environment.py
--rw-r--r--   0        0        0     5908 2024-04-17 09:59:52.870718 tenzir_platform-0.3.2/tenzir_platform/helpers/oidc.py
--rw-r--r--   0        0        0     6232 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/subcommand_admin.py
--rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.3.2/tenzir_platform/subcommand_auth.py
--rw-r--r--   0        0        0     5654 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/subcommand_node.py
--rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.3.2/tenzir_platform/subcommand_workspace.py
--rw-r--r--   0        0        0     1787 2024-04-15 11:26:22.401320 tenzir_platform-0.3.2/tenzir_platform/tenzir_platform.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.4.1/README.md
+-rw-r--r--   0        0        0      878 2024-04-19 16:42:32.082211 tenzir_platform-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.4.1/tenzir_platform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.4.1/tenzir_platform/helpers/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.4.1/tenzir_platform/helpers/auth_rule.py
+-rw-r--r--   0        0        0     1258 2024-04-18 15:13:51.338589 tenzir_platform-0.4.1/tenzir_platform/helpers/cache.py
+-rw-r--r--   0        0        0     3298 2024-04-18 15:13:51.338589 tenzir_platform-0.4.1/tenzir_platform/helpers/client.py
+-rw-r--r--   0        0        0      860 2024-04-18 15:13:51.338589 tenzir_platform-0.4.1/tenzir_platform/helpers/environment.py
+-rw-r--r--   0        0        0     5898 2024-04-19 16:42:32.082211 tenzir_platform-0.4.1/tenzir_platform/helpers/oidc.py
+-rw-r--r--   0        0        0     6230 2024-04-19 16:42:32.082211 tenzir_platform-0.4.1/tenzir_platform/subcommand_admin.py
+-rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.4.1/tenzir_platform/subcommand_auth.py
+-rw-r--r--   0        0        0     8134 2024-04-18 15:13:51.338589 tenzir_platform-0.4.1/tenzir_platform/subcommand_node.py
+-rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.4.1/tenzir_platform/subcommand_workspace.py
+-rw-r--r--   0        0        0     1787 2024-04-15 11:26:22.401320 tenzir_platform-0.4.1/tenzir_platform/tenzir_platform.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.4.1/PKG-INFO
```

### Comparing `tenzir_platform-0.3.2/pyproject.toml` & `tenzir_platform-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenzir-platform"
-version = "0.3.2"
+version = "0.4.1"
 description = "Tenzir CLI"
 authors = ["Tenzir <engineering@tenzir.com>"]
 readme = "README.md"
 packages = [{ include = "tenzir_platform" }]
 
 [tool.poetry.scripts]
 tenzir-platform = "tenzir_platform.tenzir_platform:main"
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/helpers/auth_rule.py` & `tenzir_platform-0.4.1/tenzir_platform/helpers/auth_rule.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.2/tenzir_platform/helpers/cache.py` & `tenzir_platform-0.4.1/tenzir_platform/helpers/cache.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,20 +14,22 @@
         + filename
     )
 
 
 def store_workspace(platform: PlatformEnvironment, workspace_id: str, user_key: str):
     content = json.dumps({"workspace_id": workspace_id, "user_key": user_key})
     filename = filename_in_cache(platform, "workspace")
-    print(f"saving workspace id to {filename}")
+    if platform.verbose:
+        print(f"saving workspace id to {filename}")
     os.makedirs(os.path.dirname(filename), exist_ok=True)
     with open(filename, "w") as f:
         f.write(content)
 
 
 def load_current_workspace(platform: PlatformEnvironment) -> tuple[str, str]:
     filename = filename_in_cache(platform, "workspace")
     with open(filename, "r") as f:
         content_str = f.read().rstrip()
         content = json.loads(content_str)
-        print(f"loaded workspace from {filename}")
+        if platform.verbose:
+            print(f"loaded workspace from {filename}")
         return content["workspace_id"], content["user_key"]
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/helpers/client.py` & `tenzir_platform-0.4.1/tenzir_platform/helpers/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     ADMIN = "admin"
 
 
 class AppClient:
     def __init__(
         self,
         platform: PlatformEnvironment,
-        verbose: bool = False,
     ) -> None:
-        self.verbose = verbose
+        self.verbose = platform.verbose
         self.id_token: str = UNAUTHENTICATED
         self.user_key: str = UNAUTHENTICATED
         self.endpoint_prefix = platform.api_endpoint.rstrip("/")
 
     def user_login(self, id_token: str):
         self.id_token = id_token
 
@@ -60,17 +59,20 @@
                     self.id_token != UNAUTHENTICATED
                 ), "missing user_login() before making admin api requests"
                 headers = {"X-Tenzir-AdminKey": self.id_token}
                 endpoint = self.endpoint_prefix + "/admin"
 
         for i in range(connection_retry + 1):
             try:
+                url = f"{endpoint}/{endpoint_suffix}"
+                if self.verbose:
+                    print(f"{method} {url}")
                 resp = requests.request(
                     method=method,
-                    url=f"{endpoint}/{endpoint_suffix}",
+                    url=url,
                     json=json,
                     headers=headers,
                 )
             except requests.exceptions.ConnectionError:
                 if i == connection_retry:
                     raise
                 print(f"connection error, retrying in 3s...")
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/helpers/environment.py` & `tenzir_platform-0.4.1/tenzir_platform/helpers/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from pydantic_settings import BaseSettings
 
 
 API_ENDPOINT = "https://rest.tenzir.app/production-v1"
-OIDC_ISSUER_URL = "https://tenzir.eu.auth0.com/"
-OIDC_CLIENT_ID = "vzRh8grIVu1bwutvZbbpBDCOvSzN8AXh"
+ISSUER_URL = "https://tenzir.eu.auth0.com/"
+CLIENT_ID = "vzRh8grIVu1bwutvZbbpBDCOvSzN8AXh"
 
 
 class PlatformEnvironment(BaseSettings):
     # The remote API endpoint of the platform.
     api_endpoint: str = API_ENDPOINT
 
     # An arbitrary short string to identify this environment
     # in the local cache directory.
     stage_identifier: str = "prod"
 
     # TODO: Provide a new `/oidc-config` endpoint in the public platform api
     # to load these values dynamically.
-    oidc_issuer_url: str = OIDC_ISSUER_URL
-    oidc_client_id: str = OIDC_CLIENT_ID
+    issuer_url: str = ISSUER_URL
+    client_id: str = CLIENT_ID
+
+    # Enable more verbose print statements.
+    verbose: bool = False
 
     @staticmethod
     def load():
         return PlatformEnvironment(
-            _env_prefix="TENZIR_PLATFORM_CLI", _env_nested_delimiter="__"
+            _env_prefix="TENZIR_PLATFORM_CLI_", _env_nested_delimiter="__"
         )
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/helpers/oidc.py` & `tenzir_platform-0.4.1/tenzir_platform/helpers/oidc.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     def __str__(self) -> str:
         return self._raw_oidc.__str__()
 
 
 class IdTokenClient:
     def __init__(self, platform: PlatformEnvironment):
         self.platform_environment = platform
-        self.issuer = platform.oidc_issuer_url
-        self.client_id = platform.oidc_client_id
+        self.issuer = platform.issuer_url
+        self.client_id = platform.client_id
         self.verbose = False
         discovery_url = f"{self.issuer.rstrip('/')}/.well-known/openid-configuration"
         discovered_configuration = requests.get(discovery_url).json()
         self.jwks_url = discovered_configuration["jwks_uri"]
         self.token_endpoint = discovered_configuration["token_endpoint"]
         self.device_authorization_endpoint = discovered_configuration[
             "device_authorization_endpoint"
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/subcommand_admin.py` & `tenzir_platform-0.4.1/tenzir_platform/subcommand_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from docopt import docopt
 
 
 def add_auth_rule(client: AppClient, workspace_id: str, rule: AuthRule):
     resp = client.post(
         "add-auth-function",
         target_api=TargetApi.ADMIN,
-        json={"tenant_id": workspace_id, "auth_rule": rule.model_dump()},
+        json={"tenant_id": workspace_id, "auth_fn": rule.model_dump()},
     )
     resp.raise_for_status()
     print(f"Added {rule.model_dump_json()}")
 
 
 def delete_auth_rule(client: AppClient, workspace_id: str, index: int):
     resp = client.post(
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/subcommand_auth.py` & `tenzir_platform-0.4.1/tenzir_platform/subcommand_auth.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.2/tenzir_platform/subcommand_node.py` & `tenzir_platform-0.4.1/tenzir_platform/subcommand_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,102 @@
 """Usage:
   tenzir-platform node list
-  tenzir-platform node ping <node_id>
+  tenzir-platform node ping <node>
   tenzir-platform node create [--name=<node_name>]
-  tenzir-platform node delete <node_id>
+  tenzir-platform node config <node> [-o filename] [--format=docker|tenzir|tenzir-node]
+  tenzir-platform node delete <node>
   tenzir-platform node run [--name=<node_name>] [--image=<container_image>]
 
 Options:
   --name=<node_name>         The name of the newly created node [default: CLI_Node]
   --image=<container_image>  The docker image to use for the newly created node
+  -o,--output=<filename>     Where to write the config file.
+  --format=<config_type>       The format of the downloaded config file. [default: docker]
 
 Description:
   tenzir-platform node list
     Display a list of all nodes in the current workspace.
 
   tenzir-platform node ping
     Send a ping request to a node and measure the response time.
 
+  tenzir-platform node create
+    Create a new node.
+
+  tenzir-platform node config <node> [-o filename] [--format=docker|tenzir|tenzir-node]
+    Download the configuration for an existing node.
+
+  tenzir-platform node delete <node>
+    Delete the specified node.
+
   tenzir-platform node run
     Create a new temporary node and run it in a local 'docker compose' stack.
     A new node is created in the currently selected workspace.
     The node is deleted when the command is interrupted.
     Requires the 'docker compose' binary in the current PATH.
 """
 
 from tenzir_platform.helpers.cache import load_current_workspace
 from tenzir_platform.helpers.client import AppClient
 from tenzir_platform.helpers.environment import PlatformEnvironment
 from pydantic import BaseModel
 from docopt import docopt
-from typing import Optional
+from typing import Optional, List
 import json
 import time
 import tempfile
 import os
 import subprocess
 import re
 import random
 import datetime
 
 
-def list(client: AppClient, workspace_id: str):
+def _is_node_id(identifier: str):
+    return bool(re.match(r"^n-[a-z0-9]{8}$", identifier))
+
+
+def _get_node_list(client: AppClient, workspace_id: str) -> List:
     resp = client.post(
-        "/list-nodes",
+        "list-nodes",
         json={
             "tenant_id": workspace_id,
         },
     )
     resp.raise_for_status()
-    for i, node in enumerate(resp.json()["nodes"]):
+    return resp.json()["nodes"]
+
+
+def _resolve_node_identifier(
+    client: AppClient, workspace_id: str, identifier: str
+) -> str:
+    # If we already have a node id, use that.
+    if _is_node_id(identifier):
+        return identifier
+
+    # Otherwise go through the list of nodes and look for a matching name.
+    nodes = _get_node_list(client, workspace_id)
+    name_matched = [node for node in nodes if node["name"] == identifier]
+    if len(name_matched) == 0:
+        raise Exception(f"Unknown node {identifier}")
+    if len(name_matched) > 1:
+        matching_ids = [node["node_id"] for node in name_matched]
+        raise Exception(f"Ambigous name {identifier} is shared by nodes {matching_ids}")
+    return name_matched[0]
+
+
+def list(client: AppClient, workspace_id: str):
+    nodes = _get_node_list(client, workspace_id)
+    for i, node in enumerate(nodes):
         connection_symbol = "🟢" if node["lifecycle_state"] == "connected" else "🔴"
         print(f"{connection_symbol} {node['name']} ({node['node_id']})")
 
 
-def ping(client: AppClient, workspace_id: str, node_id: str):
+def ping(client: AppClient, workspace_id: str, node: str):
+    node_id = _resolve_node_identifier(client, workspace_id, node)
     start = time.time()
     resp = client.post(
         "proxy",
         json={
             "node_id": node_id,
             "tenant_id": workspace_id,
             "http": {
@@ -126,28 +166,56 @@
 def create(client: AppClient, workspace_id: str, node_name: Optional[str]):
     if node_name is None:
         time_suffix = datetime.datetime.now(datetime.timezone.utc).strftime(
             "%Y%m%dT%H%M%SZ"
         )
         node_name = f"node-{time_suffix}"
     resp = client.post(
-        "/generate-client-config",
+        "generate-client-config",
         json={
             "tenant_id": workspace_id,
             "config_type": "docker",
             "node_name": node_name,
         },
     )
     resp.raise_for_status()
     print(f"created node {resp.json()['node_id']}")
 
 
-def delete(client: AppClient, workspace_id: str, node_id: str):
+def config(
+    client: AppClient,
+    workspace_id: str,
+    node: str,
+    config_format: str,
+    output_file: Optional[str],
+):
+    node_id = _resolve_node_identifier(client, workspace_id, node)
+    resp = client.post(
+        "generate-client-config",
+        json={
+            "tenant_id": workspace_id,
+            "config_type": config_format,
+            "node_id": node_id,
+        },
+    )
+    resp.raise_for_status()
+    response_body = resp.json()
+    node_id = response_body["node_id"]
+    if output_file is None:
+        output_file = response_body["filename"]
+    with open(output_file, "w") as f:
+        contents = response_body["contents"]
+        f.write(contents)
+    print(f"wrote config for node {node_id} to file {output_file}")
+
+
+def delete(client: AppClient, workspace_id: str, node: str):
+    node_id = _resolve_node_identifier(client, workspace_id, node)
     resp = client.post(
-        "/delete-node",
+        "delete-node",
         json={
             "tenant_id": workspace_id,
             "node_id": node_id,
         },
     )
     resp.raise_for_status()
     print(f"deleted node {node_id}")
@@ -165,19 +233,24 @@
             "Failed to load current workspace, please run 'tenzir-platform workspace select' first"
         )
         exit(1)
 
     if args["list"]:
         list(client, workspace_id)
     elif args["ping"]:
-        node_id = args["<node_id>"]
-        ping(client, workspace_id, node_id)
+        node = args["<node>"]
+        ping(client, workspace_id, node)
     elif args["run"]:
         node_name = args["--name"]
         container_image = args["--image"]
         run(client, workspace_id, node_name, container_image)
     elif args["create"]:
         node_name = args["--name"]
         create(client, workspace_id, node_name)
+    elif args["config"]:
+        node = args["<node>"]
+        format_ = args["--format"]
+        output = args["--output"]
+        config(client, workspace_id, node, format_, output)
     elif args["delete"]:
-        node_id = args["<node_id>"]
-        delete(client, workspace_id, node_id)
+        node = args["<node>"]
+        delete(client, workspace_id, node)
```

### Comparing `tenzir_platform-0.3.2/tenzir_platform/subcommand_workspace.py` & `tenzir_platform-0.4.1/tenzir_platform/subcommand_workspace.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.2/tenzir_platform/tenzir_platform.py` & `tenzir_platform-0.4.1/tenzir_platform/tenzir_platform.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.3.2/PKG-INFO` & `tenzir_platform-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenzir-platform
-Version: 0.3.2
+Version: 0.4.1
 Summary: Tenzir CLI
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

