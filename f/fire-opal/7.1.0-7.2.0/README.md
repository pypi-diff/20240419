# Comparing `tmp/fire_opal-7.1.0.tar.gz` & `tmp/fire_opal-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire_opal-7.1.0.tar", max compression
+gzip compressed data, was "fire_opal-7.2.0.tar", max compression
```

## Comparing `fire_opal-7.1.0.tar` & `fire_opal-7.2.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
--rw-r--r--   0        0        0    36587 2024-03-15 17:46:47.888403 fire_opal-7.1.0/LICENSE
--rw-r--r--   0        0        0      532 2024-03-15 17:46:47.888403 fire_opal-7.1.0/README.md
--rw-r--r--   0        0        0     1528 2024-03-15 17:47:12.596505 fire_opal-7.1.0/fireopal/__init__.py
--rw-r--r--   0        0        0    11489 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/_event_tracker.py
--rw-r--r--   0        0        0     2129 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/_utils.py
--rw-r--r--   0        0        0      705 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/admin.py
--rw-r--r--   0        0        0     4633 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/config.py
--rw-r--r--   0        0        0      947 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/constants.py
--rw-r--r--   0        0        0      909 2024-03-15 17:47:12.596505 fire_opal-7.1.0/fireopal/credentials/__init__.py
--rw-r--r--   0        0        0     3918 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/credentials/_credentials.py
--rw-r--r--   0        0        0     1060 2024-03-15 17:47:12.600505 fire_opal-7.1.0/fireopal/functions/__init__.py
--rw-r--r--   0        0        0     6875 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/activity_monitor.py
--rw-r--r--   0        0        0     2620 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/authenticate.py
--rw-r--r--   0        0        0     1058 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/base.py
--rw-r--r--   0        0        0     1494 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/benchmark.py
--rw-r--r--   0        0        0     2385 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/create_calibration_data.py
--rw-r--r--   0        0        0     1410 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/create_mitigation_data.py
--rw-r--r--   0        0        0     7004 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/execute.py
--rw-r--r--   0        0        0     2265 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/get_result.py
--rw-r--r--   0        0        0     1140 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/read_data.py
--rw-r--r--   0        0        0     1178 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/show_supported_devices.py
--rw-r--r--   0        0        0     3414 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/solve_qaoa.py
--rw-r--r--   0        0        0     1786 2024-03-15 17:46:47.888403 fire_opal-7.1.0/fireopal/functions/validate.py
--rw-r--r--   0        0        0     2931 2024-03-15 17:47:12.584505 fire_opal-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 fire_opal-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-04-18 23:43:46.772082 fire_opal-7.2.0/LICENSE
+-rw-r--r--   0        0        0      532 2024-04-18 23:43:46.772082 fire_opal-7.2.0/README.md
+-rw-r--r--   0        0        0     1335 2024-04-18 23:44:11.760151 fire_opal-7.2.0/fireopal/__init__.py
+-rw-r--r--   0        0        0    11489 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/_event_tracker.py
+-rw-r--r--   0        0        0     2129 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/_utils.py
+-rw-r--r--   0        0        0      624 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/admin.py
+-rw-r--r--   0        0        0     4718 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/config.py
+-rw-r--r--   0        0        0     1198 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/constants.py
+-rw-r--r--   0        0        0      909 2024-04-18 23:44:11.760151 fire_opal-7.2.0/fireopal/credentials/__init__.py
+-rw-r--r--   0        0        0     3840 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/credentials/_credentials.py
+-rw-r--r--   0        0        0      907 2024-04-18 23:44:11.756151 fire_opal-7.2.0/fireopal/functions/__init__.py
+-rw-r--r--   0        0        0     6800 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/activity_monitor.py
+-rw-r--r--   0        0        0     2686 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/authenticate.py
+-rw-r--r--   0        0        0     1058 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/base.py
+-rw-r--r--   0        0        0     7004 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/execute.py
+-rw-r--r--   0        0        0     2252 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/get_result.py
+-rw-r--r--   0        0        0     1106 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/read_data.py
+-rw-r--r--   0        0        0     1163 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/show_supported_devices.py
+-rw-r--r--   0        0        0     3414 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/solve_qaoa.py
+-rw-r--r--   0        0        0     1754 2024-04-18 23:43:46.772082 fire_opal-7.2.0/fireopal/functions/validate.py
+-rw-r--r--   0        0        0     2966 2024-04-18 23:44:11.752151 fire_opal-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2612 1970-01-01 00:00:00.000000 fire_opal-7.2.0/PKG-INFO
```

### Comparing `fire_opal-7.1.0/LICENSE` & `fire_opal-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/README.md` & `fire_opal-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/_event_tracker.py` & `fire_opal-7.2.0/fireopal/_event_tracker.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/_utils.py` & `fire_opal-7.2.0/fireopal/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 # once support for Primitives V1 is dropped.
 PACKAGE_NAMES = [
     # External packages.
     "matplotlib",
     "networkx",
     "numpy",
     "qiskit",
-    "qiskit-ibm-provider",
-    "qiskit-ibm-runtime",
+    "qiskit_ibm_provider",
+    "qiskit_ibm_runtime",
     "sympy",
     # Q-CTRL packages.
     "fireopal",
     "qctrlvisualizer",
     "qctrlworkflowclient",
 ]
```

### Comparing `fire_opal-7.1.0/fireopal/config.py` & `fire_opal-7.2.0/fireopal/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,30 @@
 from qctrlworkflowclient.defaults import CliAuth
 from qctrlworkflowclient.globals import global_value
 
 from .constants import (
     API_KEY_NAME,
     FIRE_OPAL_USER_ROLE,
     INVALID_SUBSCRIPTION_ERROR,
+    PACKAGE_INFO,
 )
 
 
 def get_default_router() -> ApiRouter:
     """Returns the default router that the Fire Opal
     client uses.
     """
     api_key = os.getenv(API_KEY_NAME)
     if api_key:
         auth = get_default_api_key_auth(api_key)
     else:
         auth = get_default_cli_auth()
     client = get_authenticated_client_for_product(
         FIRE_OPAL_USER_ROLE,
+        PACKAGE_INFO.install_name,
         get_default_api_url(),
         auth,
         INVALID_SUBSCRIPTION_ERROR,
     )
     settings = get_config()
     return ApiRouter(client, settings)
 
@@ -121,15 +123,16 @@
     ----------
     api_url : str
         URL of the GraphQL schema
     oidc_url : str
         Base URL of the OIDC provider, for example Keycloak.
     """
     client = get_authenticated_client_for_product(
-        "fire-opal-cli-access",
+        FIRE_OPAL_USER_ROLE,
+        PACKAGE_INFO.install_name,
         api_url,
         CliAuth(oidc_url),
         INVALID_SUBSCRIPTION_ERROR,
     )
     settings = get_config()
 
     configure(router=ApiRouter(client, settings))
```

### Comparing `fire_opal-7.1.0/fireopal/constants.py` & `fire_opal-7.2.0/fireopal/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,10 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-INVALID_SUBSCRIPTION_ERROR = """
----------------------------------------------------------------------
-Your authentication succeeded, but your subscription is invalid for
-this product.
+# pylint:disable=unused-import
 
-Please access `https://fire.q-ctrl.com` for more details.
----------------------------------------------------------------------
-"""
-
-FIRE_OPAL_USER_ROLE = "fire-opal-cli-access"
-
-API_KEY_NAME = "QCTRL_API_KEY"
+from .functions import read_data  # noqa
```

### Comparing `fire_opal-7.1.0/fireopal/credentials/__init__.py` & `fire_opal-7.2.0/fireopal/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/credentials/_credentials.py` & `fire_opal-7.2.0/fireopal/credentials/_credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,15 @@
     _get_user_payload,
 )
 
 Credentials = Dict[str, str]
 
 
 def make_credentials_for_ibmq(
-    token: str,
-    group: str,
-    hub: str,
-    project: str,
+    token: str, group: str, hub: str, project: str
 ) -> Credentials:
     """
     Make a Credentials dictionary for IBM Quantum.
 
     Parameters
     ----------
     token : str
@@ -66,18 +63,15 @@
         "group": group,
         "hub": hub,
         "project": project,
         "provider": "ibmq",
     }
 
 
-def make_credentials_for_ibm_cloud(
-    token: str,
-    instance: str,
-) -> Credentials:
+def make_credentials_for_ibm_cloud(token: str, instance: str) -> Credentials:
     """
     The Credentials builder for IBM cloud devices.
 
     Parameters
     ----------
     token : str
         The IBM API account token.
@@ -90,19 +84,15 @@
         A dictionary usable for the `credentials`
         argument of any Fire Opal function using IBM Cloud.
     """
     if _check_for_remote_router():
         user_traits = UserTraits(_get_user_payload())
         _EVENT_TRACKER.track_make_credentials_for_ibm_cloud(user_traits=user_traits)
     _check_all_strings(token=token, instance=instance)
-    return {
-        "token": token,
-        "instance": instance,
-        "provider": "ibm_cloud",
-    }
+    return {"token": token, "instance": instance, "provider": "ibm_cloud"}
 
 
 def make_credentials_for_braket(arn: str) -> Credentials:
     """
     Make a Credentials dictionary for Braket.
 
     Parameters
@@ -121,18 +111,15 @@
     Notes
     -----
     This function performs only basic type checking of
     the credentials it receives. It does not check whether
     the credentials are valid for hardware access.
     """
     _check_all_strings(arn=arn)
-    return {
-        "arn": arn,
-        "provider": "braket",
-    }
+    return {"arn": arn, "provider": "braket"}
 
 
 def _check_all_strings(**kwargs: str) -> None:
     """
     Check whether all arguments are strings.
 
     Raises
```

### Comparing `fire_opal-7.1.0/fireopal/functions/__init__.py` & `fire_opal-7.2.0/fireopal/functions/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,13 @@
 # License for the specific language.
 
 from .activity_monitor import (
     activity_monitor,
     get_action_metadata,
 )
 from .authenticate import authenticate_qctrl_account
-from .benchmark import benchmark
-from .create_calibration_data import create_calibration_data
-from .create_mitigation_data import create_mitigation_data
 from .execute import execute
 from .get_result import get_result
 from .read_data import read_data
 from .show_supported_devices import show_supported_devices
 from .solve_qaoa import solve_qaoa
 from .validate import validate
```

### Comparing `fire_opal-7.1.0/fireopal/functions/activity_monitor.py` & `fire_opal-7.2.0/fireopal/functions/activity_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,15 @@
         The number of recent actions to ignore before starting to print.
         Defaults to 0.
     status : str or None, optional
         The filter for action status. If None, fetches actions of all
         statuses. Defaults to None.
     """
     log_activity(
-        function_called="activity_monitor",
-        limit=limit,
-        offset=offset,
-        status=status,
+        function_called="activity_monitor", limit=limit, offset=offset, status=status
     )
 
     if _check_for_remote_router():
         user_traits = UserTraits(_get_user_payload())
         _EVENT_TRACKER.track_activity_monitor(
             user_traits=user_traits, limit=limit, offset=offset, status=status
         )
@@ -138,31 +135,27 @@
     -------
     list[ActionMetadata]
         Action metadata.
     """
     if limit > 50:
         logging.error("QCTRL - The limit cannot exceed 50.")
         raise QctrlArgumentsValueError(
-            "The limit cannot exceed 50.",
-            arguments={"limit": limit},
+            "The limit cannot exceed 50.", arguments={"limit": limit}
         )
     if status is None:
         print(
             "Getting jobs for all statuses. To filter jobs by status, ",
             "use the status keyword argument. Valid status values are: "
             f"{', '.join([status.value for status in ActionStatus])}.\n",
         )
     router: ApiRouter = get_config().get_router()
     if _check_for_remote_router():
         user_traits = UserTraits(_get_user_payload(router=router))
         _EVENT_TRACKER.track_get_action_metadata(
-            user_traits=user_traits,
-            limit=limit,
-            offset=offset,
-            status=status,
+            user_traits=user_traits, limit=limit, offset=offset, status=status
         )
 
     action_metadata: list[dict[str, Any]] = router.activity_monitor(
         limit, offset, status
     )
 
     # Filter to relevant fields.
```

### Comparing `fire_opal-7.1.0/fireopal/functions/authenticate.py` & `fire_opal-7.2.0/fireopal/functions/authenticate.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     get_config,
     get_default_api_key_auth,
 )
 from fireopal.constants import (
     API_KEY_NAME,
     FIRE_OPAL_USER_ROLE,
     INVALID_SUBSCRIPTION_ERROR,
+    PACKAGE_INFO,
 )
 
 
 def authenticate_qctrl_account(api_key: Optional[str] = None) -> None:
     """
     Authenticate a Fire Opal session.
 
@@ -60,14 +61,15 @@
     # whose internal GQL client uses browser-based authentication.
     settings = get_config()
 
     # Create a router that uses the global settings and an internal
     # client with token-based authentication.
     client = get_authenticated_client_for_product(
         product_access_required=FIRE_OPAL_USER_ROLE,
+        package_name=PACKAGE_INFO.install_name,
         api_url=_DEFAULT_API_URL,
         auth=api_key_auth,
         invalid_access_error_message=INVALID_SUBSCRIPTION_ERROR,
     )
     router = ApiRouter(client, settings)
 
     # Configure the global settings to use the router with token-based
```

### Comparing `fire_opal-7.1.0/fireopal/functions/base.py` & `fire_opal-7.2.0/fireopal/functions/base.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/functions/execute.py` & `fire_opal-7.2.0/fireopal/functions/execute.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/functions/get_result.py` & `fire_opal-7.2.0/fireopal/functions/get_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,16 +50,15 @@
         will be the same as that of the result returned
         from the function that was previously called
         to create this action.
     """
     if not str(action_id).isnumeric():
         logging.error("QCTRL - The action ID must be an integer.")
         raise QctrlArgumentsValueError(
-            "The action ID must be an integer.",
-            arguments={"action_id": action_id},
+            "The action ID must be an integer.", arguments={"action_id": action_id}
         )
     router: ApiRouter = get_config().get_router()
 
     action = Action(action_id=str(action_id))
     decoded_result = router.get_result(action).decoded
     assert isinstance(decoded_result, dict)
```

### Comparing `fire_opal-7.1.0/fireopal/functions/read_data.py` & `fire_opal-7.2.0/fireopal/functions/read_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 
 from typing import Dict
 
 from .base import fire_opal_workflow
 
 
 @fire_opal_workflow("read_database_workflow")
-def read_data(
-    ibm_device_name: str,
-    entry: str,
-) -> Dict:
+def read_data(ibm_device_name: str, entry: str) -> Dict:
     """
     Reads an entry from the Fire Opal database.
 
     Parameters
     ----------
     ibm_device_name : str
         The name of the ibm device associated with the desired data.
@@ -32,11 +29,8 @@
         The database entry label.
 
     Returns
     -------
     Dict
         The output of the read database workflow.
     """
-    return {
-        "ibm_device_name": ibm_device_name,
-        "entry": entry,
-    }
+    return {"ibm_device_name": ibm_device_name, "entry": entry}
```

### Comparing `fire_opal-7.1.0/fireopal/functions/show_supported_devices.py` & `fire_opal-7.2.0/fireopal/functions/show_supported_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,10 +28,8 @@
         for functions to generate credentials for your desired provider.
 
     Returns
     -------
     dict
         The output of the show supported devices workflow.
     """
-    return {
-        "credentials": credentials,
-    }
+    return {"credentials": credentials}
```

### Comparing `fire_opal-7.1.0/fireopal/functions/solve_qaoa.py` & `fire_opal-7.2.0/fireopal/functions/solve_qaoa.py`

 * *Files identical despite different names*

### Comparing `fire_opal-7.1.0/fireopal/functions/validate.py` & `fire_opal-7.2.0/fireopal/functions/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 from fireopal._utils import log_activity
 from fireopal.credentials import Credentials
 
 from .base import fire_opal_workflow
 
 
 @fire_opal_workflow("validate_input_circuits_workflow")
-def validate(
-    circuits: list[str],
-    credentials: Credentials,
-    backend_name: str,
-) -> dict:
+def validate(circuits: list[str], credentials: Credentials, backend_name: str) -> dict:
     """
     Validate the compatibility of a batch of circuits for Fire Opal.
 
     Parameters
     ----------
     circuits : list[str]
         A list of quantum circuit in the form QASM string. You can use Qiskit to
@@ -41,17 +37,15 @@
 
     Returns
     -------
     dict
         The output of the validate workflow.
     """
     log_activity(
-        function_called="validate",
-        circuits=circuits,
-        backend_name=backend_name,
+        function_called="validate", circuits=circuits, backend_name=backend_name
     )
 
     return {
         "circuits": circuits,
         "credentials": credentials,
         "backend_name": backend_name,
     }
```

### Comparing `fire_opal-7.1.0/pyproject.toml` & `fire_opal-7.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fire-opal"
-version = "7.1.0"
+version = "7.2.0"
 description = "Fire Opal Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com/fire-opal"
@@ -74,33 +74,34 @@
 name = "Q-CTRL PyPI"
 url = "https://pypi.q-ctrl.com/simple"
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 qctrl-commons = { version = "^22.0.0", source = "PyPI" }
-qctrl-workflow-client = { version = "^2.3.1", source = "PyPI" }
+qctrl-workflow-client = { version = "~3.0.0", source = "PyPI" }
 segment-analytics-python = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = "^24.3.0"
 isort = "^5.12.0"
 autoflake = "2.2.0"
 mypy = "^1.4.1"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.11.1"
 pylint = "^2.17.5"
 pylint_runner = "^0.6.0"
 pre-commit = "^3.3.3"
 tomli = "^2.0.1"
 qctrl-core-workflow-manager = "^3.0.0"
 qctrl-client = { version = "9.1.0", source = "PyPI" }
 qctrl-sphinx-theme = "^2.1.4"
 sphinx = "^5.3.0"
+sphinx-markdown-builder = "^0.6.6"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = "2"
 
 [tool.pytest.ini_options]
 addopts = "--cov=fireopal --cov-fail-under=90 --cov-report=term-missing:skip-covered"
```

### Comparing `fire_opal-7.1.0/PKG-INFO` & `fire_opal-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fire-opal
-Version: 7.1.0
+Version: 7.2.0
 Summary: Fire Opal Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: qctrl-commons (>=22.0.0,<23.0.0)
-Requires-Dist: qctrl-workflow-client (>=2.3.1,<3.0.0)
+Requires-Dist: qctrl-workflow-client (>=3.0.0,<3.1.0)
 Requires-Dist: segment-analytics-python (>=2.2.2,<3.0.0)
 Project-URL: Documentation, https://docs.q-ctrl.com/fire-opal
 Project-URL: Facebook, https://www.facebook.com/qctrl
 Project-URL: GitHub, https://github.com/qctrl
 Project-URL: LinkedIn, https://www.linkedin.com/company/q-ctrl/
 Project-URL: Twitter, https://twitter.com/qctrlHQ
 Project-URL: YouTube, https://www.youtube.com/qctrl
```

