# Comparing `tmp/scsd-0.0.71.tar.gz` & `tmp/scsd-0.0.8.tar.gz`

## Comparing `scsd-0.0.71.tar` & `scsd-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,21 @@
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 scsd-0.0.71/.pre-commit-config.yaml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 scsd-0.0.71/Dockerfile
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scsd-0.0.71/requirements-dev.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 scsd-0.0.71/requirements.txt
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.71/scsd
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scsd-0.0.71/scsd.conf.sample
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 scsd-0.0.71/version.txt
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 scsd-0.0.71/.github/workflows/check-test-build.yml
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 scsd-0.0.71/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 scsd-0.0.71/docker/entry.sh
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scsd-0.0.71/docker/run.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 scsd-0.0.71/docker/scsd_auth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/__init__.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/__main__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/args.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/auth.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/config.py
--rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/db.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/err.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/notifier.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/parser.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/storage.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/stored.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/summary.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/ver.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 scsd-0.0.71/steamCloudSaveDownloader/web.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 scsd-0.0.71/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.71/LICENSE
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 scsd-0.0.71/README.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 scsd-0.0.71/pyproject.toml
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 scsd-0.0.71/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 scsd-0.0.8/Dockerfile
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 scsd-0.0.8/requirements.txt
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 scsd-0.0.8/scsd
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scsd-0.0.8/scsd.conf.sample
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 scsd-0.0.8/docker/cron-root
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/__main__.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/args.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/auth.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/config.py
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/db.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/err.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/notifier.py
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/parser.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/storage.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 scsd-0.0.8/steamCloudSaveDownloader/web.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 scsd-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 scsd-0.0.8/LICENSE
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 scsd-0.0.8/README.md
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 scsd-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 scsd-0.0.8/PKG-INFO
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/args.py` & `scsd-0.0.8/steamCloudSaveDownloader/args.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,100 @@
 import argparse
 import os
 import pathlib
 import logging
 from .notifier import notifier
 from . import config
-from . import ver
 
 class args:
     def __init__(self):
         self.parser = argparse.ArgumentParser(
             formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
+        # Config file has highest priority
         self.parser.add_argument(
             "-f",
             metavar="conf",
             dest="conf",
             type=self.is_file,
             default="",
-            help="Path to config file. If given, use the settings and the command arguments will override if same option is specified as well"
+            help="Path to config file. If given, use the settings and ignore all command arguments"
         )
 
+        options, remainder = self.parser.parse_known_args()
+
+        # Break if config file is given
+        if options.conf is not None:
+            return
+
         self.parser.add_argument(
             "-a",
             metavar="username",
             type=str,
             dest="auth",
             help="Save authentication"
         )
 
         self.parser.add_argument(
-            "-v",
-            "--version",
-            dest="version",
-            action='version',
-            version='%(prog)s-{version}'.format(version=ver.__version__)
-        )
-
-        self.parser.add_argument(
             "-d",
             metavar="save_dir",
             dest="save_dir",
-            type=str,
-            default=config.Defaults['General']['save_dir'][1],
+            type=self.is_path,
+            required=True,
             help="Directory to save the downloaded saves and db"
         )
 
         self.parser.add_argument(
             "-r",
             metavar="rotation_count",
             dest="rotation",
             type=int,
-            default=config.Defaults['Rotation']['rotation'][1],
+            default=config.Defaults['rotation'],
             help="The amount of version for each file to keep"
         )
 
         self.parser.add_argument(
             "-l",
             metavar="log_level",
             dest="log_level",
             type=int,
-            default=config.Defaults['Log']['log_level'][1],
+            default=config.Defaults['log_level'],
             help="How detail should the log be"
         )
 
         self.parser.add_argument(
-            "-s",
-            nargs="?",
-            metavar="[app_id1,app_id2,...]",
-            dest="stored",
-            type=self.is_int_list, # TODO array type
-            default=[-1],
-            help="Show the files saved locally"
+            "-n",
+            metavar="notifier",
+            dest="notifier",
+            type=self.supported_notifier,
+            default=config.Defaults['notifier'],
+            help="Supported notifier: Discord"
+        )
+
+        self.parser.add_argument(
+            "--webhook",
+            metavar="webhook",
+            dest="webhook",
+            default=config.Defaults['webhook'],
+            required=False,
+            help="Notifier option"
         )
 
     def convert_log_level(level:int):
         if (level == 0):
             return logging.ERROR
         elif (level == 1):
             return logging.WARNING
         elif (level == 2):
             return logging.INFO
         else:
             return logging.DEBUG
 
+
+
     def parse(self, raw_args):
         parsed_args = self.parser.parse_args(raw_args)
         return vars(parsed_args)
 
     def supported_notifier(self, arg):
         if notifier.is_supported(arg):
             return arg
@@ -102,14 +110,7 @@
             self.parser.error(f"The config file '{arg}' does not exist.")
 
     def is_path(self, arg):
         if os.path.isdir(arg):
             return pathlib.Path(arg)
         else:
             self.parser.error(f"The directory '{arg}' does not exist.")
-
-    def is_int_list(self, arg):
-        tokens = arg.split(',')
-        try:
-            return [int(token) for token in tokens]
-        except:
-            self.parser.error(f"The appid list '{arg}' is invalid. Should be 'app_id1,app_id2,...'")
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/db.py` & `scsd-0.0.8/steamCloudSaveDownloader/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,58 +21,41 @@
 
 TABLE VERSION
 version_id (INT) PK AUTOINC
 file_id foreign key
 time (datetime)
 version_num (INT) >= 0
 
-TABLE REQUESTS
-id (INT) PK NOT NULL DEFAULT 0
-time (datetime)
-count (int)
-## Enforce single row
-
-
 '''
-
 logger = logging.getLogger('scsd')
-
 class db:
-    requests_limit = 85000
-    def __init__(self, db_location:str, rotation:int=0):
+    def __init__(self, db_location:str, rotation:int):
         self.location = db_location
         self.rotation = rotation
         self.db_file = os.path.join(db_location, DB_FILENAME)
 
         self.con = sqlite3.connect(self.db_file, detect_types=sqlite3.PARSE_DECLTYPES)
 
         if not self.schema_ok():
             self.initialize_schema()
 
     def __del__(self):
         if hasattr(self, 'con'):
             self.con.close()
 
-    def commit(self):
-        self.con.commit()
-
     def schema_ok(self) -> bool:
         cur = self.con.cursor()
         res = cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='GAMES';")
         if res.fetchone() is None:
             return False
 
         res = cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='FILES';")
         if res.fetchone() is None:
             return False
 
-        res = cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='REQUESTS';")
-        if res.fetchone() is None:
-            return False
-
         res = cur.execute("SELECT name FROM sqlite_master WHERE type='table' AND name='VERSION';")
         if res.fetchone() is None:
             return False
 
         return True
 
     def initialize_schema(self):
@@ -99,48 +82,17 @@
             "  version_id INTEGER PRIMARY KEY AUTOINCREMENT,"
             "  file_id INTEGER,"
             "  time timestamp,"
             "  version_num INTEGER CHECK (version_num>=0),"
             "  FOREIGN KEY (file_id) REFERENCES FILES(file_id)"
             ");")
 
-        res = cur.execute(
-            "CREATE TABLE REQUESTS("
-            "  id INTEGER PRIMARY KEY CHECK (id = 0),"
-            "  time timestamp,"
-            "  num int DEFAULT 0"
-            ");")
-
-        res = cur.execute("INSERT INTO REQUESTS VALUES (?, ?, 0);", (0, datetime.datetime.now()))
-
-        self.con.commit()
-
         if not self.schema_ok():
             raise err.err(err_enum.CANNOT_INITIALIZE_DB)
 
-    def add_requests_count(self, count:int):
-        cur = self.con.cursor()
-        res = cur.execute("SELECT time FROM REQUESTS WHERE id = 0;");
-        db_time = res.fetchone()[0]
-
-        now = datetime.datetime.now()
-        if (db_time.date() == now.date()):
-            res = cur.execute("UPDATE REQUESTS SET num = num + ? WHERE id = 0;", (count,))
-        else:
-            res = cur.execute("UPDATE REQUESTS SET num = ?, time = ? WHERE id = 0;", (count, now))
-        self.con.commit()
-
-    def is_requests_limit_exceed(self) -> bool:
-        cur = self.con.cursor()
-        res = cur.execute("SELECT num FROM REQUESTS WHERE id = 0;")
-
-        count = res.fetchone()[0]
-
-        return count >= db.requests_limit
-
     def add_new_game(self, app_id:int, game_name:str):
         cur = self.con.cursor()
         res = cur.execute("INSERT INTO GAMES VALUES (?, ?, NULL);", (app_id, game_name))
         self.con.commit()
 
     def set_game_dir(self, app_id:int, dir_name:str):
         cur = self.con.cursor()
@@ -153,17 +105,17 @@
         game_dir_tuple = res.fetchone()
 
         if game_dir_tuple is None:
             return None
 
         return game_dir_tuple[0]
 
-    def get_file_id(self, app_id:int, path:str, filename:str) -> int:
+    def get_file_id(self, app_id:int, filename:str) -> int:
         cur = self.con.cursor()
-        res = cur.execute("SELECT file_id FROM FILES WHERE app_id=? AND path=? AND filename=?;", (app_id, path, filename))
+        res = cur.execute("SELECT file_id FROM FILES WHERE app_id=? AND filename=?;", (app_id, filename))
         file_id_tuple = res.fetchone()
         if file_id_tuple is None:
             return None
         return file_id_tuple[0]
 
     def is_game_exist(self, app_id:int):
         cur = self.con.cursor()
@@ -181,30 +133,31 @@
             file_id = cur.lastrowid
 
             no_tz_time = tup[3].replace(tzinfo=None)
             res = cur.execute("INSERT INTO VERSION VALUES (NULL, ?, ?, ?);", (file_id, no_tz_time, 0))
 
         self.con.commit()
 
-    def is_file_outdated(self, file_id:int, server_time:datetime) -> tuple:
+    def is_file_outdated(self, file_id:int, server_time:datetime) -> bool:
         cur = self.con.cursor()
+        # TODO: Bug timezone in DB
         res = cur.execute("SELECT time FROM VERSION WHERE file_id = ? and version_num = 0;", (file_id,))
         db_time_tuple = res.fetchone()
         if db_time_tuple is None:
             logger.warning(f'Failed to retrieve newest version time for file_id {file_id}')
-            return (True, None)
+            return True
 
         tz_db_time = db_time_tuple[0].replace(tzinfo=datetime.timezone.utc)
 
         logger.debug(f'DB time: {tz_db_time}, Server time: {server_time}')
 
         if tz_db_time < server_time:
-            return (True, tz_db_time)
+            return True
         else:
-            return (False, tz_db_time)
+            return False
 
     # +1 for each version
     # Insert 0 as now
     # Return max version
     def update_file_update_time_to_now(self, file_id:int, newest_file_time: datetime.datetime) -> int:
         cur = self.con.cursor()
 
@@ -232,42 +185,7 @@
         res = cur.execute("DELETE FROM VERSION WHERE file_id = ? AND version_num >= ?", (file_id, self.rotation))
 
         self.con.commit()
 
         logger.debug(f"DB Removing version {outdated_version_num}")
 
         return outdated_version_num
-
-    def get_stored_game_names(self, ids:list):
-        # Performance should be negligible other wise think of better
-        # way to query
-        cur = self.con.cursor()
-        query = "SELECT app_id, game_name FROM GAMES";
-        res = cur.execute(query)
-        result = res.fetchall();
-        if len(ids) == 0:
-            return_payload = {tup for tup in result}
-        else:
-            return_payload = {tup for tup in result if tup[0] in ids}
-        if len(ids) == 0 or len(return_payload) == len(ids):
-            return return_payload
-
-        result_set = {tup[0] for tup in result if tup[0] in ids}
-        query_set = set(ids)
-
-        diff_set = query_set - result_set
-        logger.warning(f'AppID set {diff_set} not found in database')
-        return return_payload
-
-    def get_files_info_by_appid(self, appid:int):
-        cur = self.con.cursor()
-        query = "SELECT file_id, filename, path FROM FILES WHERE app_id = ?";
-        res = cur.execute(query, (appid,))
-        result = res.fetchall();
-        return result
-
-    def get_file_version_by_file_id(self, file_id:int):
-        cur = self.con.cursor()
-        query = "SELECT time, version_num FROM VERSION WHERE file_id = ? ORDER BY version_num ASC;";
-        res = cur.execute(query, (file_id,))
-        result = res.fetchall();
-        return result
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/err.py` & `scsd-0.0.8/steamCloudSaveDownloader/err.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,29 +12,24 @@
     CANNOT_INITIALIZE_DB = 5
     CANNOT_CREATE_DIRECTORY = 6
     INVALID_WEBHOOK_URL = 7
     INVALID_COOKIE_FORMAT = 8,
     INVALID_CONFIG = 9,
     LOGIN_FAIL = 10,
     NO_SESSION = 11,
-    CANNOT_REMOVE_OUTDATED = 12,
-    REQUESTS_LIMIT_EXCEED = 13,
-    LOCKED = 14,
-    INVALID_SCRIPT_PATH = 15,
-    KB_INTERRUPT = 255
-    UNKNOWN_EXCEPTION = 256
+    CANNOT_REMOVE_OUTDATED = 12
 
 ERR_INFO = {
     err_enum.CANNOT_RETRIEVE_LIST: [
         logging.ERROR,
-        "Cannot retrieve list from Steam. Please make sure connected to Internet."
+        "Cannot retrieve list from steam. Please make sure connected to Internet and cookie is valid."
     ],
     err_enum.CANNOT_PARSE_LIST: [
         logging.ERROR,
-        "Cannot parse the list. (Session expired or program outdated)"
+        "Cannot parse the list."
     ],
     err_enum.CANNOT_RETRIEVE_GAME_FILES: [
         logging.ERROR,
         "Cannot get game files."
     ],
     err_enum.CANNOT_PARSE_GAME_FILES: [
         logging.ERROR,
@@ -62,35 +57,19 @@
     ],
     err_enum.LOGIN_FAIL: [
         logging.ERROR,
         "Login fail, please try again"
     ],
     err_enum.NO_SESSION: [
         logging.ERROR,
-        "No session found. Please re-run the program with -a <username> first"
+        "No session found. Please re-run the program with -a <username> -d <data_dir> first"
     ],
     err_enum.CANNOT_REMOVE_OUTDATED: [
         logging.WARNING,
         "Cannot remove outdated file: "
-    ],
-    err_enum.REQUESTS_LIMIT_EXCEED: [
-        logging.ERROR,
-        "Request limit exceed. Please wait until another day"
-    ],
-    err_enum.LOCKED: [
-        logging.ERROR,
-        "Cannot create lock file. Please check if another instance is running or delete if program exit unexpectedly last time."
-    ],
-    err_enum.INVALID_SCRIPT_PATH: [
-        logging.ERROR,
-        "Invalid script path. The script file does not exist or insufficient permission."
-    ],
-    err_enum.UNKNOWN_EXCEPTION: [
-        logging.ERROR,
-        "Unknown exception"
     ]
 }
 
 
 class err(Exception):
     def log(self):
         msg = self.message
@@ -102,15 +81,18 @@
             logger.warning(msg)
         elif self.level == logging.INFO:
             logger.info(msg)
         else:
             logger.debug(msg)
 
     def get_msg(err_enum: err_enum) -> str:
-        return ERR_INFO[err_enum][1]
+        if self.additional_info is None:
+            return ERR_INFO[err_enum][1]
+        else:
+            return ERR_INFO[err_enum][1] + self.additional_info
 
     def get_msg(self) -> str:
         if self.additional_info is None:
             return self.message
         else:
             return self.message + self.additional_info
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/notifier.py` & `scsd-0.0.8/steamCloudSaveDownloader/notifier.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 from enum import Enum
 from .err import err
 from .err import err_enum
-from . import ver
 import logging
 from discord_webhook import DiscordWebhook
-import subprocess
-import os
+import importlib.metadata
+
+__version__ = None
+try:
+    __version__ = importlib.metadata.version("scsd")
+except:
+    pass
 
 logger = logging.getLogger(__name__)
 
 class notify_method(Enum):
     Nop = 0
     Discord = 1
-    Script = 2
 
 class notifier:
 
     '''
     Method: Nop (Do nothing)
     Method: Discord
         Required: webhook
-    Method: Script
-        Required: path
     '''
     instance = None
 
     def get_enum(name:str):
         if name.lower() == 'discord':
             return notify_method.Discord
-        elif name.lower() == 'script':
-            return notify_method.Script
         else:
             return notify_method.Nop
 
     def is_supported(name:str):
         if len(name) == 0:
             return True
         enum_ = notifier.get_enum(name)
@@ -56,47 +55,32 @@
         if (self.method == notify_method.Nop):
             pass
         elif (self.method == notify_method.Discord):
             assert 'webhook' in kwargs, 'Discord method requires webhook'
             self.webhook = kwargs['webhook']
 
             if len(self.webhook) == 0:
-                raise(err(err_enum.INVALID_WEBHOOK_URL))
-        elif (self.method == notify_method.Script):
-            assert 'path' in kwargs, 'Script method requires path'
-            self.path = kwargs['path']
-
-            if len(self.path) == 0 or not os.path.isfile(self.path):
-                raise(err(err_enum.INVALID_SCRIPT_PATH))
+                logger.error(err.get_msg(err_enum.INVALID_WEBHOOK_URL))
+                exit(1)
         else:
             assert False, 'Unsupported notifier method'
 
     def discord_send(self, msg:str):
         webhook = DiscordWebhook(url=self.webhook, content=msg)
         webhook = webhook.execute()
 
-    def script_send(self, msg:str):
-        try:
-            subprocess.run([self.path, msg])
-        except FileNotFoundError:
-            raise(err(err_enum.INVALID_SCRIPT_PATH))
-
-    def send(self, msg:str, ok:bool) -> bool:
-        actual_msg = f'[scsd-{ver.__version__}] '
+    def send(self, msg:str, ok:bool):
+        if __version__ is None:
+            actual_msg = f'[scsd] '
+        else:
+            actual_msg = f'[scsd-{__version__}] '
         if ok:
             actual_msg += ":white_check_mark: "
         else:
             actual_msg += ":x: "
         actual_msg += f' {msg}'
-        try:
-            if self.method == notify_method.Nop:
-                pass
-            elif self.method == notify_method.Discord:
-                self.discord_send(actual_msg)
-            elif self.method == notify_method.Script:
-                self.script_send(actual_msg)
-            else:
-                assert False
-            return True
-        except Exception as e:
-            self.exception = e
-            return False
+        if self.method == notify_method.Nop:
+            return
+        elif self.method == notify_method.Discord:
+            self.discord_send(actual_msg)
+        else:
+            assert False
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/parser.py` & `scsd-0.0.8/steamCloudSaveDownloader/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,66 +4,46 @@
 from bs4 import BeautifulSoup
 import datetime
 import os
 import logging
 
 logger = logging.getLogger('scsd')
 
-g_language_specifier = "l=english"
-
 def get_tbody(soup):
     main_content = soup.find(id='main_content')
 
     if (main_content is None):
         raise err.err(err_enum.CANNOT_PARSE_LIST)
 
     if (not hasattr(main_content, "table")):
         raise err.err(err_enum.CANNOT_PARSE_LIST)
 
     return main_content.table.tbody
 
 def parse_time(input:str) -> datetime.datetime:
-    dm_format = "%d %b @ %I:%M%p %Y"
-    md_format = "%b %d @ %I:%M%p %Y"
-    dmy_format = "%d %b, %Y @ %I:%M%p"
-    mdy_format = "%b %d, %Y @ %I:%M%p"
-
-    def is_dm_format(tokens):
-        return tokens[0].isdigit()
-
     if '@' not in input:
         raise err.err(err_enum.CANNOT_PARSE_GAME_FILES)
 
     # Assume 'DD MMM [YYYY] @ HH:MM{a|p}m' format
 
     tokens = input.split(' ')
     datetime_ = None
     try:
         if len(tokens) == 4:
             now = datetime.datetime.now(tz=datetime.timezone.utc)
             year = now.year
-
-            # strptime treat date as 1900, with no Feb 29, set to
-            # leap year to circulate this problem
-            if is_dm_format(tokens):
-                d = datetime.datetime.strptime(input + " 2024", dm_format)
-            else:
-                d = datetime.datetime.strptime(input + " 2024", md_format)
+            d = datetime.datetime.strptime(input, "%d %b @ %I:%M%p")
             datetime_ = d.replace(year=year, tzinfo=datetime.timezone.utc)
         elif len(tokens) == 5:
-            if is_dm_format(tokens):
-                datetime_ = datetime.datetime.strptime(input, dmy_format).replace(tzinfo=datetime.timezone.utc)
-            else:
-                datetime_ = datetime.datetime.strptime(input, mdy_format).replace(tzinfo=datetime.timezone.utc)
+            datetime_ = datetime.datetime.strptime(input, "%d %b, %Y @ %I:%M%p")
+            datetime_ = d.replace(tzinfo=datetime.timezone.utc)
         else:
-            logger.error(f"Unable to parse time token {input}")
-            raise err.err(err_enum.CANNOT_PARSE_GAME_FILES)
+            raise err.err(er_enum.CANNOT_PARSE_GAME_FILES)
     except ValueError:
-        logger.error(f"Unable to parse time token {input}")
-        raise err.err(err_enum.CANNOT_PARSE_GAME_FILES)
+        raise err.err(er_enum.CANNOT_PARSE_GAME_FILES)
 
     return datetime_
 
 def get_appid(link:str) -> int:
     appid_token = 'appid='
     appid_location = link.find(appid_token)
 
@@ -91,20 +71,27 @@
         data = list()
 
         rows = tbody.find_all('tr')
         for row in rows:
             cols = row.find_all('td')
             data.append({
                 "name": cols[0].text.strip(),
-                "link": f"{cols[3].a['href']}&{g_language_specifier}",
+                "link": cols[3].a['href'],
                 "app_id": get_appid(cols[3].a['href'])
             })
         return data
 
     def parse_game_file(self, content) -> tuple:
+        try:
+            return self._parse_game_file(content)
+        except err.err as e:
+            e.print()
+            exit(e.err_enum)
+
+    def _parse_game_file(self, content) -> tuple:
         soup = BeautifulSoup(content, 'html.parser')
 
         tbody = get_tbody(soup)
 
         data = list()
         rows = tbody.find_all('tr')
 
@@ -122,7 +109,8 @@
 
         has_next = soup.find('a', text='next >>')
 
         if (has_next is None):
             return (data, None)
         else:
             return (data, has_next['href'])
+
```

### Comparing `scsd-0.0.71/steamCloudSaveDownloader/storage.py` & `scsd-0.0.8/steamCloudSaveDownloader/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,17 @@
 import os
 import pathlib
 from . import db
 from . import err
 from .err import err_enum
 import datetime
 import logging
-import signal
 
 logger = logging.getLogger('scsd')
 
-class keyboard_interrupt_handler:
-    def __enter__(self):
-        self.signal_received = False
-        self.old_handler = signal.signal(signal.SIGINT, self.handler)
-
-    def handler(self, sig, frame):
-        self.signal_received = (sig, frame)
-        logger.warning('SIGINT received. Delaying to ensure consistency.')
-
-    def __exit__(self, type, value, traceback):
-        signal.signal(signal.SIGINT, self.old_handler)
-        if self.signal_received:
-            self.old_handler(*self.signal_received)
-
-def key_interrupt_atomic(func):
-    def wrapper(*args, **kwargs):
-        with keyboard_interrupt_handler():
-            retval = func(*args, **kwargs)
-        return retval
-    return wrapper
-
 class storage:
     s_version_prefix = '.scsd_'
 
     def __init__(self, location:str, db_:db.db):
         self.location = location
         self.db_ = db_
 
@@ -42,15 +20,15 @@
 
         if (db_game_dir is not None):
             if os.path.isdir(os.path.join(self.location, db_game_dir)):
                 return
             else:
                 dir_name = db_game_dir
         else:
-            dir_name = f"{app_id}"
+            dir_name = f"{app_id}__{game_name}"
 
         target_dir = os.path.join(self.location, dir_name)
 
         if os.path.isdir(target_dir):
             return
 
         try:
@@ -95,15 +73,14 @@
         path_to_save = os.path.join(self.location, db_game_dir, file_path)
 
         if not os.path.isdir(path_to_save):
             os.makedirs(path_to_save)
 
         return os.path.join(path_to_save, filename + version_suffix)
 
-    @key_interrupt_atomic
     def increment_file_version(self,
                                app_id:int,
                                filename:str,
                                file_path:str,
                                current_max_version:int):
         db_game_dir = self.db_.get_game_dir(app_id)
 
@@ -124,21 +101,18 @@
 
             os.rename(
                 os.path.join(path_to_save, filename + old_version_suffix),
                 os.path.join(path_to_save, filename + new_version_suffix))
 
     # Move current version 0 to 1, 1 to 2, etc
     # Should be done before download file
-
-    @key_interrupt_atomic
     def rotate_file(self, app_id:int, filename:str, file_path:str, file_id:int, newest_file_time: datetime.datetime):
         num_of_version = self.db_.update_file_update_time_to_now(file_id, newest_file_time)
         self.increment_file_version(app_id, filename, file_path, num_of_version)
 
-    @key_interrupt_atomic
     def remove_outdated(self,
                         app_id:int,
                         filename:str,
                         file_path:str,
                         file_id:int):
         outdated_version_num = self.db_.remove_outdated_file(file_id)
```

### Comparing `scsd-0.0.71/.gitignore` & `scsd-0.0.8/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -133,8 +133,7 @@
 dev_env/
 cookies-store-steampowered-com.txt
 data/
 empty_cookie.txt
 invalid_cookies.txt
 scsd.conf
 docker_vol/
-.sentry/
```

### Comparing `scsd-0.0.71/LICENSE` & `scsd-0.0.8/LICENSE`

 * *Files identical despite different names*

