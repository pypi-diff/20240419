# Comparing `tmp/pictorus-0.2.3.tar.gz` & `tmp/pictorus-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.2.3.tar", last modified: Fri Apr  5 23:52:04 2024, max compression
+gzip compressed data, was "pictorus-0.2.4.tar", last modified: Fri Apr 19 20:13:43 2024, max compression
```

## Comparing `pictorus-0.2.3.tar` & `pictorus-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0       31 2024-02-05 17:27:18.447001 pictorus-0.2.3/.flake8
--rw-r--r--   0        0        0     1358 2024-02-15 20:20:41.417522 pictorus-0.2.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.2.3/.gitignore
--rw-r--r--   0        0        0      987 2024-02-15 20:20:41.417758 pictorus-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.2.3/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.2.3/LICENSE
--rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.2.3/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.2.3/README.md
--rw-r--r--   0        0        0     1228 2024-02-15 20:20:41.418116 pictorus-0.2.3/pyproject.toml
--rwxr-xr-x   0        0        0      483 2024-02-15 20:20:41.418402 pictorus-0.2.3/script/setup
--rw-r--r--   0        0        0       61 2024-04-05 23:51:46.293614 pictorus-0.2.3/src/pictorus/__init__.py
--rw-r--r--   0        0        0    16894 2024-04-05 23:51:42.048910 pictorus-0.2.3/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     1995 2024-02-15 20:20:41.419443 pictorus-0.2.3/src/pictorus/command.py
--rw-r--r--   0        0        0     3614 2024-02-05 17:27:18.448390 pictorus-0.2.3/src/pictorus/config.py
--rw-r--r--   0        0        0      875 2024-02-15 20:20:41.419712 pictorus-0.2.3/src/pictorus/constants.py
--rw-r--r--   0        0        0      264 2024-02-15 20:20:41.419940 pictorus-0.2.3/src/pictorus/date_utils.py
--rw-r--r--   0        0        0     1945 2024-02-15 20:20:41.420191 pictorus-0.2.3/src/pictorus/embedded_target_manager.py
--rw-r--r--   0        0        0     6117 2024-04-02 20:10:52.936065 pictorus-0.2.3/src/pictorus/local_server.py
--rw-r--r--   0        0        0      244 2023-09-28 16:25:58.267963 pictorus-0.2.3/src/pictorus/logging_utils.py
--rw-r--r--   0        0        0     5578 2024-02-15 20:20:41.421375 pictorus-0.2.3/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0      695 2024-02-15 20:20:41.421617 pictorus-0.2.3/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     6786 2024-02-15 20:20:41.422156 pictorus-0.2.3/src/pictorus/proc_target_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.2.3/src/pictorus/systemd.py
--rw-r--r--   0        0        0     5097 2024-02-05 17:27:18.450570 pictorus-0.2.3/src/pictorus/target_manager.py
--rw-r--r--   0        0        0      577 2024-02-15 20:20:41.422410 pictorus-0.2.3/src/pictorus/target_state.py
--rw-r--r--   0        0        0     4704 2024-02-15 20:20:41.422916 pictorus-0.2.3/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3602 2024-02-15 20:20:41.423093 pictorus-0.2.3/src/pictorus/version_manager.py
--rw-r--r--   0        0        0        0 2023-09-28 16:25:58.268901 pictorus-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      347 2024-02-05 17:27:18.451098 pictorus-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-09-28 16:25:58.269155 pictorus-0.2.3/tests/pictorus/__init__.py
--rw-r--r--   0        0        0     7630 2024-02-28 21:05:41.097625 pictorus-0.2.3/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     4022 2024-02-05 17:27:18.451666 pictorus-0.2.3/tests/pictorus/test_embedded_target_manager.py
--rw-r--r--   0        0        0     5448 2024-02-05 17:27:18.452034 pictorus-0.2.3/tests/pictorus/test_local_server.py
--rw-r--r--   0        0        0     8176 2024-02-05 17:27:18.452295 pictorus-0.2.3/tests/pictorus/test_proc_target_manager.py
--rw-r--r--   0        0        0     2758 2024-01-09 22:24:36.010715 pictorus-0.2.3/tests/pictorus/test_telemetry_manager.py
--rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.2.3/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1400 2024-02-05 17:27:18.452565 pictorus-0.2.3/tests/utils.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 pictorus-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       31 2024-02-05 17:27:18.447001 pictorus-0.2.4/.flake8
+-rw-r--r--   0        0        0     1358 2024-02-15 20:20:41.417522 pictorus-0.2.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.2.4/.gitignore
+-rw-r--r--   0        0        0      987 2024-02-15 20:20:41.417758 pictorus-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.2.4/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.2.4/LICENSE
+-rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.2.4/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.2.4/README.md
+-rw-r--r--   0        0        0     1228 2024-04-15 21:04:12.704637 pictorus-0.2.4/pyproject.toml
+-rwxr-xr-x   0        0        0      483 2024-02-15 20:20:41.418402 pictorus-0.2.4/script/setup
+-rw-r--r--   0        0        0       61 2024-04-19 20:13:10.776219 pictorus-0.2.4/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    17089 2024-04-19 20:12:56.204676 pictorus-0.2.4/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     1995 2024-04-15 21:04:12.705696 pictorus-0.2.4/src/pictorus/command.py
+-rw-r--r--   0        0        0     3614 2024-02-05 17:27:18.448390 pictorus-0.2.4/src/pictorus/config.py
+-rw-r--r--   0        0        0      875 2024-02-15 20:20:41.419712 pictorus-0.2.4/src/pictorus/constants.py
+-rw-r--r--   0        0        0      264 2024-02-15 20:20:41.419940 pictorus-0.2.4/src/pictorus/date_utils.py
+-rw-r--r--   0        0        0     3718 2024-04-18 22:19:09.217018 pictorus-0.2.4/src/pictorus/embedded_target_manager.py
+-rw-r--r--   0        0        0      381 2024-04-18 22:19:09.217346 pictorus-0.2.4/src/pictorus/exceptions.py
+-rw-r--r--   0        0        0     6019 2024-04-18 22:19:09.217736 pictorus-0.2.4/src/pictorus/local_server.py
+-rw-r--r--   0        0        0      244 2023-09-28 16:25:58.267963 pictorus-0.2.4/src/pictorus/logging_utils.py
+-rw-r--r--   0        0        0     5578 2024-02-15 20:20:41.421375 pictorus-0.2.4/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0      695 2024-04-17 22:21:11.522305 pictorus-0.2.4/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     6808 2024-04-19 20:12:56.205345 pictorus-0.2.4/src/pictorus/proc_target_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.2.4/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     6603 2024-04-18 22:19:09.218374 pictorus-0.2.4/src/pictorus/target_manager.py
+-rw-r--r--   0        0        0      577 2024-02-15 20:20:41.422410 pictorus-0.2.4/src/pictorus/target_state.py
+-rw-r--r--   0        0        0     4704 2024-04-19 20:12:56.205638 pictorus-0.2.4/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     4758 2024-04-17 22:21:11.523211 pictorus-0.2.4/src/pictorus/updates_manager.py
+-rw-r--r--   0        0        0        0 2023-09-28 16:25:58.268901 pictorus-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      347 2024-02-05 17:27:18.451098 pictorus-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-09-28 16:25:58.269155 pictorus-0.2.4/tests/pictorus/__init__.py
+-rw-r--r--   0        0        0     7988 2024-04-17 22:21:11.523512 pictorus-0.2.4/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     6235 2024-04-17 22:21:11.523810 pictorus-0.2.4/tests/pictorus/test_embedded_target_manager.py
+-rw-r--r--   0        0        0     5448 2024-02-05 17:27:18.452034 pictorus-0.2.4/tests/pictorus/test_local_server.py
+-rw-r--r--   0        0        0     8454 2024-04-17 22:21:11.524168 pictorus-0.2.4/tests/pictorus/test_proc_target_manager.py
+-rw-r--r--   0        0        0     2758 2024-01-09 22:24:36.010715 pictorus-0.2.4/tests/pictorus/test_telemetry_manager.py
+-rw-r--r--   0        0        0     3985 2024-04-17 22:21:11.524407 pictorus-0.2.4/tests/pictorus/test_updates_manager.py
+-rw-r--r--   0        0        0     1510 2024-04-17 22:21:11.524631 pictorus-0.2.4/tests/utils.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 pictorus-0.2.4/PKG-INFO
```

### Comparing `pictorus-0.2.3/.github/workflows/test.yaml` & `pictorus-0.2.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/.gitignore` & `pictorus-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/.pre-commit-config.yaml` & `pictorus-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/LICENSE` & `pictorus-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/PUB_README.md` & `pictorus-0.2.4/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/README.md` & `pictorus-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/pyproject.toml` & `pictorus-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/app_manager.py` & `pictorus-0.2.4/src/pictorus/app_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,36 +10,34 @@
 from typing import Dict, Union
 
 import requests
 from awscrt import mqtt
 from awscrt.exceptions import AwsCrtError
 from awsiot import iotshadow, mqtt_connection_builder
 
+
 from . import __version__ as CURRENT_VERSION
-from .version_manager import VersionManager
+from .exceptions import TargetMissingError
+from .updates_manager import UpdatesManager
 from .config import load_app_manifest, store_app_manifest, Config
 from .logging_utils import get_logger
 from .command import Command, CmdType, DeployTarget, DeployTargetType
 from .target_state import TargetState
-from .target_manager import TargetManager
+from .target_manager import CommandCtxt, TargetManager
 from .proc_target_manager import ProcTargetManager
 from .embedded_target_manager import EmbeddedTargetManager
 from .constants import PICTORUS_SERVICE_NAME, THREAD_SLEEP_TIME_S
 from .local_server import create_server, COMMS
 
 logger = get_logger()
 config = Config()
 
 CONNECT_RETRY_TIMEOUT_S = 15
 
 
-class TargetMissingError(Exception):
-    pass
-
-
 def connect_mqtt(mqtt_connection: mqtt.Connection):
     connect_future = mqtt_connection.connect()
     while True:
         try:
             connect_future.result()
             break
         except AwsCrtError:
@@ -75,15 +73,15 @@
 
     TARGET_STATES_SHADOW_PROP = "target_states"
     RUN_APP_SHADOW_PROP = "run_app"
 
     CMD_REQUEST_SUBTOPIC = "req"
     RETAINED_CMD_SUBTOPIC = "ret"
 
-    def __init__(self, version_mgr: VersionManager):
+    def __init__(self, version_mgr: UpdatesManager):
         self._mqtt_connection = self._create_mqtt_connection()
         threading.Thread(target=connect_mqtt, args=(self._mqtt_connection,), daemon=True).start()
 
         self._version_manager = version_mgr
         self._shadow_client = iotshadow.IotShadowClient(self._mqtt_connection)
         self._last_published_shadow_state = None
 
@@ -362,15 +360,16 @@
 
         # First handle any commands that aren't target-specific
         if cmd.type == CmdType.UPLOAD_LOGS:
             self._upload_logs(cmd)
             return
 
         manager = self._get_target_manager(cmd, target=target)
-        manager.handle_command(cmd)
+        cmd_ctxt = CommandCtxt(cmd=cmd, updates_mgr=self._version_manager)
+        manager.handle_command(cmd_ctxt)
 
     def _on_retained_cmd(self, topic: str, payload: bytes):
         # This is an echo of the message we published to clear the retained message
         if not payload:
             return
 
         try:
@@ -392,14 +391,16 @@
 
         cmd_data = json.loads(payload)
         cmd = Command(cmd_data)
         target = DeployTarget(cmd_data["target"])
 
         try:
             self._process_cmd(cmd, target=target)
+        except Exception as e:
+            logger.error("Error processing command: %s", e, exc_info=True)
         finally:
             self._persist_changes()
 
     def _on_shadow_delta_updated(self, delta: iotshadow.ShadowDeltaUpdatedEvent):
         if not delta.state:
             return
```

### Comparing `pictorus-0.2.3/src/pictorus/command.py` & `pictorus-0.2.4/src/pictorus/command.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/config.py` & `pictorus-0.2.4/src/pictorus/config.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/constants.py` & `pictorus-0.2.4/src/pictorus/constants.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/local_server.py` & `pictorus-0.2.4/src/pictorus/local_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from functools import wraps
 import json
 import http.server
 import urllib.parse
 
 from jose import jwt
 
+
+from .exceptions import AuthenticationError
 from .config import Config
 from .constants import JWT_ALGORITHM, JWT_PUB_KEY
 from .command import CmdType
 from .date_utils import utc_timestamp_ms
 
 config = Config()
 
@@ -70,20 +72,14 @@
         self.reported_state = None
         self.commands = Queue()
 
 
 COMMS = ThreadComms()
 
 
-class AuthenticationError(Exception):
-    def __init__(self, message: str):
-        self.message = message
-        super().__init__(message)
-
-
 def authenticated(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         req = args[0]
         try:
             if "Authorization" not in req.headers:
                 raise AuthenticationError("Missing authorization header")
```

### Comparing `pictorus-0.2.3/src/pictorus/pictorus_cli.py` & `pictorus-0.2.4/src/pictorus/pictorus_cli.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/pictorus_device_manager.py` & `pictorus-0.2.4/src/pictorus/pictorus_device_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """ Daemon process for handling IoT interactions """
 import sys
 import os
 
 from pictorus.config import Config
 from pictorus.logging_utils import get_logger
 from pictorus.app_manager import AppManager
-from pictorus.version_manager import VersionManager
+from pictorus.updates_manager import UpdatesManager
 
 logger = get_logger()
 config = Config()
 
 
 def main():
     """Main run function"""
     log_level = os.environ.get("LOG_LEVEL", default="INFO").upper()
     logger.setLevel(log_level)
     logger.info("Starting device manager for device: %s", config.client_id)
 
-    with VersionManager() as version_mgr, AppManager(version_mgr) as app_mgr:
+    with UpdatesManager() as version_mgr, AppManager(version_mgr) as app_mgr:
         app_mgr.complete.wait()
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `pictorus-0.2.3/src/pictorus/proc_target_manager.py` & `pictorus-0.2.4/src/pictorus/proc_target_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Callable, Union
 
 from awscrt import mqtt
 
 from .target_state import TargetState
 from .config import Config
 from .logging_utils import get_logger
-from .target_manager import TargetManager
+from .target_manager import TargetManager, CommandCtxt
 from .telemetry_manager import TelemetryManager
-from .command import Command, DeployTarget
+from .command import DeployTarget
 from .constants import AppLogLevel, THREAD_SLEEP_TIME_S, EMPTY_ERROR
 
 config = Config()
 logger = get_logger()
 
 
 # Mocking os.path.exists directly on this module causes issues with requests
@@ -50,25 +50,23 @@
         self._app_watcher_thread.start()
 
     @property
     def app_is_running(self) -> bool:
         """Return whether the app is currently running"""
         return bool(self._pictorus_app_process)
 
-    def handle_update_app_cmd(self, cmd: Command):
-        self._download_app_files(cmd)
-
+    def _deploy_app(self, target: DeployTarget, cmd_ctxt: CommandCtxt):
         self._target_state.error_log = EMPTY_ERROR.copy()
         self._maybe_start_app()
 
-    def handle_set_ttl_cmd(self, cmd: Command):
-        self._telemetry_manager.set_ttl(cmd.data["ttl_s"])
+    def handle_set_ttl_cmd(self, cmd_ctxt: CommandCtxt):
+        self._telemetry_manager.set_ttl(cmd_ctxt.cmd.data["ttl_s"])
 
-    def handle_set_log_level_cmd(self, cmd: Command):
-        log_level = cmd.data["log_level"]
+    def handle_set_log_level_cmd(self, cmd_ctxt: CommandCtxt):
+        log_level = cmd_ctxt.cmd.data["log_level"]
         try:
             log_level = AppLogLevel(log_level)
         except ValueError:
             logger.warning("Received invalid log level: %s", log_level)
             return
 
         self._app_log_level = log_level
```

### Comparing `pictorus-0.2.3/src/pictorus/systemd.py` & `pictorus-0.2.4/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/target_manager.py` & `pictorus-0.2.4/src/pictorus/target_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 import os
 
 import requests
 
+
+from .exceptions import CommandError
+from .updates_manager import UpdatesManager
 from .config import APP_ASSETS_DIR
 from .target_state import TargetState
 from .command import Command, DeployTarget, DeployTargetType, CmdType
 from .logging_utils import get_logger
 from .local_server import COMMS
 
 logger = get_logger()
@@ -23,14 +26,27 @@
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     with requests.get(url, stream=True) as req, open(file_path, "wb") as in_file:
         req.raise_for_status()
         for chunk in req.iter_content(chunk_size=8192):
             in_file.write(chunk)
 
 
+class CommandCtxt:
+    def __init__(self, cmd: Command, updates_mgr: UpdatesManager) -> None:
+        self.cmd = cmd
+        self.updates_mgr = updates_mgr
+
+    def __eq__(self, __value: object) -> bool:
+        # Convenience method for tests. We only care about the command data for now
+        if not isinstance(__value, CommandCtxt):
+            return False
+
+        return self.cmd == __value.cmd
+
+
 class TargetManager(ABC):
     def __init__(self, target: DeployTarget, target_state: TargetState) -> None:
         logger.info("Initializing %s target with ID: %s", target.type.value, target.id)
         self._target = target
         self._target_state = target_state
         self._assets_dir = os.path.join(APP_ASSETS_DIR, target.id)
         self._bin_path = os.path.join(self._assets_dir, "pictorus_managed_app")
@@ -47,49 +63,68 @@
     def target_state_data(self) -> dict:
         return self._target_state.to_dict()
 
     @property
     def target_data(self) -> dict:
         return self._target.to_dict()
 
-    def handle_command(self, cmd: Command):
+    def handle_command(self, cmd_ctxt: CommandCtxt):
         """Handle a command"""
-        if cmd.type == CmdType.UPDATE_APP:
-            self.handle_update_app_cmd(cmd)
-        elif cmd.type == CmdType.SET_TELEMETRY_TLL:
-            self.handle_set_ttl_cmd(cmd)
-        elif cmd.type == CmdType.SET_LOG_LEVEL:
-            self.handle_set_log_level_cmd(cmd)
-        elif cmd.type == CmdType.RUN_APP:
-            self.handle_run_app_cmd(cmd)
-        else:
-            logger.warning("Unknown command: %s", cmd.type)
+        cmd = cmd_ctxt.cmd
+        try:
+            if cmd.type == CmdType.UPDATE_APP:
+                self.handle_update_app_cmd(cmd_ctxt)
+            elif cmd.type == CmdType.SET_TELEMETRY_TLL:
+                self.handle_set_ttl_cmd(cmd_ctxt)
+            elif cmd.type == CmdType.SET_LOG_LEVEL:
+                self.handle_set_log_level_cmd(cmd_ctxt)
+            elif cmd.type == CmdType.RUN_APP:
+                self.handle_run_app_cmd(cmd_ctxt)
+            else:
+                logger.warning("Unknown command: %s", cmd.type)
+        except CommandError as e:
+            logger.error("Failed to handle command: %s", e)
+            self._target_state.error_log = {
+                "err_type": e.err_type,
+                "message": e.message,
+            }
+        except Exception as e:
+            logger.error("Failed to handle command: %s", e, exc_info=True)
+            self._target_state.error_log = {
+                "err_type": "UnknownError",
+                "message": f"Command failed: {e}",
+            }
 
-    @abstractmethod
-    def handle_update_app_cmd(self, cmd: Command):
+    def handle_update_app_cmd(self, cmd_ctxt: CommandCtxt):
         """Update the app version for this target"""
-        pass
+        self._download_app_files(cmd_ctxt.cmd)
+        self._deploy_app(self._target, cmd_ctxt)
 
     @abstractmethod
-    def handle_set_ttl_cmd(self, cmd: Command):
+    def handle_set_ttl_cmd(self, cmd_ctxt: CommandCtxt):
         """Set the telemetry ttl for this target"""
         pass
 
     @abstractmethod
-    def handle_set_log_level_cmd(self, cmd: Command):
+    def handle_set_log_level_cmd(self, cmd_ctxt: CommandCtxt):
         """Set the log level for this target"""
         pass
 
-    def handle_run_app_cmd(self, cmd: Command):
+    def handle_run_app_cmd(self, cmd_ctxt: CommandCtxt):
         """Control whether the app is running or not"""
-        run_app = cmd.data["run_app"]
+        run_app = cmd_ctxt.cmd.data["run_app"]
         self._target_state.run_app = run_app
         self._control_app_running(run_app)
 
     @abstractmethod
+    def _deploy_app(self, target: DeployTarget, cmd_ctxt: CommandCtxt):
+        """Deploy the app to the target"""
+        pass
+
+    @abstractmethod
     def _control_app_running(self, run_app: bool):
         """Start/stop the app.
 
         This is used by some internal methods so is separated from
         the public method for handling commands
         """
         pass
@@ -109,15 +144,15 @@
         app_bin_url = cmd.data.get("app_bin_url")
         params_hash = cmd.data.get("params_hash")
         params_url = cmd.data.get("params_url")
 
         params_valid = params_hash and params_url if _is_process_target(self._target) else True
         if not build_hash or not app_bin_url or not params_valid:
             logger.error("Invalid app update request: %s", cmd.data)
-            return
+            raise CommandError("InvalidUpdateRequest", "Missing required fields for app update.")
 
         download_paths = []
         if self._target_state.build_hash != build_hash:
             logger.info("Updating binary")
             download_paths.append((self._bin_path, app_bin_url))
 
         if self._target_state.params_hash != params_hash and params_url:
@@ -132,16 +167,17 @@
                 ]
 
             try:
                 for fut in futures:
                     fut.result()
             except requests.exceptions.HTTPError:
                 logger.error("Failed to update app", exc_info=True)
+                raise CommandError("DownloadError", "Failed to download app files.")
             else:
                 os.chmod(self._bin_path, 0o755)
                 self._target_state.build_hash = build_hash
                 self._target_state.params_hash = params_hash
                 logger.info("Successfully updated app")
                 # We need to clear telemetry whenever the app updates, so all signal lengths line up
                 COMMS.clear()
         else:
-            logger.info("No app updates required")
+            logger.info("Using cached app files")
```

### Comparing `pictorus-0.2.3/src/pictorus/target_state.py` & `pictorus-0.2.4/src/pictorus/target_state.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/telemetry_manager.py` & `pictorus-0.2.4/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/src/pictorus/version_manager.py` & `pictorus-0.2.4/src/pictorus/updates_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,81 @@
 import sys
 import time
 import subprocess as sp
 from threading import Thread
-from semver import VersionInfo
 from typing import Union
+from concurrent.futures import ThreadPoolExecutor
+from functools import wraps
 
 import requests
+import cmsis_pack_manager as cp
+from semver import VersionInfo
 
 import pictorus
 from pictorus.logging_utils import get_logger
 from pictorus.config import Config
 
 logger = get_logger()
 config = Config()
 
 
-class VersionManager:
-    """Version manager for pictorus package"""
+def run_until_cancelled(method):
+    @wraps(method)
+    def wrapper(self, *args, **kwargs):
+        next_cb_time = 0
+        while self._run:
+            should_run_cb = time.time() > next_cb_time
+            if should_run_cb:
+                next_sleep_duration = method(self, *args, **kwargs)
+                if next_sleep_duration is None:
+                    break
+
+                next_cb_time = time.time() + next_sleep_duration
+            else:
+                time.sleep(1)
+
+    return wrapper
+
+
+class UpdatesManager:
+    """Manage any necessary updates"""
 
     # Check for new version every 30 minutes
     CHECK_FREQUENCY_S = 60 * 30
     # If the check fails due to a transient error, try again after 1 minute
     TRANSIENT_FAIL_CHECK_FREQUENCY_S = 60
 
     def __init__(self):
         self._last_installed: Union[str, None] = None
         self._transient_check_fail = False
         self._run = True
         self._run_thread: Union[Thread, None] = None
 
     def __enter__(self):
+        executor = ThreadPoolExecutor()
+        self.ocd_update_future = executor.submit(self.update_ocd_cache)
+
         if not config.auto_update:
             return self
 
         # Start run_continuously in a separate thread
         self._run = True
-        self._run_thread = Thread(target=self._run_continuously)
+        self._run_thread = Thread(target=self._check_pictorus_updates)
         self._run_thread.start()
+
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self._run = False
         if self._run_thread:
             self._run_thread.join()
 
+        if not self.ocd_update_future.done():
+            self.ocd_update_future.cancel()
+
     @property
     def last_installed(self) -> Union[str, None]:
         return self._last_installed
 
     def check_for_newer_version(self):
         """Check if there is a new version available on pip"""
         try:
@@ -86,24 +114,34 @@
         try:
             self.install_version(new_version)
         except sp.CalledProcessError:
             logger.error("Could not update pictorus. Please update manually.", exc_info=True)
         else:
             logger.info("Update complete. Please restart pictorus to apply.")
 
-    def _run_continuously(self):
-        """Run the version manager continuously"""
-        next_check_time = 0
+    @run_until_cancelled
+    def update_ocd_cache(self):
+        cache = cp.Cache(True, False)
+        # If the cache is already populated, no need to update
+        if cache.index:
+            return None
 
-        while self._run:
-            should_check = time.time() > next_check_time
-            if should_check:
-                self._try_update_version()
-
-                check_delay = (
-                    self.TRANSIENT_FAIL_CHECK_FREQUENCY_S
-                    if self._transient_check_fail
-                    else self.CHECK_FREQUENCY_S
-                )
-                next_check_time = time.time() + check_delay
-            else:
-                time.sleep(1)
+        logger.info("Attempting to update OCD cache")
+        cache.cache_descriptors()
+        if cache.index:
+            logger.info("OCD cache updated successfully")
+            return None
+
+        # If the cache is still empty, try again after 1 minute
+        logger.warning("Failed to update OCD cache. Will try again later.")
+        return self.TRANSIENT_FAIL_CHECK_FREQUENCY_S
+
+    @run_until_cancelled
+    def _check_pictorus_updates(self):
+        """Continuously check for updates to pictorus package"""
+        self._try_update_version()
+
+        return (
+            self.TRANSIENT_FAIL_CHECK_FREQUENCY_S
+            if self._transient_check_fail
+            else self.CHECK_FREQUENCY_S
+        )
```

### Comparing `pictorus-0.2.3/tests/pictorus/test_app_manager.py` & `pictorus-0.2.4/tests/pictorus/test_app_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from awscrt import mqtt
 from awsiot.iotshadow import ShadowDeltaUpdatedEvent
 import responses
 
 from pictorus.config import Config
 from pictorus.app_manager import AppManager, COMMS
 from pictorus.command import CmdType, Command
+from pictorus.target_manager import CommandCtxt
 from ..utils import wait_for_condition
 
 config = Config()
 
 ADDR_DATA = ("127.0.0.1", 1234)
 BUILD_HASH = "bob"
 
@@ -59,38 +60,44 @@
             mgr._target_managers = {target_id: target_mgr}
 
             # Start the app
             mgr._on_shadow_delta_updated(
                 ShadowDeltaUpdatedEvent(state={"target_states": {target_id: {"run_app": True}}})
             )
             target_mgr.handle_command.assert_called_once_with(
-                Command(
-                    {
-                        "type": CmdType.RUN_APP.value,
-                        "data": {"run_app": True},
-                        "target_id": target_id,
-                    }
+                CommandCtxt(
+                    Command(
+                        {
+                            "type": CmdType.RUN_APP.value,
+                            "data": {"run_app": True},
+                            "target_id": target_id,
+                        }
+                    ),
+                    Mock(),
                 )
             )
             handle = m_write()
             handle.write.assert_called_once_with(json.dumps(manifest_data))
             assert m_shadow_req.mock_calls[1][2]["state"].reported["target_states"] == target_states
 
             # Stop the app
             target_mgr.handle_command.reset_mock()
             mgr._on_shadow_delta_updated(
                 ShadowDeltaUpdatedEvent(state={"target_states": {target_id: {"run_app": False}}})
             )
             target_mgr.handle_command.assert_called_once_with(
-                Command(
-                    {
-                        "type": CmdType.RUN_APP.value,
-                        "data": {"run_app": False},
-                        "target_id": target_id,
-                    }
+                CommandCtxt(
+                    Command(
+                        {
+                            "type": CmdType.RUN_APP.value,
+                            "data": {"run_app": False},
+                            "target_id": target_id,
+                        }
+                    ),
+                    Mock(),
                 )
             )
 
     @patch("pictorus.app_manager.iotshadow.UpdateShadowRequest")
     def test_run_deleted_target_removes_from_desired_state(self, m_shadow_req, _):
         target_id = "foo"
 
@@ -125,29 +132,33 @@
             cmd_data = {
                 "type": CmdType.RUN_APP.value,
                 "data": {"run_app": True},
                 "target_id": target_id,
             }
             COMMS.add_command(cmd_data)
             wait_for_condition(lambda: COMMS.commands.qsize() == 0)
-            target_mgr.handle_command.assert_called_once_with(Command(cmd_data))
+            target_mgr.handle_command.assert_called_once_with(
+                CommandCtxt(Command(cmd_data), Mock())
+            )
             handle = m_write()
             handle.write.assert_called_once_with(json.dumps(manifest_data))
             assert m_shadow_req.mock_calls[1][2]["state"].reported["target_states"] == target_states
 
             # Stop the app
             target_mgr.handle_command.reset_mock()
             cmd_data = {
                 "type": CmdType.RUN_APP.value,
                 "data": {"run_app": False},
                 "target_id": target_id,
             }
             COMMS.add_command(cmd_data)
             wait_for_condition(lambda: COMMS.commands.qsize() == 0)
-            target_mgr.handle_command.assert_called_once_with(Command(cmd_data))
+            target_mgr.handle_command.assert_called_once_with(
+                CommandCtxt(Command(cmd_data), Mock())
+            )
 
     @responses.activate
     @patch("pictorus.app_manager.run")
     def test_set_upload_logs(self, m_run, m_mqtt_builder):
         upload_url = "https://example.com/upload"
 
         upload_logs_cmd = json.dumps(
```

### Comparing `pictorus-0.2.3/tests/pictorus/test_embedded_target_manager.py` & `pictorus-0.2.4/tests/pictorus/test_embedded_target_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,57 +5,56 @@
 
 from pictorus.command import DeployTarget
 from pictorus.target_state import TargetState
 from pictorus.embedded_target_manager import EmbeddedTargetManager
 from ..utils import expected_bin_path, setup_update_cmd
 
 
+def basic_update_command(target_data: dict):
+    return setup_update_cmd(
+        version_url="http://foo.bar/baz",
+        params_url="",
+        build_id="newfoo",
+        params_hash="",
+        target_data=target_data,
+    )
+
+
 @patch("pictorus.target_manager.os.makedirs", new=Mock())
 @patch("pictorus.target_manager.os.chmod", new=Mock())
+@patch("pictorus.embedded_target_manager.is_pack_target_available", return_value=True)
 @patch("pictorus.embedded_target_manager.ConnectHelper.session_with_chosen_probe")
 @patch("pictorus.embedded_target_manager.FileProgrammer")
 class TestEmbeddedTargetManager(TestCase):
     @responses.activate
-    def test_successful_deploy_to_embedded_target(self, m_prog, m_session):
+    def test_successful_deploy(self, m_prog, m_session, _):
         ocd_target = "stm32f4disco"
         target_id = "foo"
         target_data = {"id": target_id, "type": "embedded", "options": {"ocd_target": ocd_target}}
-        update_app_cmd, expected_target_state = setup_update_cmd(
-            version_url="http://foo.bar/baz",
-            params_url="",
-            build_id="newfoo",
-            params_hash="",
-            target_data=target_data,
-        )
+        update_app_cmd, expected_target_state = basic_update_command(target_data)
 
         target_mgr = EmbeddedTargetManager(DeployTarget(target_data), TargetState({}))
         with patch("builtins.open"):
             target_mgr.handle_command(update_app_cmd)
 
         m_session.assert_called_once_with(
             blocking=False, return_first=True, target_override=ocd_target
         )
         m_prog.return_value.program.assert_called_once_with(
             expected_bin_path(target_id), file_format="elf"
         )
         assert target_mgr.target_state_data == expected_target_state.to_dict()
 
     @responses.activate
-    def test_failed_deploy_to_embedded_target_unconnected(self, m_prog, m_session):
+    def test_failed_deploy_unconnected(self, m_prog, m_session, _):
         m_session.return_value = None
 
         ocd_target = "stm32f4disco"
         target_data = {"id": "foo", "type": "embedded", "options": {"ocd_target": ocd_target}}
-        update_app_cmd, expected_target_state = setup_update_cmd(
-            version_url="http://foo.bar/baz",
-            params_url="",
-            build_id="newfoo",
-            params_hash="",
-            target_data=target_data,
-        )
+        update_app_cmd, expected_target_state = basic_update_command(target_data)
 
         target_mgr = EmbeddedTargetManager(DeployTarget(target_data), TargetState({}))
         with patch("builtins.open"):
             target_mgr.handle_command(update_app_cmd)
 
         m_session.assert_called_once_with(
             blocking=False, return_first=True, target_override=ocd_target
@@ -65,27 +64,21 @@
         expected_target_state.error_log = {
             "err_type": "TargetConnectionError",
             "message": "Failed to connect to target. Make sure it is connected and powered on.",
         }
         assert target_mgr.target_state_data == expected_target_state.to_dict()
 
     @responses.activate
-    def test_failed_deploy_to_embedded_target_failed_flash(self, m_prog, m_session):
+    def test_failed_deploy_failed_flash(self, m_prog, m_session, _):
         m_prog.return_value.program.side_effect = ValueError("foo")
 
         ocd_target = "stm32f4disco"
         target_id = "foo"
         target_data = {"id": target_id, "type": "embedded", "options": {"ocd_target": ocd_target}}
-        update_app_cmd, expected_target_state = setup_update_cmd(
-            version_url="http://foo.bar/baz",
-            params_url="",
-            build_id="newfoo",
-            params_hash="",
-            target_data=target_data,
-        )
+        update_app_cmd, expected_target_state = basic_update_command(target_data)
 
         target_mgr = EmbeddedTargetManager(DeployTarget(target_data), TargetState({}))
         with patch("builtins.open"):
             target_mgr.handle_command(update_app_cmd)
 
         m_session.assert_called_once_with(
             blocking=False, return_first=True, target_override=ocd_target
@@ -96,7 +89,61 @@
         )
 
         expected_target_state.error_log = {
             "err_type": "TargetFlashError",
             "message": "Failed to flash target: foo",
         }
         assert target_mgr.target_state_data == expected_target_state.to_dict()
+
+    @responses.activate
+    def test_auto_selects_target_name(self, m_prog, m_session, _):
+        ocd_target = "stm32f45678"
+        target_id = "foo"
+        # No OCD target specified in the target data
+        target_data = {"id": target_id, "type": "embedded", "options": {}}
+        update_app_cmd, expected_target_state = basic_update_command(target_data)
+
+        target_mgr = EmbeddedTargetManager(DeployTarget(target_data), TargetState({}))
+        with patch("builtins.open"), patch(
+            "pictorus.embedded_target_manager.ConnectHelper.choose_probe"
+        ) as m_probe:
+            # Probe lookup returns a target name
+            m_probe.return_value.associated_board_info.target = ocd_target
+            target_mgr.handle_command(update_app_cmd)
+
+        m_session.assert_called_once_with(
+            blocking=False, return_first=True, target_override=ocd_target
+        )
+        m_prog.return_value.program.assert_called_once_with(
+            expected_bin_path(target_id), file_format="elf"
+        )
+        assert target_mgr.target_state_data == expected_target_state.to_dict()
+
+    @responses.activate
+    def test_installs_missing_target(self, m_prog, m_session, m_target_avail):
+        # Target is not installed
+        m_target_avail.return_value = False
+
+        ocd_target = "stm32f4disco"
+        target_id = "foo"
+        target_data = {"id": target_id, "type": "embedded", "options": {"ocd_target": ocd_target}}
+        update_app_cmd, expected_target_state = basic_update_command(target_data)
+
+        target_mgr = EmbeddedTargetManager(DeployTarget(target_data), TargetState({}))
+        with patch("builtins.open"), patch(
+            "pictorus.embedded_target_manager.cp.Cache"
+        ) as m_cache, patch("pictorus.embedded_target_manager.futures.wait"):
+            cache = m_cache.return_value
+            cache.index = {ocd_target: "bar"}
+            packs = ["baz"]
+            cache.packs_for_devices.return_value = packs
+
+            target_mgr.handle_command(update_app_cmd)
+            cache.download_pack_list.assert_called_once_with(packs)
+
+        m_session.assert_called_once_with(
+            blocking=False, return_first=True, target_override=ocd_target
+        )
+        m_prog.return_value.program.assert_called_once_with(
+            expected_bin_path(target_id), file_format="elf"
+        )
+        assert target_mgr.target_state_data == expected_target_state.to_dict()
```

### Comparing `pictorus-0.2.3/tests/pictorus/test_local_server.py` & `pictorus-0.2.4/tests/pictorus/test_local_server.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/tests/pictorus/test_proc_target_manager.py` & `pictorus-0.2.4/tests/pictorus/test_proc_target_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from unittest import TestCase
-from unittest.mock import patch, Mock, mock_open
+from unittest.mock import MagicMock, patch, Mock, mock_open
 import threading
 import json
 
 import responses
 
 from pictorus.constants import AppLogLevel, EMPTY_ERROR
+from pictorus.target_manager import CommandCtxt
 from pictorus.proc_target_manager import ProcTargetManager
 from pictorus.command import DeployTarget, Command, CmdType
 from pictorus.target_state import TargetState
 from ..utils import (
     expected_assets_dir,
     expected_bin_path,
     expected_error_log_path,
@@ -65,38 +66,40 @@
             start_app_cmd = Command(
                 {
                     "type": CmdType.RUN_APP.value,
                     "data": {"run_app": True},
                     "target_id": self.TARGET_ID,
                 }
             )
+            cmd_ctxt = CommandCtxt(start_app_cmd, MagicMock())
             m_telem.reset_mock()
             m_popen.reset_mock()
-            mgr.handle_command(start_app_cmd)
+            mgr.handle_command(cmd_ctxt)
             m_telem.return_value.start_listening.assert_called_once_with(self.BUILD_HASH)
             _assert_correct_app_start(m_popen, self.TARGET_ID)
 
             # Calling start again should do nothing
             m_telem.reset_mock()
             m_popen.reset_mock()
-            mgr.handle_command(start_app_cmd)
+            mgr.handle_command(cmd_ctxt)
             m_telem.return_value.start_listening.assert_not_called()
             m_popen.assert_not_called()
 
             # Stop the app
             stop_app_cmd = Command(
                 {
                     "type": CmdType.RUN_APP.value,
                     "data": {"run_app": False},
                     "target_id": self.TARGET_ID,
                 }
             )
+            cmd_ctxt = CommandCtxt(stop_app_cmd, MagicMock())
             m_telem.reset_mock()
             m_popen.reset_mock()
-            mgr.handle_command(stop_app_cmd)
+            mgr.handle_command(cmd_ctxt)
             m_telem.return_value.start_listening.assert_not_called()
             m_popen.assert_not_called()
             m_popen.return_value.terminate.assert_called_once()
 
     @responses.activate
     def test_starts_app_on_update(self, m_telem, m_popen, _):
         new_build_id = "newfoo"
@@ -127,33 +130,35 @@
         set_ttl_cmd = Command(
             {
                 "type": CmdType.SET_TELEMETRY_TLL.value,
                 "data": {"ttl_s": ttl_s},
                 "target_id": self.TARGET_ID,
             }
         )
+        cmd_ctxt = CommandCtxt(set_ttl_cmd, MagicMock())
         target_state = TargetState({"run_app": False, "build_hash": self.BUILD_HASH})
         with ProcTargetManager(self.TARGET, target_state, Mock(), Mock()) as mgr:
-            mgr.handle_command(set_ttl_cmd)
+            mgr.handle_command(cmd_ctxt)
             m_telem.return_value.set_ttl.assert_called_once_with(ttl_s)
 
     def test_set_log_level(self, _, m_popen, __):
         log_level = AppLogLevel.DEBUG
         set_ttl_cmd = Command(
             {
                 "type": CmdType.SET_LOG_LEVEL.value,
                 "data": {"log_level": log_level.value},
                 "target_id": self.TARGET_ID,
             }
         )
+        cmd_ctxt = CommandCtxt(set_ttl_cmd, MagicMock())
 
         target_state = TargetState({"run_app": True, "build_hash": self.BUILD_HASH})
         with ProcTargetManager(self.TARGET, target_state, Mock(), Mock()) as mgr:
             m_popen.reset_mock()
-            mgr.handle_command(set_ttl_cmd)
+            mgr.handle_command(cmd_ctxt)
             _assert_correct_app_start(m_popen, self.TARGET_ID, log_level=log_level)
 
     @patch("pictorus.proc_target_manager.os.remove")
     def test_sets_error_from_file_on_unexpected_crash(self, m_remove, _, m_popen, __):
         app_complete = threading.Event()
         m_popen.return_value.wait.side_effect = app_complete.wait
```

### Comparing `pictorus-0.2.3/tests/pictorus/test_telemetry_manager.py` & `pictorus-0.2.4/tests/pictorus/test_telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.2.3/tests/utils.py` & `pictorus-0.2.4/tests/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import time
 from typing import Callable
+from unittest.mock import MagicMock
 
 import responses
 
 from pictorus.config import APP_ASSETS_DIR
 from pictorus.command import Command, CmdType
+from pictorus.target_manager import CommandCtxt
 from pictorus.target_state import TargetState
 
 
 def wait_for_condition(condition: Callable[[], bool], timeout=1):
     start = time.time()
     while not condition():
         if time.time() - start > timeout:
@@ -42,8 +44,8 @@
         "params_hash": params_hash,
         "params_url": params_url,
     }
 
     expected_target_state = TargetState({"build_hash": build_id, "params_hash": params_hash})
     cmd_data = {"type": CmdType.UPDATE_APP.value, "data": version_data, "target": target_data}
 
-    return Command(cmd_data), expected_target_state
+    return CommandCtxt(Command(cmd_data), MagicMock()), expected_target_state
```

### Comparing `pictorus-0.2.3/PKG-INFO` & `pictorus-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.9; python_version <= "3.6"
 Requires-Dist: awsiotsdk~=1.19.0; python_version > "3.6"
```

