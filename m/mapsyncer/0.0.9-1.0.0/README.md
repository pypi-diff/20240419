# Comparing `tmp/mapsyncer-0.0.9.tar.gz` & `tmp/mapsyncer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapsyncer-0.0.9.tar", last modified: Fri Mar 15 13:01:48 2024, max compression
+gzip compressed data, was "mapsyncer-1.0.0.tar", last modified: Fri Apr 19 14:15:52 2024, max compression
```

## Comparing `mapsyncer-0.0.9.tar` & `mapsyncer-1.0.0.tar`

### file list

```diff
@@ -1,40 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.071491 mapsyncer-0.0.9/MapSyncer/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/MapSyncer/components/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/common_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/get_exif.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/login_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/osc_api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20297 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/osc_api_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/osc_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/osm_access.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/MapSyncer/components/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/MapSyncer/components/parsers/exif/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/exif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/exif/exif.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/exif/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/MapSyncer/components/parsers/osc_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/osc_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/parsers/osc_metadata/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/components/version_.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/MapSyncer/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/mapsyncer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 13:01:48.000000 mapsyncer-0.0.9/mapsyncer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 13:01:48.075492 mapsyncer-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-15 13:01:24.000000 mapsyncer-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.793069 mapsyncer-1.0.0/MapSyncer/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13578 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/get_exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19217 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/osc_api_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/exif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/exif/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.797068 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/components/version_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/MapSyncer/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/edit-sequence.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/static/mapilio_fav.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/MapSyncer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/details.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/display-sequence.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/kartaview-login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/mapilio-login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/MapSyncer/templates/sequence-edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/mapsyncer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 14:15:52.000000 mapsyncer-1.0.0/mapsyncer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:15:52.801068 mapsyncer-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 14:15:32.000000 mapsyncer-1.0.0/setup.py
```

### Comparing `mapsyncer-0.0.9/LICENSE` & `mapsyncer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/common_models.py` & `mapsyncer-1.0.0/MapSyncer/components/common_models.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/download.py` & `mapsyncer-1.0.0/MapSyncer/components/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,38 @@
 )
 from typing import List, Tuple
 
 from tqdm.auto import tqdm
 
 from common_models import GPS
 from storage import Local
-from login_controller import LoginController
 from osc_api_config import OSCAPISubDomain
 from osc_api_gateway import OSCApi
 from osc_api_models import OSCPhoto
 from parsers.exif.exif import ExifParser
 from get_exif import get_exif
 from colorama import Fore
 progress = {}
 
 LOGGER = logging.getLogger('osc_tools.osc_utils')
 
+DOWNLOAD_LOGS = os.path.join(
+        os.path.expanduser("~"),
+        ".config",
+        "mapilio",
+        "configs",
+        "MapSyncer",
+        "download_logs.json"
+    )
+
 def check_sequence_status(sequence_id):
-    log_file = ".download_logs.json"
-    if os.path.exists(log_file):
-        if os.path.getsize(log_file) == 0:
+    if os.path.exists(DOWNLOAD_LOGS):
+        if os.path.getsize(DOWNLOAD_LOGS) == 0:
             return False
-        with open(log_file, 'r') as f:
+        with open(DOWNLOAD_LOGS, 'r') as f:
             log_data_list = json.load(f)
             for entry in log_data_list:
                 if entry.get("seq_id") == sequence_id and entry.get("download_success") and entry.get("upload_success"):
                     return True
     return False
 
 
@@ -84,36 +91,58 @@
                 selected_sequences.append(sequences[index - 1])
             else:
                 return None
         else:
             return None
     return selected_sequences
 
-def flask_app(folder_path):
-    login_controller = LoginController(OSCAPISubDomain.PRODUCTION)
-    user = login_controller.login()
-    flaskPath = os.path.join('/'.join(os.path.dirname(os.path.abspath(__file__)).split("/")[:-1]), "app.py")
-    command = f"python {flaskPath} --username {user.name} --to_path {folder_path} "
-    if platform.system() == "Windows":
-        subprocess.Popen(['cmd', '/c', 'start', 'cmd', '/k', command])
-    elif platform.system() == "Linux":
-        subprocess.Popen(['gnome-terminal', '--', 'bash', '-c', f"{command}; read -p 'Press Enter to exit'"])
-    elif platform.system() == "Darwin":  # macOS
-        subprocess.Popen(['open', '-a', 'Terminal', 'app.py'])
-    else:
-        print("Unsupported operating system")
+# def flask_app(folder_path):
+#     #TODO: Flask will be up by app.app, shouldnt use subprocesser
+#     login_controller = LoginController(OSCAPISubDomain.PRODUCTION)
+#     user = login_controller.login()
+#     flaskPath = os.path.join('/'.join(os.path.dirname(os.path.abspath(__file__)).split("/")[:-1]), "app.py")
+#     command = f"python3 {flaskPath} --username {user.name} --to_path {folder_path}"
+#     if platform.system() == "Windows":
+#         command = f"python {flaskPath} --username {user.name} --to_path {folder_path} "
+#         subprocess.Popen(['cmd', '/c', 'start', 'cmd', '/k', command])
+#     elif platform.system() == "Linux":
+#         try:
+#             subprocess.Popen(['gnome-terminal', '--', 'bash', '-c', f"{command}; read -p 'Press Enter to exit'"])
+#         except:
+#             subprocess.Popen(['bash', '-c', f"{command}; read -p 'Press Enter to exit'"])
+#     elif platform.system() == "Darwin":  # macOS
+#         def get_virtualenv_path():
+#             try:
+#                 venv_path = subprocess.check_output(['which', 'python']).decode().strip()
+#                 if 'usr' not in venv_path:
+#                     return venv_path.split('bin')[0]
+#             except subprocess.CalledProcessError:
+#                 pass
+#                 return None
+#
+#         venv_path = get_virtualenv_path()
+#         if venv_path:
+#             venv_activate_command = f'source {venv_path}/bin/activate && '
+#         else:
+#             venv_activate_command = ''
+#
+#         applescript = f'tell application "Terminal" to do script "{venv_activate_command}python3 {flaskPath} --username {user.name} --to_path {folder_path}"'
+#         subprocess.run(['osascript', '-e', applescript])
+#     else:
+#         print("Unsupported operating system")
 
 
-def download_user_images(to_path, selected_sequences_id=None):
-    login_controller = LoginController(OSCAPISubDomain.PRODUCTION)
+def download_user_images(to_path,user_name,selected_sequences_id=None):
+    # login_controller = LoginController(OSCAPISubDomain.PRODUCTION)
     # login to get the valid user
-    user = login_controller.login()
-    osc_api = login_controller.osc_api
+    # user = login_controller.login()
+    # osc_api = login_controller.osc_api
+    osc_api = OSCApi(OSCAPISubDomain.PRODUCTION)
     # get all the sequneces for this user
-    sequences, error = osc_api.user_sequences(user.name, to_path)
+    sequences, error = osc_api.user_sequences(user_name)
 
     if error:
         print("Could not get sequences for the current user, try again or report a issue on "
               "github")
         return
     if selected_sequences_id is None:
         selected_sequences = select_sequences_to_download(sequences)
@@ -177,35 +206,35 @@
             if filePath is not None:
                 lth_images.append(filePath)
             download_success = download_success and photo_success
             download_bar.update(1)
             current_item_index = download_bar.n
             progress[sequence.online_id] = current_item_index
 
-    log_file = ".download_logs.json"
+
     log_data = {
         "seq_id": sequence.online_id,
         "download_success": download_success,
         "upload_success": False,
         "json_success": False
     }
 
     log_data_list = []
-    if os.path.exists(log_file):
-        with open(log_file, 'r') as f:
+    if os.path.exists(DOWNLOAD_LOGS):
+        with open(DOWNLOAD_LOGS, 'r') as f:
             log_data_list = json.load(f)
 
     for entry in log_data_list:
         if entry["seq_id"] == sequence.online_id:
             entry["download_success"] = download_success
             break
     else:
         log_data_list.append(log_data)
 
-    with open(log_file, 'w') as f:
+    with open(DOWNLOAD_LOGS, 'w') as f:
         json.dump(log_data_list, f, indent=4)
 
     if not download_success:
         LOGGER.info("Download failed for sequence %s", str(sequence.online_id))
         return False, [], []
     return True, photos, lth_images
 
@@ -220,15 +249,18 @@
                                                                 photo_download_name,
                                                                 local_storage)
 
     if error or photo_success:
         LOGGER.debug("Failed to download image: %s", photo.photo_url())
 
     if add_gps_to_exif and photo_success:
-        parser = ExifParser(photo_download_name, local_storage)
+        try:
+            parser = ExifParser(photo_download_name, local_storage)
+        except FileNotFoundError:
+            print("File not found: " + photo_download_name)
         if len(parser.items_with_class(GPS)) == 0:
             item = GPS()
             item.latitude = photo.latitude
             item.longitude = photo.longitude
             item.timestamp = photo.timestamp
             parser.add_items([item])
             parser.serialize()
```

### Comparing `mapsyncer-0.0.9/MapSyncer/components/get_exif.py` & `mapsyncer-1.0.0/MapSyncer/components/get_exif.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os.path
 import random
 import requests
 import json
-import cv2
 import string
 from colorama import Fore, Style, init
 import version_
 from calculation.distance import Distance
+import imagesize
 
 
-
-def check_seq(prev_lon,prev_lat,curr_lon,curr_lat,next_lon,next_lat,threshold=50):
+def check_seq(prev_lon, prev_lat, curr_lon, curr_lat, next_lon, next_lat, threshold=50):
     """
                                                             next_coord
                                                                     *
         prev_coord
                 *
 
                                 curr_coord
@@ -27,21 +26,21 @@
         curr_lat:
         next_lon:
         next_lat:
 
     Returns:
         situation
     """
-    dist1=Distance.haversine(lon1=prev_lon, lat1=prev_lat, lon2=curr_lon, lat2=curr_lat)
-    dist2=Distance.haversine(lon1=curr_lon,lat1=curr_lat,lon2=next_lon,lat2=next_lat)
-    if dist1>threshold and dist2<=threshold:
+    dist1 = Distance.haversine(lon1=prev_lon, lat1=prev_lat, lon2=curr_lon, lat2=curr_lat)
+    dist2 = Distance.haversine(lon1=curr_lon, lat1=curr_lat, lon2=next_lon, lat2=next_lat)
+    if dist1 > threshold and dist2 <= threshold:
         return True
-    elif dist1<threshold:
+    elif dist1 < threshold:
         return False
-    elif dist1>threshold and dist2>threshold:
+    elif dist1 > threshold and dist2 > threshold:
         print(f"{Fore.YELLOW} The current point is far away from other points.{Fore.RESET}")
         return False
 
 
 def unique_sequence_id_generator(letter_count: int = 8, digit_count: int = 4) -> str:
     """
     :param letter_count: Count of random letter
@@ -54,46 +53,63 @@
     str1 += ''.join((random.choice(string.digits) for x in range(digit_count))) + '-'
     str1 += ''.join((random.choice(string.digits) for x in range(digit_count))) + '-'
     str1 += ''.join((random.choice(string.ascii_letters) for x in range(letter_count)))
     sam_list = list(str1)
     final_string = ''.join(sam_list)
     return final_string
 
-def get_api_access_token():
-    """
-    This function retrieves the OpenStreetCam API access token from the credentials.json file.
-    """
-    credentials_file_path = 'credentials.json'
 
-    try:
-        with open(credentials_file_path, 'r') as credentials_file:
-            credentials = json.load(credentials_file)
-            osm_token = credentials.get("osm", {}).get("token")
-            return osm_token
-    except FileNotFoundError:
-        print(f"Error: {credentials_file_path} not found.")
-        return None
-    except json.JSONDecodeError as e:
-        print(f"Error decoding JSON in {credentials_file_path}: {e}")
-        return None
+# def get_api_access_token():
+#     """
+#     This function retrieves the OpenStreetCam API access token from the credentials.json file.
+#     """
+#     CREDENTIALS_FILE = os.path.join(
+#         os.path.expanduser("~"),
+#         ".config",
+#         "mapilio",
+#         "configs",
+#         "MapSyncer",
+#         "credentials.json"
+#     )
+#
+#     try:
+#         with open(CREDENTIALS_FILE, 'r') as credentials_file:
+#             credentials = json.load(credentials_file)
+#             osm_token = credentials.get("osm", {}).get("token")
+#             return osm_token
+#     except FileNotFoundError:
+#         print(f"Error: {CREDENTIALS_FILE} not found.")
+#         return None
+#     except json.JSONDecodeError as e:
+#         print(f"Error decoding JSON in {CREDENTIALS_FILE}: {e}")
+#         return None
 
 
 def get_exif(seq_id, sequence_path, lth_images):
     """
     This function gets the exif data from the OpenStreetCam API and saves it to a JSON file.
 
     Args:
         seq_id (str): The sequence ID.
         sequence_path (str): The path to the sequence folder.
     """
-    access_token = get_api_access_token()
-
-    if access_token is None:
-        print("Access token not found. Please check your credentials.")
-        return sequence_path
+    DOWNLOAD_LOGS = os.path.join(
+        os.path.expanduser("~"),
+        ".config",
+        "mapilio",
+        "configs",
+        "MapSyncer",
+        "download_logs.json"
+    )
+
+    # access_token = get_api_access_token()
+
+    # if access_token is None:
+    #     print("Access token not found. Please check your credentials.")
+    #     return sequence_path
 
     url_details = f"https://api.openstreetcam.org/details"
     params = {
         'id': seq_id
     }
     mapilio_description = []
     page_count = 1
@@ -101,15 +117,17 @@
         hasMoreData = True
         processed_count = 0
 
         response_details = requests.post(url_details, data=params)
         api_data_details = response_details.json()
 
         while hasMoreData:
-            url = f"https://api.openstreetcam.org/2.0/photo/?access_token={access_token}&sequenceId={seq_id}&page={page_count}"
+            # There is no need to use acces token.
+            # url = f"https://api.openstreetcam.org/2.0/photo/?access_token={access_token}&sequenceId={seq_id}&page={page_count}"
+            url = f"https://api.openstreetcam.org/2.0/photo/?&sequenceId={seq_id}&page={page_count}"
             response_photos = requests.get(url)
             api_data_photos = response_photos.json()
 
             if response_details.status_code != 200 or response_photos.status_code != 200:
                 print(
                     f"\n{Fore.RED}Operation of sequence id: '{seq_id}' was skipped due to a '{response_details.status_code}' status code error.{Fore.RESET}")
                 json_file = ".download_logs.json"
@@ -132,36 +150,36 @@
                     curr_lat = float(api_photo_data["matchLat"]) if api_photo_data.get(
                         "matchLat") is not None else float(api_photo_data["lat"])
                     curr_lon = float(api_photo_data["matchLng"]) if api_photo_data.get(
                         "matchLng") is not None else float(api_photo_data["lng"])
                     if idx + 2 < len(api_data_photos['result'][
                                          'data']) and idx > 1:  # cannot use idx + 1 ,idx >0 in this condition. in this situation the last and first items that should not stand alone in sequence.
                         prev_lat = float(api_data_photos['result']['data'][idx - 1]["matchLat"]) if \
-                        api_data_photos['result']['data'][idx - 1].get("matchLat") is not None else float(
+                            api_data_photos['result']['data'][idx - 1].get("matchLat") is not None else float(
                             api_data_photos['result']['data'][idx - 1]["lat"])
                         next_lat = float(api_data_photos['result']['data'][idx + 1]["matchLat"]) if \
-                        api_data_photos['result']['data'][idx + 1].get("matchLat") is not None else float(
+                            api_data_photos['result']['data'][idx + 1].get("matchLat") is not None else float(
                             api_data_photos['result']['data'][idx + 1]["lat"])
                         prev_lon = float(api_data_photos['result']['data'][idx - 1]["matchLng"]) if \
-                        api_data_photos['result']['data'][idx - 1].get("matchLng") is not None else float(
+                            api_data_photos['result']['data'][idx - 1].get("matchLng") is not None else float(
                             api_data_photos['result']['data'][idx - 1]["lng"])
                         next_lon = float(api_data_photos['result']['data'][idx + 1]["matchLng"]) if \
-                        api_data_photos['result']['data'][idx + 1].get("matchLng") is not None else float(
+                            api_data_photos['result']['data'][idx + 1].get("matchLng") is not None else float(
                             api_data_photos['result']['data'][idx + 1]["lng"])
                         situation = check_seq(prev_lon, prev_lat, curr_lon, curr_lat, next_lon, next_lat)
                     else:
                         situation = False
                     if idx % 250 == 0 or situation:
                         current_unique_id = unique_sequence_id_generator(letter_count=8, digit_count=4)
 
                     absolute_path = os.path.abspath(f'{sequence_path}/{api_photo_data["name"]}')
                     if absolute_path in lth_images:
-                        img = cv2.imread(absolute_path)
-                        api_photo_data["width"] = str(img.shape[1])
-                        api_photo_data["height"] = str(img.shape[0])
+                        width, height = imagesize.get(absolute_path)
+                        api_photo_data["width"] = str(width)
+                        api_photo_data["height"] = str(height)
 
                     if api_data_details["osv"]["cameraParameters"] is not None:
                         vfov = api_data_details["osv"]["cameraParameters"]["vFoV"]
                         fov = api_data_details["osv"]["cameraParameters"]["hFoV"]
                         fLen = api_data_details["osv"]["cameraParameters"]["fLen"]
 
                     device_name = api_data_details.get("osv", {}).get("deviceName", "")
@@ -235,21 +253,21 @@
                 "device_type": "Desktop"
             }
         }
         mapilio_description.append(description_information)
         save_path = os.path.join(sequence_path, 'mapilio_image_description.json')
         with open(save_path, 'w') as outfile:
             json.dump(mapilio_description, outfile)
-        json_file = ".download_logs.json"
-        with open(json_file, 'r') as f:
+
+        with open(DOWNLOAD_LOGS, 'r') as f:
             data = json.load(f)
         for item in data:
             if item.get('seq_id') == seq_id:
                 item['json_success'] = True
-        with open(json_file, 'w') as f:
+        with open(DOWNLOAD_LOGS, 'w') as f:
             json.dump(data, f)
 
     except requests.exceptions.RequestException as e:
         print(f"Error making the request: {e}")
     except json.JSONDecodeError as e:
         print(f"Error decoding JSON: {e}")
```

### Comparing `mapsyncer-0.0.9/MapSyncer/components/osc_api_gateway.py` & `mapsyncer-1.0.0/MapSyncer/components/osc_api_gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """This module is used as a gateway to the OSC api."""
 import asyncio
 import concurrent.futures
+import json
+import logging
 import os.path
 import shutil
-import logging
 from typing import Tuple, Optional, List
 
+import psutil
 import requests
+from colorama import Fore
+from tqdm import tqdm
+
 import osc_api_config
-from storage import Storage
 from osc_api_config import OSCAPISubDomain
 from osc_api_models import OSCSequence, OSCPhoto, OSCUser
-from colorama import Fore, init
-import json
-import subprocess
-import platform
-import psutil
-from tqdm import tqdm
+from storage import Storage
 
 LOGGER = logging.getLogger('osc_tools.osc_api_gateway')
 
 
 def _upload_url(env: OSCAPISubDomain, resource: str) -> str:
     return _osc_url(env) + '/' + _version() + '/' + resource + '/'
 
@@ -110,38 +109,23 @@
         return _osc_url(env) + '/' + resource_name
 
     @classmethod
     def photo_list(cls, env: OSCAPISubDomain) -> str:
         """this method returns photo list URL"""
         return _osc_url(env) + '/' + _version() + '/sequence/photo-list/'
 
-    @classmethod
-    def video_upload(cls, env: OSCAPISubDomain) -> str:
-        """this method returns video upload URL"""
-        return _upload_url(env, 'video')
-
-    @classmethod
-    def photo_upload(cls, env: OSCAPISubDomain) -> str:
-        """this method returns photo upload URL"""
-        return _upload_url(env, 'photo')
-
-    @classmethod
-    def login(cls, env: OSCAPISubDomain, provider: str) -> Optional[str]:
-        """this method returns login URL"""
-        if provider == "google":
-            return _osc_url(env) + '/auth/google/client_auth'
-        if provider == "facebook":
-            return _osc_url(env) + '/auth/facebook/client_auth'
-        # default to OSM
-        return _osc_url(env) + '/auth/openstreetmap/client_auth'
-
-    @classmethod
-    def finish_upload(cls, env: OSCAPISubDomain) -> str:
-        """this method returns a finish upload url"""
-        return _osc_url(env) + '/' + _version() + '/sequence/finished-uploading/'
+    # @classmethod
+    # def login(cls, env: OSCAPISubDomain, provider: str) -> Optional[str]:
+    #     """this method returns login URL"""
+    #     if provider == "google":
+    #         return _osc_url(env) + '/auth/google/client_auth'
+    #     if provider == "facebook":
+    #         return _osc_url(env) + '/auth/facebook/client_auth'
+    #     # default to OSM
+    #     return _osc_url(env) + '/auth/openstreetmap/client_auth'
 
 
 class OSCApi:
     """This class is a gateway for the API"""
 
     def __init__(self, env: OSCAPISubDomain):
         self.environment = env
@@ -162,48 +146,14 @@
         elif choice == 'no' or choice == 'n':
             print(f"{Fore.LIGHTRED_EX}Operation canceled.")
             exit()
         else:
             print("Invalid choice!")
             self.calculate_disk_space(total_items, path)
 
-    @classmethod
-    def __upload_response_success(cls, response: requests.Response,
-                                  upload_type: str,
-                                  index: int,
-                                  sequence_id: int) -> bool:
-        if response is None:
-            return False
-        try:
-            json_response = response.json()
-            if response.status_code != 200:
-                if "status" in json_response and \
-                        "apiMessage" in json_response["status"] and \
-                        "duplicate entry" in json_response["status"]["apiMessage"]:
-                    LOGGER.debug("Received duplicate %s index: %d, photo_id %s sequence_id %s",
-                                 upload_type,
-                                 index,
-                                 None,
-                                 sequence_id)
-                    return True
-                LOGGER.debug("Failed to upload %s index: %d response:%s sequence_id %s",
-                             upload_type,
-                             index,
-                             json_response,
-                             sequence_id)
-                return False
-
-            if ("osv" in json_response and
-                    (("photo" in json_response["osv"] and "id" in json_response["osv"]["photo"]) or
-                     ("video" in json_response["osv"] and "id" in json_response["osv"]["video"]))):
-                return True
-        except ValueError:
-            return False
-        return False
-
     def _sequence_page(self, user_name, page, pbar) -> Tuple[List[OSCSequence], Exception]:
         try:
             parameters = {'ipp': 500,
                           'page': page,
                           'username': user_name}
             login_url = OSCApiMethods.user_sequences(self.environment)
             response = requests.post(url=login_url, data=parameters)
@@ -221,58 +171,58 @@
             # Update the progress bar once per page
             pbar.update(1)
 
             return sequences, json_response, None
         except requests.RequestException as ex:
             return None, ex
 
-    def authorized_user(self, provider: str, token: str, secret: str) -> Tuple[OSCUser, Exception]:
-        """This method will get a authorization token for OSC API"""
-        try:
-            data_access = {'request_token': token,
-                           'secret_token': secret
-                           }
-            login_url = OSCApiMethods.login(self.environment, provider)
-            response = requests.post(url=login_url, data=data_access)
-            json_response = response.json()
-
-            if 'osv' in json_response:
-                osc_data = json_response['osv']
-                user = OSCUser()
-                missing_field = None
-                if 'access_token' in osc_data:
-                    user.access_token = osc_data['access_token']
-                else:
-                    missing_field = "access token"
-
-                if 'id' in osc_data:
-                    user.user_id = osc_data['id']
-                else:
-                    missing_field = "id"
-
-                if 'username' in osc_data:
-                    user.name = osc_data['username']
-                else:
-                    missing_field = "username"
-
-                if 'full_name' in osc_data:
-                    user.full_name = osc_data['full_name']
-                else:
-                    missing_field = "fullname"
-
-                if missing_field is not None:
-                    return None, Exception("OSC API bug. OSCUser missing " + missing_field)
-
-            else:
-                return None, Exception("OSC API bug. OSCUser missing username")
-
-        except requests.RequestException as ex:
-            return None, ex
-
-        return user, None
+    # def authorized_user(self, provider: str, token: str, secret: str) -> Tuple[OSCUser, Exception]:
+    #     """This method will get a authorization token for OSC API"""
+    #     try:
+    #         data_access = {'request_token': token,
+    #                        'secret_token': secret
+    #                        }
+    #         login_url = OSCApiMethods.login(self.environment, provider)
+    #         response = requests.post(url=login_url, data=data_access)
+    #         json_response = response.json()
+    #
+    #         if 'osv' in json_response:
+    #             osc_data = json_response['osv']
+    #             user = OSCUser()
+    #             missing_field = None
+    #             if 'access_token' in osc_data:
+    #                 user.access_token = osc_data['access_token']
+    #             else:
+    #                 missing_field = "access token"
+    #
+    #             if 'id' in osc_data:
+    #                 user.user_id = osc_data['id']
+    #             else:
+    #                 missing_field = "id"
+    #
+    #             if 'username' in osc_data:
+    #                 user.name = osc_data['username']
+    #             else:
+    #                 missing_field = "username"
+    #
+    #             if 'full_name' in osc_data:
+    #                 user.full_name = osc_data['full_name']
+    #             else:
+    #                 missing_field = "fullname"
+    #
+    #             if missing_field is not None:
+    #                 return None, Exception("OSC API bug. OSCUser missing " + missing_field)
+    #
+    #         else:
+    #             return None, Exception("OSC API bug. OSCUser missing username")
+    #
+    #     except requests.RequestException as ex:
+    #         return None, ex
+    #
+    #     return user, None
 
     def get_photos(self, sequence_id, page=None) -> Tuple[List[OSCPhoto], Optional[Exception]]:
         try:
             photo_url = OSCAPIResource.photo(self.environment)
             has_more_data = True
             photos = []
             current_page = page
@@ -332,33 +282,57 @@
                 with open(jpg_name, 'wb') as file:
                     response.raw.decode_content = True
                     shutil.copyfileobj(response.raw, file)
         except requests.RequestException as ex:
             return ex
         return None
 
-    def user_sequences(self, user_name: str, to_path: str) -> Tuple[List[OSCSequence], Exception]:
-        merged_json = f".{user_name}_merged_response.json"
-        if not os.path.exists(merged_json):
-            sequences, error = self._user_sequences(user_name, to_path)
+    def user_sequences(self, user_name: str) -> Tuple[List[OSCSequence], Exception]:
+        MERGED_RESPONSE = os.path.join(
+            os.path.expanduser("~"),
+            ".config",
+            "mapilio",
+            "configs",
+            "MapSyncer",
+            f"{user_name}_sequences_logs.json"
+        )
+        if not os.path.exists(MERGED_RESPONSE):
+            sequences, error = self._user_sequences(user_name)
         else:
             sequences = []
-            with open(merged_json, 'r') as f:
+            with open(MERGED_RESPONSE, 'r') as f:
                 responses = json.load(f)
             for r in responses:
                 response = responses[r]
                 if 'currentPageItems' in response:
                     items = response['currentPageItems']
                     for item in items:
                         sequence = OSCSequence.sequence_from_json(item)
                         sequences.append(sequence)
             error = None
         return sequences, error
 
-    def _user_sequences(self, user_name: str, to_path: str) -> Tuple[List[OSCSequence], Exception]:
+    def get_missing_sequences(self, user_name: str) -> Tuple[List[OSCSequence], Exception]:
+        MERGED_RESPONSE = os.path.join(
+            os.path.expanduser("~"),
+            ".config",
+            "mapilio",
+            "configs",
+            "MapSyncer",
+            f"{user_name}_sequences_logs.json"
+        )
+        if os.path.exists(MERGED_RESPONSE):
+            sequences, error = self._user_sequences(user_name)
+        else:
+            print("Json response not found")
+
+        return sequences, error
+
+
+    def _user_sequences(self, user_name: str) -> Tuple[List[OSCSequence], Exception]:
         """get all tracks for a user id """
         merged_json_response = {}
         print(
             f"Getting all sequences for user:{Fore.BLUE} {user_name}{Fore.RESET} from KartaView. It can take a while according to the number of sequences.")
         parameters = {'ipp': 500,
                       'page': 1,
                       'username': user_name}
@@ -374,31 +348,40 @@
             return [], Exception("OSC API bug missing totalFilteredItems from response")
 
         total_items = int(json_response['totalFilteredItems'][0])
         pages_count = int(total_items / parameters['ipp']) + 1
         print(
             f"{Fore.BLUE}Total count of images: {Fore.LIGHTBLUE_EX}{total_items}{Fore.RESET}{Fore.BLUE} Total count of pages: {Fore.LIGHTBLUE_EX}{pages_count}")
 
-        self.calculate_disk_space(total_items, to_path)
-
         sequences = []
         if 'currentPageItems' in json_response:
             for item in json_response['currentPageItems']:
                 sequences.append(OSCSequence.sequence_from_json(item))
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=10) as executor:
             loop = asyncio.new_event_loop()
-            print(f"{Fore.LIGHTCYAN_EX}Fetching from Kartaview is a singular event. Future synchronizations will be completed more swiftly. Feel free to focus on other tasks while we handle this for you ☕️.{Fore.RESET}")
+            print(
+                f"{Fore.LIGHTCYAN_EX}Fetching from Kartaview is a singular event. Future synchronizations will be completed more swiftly. Feel free to focus on other tasks while we handle this for you ☕️.{Fore.RESET}")
             pbar = tqdm(total=30, desc="Fetching sequences")  # Total is pages_count - 1 because range starts from 2
             futures = [
                 loop.run_in_executor(executor,
                                      self._sequence_page, user_name, page, pbar)
                 for page in range(2, 30)
             ]
-            with open(f".{user_name}_merged_response.json", "w") as file:
+
+            MERGED_RESPONSE = os.path.join(
+                os.path.expanduser("~"),
+                ".config",
+                "mapilio",
+                "configs",
+                "MapSyncer",
+                f"{user_name}_sequences_logs.json"
+            )
+
+            with open(MERGED_RESPONSE, "w") as file:
                 json.dump(merged_json_response, file)
 
             if not futures:
                 loop.close()
                 return sequences, None
 
             done = loop.run_until_complete(asyncio.gather(*futures))
@@ -408,15 +391,15 @@
             for idx, sequence_page_return in enumerate(done):
                 # sequence_page method will return a tuple the first element
                 # is a list of sequences
 
                 merged_json_response.update({str(idx + 1): sequence_page_return[1]})
 
                 sequences = sequences + sequence_page_return[0]
-            with open(f".{user_name}_merged_response.json", "w") as file:
+            with open(MERGED_RESPONSE, "w") as file:
                 json.dump(merged_json_response, file)
             return sequences, None
 
     def sequence_link(self, sequence) -> str:
         """This method will return a link to OSC website page displaying the sequence
         sent as parameter"""
         sequence_details_url = OSCApiMethods.sequence_details(self.environment)
@@ -468,15 +451,16 @@
                           override=False) -> Tuple[bool, Optional[Exception]]:
         if not override and storage.isfile(file_path):
             return True, None, None
         try:
             with requests.get(resource_url) as response:
                 response.raise_for_status()
                 storage.put(response.content, file_path + "partial")
-                storage.rename(file_path + "partial", file_path)
+                if os.path.exists(file_path + "partial"):
+                    storage.rename(file_path + "partial", file_path)
             return True, None, None
         except requests.exceptions.RequestException as ex:
             if isinstance(ex, requests.exceptions.HTTPError) and ex.response.status_code == 404:
                 modified_url = resource_url.replace("proc", "lth")
                 try:
                     with requests.get(modified_url) as response:
                         response.raise_for_status()
```

### Comparing `mapsyncer-0.0.9/MapSyncer/components/osc_api_models.py` & `mapsyncer-1.0.0/MapSyncer/components/osc_api_models.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/parsers/base.py` & `mapsyncer-1.0.0/MapSyncer/components/parsers/base.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/parsers/exif/exif.py` & `mapsyncer-1.0.0/MapSyncer/components/parsers/exif/exif.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/parsers/exif/utils.py` & `mapsyncer-1.0.0/MapSyncer/components/parsers/exif/utils.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/parsers/osc_metadata/parser.py` & `mapsyncer-1.0.0/MapSyncer/components/parsers/osc_metadata/parser.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/components/storage.py` & `mapsyncer-1.0.0/MapSyncer/components/storage.py`

 * *Files identical despite different names*

### Comparing `mapsyncer-0.0.9/MapSyncer/run.py` & `mapsyncer-1.0.0/MapSyncer/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 # run.py
 import os
+import shutil
 import json
-from MapSyncer.app import app as flask_app
 from mapilio_kit.components.login import list_all_users
 from mapilio_kit.components.edit_config import edit_config
 from mapilio_kit.base import authenticator
 from .components.download import download_user_images,flask_app
 import getpass
 from colorama import (Fore,
                       init as init_colorama)
 import requests
 from .components.version_ import __version__
 
+DOWNLOAD_LOGS = os.path.join(
+        os.path.expanduser("~"),
+        ".config",
+        "mapilio",
+        "configs",
+        "MapSyncer",
+        "download_logs.json"
+    )
+
+IMAGES_DOWNLOAD_PATH = os.path.join(
+        os.path.expanduser("~"),
+        ".cache",
+        "mapilio",
+        "MapSyncer",
+        "images"
+    )
+
 def get_latest_version():
     url = "https://raw.githubusercontent.com/mapilio/MapSyncer/main/MapSyncer/components/version_.py"
     response = requests.get(url)
     if response.status_code == 200:
         content = response.text
         version_line = [line for line in content.split('\n') if '__version__' in line][0]
         latest_version = version_line.split('"')[1]
@@ -31,44 +48,22 @@
             print(f'{Fore.RED}For latest MapSyncer version please update with "pip install mapsyncer --upgrade" \n')
         else:
             print(f"{Fore.GREEN}You have the latest MapSyncer version ({__version__}) installed.\n")
     else:
         print(f"{Fore.RED}Unable to fetch the latest MapSyncer version information.\n")
 
     init_colorama()
+
     print(f"{Fore.LIGHTCYAN_EX}To access the web interface of MapSyncer, simply navigate to the following URL:\n"
           f"http://localhost:5050/ in your web browser's address bar.\n{Fore.RESET}")
 
-    folder_path = input(f"{Fore.LIGHTYELLOW_EX}Please enter the path to the folder to download images to:\n{Fore.RESET}")
-    folder_path = folder_path.strip('\'"')
-
-    if 'mapilio_images' not in folder_path:
-        folder_path = os.path.join(folder_path, 'mapilio_images')
-        if not os.path.exists(folder_path):
-            os.makedirs(folder_path)
-
-    flask_app(folder_path)
-    download_user_images(folder_path)
-
-    check_authenticate = False
-
-    if len(list_all_users()) == 0:
-        check_authenticate = check_auth()
-    elif len(list_all_users()) >= 2:
-        username = input("Found multiple Mapilio accounts. Please specify your username.\n")
-    else:
-        check_authenticate = True
-
-    if check_authenticate:
+    if not os.path.exists(IMAGES_DOWNLOAD_PATH):
+        os.makedirs(IMAGES_DOWNLOAD_PATH)
 
-        if folder_path is not None and len(os.listdir(folder_path)) == 0:
-            print(f"{Fore.RED}Something went wrong. Please check your destination path.{Fore.RESET}")
-            exit()
-
-        folder_selection(folder_path)
+    flask_app(IMAGES_DOWNLOAD_PATH)
 
 
 def get_args_mapilio(func):
     arg_names = func.__code__.co_varnames[:func.__code__.co_argcount]
     return {arg: None for arg in arg_names}
 
 
@@ -94,50 +89,58 @@
         args["user_email"] = user_email
         args["user_password"] = user_password
         check_authenticate = authenticator().perform_task(args)
         if check_authenticate:
             return check_authenticate
         else:
             check_auth()
-
     else:
         print("Please enter your username, email and password properly \n\n\n\n\n")
         check_auth()
-
 def update_folder_status(folder_name_numeric, json_file):
     with open(json_file, 'r') as f:
         data = json.load(f)
         for folder in data:
             if folder.get('seq_id') == folder_name_numeric:
+                uploaded_path = os.path.join(IMAGES_DOWNLOAD_PATH, folder.get('seq_id'))
+                try:
+                    shutil.rmtree(uploaded_path)
+                except OSError as err:
+                    print(f"Error: {uploaded_path} could not be deleted. - {err}")
                 folder['upload_success'] = True
                 break
     with open(json_file, 'w') as f:
         json.dump(data, f, indent=2)
 
 def folder_selection(path):
     print("Choose an option:")
     print("1. Upload all folders")
     print("2. Upload a specific folder")
 
     choice = input(f"{Fore.LIGHTGREEN_EX}Enter your choice (1 or 2): {Fore.RESET}")
 
     if choice == '1':
         print(f"{Fore.LIGHTYELLOW_EX}Uploading all folders...")
-        json_file_path = ".download_logs.json"
         folders_to_upload = []
 
-        with open(json_file_path, 'r') as f:
+        with open(DOWNLOAD_LOGS, 'r') as f:
             data = json.load(f)
             for folder in data:
                 if not folder.get('json_success'):
                     print(f"{Fore.RED}The json file of the file with sequence id: {folder['seq_id']} was not found, please download the folder again.")
                     continue
                 elif not folder.get('upload_success'):
                     folders_to_upload.append(folder.get('seq_id'))
 
+        files = os.listdir(path)
+        for file in files:
+            file_path = os.path.join(path, file)
+            if os.path.isfile(file_path):
+                os.remove(file_path)
+
         for folder_name in os.listdir(path):
             folder_path = os.path.join(path, folder_name)
             if len(os.listdir(folder_path)) < 5:
                 continue
 
             folder_name_numeric = ''.join(filter(str.isdigit, folder_name))
 
@@ -145,43 +148,42 @@
                 upload_command = f"mapilio_kit upload --processed {folder_path}"
                 result = os.system(upload_command)
 
                 if result != 0:
                     print(f"{Fore.RED}Error occurred while uploading {folder_path}")
                     continue
 
-                update_folder_status(folder_name_numeric, json_file_path)
+            update_folder_status(folder_name_numeric, DOWNLOAD_LOGS)
         print(f"{Fore.LIGHTGREEN_EX}All folders uploaded. 🎉")
 
     elif choice == '2':
         print(f"{Fore.BLUE}Available folders: {Fore.RESET}")
         print_folder_structure(path)
 
         folder_name = input("Enter the specific folder name: ")
         folder_name_numeric = ''.join(filter(str.isdigit, folder_name))
         print(f"{Fore.YELLOW}Uploading folder '{folder_name_numeric}'... {Fore.RESET}")
 
         upload_command = f"mapilio_kit upload --processed {path + '/' + folder_name_numeric}"
-        json_file_path = ".download_logs.json"
-        with open(json_file_path, 'r') as f:
+        with open(DOWNLOAD_LOGS, 'r') as f:
             data = json.load(f)
             for folder in data:
                 if folder.get('seq_id') == folder_name_numeric:
                     if folder.get('upload_success') == True:
                         print(f"{Fore.LIGHTGREEN_EX}Folder '{folder_name_numeric}' was already uploaded 🎉.{Fore.RESET}")
                         folder_selection(path)
                     elif folder.get('json_success') == False:
                         print(f"{Fore.RED}The json file of the file with sequence id: {folder['seq_id']} was not found, please download the folder again.")
                         folder_selection(path)
         result = os.system(upload_command)
 
         if result != 0:
             print(f"{Fore.RED}Error occurred while uploading {folder_name_numeric}")
         else:
-            update_folder_status(folder_name_numeric, json_file_path)
+            update_folder_status(folder_name_numeric, DOWNLOAD_LOGS)
 
         folder_selection(path)
 
     else:
         print(f"{Fore.RED}Invalid choice. Please enter 1 or 2.{Fore.RESET}")
         folder_selection(path)
```

### Comparing `mapsyncer-0.0.9/PKG-INFO` & `mapsyncer-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mapsyncer
-Version: 0.0.9
+Version: 1.0.0
 Summary: A toolkit to download and upload the data from KartaView to Mapilio
 Home-page: https://github.com/mapilio/MapSyncer
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mapilio-kit
 Requires-Dist: ExifRead
 Requires-Dist: calculation-mapilio==0.1.39
 Requires-Dist: requests_oauthlib
-Requires-Dist: opencv-python
 Requires-Dist: imagesize
 Requires-Dist: setuptools
 Requires-Dist: psutil
 Requires-Dist: flask
 Requires-Dist: python-dotenv
+Requires-Dist: osm-login-python
 
 <div align="center">
    <a href="https://mapilio.com/" target="_blank">
    <img width="100%" src="https://github.com/mapilio/MapSyncer/blob/main/docs/assets/mapsyncer-banner2.png"></a>
 </div>
 
 <div align="center">
@@ -49,24 +49,22 @@
 
 This repository provides a streamlined process for downloading user images from Kartaview and uploading them to Mapilio.<br>
 
 Please, follow the steps below to get started:
 
 
 ## Workflow
-The download command follows these steps below:
-
-1. Authenticate the user with OpenStreetMap (OSM) account via Kartaview.
-2. Get the list of sequences uploaded by the user.
-3. Download all images and metadata for each sequence.
-4. Authenticate for Mapilio.
-5. You can select the specific sequences you want to upload to Mapilio or all downloaded sequences.
+1. Authenticate for OpenStreetMap.
+2. Authenticate for Mapilio.
+3. Get the list of sequences uploaded by the user.
+4. Download all images and metadata for each sequence.
+5. You can select specific sequences or all downloaded sequences that you want to upload to Mapilio.
 6. And the process ends successfully.
 
-Don't worry, run.py will lead all this for you 💫. 
+Don't worry, the RunMapSyncer command will check and do all these operations. 💫
 
 
 ## Install dependencies
 
 MapSyncer depends on the following libraries that need to be installed before building it.<br>
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
@@ -80,14 +78,17 @@
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
 ```
+<p>
+   When accessing the provided address, you may encounter a security warning stating <b>"Your connection is not private"</b> in your web browser. To proceed, please click the <b>"Advanced"</b> button and select the option to continue to the site. This warning is due to the SSL certificate currently being in the process of approval and will be validated shortly.
+</p>
 
 ## Manual Installation
 
 1. Clone the **MapSyncer** repository:
 
 ```bash
 git clone https://github.com/mapilio/MapSyncer.git
@@ -95,35 +96,33 @@
 ```
 
 2. Create Virtualenv **(Optional)**:
 
 ```bash
 python -m venv mapsyncer_env
 
-# Ubuntu 
+# Ubuntu & MacOS
 source mapsyncer_env/bin/activate
 
 # Windows
 mapsyncer_env/Scripts/activate
 ```
 
 3. Install the required dependencies:
 
 ```bash 
-pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Usage
 
 The whole process will take place in one line 
 
 ```bash
-cd MapSyncer
-
-python run.py
+RunMapSyncer
 ```
 
 Then you can start the whole process by giving the **folder path** where you would like to download your images 💥.
 
 
 ## Clean Up
```

#### html2text {}

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1 Name: mapsyncer Version: 0.0.9 Summary: A toolkit to
+Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.0 Summary: A toolkit to
 download and upload the data from KartaView to Mapilio Home-page: https://
 github.com/mapilio/MapSyncer Author: Mapilio License: MIT License Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: mapilio-kit Requires-Dist: ExifRead Requires-Dist: calculation-
-mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: opencv-python
-Requires-Dist: imagesize Requires-Dist: setuptools Requires-Dist: psutil
-Requires-Dist: flask Requires-Dist: python-dotenv
+mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: imagesize
+Requires-Dist: setuptools Requires-Dist: psutil Requires-Dist: flask Requires-
+Dist: python-dotenv Requires-Dist: osm-login-python
     _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_m_a_p_i_l_i_o_/_M_a_p_S_y_n_c_e_r_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_m_a_p_s_y_n_c_e_r_-
                                  _b_a_n_n_e_r_2_._p_n_g_]
  _[_M_a_p_S_y_n_c_e_r_ _C_I_]_[_m_i_t_-_l_i_c_e_n_s_e_]_[_d_i_s_c_o_r_d_-_b_a_d_g_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_][stars][contributors]
             [issue-counter][release-date-badge][last-commit-badge]
 # MapSyncer This repository provides a streamlined process for downloading user
 images from Kartaview and uploading them to Mapilio.
-Please, follow the steps below to get started: ## Workflow The download command
-follows these steps below: 1. Authenticate the user with OpenStreetMap (OSM)
-account via Kartaview. 2. Get the list of sequences uploaded by the user. 3.
-Download all images and metadata for each sequence. 4. Authenticate for
-Mapilio. 5. You can select the specific sequences you want to upload to Mapilio
-or all downloaded sequences. 6. And the process ends successfully. Don't worry,
-run.py will lead all this for you ð«. ## Install dependencies MapSyncer
-depends on the following libraries that need to be installed before building
-it.
+Please, follow the steps below to get started: ## Workflow 1. Authenticate for
+OpenStreetMap. 2. Authenticate for Mapilio. 3. Get the list of sequences
+uploaded by the user. 4. Download all images and metadata for each sequence. 5.
+You can select specific sequences or all downloaded sequences that you want to
+upload to Mapilio. 6. And the process ends successfully. Don't worry, the
+RunMapSyncer command will check and do all these operations. ð« ## Install
+dependencies MapSyncer depends on the following libraries that need to be
+installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
 (https://exiftool.org/install.html) ## Pip Installation and Usage You may
 simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ``` ## Manual
-Installation 1. Clone the **MapSyncer** repository: ```bash git clone https://
-github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv **
-(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu source
+Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+When accessing the provided address, you may encounter a security warning
+stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
+please click the ""AAddvvaanncceedd"" button and select the option to continue to the
+site. This warning is due to the SSL certificate currently being in the process
+of approval and will be validated shortly.
+## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
+https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
+**(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu & MacOS source
 mapsyncer_env/bin/activate # Windows mapsyncer_env/Scripts/activate ``` 3.
-Install the required dependencies: ```bash pip install -r requirements.txt ```
-## Usage The whole process will take place in one line ```bash cd MapSyncer
-python run.py ``` Then you can start the whole process by giving the **folder
-path** where you would like to download your images ð¥. ## Clean Up If you
-need to remove and uninstall everything except images, please refer to the
-[Clean Up instructions](CleanUp.md). ## Contributing If you encounter issues or
-have suggestions for improvements, please report them on the GitHub repository
-ð. ## License This project is licensed under the [MIT License](https://
-github.com/mapilio/MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact
-Feel free to reach out [GitHub Issues]() if you have any questions,
-contribution idea or need further assistance!
+Install the required dependencies: ```bash pip install -e . ``` ## Usage The
+whole process will take place in one line ```bash RunMapSyncer ``` Then you can
+start the whole process by giving the **folder path** where you would like to
+download your images ð¥. ## Clean Up If you need to remove and uninstall
+everything except images, please refer to the [Clean Up instructions]
+(CleanUp.md). ## Contributing If you encounter issues or have suggestions for
+improvements, please report them on the GitHub repository ð. ## License This
+project is licensed under the [MIT License](https://github.com/mapilio/
+MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact Feel free to reach
+out [GitHub Issues]() if you have any questions, contribution idea or need
+further assistance!
 [Mapilio](https://mapilio.com/) is everywhere in the world! ð
```

### Comparing `mapsyncer-0.0.9/README.md` & `mapsyncer-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,22 @@
 
 This repository provides a streamlined process for downloading user images from Kartaview and uploading them to Mapilio.<br>
 
 Please, follow the steps below to get started:
 
 
 ## Workflow
-The download command follows these steps below:
-
-1. Authenticate the user with OpenStreetMap (OSM) account via Kartaview.
-2. Get the list of sequences uploaded by the user.
-3. Download all images and metadata for each sequence.
-4. Authenticate for Mapilio.
-5. You can select the specific sequences you want to upload to Mapilio or all downloaded sequences.
+1. Authenticate for OpenStreetMap.
+2. Authenticate for Mapilio.
+3. Get the list of sequences uploaded by the user.
+4. Download all images and metadata for each sequence.
+5. You can select specific sequences or all downloaded sequences that you want to upload to Mapilio.
 6. And the process ends successfully.
 
-Don't worry, run.py will lead all this for you 💫. 
+Don't worry, the RunMapSyncer command will check and do all these operations. 💫
 
 
 ## Install dependencies
 
 MapSyncer depends on the following libraries that need to be installed before building it.<br>
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
@@ -59,14 +57,17 @@
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
 ```
+<p>
+   When accessing the provided address, you may encounter a security warning stating <b>"Your connection is not private"</b> in your web browser. To proceed, please click the <b>"Advanced"</b> button and select the option to continue to the site. This warning is due to the SSL certificate currently being in the process of approval and will be validated shortly.
+</p>
 
 ## Manual Installation
 
 1. Clone the **MapSyncer** repository:
 
 ```bash
 git clone https://github.com/mapilio/MapSyncer.git
@@ -74,35 +75,33 @@
 ```
 
 2. Create Virtualenv **(Optional)**:
 
 ```bash
 python -m venv mapsyncer_env
 
-# Ubuntu 
+# Ubuntu & MacOS
 source mapsyncer_env/bin/activate
 
 # Windows
 mapsyncer_env/Scripts/activate
 ```
 
 3. Install the required dependencies:
 
 ```bash 
-pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Usage
 
 The whole process will take place in one line 
 
 ```bash
-cd MapSyncer
-
-python run.py
+RunMapSyncer
 ```
 
 Then you can start the whole process by giving the **folder path** where you would like to download your images 💥.
 
 
 ## Clean Up
```

#### html2text {}

```diff
@@ -1,36 +1,40 @@
     _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_m_a_p_i_l_i_o_/_M_a_p_S_y_n_c_e_r_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_m_a_p_s_y_n_c_e_r_-
                                  _b_a_n_n_e_r_2_._p_n_g_]
  _[_M_a_p_S_y_n_c_e_r_ _C_I_]_[_m_i_t_-_l_i_c_e_n_s_e_]_[_d_i_s_c_o_r_d_-_b_a_d_g_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_][stars][contributors]
             [issue-counter][release-date-badge][last-commit-badge]
 # MapSyncer This repository provides a streamlined process for downloading user
 images from Kartaview and uploading them to Mapilio.
-Please, follow the steps below to get started: ## Workflow The download command
-follows these steps below: 1. Authenticate the user with OpenStreetMap (OSM)
-account via Kartaview. 2. Get the list of sequences uploaded by the user. 3.
-Download all images and metadata for each sequence. 4. Authenticate for
-Mapilio. 5. You can select the specific sequences you want to upload to Mapilio
-or all downloaded sequences. 6. And the process ends successfully. Don't worry,
-run.py will lead all this for you ð«. ## Install dependencies MapSyncer
-depends on the following libraries that need to be installed before building
-it.
+Please, follow the steps below to get started: ## Workflow 1. Authenticate for
+OpenStreetMap. 2. Authenticate for Mapilio. 3. Get the list of sequences
+uploaded by the user. 4. Download all images and metadata for each sequence. 5.
+You can select specific sequences or all downloaded sequences that you want to
+upload to Mapilio. 6. And the process ends successfully. Don't worry, the
+RunMapSyncer command will check and do all these operations. ð« ## Install
+dependencies MapSyncer depends on the following libraries that need to be
+installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
 (https://exiftool.org/install.html) ## Pip Installation and Usage You may
 simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ``` ## Manual
-Installation 1. Clone the **MapSyncer** repository: ```bash git clone https://
-github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv **
-(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu source
+Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+When accessing the provided address, you may encounter a security warning
+stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
+please click the ""AAddvvaanncceedd"" button and select the option to continue to the
+site. This warning is due to the SSL certificate currently being in the process
+of approval and will be validated shortly.
+## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
+https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
+**(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu & MacOS source
 mapsyncer_env/bin/activate # Windows mapsyncer_env/Scripts/activate ``` 3.
-Install the required dependencies: ```bash pip install -r requirements.txt ```
-## Usage The whole process will take place in one line ```bash cd MapSyncer
-python run.py ``` Then you can start the whole process by giving the **folder
-path** where you would like to download your images ð¥. ## Clean Up If you
-need to remove and uninstall everything except images, please refer to the
-[Clean Up instructions](CleanUp.md). ## Contributing If you encounter issues or
-have suggestions for improvements, please report them on the GitHub repository
-ð. ## License This project is licensed under the [MIT License](https://
-github.com/mapilio/MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact
-Feel free to reach out [GitHub Issues]() if you have any questions,
-contribution idea or need further assistance!
+Install the required dependencies: ```bash pip install -e . ``` ## Usage The
+whole process will take place in one line ```bash RunMapSyncer ``` Then you can
+start the whole process by giving the **folder path** where you would like to
+download your images ð¥. ## Clean Up If you need to remove and uninstall
+everything except images, please refer to the [Clean Up instructions]
+(CleanUp.md). ## Contributing If you encounter issues or have suggestions for
+improvements, please report them on the GitHub repository ð. ## License This
+project is licensed under the [MIT License](https://github.com/mapilio/
+MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact Feel free to reach
+out [GitHub Issues]() if you have any questions, contribution idea or need
+further assistance!
 [Mapilio](https://mapilio.com/) is everywhere in the world! ð
```

### Comparing `mapsyncer-0.0.9/mapsyncer.egg-info/PKG-INFO` & `mapsyncer-1.0.0/mapsyncer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mapsyncer
-Version: 0.0.9
+Version: 1.0.0
 Summary: A toolkit to download and upload the data from KartaView to Mapilio
 Home-page: https://github.com/mapilio/MapSyncer
 Author: Mapilio
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mapilio-kit
 Requires-Dist: ExifRead
 Requires-Dist: calculation-mapilio==0.1.39
 Requires-Dist: requests_oauthlib
-Requires-Dist: opencv-python
 Requires-Dist: imagesize
 Requires-Dist: setuptools
 Requires-Dist: psutil
 Requires-Dist: flask
 Requires-Dist: python-dotenv
+Requires-Dist: osm-login-python
 
 <div align="center">
    <a href="https://mapilio.com/" target="_blank">
    <img width="100%" src="https://github.com/mapilio/MapSyncer/blob/main/docs/assets/mapsyncer-banner2.png"></a>
 </div>
 
 <div align="center">
@@ -49,24 +49,22 @@
 
 This repository provides a streamlined process for downloading user images from Kartaview and uploading them to Mapilio.<br>
 
 Please, follow the steps below to get started:
 
 
 ## Workflow
-The download command follows these steps below:
-
-1. Authenticate the user with OpenStreetMap (OSM) account via Kartaview.
-2. Get the list of sequences uploaded by the user.
-3. Download all images and metadata for each sequence.
-4. Authenticate for Mapilio.
-5. You can select the specific sequences you want to upload to Mapilio or all downloaded sequences.
+1. Authenticate for OpenStreetMap.
+2. Authenticate for Mapilio.
+3. Get the list of sequences uploaded by the user.
+4. Download all images and metadata for each sequence.
+5. You can select specific sequences or all downloaded sequences that you want to upload to Mapilio.
 6. And the process ends successfully.
 
-Don't worry, run.py will lead all this for you 💫. 
+Don't worry, the RunMapSyncer command will check and do all these operations. 💫
 
 
 ## Install dependencies
 
 MapSyncer depends on the following libraries that need to be installed before building it.<br>
 
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like to follow the manual way you should install mapilio-kit manually.`
@@ -80,14 +78,17 @@
 ```bash
 # Installation
 pip install mapsyncer
 
 # CLI Usage
 RunMapSyncer
 ```
+<p>
+   When accessing the provided address, you may encounter a security warning stating <b>"Your connection is not private"</b> in your web browser. To proceed, please click the <b>"Advanced"</b> button and select the option to continue to the site. This warning is due to the SSL certificate currently being in the process of approval and will be validated shortly.
+</p>
 
 ## Manual Installation
 
 1. Clone the **MapSyncer** repository:
 
 ```bash
 git clone https://github.com/mapilio/MapSyncer.git
@@ -95,35 +96,33 @@
 ```
 
 2. Create Virtualenv **(Optional)**:
 
 ```bash
 python -m venv mapsyncer_env
 
-# Ubuntu 
+# Ubuntu & MacOS
 source mapsyncer_env/bin/activate
 
 # Windows
 mapsyncer_env/Scripts/activate
 ```
 
 3. Install the required dependencies:
 
 ```bash 
-pip install -r requirements.txt
+pip install -e .
 ```
 
 ## Usage
 
 The whole process will take place in one line 
 
 ```bash
-cd MapSyncer
-
-python run.py
+RunMapSyncer
 ```
 
 Then you can start the whole process by giving the **folder path** where you would like to download your images 💥.
 
 
 ## Clean Up
```

#### html2text {}

```diff
@@ -1,44 +1,48 @@
-Metadata-Version: 2.1 Name: mapsyncer Version: 0.0.9 Summary: A toolkit to
+Metadata-Version: 2.1 Name: mapsyncer Version: 1.0.0 Summary: A toolkit to
 download and upload the data from KartaView to Mapilio Home-page: https://
 github.com/mapilio/MapSyncer Author: Mapilio License: MIT License Requires-
 Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: mapilio-kit Requires-Dist: ExifRead Requires-Dist: calculation-
-mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: opencv-python
-Requires-Dist: imagesize Requires-Dist: setuptools Requires-Dist: psutil
-Requires-Dist: flask Requires-Dist: python-dotenv
+mapilio==0.1.39 Requires-Dist: requests_oauthlib Requires-Dist: imagesize
+Requires-Dist: setuptools Requires-Dist: psutil Requires-Dist: flask Requires-
+Dist: python-dotenv Requires-Dist: osm-login-python
     _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_m_a_p_i_l_i_o_/_M_a_p_S_y_n_c_e_r_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_a_s_s_e_t_s_/_m_a_p_s_y_n_c_e_r_-
                                  _b_a_n_n_e_r_2_._p_n_g_]
  _[_M_a_p_S_y_n_c_e_r_ _C_I_]_[_m_i_t_-_l_i_c_e_n_s_e_]_[_d_i_s_c_o_r_d_-_b_a_d_g_e_]_[_P_y_P_I_ _v_e_r_s_i_o_n_][stars][contributors]
             [issue-counter][release-date-badge][last-commit-badge]
 # MapSyncer This repository provides a streamlined process for downloading user
 images from Kartaview and uploading them to Mapilio.
-Please, follow the steps below to get started: ## Workflow The download command
-follows these steps below: 1. Authenticate the user with OpenStreetMap (OSM)
-account via Kartaview. 2. Get the list of sequences uploaded by the user. 3.
-Download all images and metadata for each sequence. 4. Authenticate for
-Mapilio. 5. You can select the specific sequences you want to upload to Mapilio
-or all downloaded sequences. 6. And the process ends successfully. Don't worry,
-run.py will lead all this for you ð«. ## Install dependencies MapSyncer
-depends on the following libraries that need to be installed before building
-it.
+Please, follow the steps below to get started: ## Workflow 1. Authenticate for
+OpenStreetMap. 2. Authenticate for Mapilio. 3. Get the list of sequences
+uploaded by the user. 4. Download all images and metadata for each sequence. 5.
+You can select specific sequences or all downloaded sequences that you want to
+upload to Mapilio. 6. And the process ends successfully. Don't worry, the
+RunMapSyncer command will check and do all these operations. ð« ## Install
+dependencies MapSyncer depends on the following libraries that need to be
+installed before building it.
 * [Mapilio Kit](https://github.com/mapilio/mapilio-kit) `In case you would like
 to follow the manual way you should install mapilio-kit manually.` * [Exiftool]
 (https://exiftool.org/install.html) ## Pip Installation and Usage You may
 simply install and use the MapSyncer by using these commands below; ```bash #
-Installation pip install mapsyncer # CLI Usage RunMapSyncer ``` ## Manual
-Installation 1. Clone the **MapSyncer** repository: ```bash git clone https://
-github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv **
-(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu source
+Installation pip install mapsyncer # CLI Usage RunMapSyncer ```
+When accessing the provided address, you may encounter a security warning
+stating ""YYoouurr ccoonnnneeccttiioonn iiss nnoott pprriivvaattee"" in your web browser. To proceed,
+please click the ""AAddvvaanncceedd"" button and select the option to continue to the
+site. This warning is due to the SSL certificate currently being in the process
+of approval and will be validated shortly.
+## Manual Installation 1. Clone the **MapSyncer** repository: ```bash git clone
+https://github.com/mapilio/MapSyncer.git cd MapSyncer ``` 2. Create Virtualenv
+**(Optional)**: ```bash python -m venv mapsyncer_env # Ubuntu & MacOS source
 mapsyncer_env/bin/activate # Windows mapsyncer_env/Scripts/activate ``` 3.
-Install the required dependencies: ```bash pip install -r requirements.txt ```
-## Usage The whole process will take place in one line ```bash cd MapSyncer
-python run.py ``` Then you can start the whole process by giving the **folder
-path** where you would like to download your images ð¥. ## Clean Up If you
-need to remove and uninstall everything except images, please refer to the
-[Clean Up instructions](CleanUp.md). ## Contributing If you encounter issues or
-have suggestions for improvements, please report them on the GitHub repository
-ð. ## License This project is licensed under the [MIT License](https://
-github.com/mapilio/MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact
-Feel free to reach out [GitHub Issues]() if you have any questions,
-contribution idea or need further assistance!
+Install the required dependencies: ```bash pip install -e . ``` ## Usage The
+whole process will take place in one line ```bash RunMapSyncer ``` Then you can
+start the whole process by giving the **folder path** where you would like to
+download your images ð¥. ## Clean Up If you need to remove and uninstall
+everything except images, please refer to the [Clean Up instructions]
+(CleanUp.md). ## Contributing If you encounter issues or have suggestions for
+improvements, please report them on the GitHub repository ð. ## License This
+project is licensed under the [MIT License](https://github.com/mapilio/
+MapSyncer?tab=MIT-1-ov-file). ## Contributions and Contact Feel free to reach
+out [GitHub Issues]() if you have any questions, contribution idea or need
+further assistance!
 [Mapilio](https://mapilio.com/) is everywhere in the world! ð
```

### Comparing `mapsyncer-0.0.9/mapsyncer.egg-info/SOURCES.txt` & `mapsyncer-1.0.0/mapsyncer.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 MapSyncer/app.py
 MapSyncer/run.py
 MapSyncer/components/__init__.py
 MapSyncer/components/common_models.py
 MapSyncer/components/constants.py
 MapSyncer/components/download.py
 MapSyncer/components/get_exif.py
-MapSyncer/components/login_controller.py
 MapSyncer/components/osc_api_config.py
 MapSyncer/components/osc_api_gateway.py
 MapSyncer/components/osc_api_models.py
-MapSyncer/components/osm_access.py
+MapSyncer/components/ssl.py
 MapSyncer/components/storage.py
 MapSyncer/components/version_.py
 MapSyncer/components/parsers/__init__.py
 MapSyncer/components/parsers/base.py
 MapSyncer/components/parsers/exif/__init__.py
 MapSyncer/components/parsers/exif/exif.py
 MapSyncer/components/parsers/exif/utils.py
 MapSyncer/components/parsers/osc_metadata/__init__.py
 MapSyncer/components/parsers/osc_metadata/parser.py
+MapSyncer/static/__init__.py
+MapSyncer/static/app.js
+MapSyncer/static/edit-sequence.js
+MapSyncer/static/global.js
+MapSyncer/static/mapilio_fav.png
+MapSyncer/templates/__init__.py
+MapSyncer/templates/details.html
+MapSyncer/templates/display-sequence.html
+MapSyncer/templates/kartaview-login.html
+MapSyncer/templates/mapilio-login.html
+MapSyncer/templates/sequence-edit.html
 mapsyncer.egg-info/PKG-INFO
 mapsyncer.egg-info/SOURCES.txt
 mapsyncer.egg-info/dependency_links.txt
 mapsyncer.egg-info/entry_points.txt
 mapsyncer.egg-info/requires.txt
 mapsyncer.egg-info/top_level.txt
```

### Comparing `mapsyncer-0.0.9/setup.py` & `mapsyncer-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,45 +6,53 @@
 
 
 def get_long_desc():
     basedir = os.path.abspath(os.path.dirname(__file__))
     with io.open(os.path.join(basedir, "README.md"), encoding="utf-8") as f:
         return f.read()
 
+
 def get_version():
     cwd = os.path.abspath(os.path.dirname(__file__))
     current_version = os.path.join(cwd, "MapSyncer", "components", "version_.py")
     with io.open(current_version, encoding="utf-8") as f:
         return re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', f.read(), re.M).group(1)
 
+
 # TODO: This part will be removed with an alternative solution.
 INSTALL_REQUIRES = [
     'mapilio-kit',
     'ExifRead',
     'calculation-mapilio==0.1.39',
     'requests_oauthlib',
-    'opencv-python',
     'imagesize',
     'setuptools',
     'psutil',
     'flask',
-    'python-dotenv'
-
+    'python-dotenv',
+    'osm-login-python'
 ]
 
 setuptools.setup(
     name="mapsyncer",
     version=get_version(),
     author="Mapilio",
     description="A toolkit to download and upload the data from KartaView to Mapilio",
     long_description=get_long_desc(),
     long_description_content_type='text/markdown',
     url="https://github.com/mapilio/MapSyncer",
+    packages=setuptools.find_packages(),
+    package_data={
+        'MapSyncer': [
+            'static/*',
+            'templates/*'
+        ]
+    },
     license='MIT License',
     python_requires='>=3.6',
     install_requires=INSTALL_REQUIRES,
     entry_points={
         "console_scripts": [
-            "RunMapSyncer=MapSyncer.run:main"
+            "RunMapSyncer=MapSyncer.app:main"
         ]
     }
 )
```

