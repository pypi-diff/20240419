# Comparing `tmp/bec_ipython_client-2.5.0.tar.gz` & `tmp/bec_ipython_client-2.6.0.tar.gz`

## Comparing `bec_ipython_client-2.5.0.tar` & `bec_ipython_client-2.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/demo.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/__init__.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/beamline_mixin.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/bec_magics.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/bec_startup.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/main.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/prettytable.py
--rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/progressbar.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/signals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/__init__.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/ipython_live_updates.py
--rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/live_table.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/move_device.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/scan_progress.py
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/callbacks/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/bec_hli.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/spec_hli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/__init__.py
--rw-r--r--   0        0        0    49460 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/LamNI_logo.png
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/__init__.py
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
--rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py
--rw-r--r--   0        0        0    54701 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/__init__.py
--rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/sls_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/x-treme.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/__init__.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/beamline_info.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/__init__.py
--rw-r--r--   0        0        0    80400 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni.py
--rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_test_config.yaml
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/conftest.py
--rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_beamline_mixins.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_bec_client.py
--rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_ipython_live_updates.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_live_table.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_move_callback.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_pretty_table.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_scan_progress.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/client_tests/test_x_ray_eye_align.py
--rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/end-2-end/test_scans_e2e.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/tests/end-2-end/test_scans_lib_e2e.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/.gitignore
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_ipython_client-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/demo.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/beamline_mixin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/bec_magics.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/bec_startup.py
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/main.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/prettytable.py
+-rw-r--r--   0        0        0    11165 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/progressbar.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/signals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/__init__.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0        0        0    11964 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/live_table.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/move_device.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/scan_progress.py
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/high_level_interfaces/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/high_level_interfaces/bec_hli.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/high_level_interfaces/spec_hli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/__init__.py
+-rw-r--r--   0        0        0    49460 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/LamNI_logo.png
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/__init__.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py
+-rw-r--r--   0        0        0    54701 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/SLS/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/SLS/sls_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/XTreme/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/XTreme/x-treme.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/__init__.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/beamline_info.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/__init__.py
+-rw-r--r--   0        0        0    80400 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni.py
+-rw-r--r--   0        0        0     6399 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni_test_config.yaml
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     7510 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_beamline_mixins.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_bec_client.py
+-rw-r--r--   0        0        0     6075 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_ipython_live_updates.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_live_table.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_move_callback.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_pretty_table.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_scan_progress.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/client_tests/test_x_ray_eye_align.py
+-rw-r--r--   0        0        0    25147 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/end-2-end/test_scans_e2e.py
+-rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/tests/end-2-end/test_scans_lib_e2e.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/.gitignore
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_ipython_client-2.6.0/PKG-INFO
```

### Comparing `bec_ipython_client-2.5.0/demo.py` & `bec_ipython_client-2.6.0/demo.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/beamline_mixin.py` & `bec_ipython_client-2.6.0/bec_ipython_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/bec_magics.py` & `bec_ipython_client-2.6.0/bec_ipython_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/main.py` & `bec_ipython_client-2.6.0/bec_ipython_client/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from IPython.terminal.ipapp import TerminalIPythonApp
 from IPython.terminal.prompts import Prompts, Token
 
 from bec_ipython_client.beamline_mixin import BeamlineMixin
 from bec_ipython_client.bec_magics import BECMagics
 from bec_ipython_client.callbacks.ipython_live_updates import IPythonLiveUpdates
 from bec_ipython_client.signals import ScanInterruption, SigintHandler
-from bec_lib import ServiceConfig, bec_logger
+from bec_lib import ServiceConfig, bec_logger, plugin_helper
 from bec_lib.alarm_handler import AlarmBase
 from bec_lib.callback_handler import EventType
 from bec_lib.client import BECClient
 from bec_lib.connector import ConnectorBase
 
 logger = bec_logger.logger
 
@@ -178,35 +178,41 @@
 
 
 # pylint: disable=wrong-import-position
 # pylint: disable=protected-access
 # pylint: disable=unused-import
 # pylint: disable=ungrouped-imports
 
-try:
-    from bec_plugins.bec_client import startup
-except ImportError:
-    startup = None
-
-main_dict = {"startup": startup}
+main_dict = {}
 
 sys.modules["bec_ipython_client.main"] = sys.modules[
     __name__
 ]  # properly register module when file is executed directly, like in test
 
 
 def main():
+    """
+    Main function to start the BEC IPython client.
+    """
+
+    available_plugins = plugin_helper.get_ipython_client_startup_plugins(state="pre")
+
     parser = argparse.ArgumentParser(
         prog="BEC IPython client", description="BEC command line interface"
     )
     parser.add_argument("--version", action="store_true", default=False)
     parser.add_argument("--nogui", action="store_true", default=False)
     parser.add_argument("--config", action="store", default=None)
     parser.add_argument("--dont-wait-for-server", action="store_true", default=False)
     parser.add_argument("--post-startup-file", action="store", default=None)
+
+    for plugin in available_plugins.values():
+        if hasattr(plugin["module"], "extend_command_line_args"):
+            plugin["module"].extend_command_line_args(parser)
+
     args, left_args = parser.parse_known_args()
 
     # remove already parsed args from command line args
     sys.argv = sys.argv[:1] + left_args
 
     if args.version:
         print(f"BEC IPython client: {version('bec_ipython_client')}")
@@ -215,22 +221,20 @@
     config_file = args.config
     if config_file:
         if not os.path.isfile(config_file):
             raise FileNotFoundError("Config file not found.")
         print("Using config file: ", config_file)
         config = ServiceConfig(config_file)
 
-    if startup and "config" not in locals():
+    if available_plugins and "config" not in locals():
         # check if pre-startup.py script exists
-        file_name = os.path.join(os.path.dirname(startup.__file__), "pre_startup.py")
-        if os.path.isfile(file_name):
-            with open(file_name, "r", encoding="utf-8") as file:
-                # exec the pre-startup.py script and pass the arguments
-                # pylint: disable=exec-used
-                exec(file.read(), globals(), locals())
+        for plugin in available_plugins.values():
+            if hasattr(plugin["module"], "get_config"):
+                config = plugin.get_config()
+                break
 
     # check if config was defined in pre-startup.py
     if "config" not in locals():
         config = ServiceConfig()
 
     main_dict["config"] = config
     main_dict["args"] = args
```

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/prettytable.py` & `bec_ipython_client-2.6.0/bec_ipython_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/progressbar.py` & `bec_ipython_client-2.6.0/bec_ipython_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/signals.py` & `bec_ipython_client-2.6.0/bec_ipython_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-2.6.0/bec_ipython_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/live_table.py` & `bec_ipython_client-2.6.0/bec_ipython_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/move_device.py` & `bec_ipython_client-2.6.0/bec_ipython_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/scan_progress.py` & `bec_ipython_client-2.6.0/bec_ipython_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/callbacks/utils.py` & `bec_ipython_client-2.6.0/bec_ipython_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/bec_hli.py` & `bec_ipython_client-2.6.0/bec_ipython_client/high_level_interfaces/bec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/high_level_interfaces/spec_hli.py` & `bec_ipython_client-2.6.0/bec_ipython_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/LamNI_logo.png` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/LamNI_logo.png`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/SLS/sls_info.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/beamline_info.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/flomni_test_config.yaml` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/flomni_test_config.yaml`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py` & `bec_ipython_client-2.6.0/bec_ipython_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_beamline_mixins.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_beamline_mixins.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_bec_client.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_bec_client.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_ipython_live_updates.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_live_table.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_move_callback.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_move_callback.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_scan_progress.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/client_tests/test_x_ray_eye_align.py` & `bec_ipython_client-2.6.0/tests/client_tests/test_x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/end-2-end/test_scans_e2e.py` & `bec_ipython_client-2.6.0/tests/end-2-end/test_scans_e2e.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/tests/end-2-end/test_scans_lib_e2e.py` & `bec_ipython_client-2.6.0/tests/end-2-end/test_scans_lib_e2e.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     with pytest.raises(AlarmBase) as exc:
         scans.mv(dev.samx, 1000, relative=False).wait()
 
 
 @pytest.mark.timeout(100)
 def test_async_callback_data_matches_scan_data_lib(bec_client_lib):
     bec = bec_client_lib
+    scans = bec.scans  # not needed but to silence pylint...
     bec.metadata.update({"unit_test": "test_async_callback_data_matches_scan_data"})
     dev = bec.device_manager.devices
     reference_container = {"data": [], "metadata": {}}
 
     def dummy_callback(data, metadata):
         logger.info(f"callback metadata: {metadata}")
         reference_container["metadata"] = metadata
@@ -135,23 +136,23 @@
 @pytest.mark.timeout(100)
 @pytest.mark.parametrize(
     "config, raises_error, deletes_config, disabled_device",
     [
         (
             {
                 "hexapod": {
-                    "deviceClass": "SynDeviceOPAAS",
+                    "deviceClass": "ophyd_devices.SynDeviceOPAAS",
                     "deviceConfig": {},
                     "deviceTags": ["user motors"],
                     "readoutPriority": "baseline",
                     "enabled": True,
                     "readOnly": False,
                 },
                 "eyefoc": {
-                    "deviceClass": "SimPositioner",
+                    "deviceClass": "ophyd_devices.SimPositioner",
                     "deviceConfig": {
                         "delay": 1,
                         "limits": [-50, 50],
                         "speed": 100,
                         "tolerance": 0.01,
                         "update_frequency": 400,
                     },
@@ -163,23 +164,23 @@
             True,
             False,
             [],
         ),
         (
             {
                 "hexapod": {
-                    "deviceClass": "SynDeviceOPAAS",
+                    "deviceClass": "ophyd_devices.SynDeviceOPAAS",
                     "deviceConfig": {},
                     "deviceTags": ["user motors"],
                     "readoutPriority": "baseline",
                     "enabled": True,
                     "readOnly": False,
                 },
                 "eyefoc": {
-                    "deviceClass": "SimPositioner",
+                    "deviceClass": "ophyd_devices.SimPositioner",
                     "deviceConfig": {
                         "delay": 1,
                         "limits": [-50, 50],
                         "speed": 100,
                         "tolerance": 0.01,
                         "update_frequency": 400,
                     },
@@ -192,23 +193,23 @@
             False,
             False,
             [],
         ),
         (
             {
                 "hexapod": {
-                    "deviceClass": "SynDeviceOPAAS",
+                    "deviceClass": "ophyd_devices.SynDeviceOPAAS",
                     "deviceConfig": {},
                     "deviceTags": ["user motors"],
                     "readoutPriority": "baseline",
                     "enabled": True,
                     "readOnly": False,
                 },
                 "eyefoc": {
-                    "deviceClass": "utils:bec_utils:DeviceClassConnectionError",
+                    "deviceClass": "ophyd_devices.utils.bec_utils.DeviceClassConnectionError",
                     "deviceConfig": {},
                     "readoutPriority": "baseline",
                     "deviceTags": ["user motors"],
                     "enabled": True,
                     "readOnly": False,
                 },
             },
@@ -223,15 +224,15 @@
                     "deviceConfig": {},
                     "deviceTags": ["user motors"],
                     "readoutPriority": "baseline",
                     "enabled": True,
                     "readOnly": False,
                 },
                 "eyefoc": {
-                    "deviceClass": "utils:bec_utils:DeviceClassInitError",
+                    "deviceClass": "ophyd_devices.utils.bec_utils.DeviceClassInitError",
                     "deviceConfig": {},
                     "readoutPriority": "baseline",
                     "deviceTags": ["user motors"],
                     "enabled": True,
                     "readOnly": False,
                 },
             },
@@ -246,15 +247,15 @@
                     "deviceConfig": {},
                     "deviceTags": ["user motors"],
                     "readoutPriority": "baseline",
                     "enabled": True,
                     "readOnly": False,
                 },
                 "eyefoc": {
-                    "deviceClass": "WrongDeviceClass",
+                    "deviceClass": "ophyd_devices.WrongDeviceClass",
                     "deviceConfig": {},
                     "readoutPriority": "baseline",
                     "deviceTags": ["user motors"],
                     "enabled": True,
                     "readOnly": False,
                 },
             },
@@ -268,20 +269,15 @@
         "valid_config_no_error",
         "invalid_device_class_connection_error",
         "invalid_device_class_init",
         "invalid_device_class",
     ],
 )
 def test_config_reload(
-    bec_test_config_file_path,
-    bec_client_lib,
-    config,
-    raises_error,
-    deletes_config,
-    disabled_device,
+    bec_test_config_file_path, bec_client_lib, config, raises_error, deletes_config, disabled_device
 ):
     bec = bec_client_lib
     bec.metadata.update({"unit_test": "test_config_reload"})
     runtime_config_file_path = bec_test_config_file_path.parent / "e2e_runtime_config_test.yaml"
     try:
         # write new config to disk
         with open(runtime_config_file_path, "w") as f:
```

### Comparing `bec_ipython_client-2.5.0/.gitignore` & `bec_ipython_client-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-2.5.0/pyproject.toml` & `bec_ipython_client-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec_ipython_client"
-version = "2.5.0"
+version = "2.6.0"
 description = "BEC IPython client"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_ipython_client-2.5.0/PKG-INFO` & `bec_ipython_client-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec_ipython_client
-Version: 2.5.0
+Version: 2.6.0
 Summary: BEC IPython client
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

