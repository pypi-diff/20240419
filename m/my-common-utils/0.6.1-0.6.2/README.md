# Comparing `tmp/my_common_utils-0.6.1.tar.gz` & `tmp/my_common_utils-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_common_utils-0.6.1.tar", max compression
+gzip compressed data, was "my_common_utils-0.6.2.tar", max compression
```

## Comparing `my_common_utils-0.6.1.tar` & `my_common_utils-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      861 2024-03-21 06:33:22.875852 my_common_utils-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       14 2024-03-15 09:34:55.983080 my_common_utils-0.6.1/README.md
--rw-r--r--   0        0        0        0 2024-03-15 09:33:35.197665 my_common_utils-0.6.1/src/utils/__init__.py
--rw-r--r--   0        0        0     2670 2024-03-16 09:36:23.994007 my_common_utils-0.6.1/src/utils/apis/firebase.py
--rw-r--r--   0        0        0     5240 2024-03-18 09:40:38.382540 my_common_utils-0.6.1/src/utils/apis/notion.py
--rw-r--r--   0        0        0     1786 2024-03-21 06:33:22.891509 my_common_utils-0.6.1/src/utils/config.py
--rw-r--r--   0        0        0      109 2024-03-15 09:20:28.196925 my_common_utils-0.6.1/src/utils/distribution/pyinstaller_fix_workdir.py
--rw-r--r--   0        0        0     1959 2024-03-15 09:20:28.198922 my_common_utils-0.6.1/src/utils/logger.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 my_common_utils-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      860 2024-04-19 09:12:55.250923 my_common_utils-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       14 2024-03-15 09:34:55.983080 my_common_utils-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-15 09:33:35.197665 my_common_utils-0.6.2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2670 2024-03-16 09:36:23.994007 my_common_utils-0.6.2/src/utils/apis/firebase.py
+-rw-r--r--   0        0        0     5240 2024-03-18 09:40:38.382540 my_common_utils-0.6.2/src/utils/apis/notion.py
+-rw-r--r--   0        0        0     2188 2024-04-19 09:12:55.243921 my_common_utils-0.6.2/src/utils/config.py
+-rw-r--r--   0        0        0      109 2024-03-15 09:20:28.196925 my_common_utils-0.6.2/src/utils/distribution/pyinstaller_fix_workdir.py
+-rw-r--r--   0        0        0     1959 2024-03-15 09:20:28.198922 my_common_utils-0.6.2/src/utils/logger.py
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 my_common_utils-0.6.2/PKG-INFO
```

### Comparing `my_common_utils-0.6.1/src/utils/apis/firebase.py` & `my_common_utils-0.6.2/src/utils/apis/firebase.py`

 * *Files identical despite different names*

### Comparing `my_common_utils-0.6.1/src/utils/apis/notion.py` & `my_common_utils-0.6.2/src/utils/apis/notion.py`

 * *Files identical despite different names*

### Comparing `my_common_utils-0.6.1/src/utils/config.py` & `my_common_utils-0.6.2/src/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from os import getenv as secret  # noqa: F401
 
 from utils.logger import create_logger
 
 logged_root_dirs = []
 
 
-def get_root_dir(dunder_file):
+def get_root_dir(dunder_file: str) -> str | None:
+    """ Returns the root directory of the project, called using __file__.
+
+    Uses either 'src', 'venv' or DOCKER_WORKDIR env-var to determine the root directory.
+    """
     root_dir = None
     try:
         if "venv" in os.path.abspath(dunder_file):
             root_dir = os.path.abspath(dunder_file).split("venv")[0]
         elif "src" in os.path.abspath(dunder_file):
             root_dir = os.path.abspath(dunder_file).split("src")[0]
         elif os.getenv('DOCKER_WORKDIR'):
@@ -27,29 +31,30 @@
     finally:
         logger.debug(f"{'ROOT_DIR' if dunder_file == __file__ else 'get_root_dir'}: {root_dir}"
                      f"  -  {os.listdir(root_dir) if root_dir not in logged_root_dirs else ''}")
         logged_root_dirs.append(root_dir)
         return root_dir
 
 
-
-def load_config_yaml(file_path: str):
+def load_config_yaml(file_path: str) -> dict | None:
+    """ Loads a yaml file from the given path and returns the data as a dict. """
     try:
         _stream = open(file_path, "r", encoding="utf-8")
         return yaml.safe_load(_stream)
     except Exception as e:
         logger.error(f"Could not load config from {file_path}")
         return None
 
 
 def config_entry(key):
     return CONFIG[key]
 
 
+# Load default config from config.yml using ROOT_DIR
 logger = create_logger("Config Helper")
 load_dotenv()
 ROOT_DIR = get_root_dir(__file__)
 if ROOT_DIR:
     CONFIG = load_config_yaml(f"{ROOT_DIR}config.yml")
 else:
-    logger.debug("ROOT_DIR is None, so not loading CONFIG")
-    CONFIG = None
+    logger.debug("ROOT_DIR is None, trying to load CONFIG from config.yml in current dir")
+    CONFIG = load_config_yaml("config.yml")
```

### Comparing `my_common_utils-0.6.1/src/utils/logger.py` & `my_common_utils-0.6.2/src/utils/logger.py`

 * *Files identical despite different names*

### Comparing `my_common_utils-0.6.1/PKG-INFO` & `my_common_utils-0.6.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: my-common-utils
-Version: 0.6.1
+Version: 0.6.2
 Summary: A selection of common utility functions, and useful APIs
 Author: Oliver Stoll
 Author-email: oliverstoll.berlin@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: notion-client (>=2.2.1,<3.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
```

